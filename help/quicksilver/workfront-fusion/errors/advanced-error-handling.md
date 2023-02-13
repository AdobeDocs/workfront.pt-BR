---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
title: Tratamento de erros avançado em [!DNL Adobe] Workfront Fusion
description: As técnicas avançadas de tratamento de erros incluem filtragem e aninhamento.
author: Becky
feature: Workfront Fusion
exl-id: 57f43fc2-23ed-44f5-8785-90739329b5ee
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '913'
ht-degree: 0%

---

# Tratamento de erros avançado em [!DNL Adobe Workfront Fusion]

As técnicas avançadas de tratamento de erros incluem filtragem e aninhamento.

## Requisitos de acesso

Você deve ter o seguinte acesso para usar a funcionalidade neste artigo:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plano*</td> 
   <td> <p>[!UICONTROL Pro] ou superior</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licença*</td> 
   <td> <p>[!UICONTROL Plano], [!UICONTROL Trabalho]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da [!UICONTROL Adobe Workfront Fusion]**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] para automação e integração de trabalho] </p><p>[!UICONTROL [!DNL Workfront Fusion] para Automação de Trabalho]</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produto</td> 
   <td>Sua organização deve comprar [!DNL Adobe Workfront Fusion] bem como [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo.</td> 
  </tr> 
 </tbody> 
</table>

Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com seu [!DNL Workfront] administrador.

Para obter informações sobre [!DNL Adobe Workfront Fusion] licenças, consulte [[!DNL Adobe Workfront Fusion] licenças](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Filtros

Há dois tipos de filtragem que podem ocorrer em uma rota do manipulador de erros.

* [Adicionar um filtro à rota do manipulador de erros](#adding-a-filter-to-the-error-handler-route)
* [Adicionar um Roteador seguido de filtros à rota do manipulador de erros](#adding-a-router-followed-by-filters-to-the-error-handler)

### Adicionar um filtro à rota do manipulador de erros

Você pode usar um filtro para controlar quais erros são tratados pela rota do manipulador de erros. Isso permite processar apenas tipos específicos de erros. Se um erro não passar pelo filtro, ele será tratado como se não houvesse uma rota do manipulador de erros definida para o módulo em questão.

>[!INFO]
>
>**Exemplo:**
>
>![](assets/filter-error-handling-350x238.png)

### Adicionar um [!UICONTROL Roteador] seguido por filtros para o manipulador de erros

>[!INFO]
>
>![](assets/router-filter-error-handling-350x254.png)
>
>Neste exemplo, o erro ocorre na variável [!UICONTROL Criar uma pasta] módulo (A), que tem uma rota regular e uma rota de manipulador de erros. O último é seguido por um roteador com uma rota que tem um filtro que define um tipo específico de erro (Ocorre um Erro de Dados) e o outro é a rota padrão para todos os outros erros. A primeira rota termina com o [!UICONTROL Retomar] diretiva que contém valores substitutos para o cenário retomar do módulo A ([!UICONTROL Criar uma pasta]), enquanto a segunda rota termina com a variável [!UICONTROL Reversão] diretiva que interrompe a execução do cenário imediatamente.

Consulte [Processamento de erros no [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-processing.md) para obter mais informações sobre vários tipos de erros e sobre como [!DNL Workfront Fusion] Os processa e avalia.

### O cenário de exemplo

Você pode configurar este exemplo de cenário para entender como esses filtros funcionam para o tratamento de erros.

Usar um [!DNL Dropbox] pasta para carregar um arquivo em vez de criar um novo

Se você usar a variável [!UICONTROL Criar uma pasta] módulo em [!DNL Dropbox] e uma pasta com o mesmo nome já existir, o módulo lançará um Erro de dados, como mostrado abaixo:

![](assets/dropbox-350x276.png)

O cenário completo:

![](assets/dropbox-scenario-350x190.png)

1. O [!UICONTROL Ferramentas] > [!UICONTROL Definir variável] módulo contém o nome da pasta
1. O [!UICONTROL HTTP] >[!UICONTROL Obter um arquivo] O módulo busca o arquivo que precisa ser carregado na pasta
1. O [!UICONTROL Dropbox] >[!UICONTROL Criar uma pasta] O módulo acionará um erro se uma pasta já existir com o mesmo nome que a mapeada no módulo
1. A rota do manipulador de erros (bolhas transparentes) contém um roteador para filtrar os erros
1. A primeira rota é para um tipo especificado de erro chamado Erro de Dados, como já sabemos:

   1. Se ocorrer um erro de dados e os detalhes do erro passarem pelo filtro, a variável [!UICONTROL Dropbox] >[!UICONTROL Listar todos os arquivos/subpastas em um módulo de pasta] lista todas as pastas em [!DNL Dropbox]
   1. O filtro subsequente corresponde aos nomes da pasta
   1. O [!UICONTROL Retomar] diretiva especifica a ID da pasta e o caminho da pasta existente e a execução do cenário é retomada do [!UICONTROL Dropbox] >[!UICONTROL Criar uma pasta] , mas em vez de tentar criar uma nova pasta, desta vez ele usa os valores do [!UICONTROL Retomar] diretiva para mover para o próximo módulo e fazer upload do arquivo na pasta existente

1. A segunda rota é para todos os outros erros e termina com a variável [!UICONTROL Reversão] diretiva que resulta na interrupção imediata do cenário

Veja abaixo uma explicação detalhada da 5ª declaração:

Para usar a pasta existente nos módulos subsequentes ([!UICONTROL Carregar um arquivo] abaixo), é necessário adicionar uma rota do manipulador de erros ao módulo e buscar o caminho da pasta a ser mapeado no [!UICONTROL Retomar] módulo de diretiva que segue:

![](assets/add-error-handler-route-350x113.png)

O filtro na primeira rota é definido para lidar somente com o erro específico (Erro de dados) que aparece quando uma pasta com o mesmo nome já existe:

![](assets/condition-350x327.png)

O [!UICONTROL Dropbox] >[!UICONTROL Listar todos os arquivos em uma pasta] é configurado para retornar todas as pastas na pasta de destino. O filtro a seguir só passa no que estávamos tentando criar originalmente (o nome da pasta é armazenado no 33. Nome da pasta (item):

![](assets/condition2-350x193.png)

Eventualmente, o [!UICONTROL Retomar] A diretiva fornece o caminho da Pasta como saída para o módulo com falha. Observe que a ID da pasta foi deixada em branco, pois não é necessária para o[!UICONTROL Carregar um arquivo]Módulo &#39;:

![](assets/flow-control-350x190.png)

## Aninhamento

Independentemente de onde um módulo esteja localizado, as rotas do manipulador de erros podem ser criadas e implementadas em todos os módulos, exceto roteadores. Portanto, é possível criar uma rota do manipulador de erros para um módulo que já faz parte de uma rota do manipulador de erros existente criada para outro módulo.

Veja um exemplo de uma rota aninhada do manipulador de erros:

![](assets/nested-error-handling-route-350x174.png)

Nesse cenário, a segunda rota do manipulador de erros é aninhada na primeira rota do manipulador de erros. Assim, se a variável [!UICONTROL Dropbox] >[!UICONTROL Criar um módulo de pasta] encontra um erro, a execução é movida para a Rota 1, se a variável [!UICONTROL Ocorre um erro de dados] for transmitido, o próximo módulo será executado seguido pela função [!UICONTROL Retomar] módulo de diretiva se um erro não ocorrer com o [!UICONTROL Dropbox] >[!UICONTROL Listar todos os arquivos/subpastas] em um módulo de pasta.

No entanto, se ocorrer um erro com isso [!DNL Dropbox] em seguida, a execução é movida para a Rota 2 do Manipulador de Erros e termina com [!UICONTROL Ignorar] diretiva. O [!UICONTROL Retomar diretiva] não é executado nesse caso.

Essa é uma combinação de filtros e manipuladores de erros de aninhamento.

