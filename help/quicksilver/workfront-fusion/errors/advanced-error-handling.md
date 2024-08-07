---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
title: Tratamento de erros avançado no  [!DNL Adobe] Workfront Fusion
description: As técnicas avançadas de manipulação de erros incluem filtragem e aninhamento.
author: Becky
feature: Workfront Fusion
exl-id: 57f43fc2-23ed-44f5-8785-90739329b5ee
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '960'
ht-degree: 0%

---

# Tratamento de erros avançado em [!DNL Adobe Workfront Fusion]

As técnicas avançadas de manipulação de erros incluem filtragem e aninhamento.

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
   <td role="rowheader">Licença [!UICONTROL Adobe Workfront Fusion]**</td> 
   <td>
   <p>Requisito de licença atual: nenhum requisito de licença [!DNL Workfront Fusion].</p>
   <p>Ou</p>
   <p>Requisito de licença herdada: [!UICONTROL [!DNL Workfront Fusion] para Automação e Integração do Trabalho] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produto</td> 
   <td>
   <p>Requisito atual do produto: se você tiver o Plano [!DNL Adobe Workfront] da [!UICONTROL Select] ou da [!UICONTROL Prime], sua organização deve comprar o [!DNL Adobe Workfront Fusion] e o [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo. [!DNL Workfront Fusion] está incluído no plano [!DNL Workfront] do [!UICONTROL Ultimate].</p>
   <p>Ou</p>
   <p>Requisito de produto herdado: sua organização deve comprar o [!DNL Adobe Workfront Fusion] e o [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Para saber que plano, tipo de licença ou acesso você tem, contate o administrador do [!DNL Workfront].

Para obter informações sobre [!DNL Adobe Workfront Fusion] licenças, consulte [[!DNL Adobe Workfront Fusion] licenças](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Filtros

Há dois tipos de filtragem que podem ocorrer em uma rota de manipulador de erros.

* [Adicionar um filtro à rota do manipulador de erros](#adding-a-filter-to-the-error-handler-route)
* [Adicionar um roteador seguido de filtros à rota do manipulador de erros](#adding-a-router-followed-by-filters-to-the-error-handler)

### Adicionar um filtro à rota do manipulador de erros

Você pode usar um filtro para controlar quais erros são manipulados pela rota do manipulador de erros. Isso permite processar apenas tipos específicos de erros. Se um erro não passar pelo filtro, ele será tratado como se não houvesse nenhuma rota de manipulador de erros definida para o módulo fornecido.

>[!INFO]
>
>**Exemplo:**
>
>![](assets/filter-error-handling-350x238.png)

### Adicionando um [!UICONTROL Roteador] seguido por filtros ao manipulador de erros

>[!INFO]
>
>![](assets/router-filter-error-handling-350x254.png)
>
>Neste exemplo, o erro ocorre no módulo (A) [!UICONTROL Criar uma pasta], que tem uma rota regular e uma rota de manipulador de erros. O último é seguido por um roteador com uma rota que tem um filtro que define um tipo específico de erro (Ocorre o erro de dados) e a outra que é a rota padrão para todos os outros erros. A primeira rota termina com a diretiva [!UICONTROL Resume], que contém valores substitutos para o cenário retomar do módulo A ([!UICONTROL Criar uma pasta]), enquanto a segunda rota termina com a diretiva [!UICONTROL Rollback], que interrompe a execução do cenário imediatamente.

Consulte [Processamento de erros [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-processing.md) para obter mais informações sobre vários tipos de erros e sobre como o [!DNL Workfront Fusion] os processa e avalia.

### O exemplo de cenário

Você pode configurar esse exemplo de cenário para entender como esses filtros funcionam para a manipulação de erros.

Usar uma pasta [!DNL Dropbox] existente para carregar um arquivo em vez de criar um novo

Se você usar o módulo [!UICONTROL Criar uma pasta] em [!DNL Dropbox] e já existir uma pasta com o mesmo nome, o módulo exibirá um Erro de Dados como mostrado abaixo:

![](assets/dropbox-350x276.png)

O cenário completo:

![](assets/dropbox-scenario-350x190.png)

1. O módulo [!UICONTROL Ferramentas] > [!UICONTROL Definir Variável] contém o nome da pasta
1. O módulo [!UICONTROL HTTP] >[!UICONTROL Obter um arquivo] busca o arquivo que precisa ser carregado na pasta
1. O módulo [!UICONTROL Dropbox] >[!UICONTROL Criar uma pasta] aciona um erro se uma pasta já existir com o mesmo nome que a mapeada no módulo
1. A rota do manipulador de erros (bolhas transparentes) contém um roteador para filtrar os erros
1. A primeira rota é para um tipo específico de erro chamado Erro de Dados, pois já sabemos disso:

   1. Se ocorrer um Erro de Dados e os detalhes do erro passarem pelo filtro, o [!UICONTROL Dropbox] >[!UICONTROL Listar todos os arquivos/subpastas em um módulo de pasta] listará todas as pastas em [!DNL Dropbox]
   1. O filtro subsequente corresponde aos nomes da pasta
   1. A diretiva [!UICONTROL Resume] especifica a ID de pasta e o caminho de pasta da pasta existente, e a execução do cenário continua a partir do módulo [!UICONTROL Dropbox] >[!UICONTROL Criar uma pasta], mas em vez de tentar criar uma nova pasta, desta vez ela usa os valores da diretiva [!UICONTROL Resume] para mover para o próximo módulo e carregar o arquivo na pasta existente

1. A segunda rota é para todos os outros erros e termina com a diretiva [!UICONTROL Rollback], que resulta na interrupção imediata do cenário

Veja abaixo uma explicação detalhada da 5ª declaração:

Para usar a pasta existente em seus módulos subsequentes ([!UICONTROL Carregar um arquivo] abaixo), é necessário adicionar uma rota de manipulador de erros ao módulo e buscar o caminho da pasta a ser mapeado no módulo de diretiva [!UICONTROL Retomar] da seguinte maneira:

![](assets/add-error-handler-route-350x113.png)

O filtro na primeira rota é definido para lidar apenas com o erro específico (Erro de dados) que aparece quando uma pasta com o mesmo nome já existe:

![](assets/condition-350x327.png)

O módulo [!UICONTROL Dropbox] >[!UICONTROL List all files in a folder] está configurado para retornar todas as pastas na pasta de destino. O filtro a seguir passa apenas aquele que estávamos tentando criar originalmente (o nome da pasta é armazenado no 33. Nome da pasta (item):

![](assets/condition2-350x193.png)

Eventualmente, a diretiva [!UICONTROL Resume] fornece o caminho da Pasta como saída para o módulo com falha. Observe que a ID da Pasta foi deixada em branco, pois não é necessária para o módulo &#39;[!UICONTROL Carregar um arquivo]&#39;:

![](assets/flow-control-350x190.png)

## Aninhamento

Independentemente de onde um módulo esteja localizado, as rotas do manipulador de erros podem ser criadas e implementadas em todos os módulos, exceto roteadores. Portanto, é possível criar uma rota de manipulador de erros para um módulo que já faz parte de uma rota de manipulador de erros existente criada para outro módulo.

Este é um exemplo de uma rota de manipulador de erro aninhada:

![](assets/nested-error-handling-route-350x174.png)

Nesse cenário, a segunda rota do manipulador de erros é aninhada na primeira rota do manipulador de erros. Portanto, se o [!UICONTROL Dropbox] >[!UICONTROL Criar um módulo de pasta] encontrar um erro, a execução será movida para a Rota 1; se o filtro [!UICONTROL Erro de Dados Ocorre] for passado, o próximo módulo será executado seguido pelo módulo de diretiva [!UICONTROL Retomar] se um erro não ocorrer com o [!UICONTROL Dropbox] >[!UICONTROL Listar todos os arquivos/subpastas] em um módulo de pasta.

No entanto, se ocorrer um erro com este módulo [!DNL Dropbox], a execução será movida para a Rota 2 do Manipulador de Erros e terminará com a diretiva [!UICONTROL Ignore]. O módulo de diretiva [!UICONTROL Resume] não é executado neste caso.

Essa é uma combinação de filtragem e aninhamento de manipuladores de erro.

