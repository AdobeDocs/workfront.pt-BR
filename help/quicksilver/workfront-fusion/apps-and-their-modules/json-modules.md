---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Módulos JSON
description: O aplicativo JSON do Adobe Workfront Fusion fornece módulos para processar dados no formato JSON, de modo que o Adobe Workfront Fusion possa trabalhar ainda mais com o conteúdo de dados ou criar novo conteúdo JSON.
author: Becky
feature: Workfront Fusion
exl-id: 60540608-9d2e-4e10-9fb2-5388dda64784
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '1205'
ht-degree: 0%

---

# [!UICONTROL JSON] módulos

A variável [!DNL Adobe Workfront Fusion] [!UICONTROL JSON] O aplicativo fornece módulos para processar dados no formato JSON para que [!DNL Adobe Workfront Fusion] O pode trabalhar mais com o conteúdo de dados ou criar novo conteúdo JSON.

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
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licença**</td> 
   <td>
   <p>Requisito de licença atual: Não [!DNL Workfront Fusion] requisito de licença.</p>
   <p>Ou</p>
   <p>Requisito de licença herdada: [!UICONTROL [!DNL Workfront Fusion] para Automação e Integração do Trabalho], [!UICONTROL [!DNL Workfront Fusion] para automação de trabalho]</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produto</td> 
   <td>
   <p>Requisito atual do produto: se você tiver o [!UICONTROL Select] ou o [!UICONTROL Prime] [!DNL Adobe Workfront] Planejar, sua organização deve comprar [!DNL Adobe Workfront Fusion] bem como [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo. [!DNL Workfront Fusion] está incluído no [!UICONTROL Ultimate] [!DNL Workfront] plano.</p>
   <p>Ou</p>
   <p>Requisito de produto herdado: sua organização deve comprar [!DNL Adobe Workfront Fusion] bem como [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Para descobrir que plano, tipo de licença ou acesso você tem, entre em contato com o [!DNL Workfront] administrador.

Para obter informações sobre [!DNL Adobe Workfront Fusion] licenças, consulte [[!DNL Adobe Workfront Fusion] licenças](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Analisar JSON

* [Estrutura de dados](#data-structure)
* [Coleção versus array](#collection-vs-array)

### Estrutura de dados

A estrutura de dados descreve como os dados JSON são organizados e permite o mapeamento de itens JSON individuais para outros módulos em seu cenário. Se você não fornecer a estrutura de dados, poderá executar o módulo manualmente e [!DNL Workfront Fusion] criará a estrutura a partir do JSON fornecido:

1. Adicione o [!UICONTROL Analisar JSON] para um cenário.
1. No **[!UICONTROL String JSON]** insira o JSON no qual deseja criar uma estrutura de dados.
1. Não conecte outros módulos à [!UICONTROL Analisar JSON] módulo ainda. Porque [!DNL Workfront Fusion] ainda não conhece a estrutura dos dados JSON, ainda não é possível mapear dados do [!UICONTROL Analisar JSON] para outros módulos em seu cenário.
1. Execute o cenário manualmente. Isso permite que o [!UICONTROL Analisar JSON] para identificar a estrutura JSON do JSON fornecido.
1. Agora você pode conectar os seguintes módulos. Os itens do módulo JSON de análise agora estão disponíveis para mapeamento.

Para obter mais informações, consulte [Estruturas de dados no [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/modules/data-structures.md).

### Coleção versus array

Se o campo de string JSON contiver uma coleção `{ ... }`, A saída é um único pacote que contém os itens da coleção.

>[!INFO]
>
>**Exemplo:**
>
>```
>{
>       "name" : "Peter",
>
>    
   "ID" : 1
>}
>```
>
>![](assets/json-collection.png)

Se o campo de string JSON contiver uma matriz `[ ... ]`, a saída é uma série de pacotes. cada pacote contém um elemento da matriz.

>[!INFO]
>
>**Exemplo:**
>
>```
>[
>   {
>       "name" : "Peter",
>       "ID" : 1
>   },
>
>  
 {
>       "name" : "Mike",
>       "ID" : 2
>   }
>]
>```
>
>![](assets/json-array.png)

## [!UICONTROL JSON] módulos e seus campos

Ao configurar [!DNL JSON] módulos, [!DNL Workfront Fusion] exibe os campos listados abaixo. Junto com esses, campos JSON adicionais podem ser exibidos, dependendo de fatores como nível de acesso no aplicativo ou serviço. Um título em negrito em um módulo indica um campo obrigatório.

Se você vir o botão de mapa acima de um campo ou função, poderá usá-lo para definir variáveis e funções para esse campo. Para obter mais informações, consulte [Mapear informações de um módulo para outro no [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Agregar ao JSON](#aggregate-to-json)
* [Converter JSON em XML](#convert-json-to-xml)
* [Analisar JSON](#parse-json)
* [Criar JSON](#create-json)
* [Transformar JSON](#transform-json)

### [!UICONTROL Agregar ao JSON]

Esse módulo agregador agrega a saída de um módulo anterior no JSON.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Módulo de origem] </td> 
   <td> <p>Selecione o módulo que gera os dados que você deseja agregar ao JSON.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Estrutura de dados]</td> 
   <td> <p>Selecione a estrutura de dados que deseja usar para criar JSON. A estrutura de dados determina quais outros campos estão disponíveis nesse módulo. Para obter mais informações, consulte <a href="#data-structure" class="MCXref xref">Estrutura de dados</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Recuo]</td> 
   <td> <p> Selecione se deseja recuar o JSON usando tabulações, dois espaços ou quatro espaços.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Agrupar por]</td> 
   <td>Defina uma expressão pela qual você deseja agrupar a saída agregada. Esta expressão pode conter um ou mais itens mapeados. Os dados agregados são, então, separados em grupos usando o valor dessa expressão. Cada grupo gera um pacote separado com uma chave (a expressão avaliada) e um valor (o texto agregado). Você pode usar a chave como um filtro nos módulos subsequentes.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Parar processamento após uma agregação vazia]</td> 
   <td>Habilite essa opção para interromper o cenário quando não houver resultados.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Converter JSON em XML]

Esse módulo de ação converte uma sequência de caracteres JSON em XML.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL cadeia de caracteres JSON] </td> 
   <td> <p>Insira ou mapeie o JSON que você deseja converter em XML.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Analisar JSON]

Esse módulo de ação analisa uma sequência JSON em uma estrutura de dados, que permite acessar os dados dentro da sequência JSON.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Estrutura de dados]</td> 
   <td> <p>Selecione a estrutura de dados que deseja usar para criar JSON. Para obter mais informações, consulte <a href="#data-structure" class="MCXref xref">Estrutura de dados</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL cadeia de caracteres JSON] </td> 
   <td> <p>Insira ou mapeie o JSON que deseja analisar.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Criar JSON]

Esse módulo de ação cria o JSON a partir de uma estrutura de dados.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">Estrutura de dados</td> 
   <td> <p>Selecione a estrutura de dados que deseja usar para criar JSON. Para obter mais informações, consulte <a href="#data-structure" class="MCXref xref">Estrutura de dados</a> neste artigo.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Transformar JSON]

Esse módulo de ação transforma um objeto em uma sequência de caracteres json.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Objeto]</td> 
   <td> <p>Insira ou mapeie o objeto que deseja transformar em JSON.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Transformação de registros de dados em JSON

>[!INFO]
>
>**Exemplo:** O exemplo a seguir mostra como transformar registros de dados de [!DNL Google Sheets] para o formato JSON:
>
>1. Coloque o [!DNL Google Sheets] > [!UICONTROL Selecionar linhas] em seu cenário para buscar os dados. Configure o módulo para recuperar linhas do [!DNL Google] planilha eletrônica. Defina o&#x200B;**[!UICONTROL Número máximo de linhas retornadas]** para um número pequeno, mas maior que um para fins de teste (Exemplo, três). Execute o [!DNL Google Sheets] clicando com o botão direito do mouse e escolhendo &quot;**[!UICONTROL Executar este módulo somente]**.&quot; Verifique a saída do módulo.
>
1. Conecte o [!UICONTROL Agregador de matrizes] módulo após a variável [!DNL Google Sheets] módulo. Na configuração do módulo, escolha a variável [!DNL Google Sheets] módulo no **[!UICONTROL Nó de origem]** campo. Deixe os outros campos como estão para o momento.
>
1. Conectar [!UICONTROL JSON] > [!UICONTROL Criar JSON] módulo após a variável [!UICONTROL Agregador de matrizes] módulo. A configuração do módulo requer uma estrutura de dados que descreva o formato JSON. Clique em **[!UICONTROL Adicionar]** para abrir a configuração da estrutura de dados. A maneira mais fácil de criar essa estrutura de dados é gerá-la automaticamente a partir de uma amostra JSON. Clique em **[!UICONTROL Gerador]** e cole sua amostra JSON no **[!UICONTROL Dados de exemplo]** campo:
>
**Exemplo:**
>   
>```
>{
>
>"books": [
>
>{
>
>"id": "ID",
>
>"title": "Title",
>
>"author": "Author"
>
>}
>
>]
>
>}
>```
>
1. Clique em **[!UICONTROL Salvar]**. A variável [!UICONTROL Especificação] O campo na estrutura de dados agora contém a estrutura gerada.
1. Altere o nome da estrutura de dados para algo mais específico e clique em **[!UICONTROL Salvar]**. Um campo correspondente ao atributo de matriz raiz aparece como um campo mapeável na configuração do módulo JSON.
>
1. Clique em **[!UICONTROL Mapa]** ao lado do campo e mapear o `Array[]` da saída do agregador de matriz para ele.
>
1. Clique em **[!UICONTROL OK]** para fechar o [!UICONTROL JSON] configuração do módulo.
>
1. Abra a configuração do [!UICONTROL Agregador de matrizes] módulo. Altere o **[!UICONTROL Estrutura de destino]** de [!UICONTROL Personalizado] para o [!UICONTROL JSON] campo do módulo correspondente ao atributo de matriz raiz. Mapear itens do [!DNL Google Sheets] para os campos apropriados.
>
1. Clique em **[!UICONTROL OK]** para fechar o [!UICONTROL Agregador de matrizes] configuração do módulo.
>
1. Execute o cenário.
>
A variável [!UICONTROL JSON] O módulo do gera o formato JSON correto.
>
1. Abra a configuração do [!DNL Google Sheets] e aumentar o [!UICONTROL Número máximo de linhas retornadas] para ser maior que o número de linhas na planilha para processar todos os dados.

## Solução de problemas

### Não é possível mapear dados do [!UICONTROL Analisar JSON] módulo

Verifique se o conteúdo JSON está mapeado corretamente na variável [!UICONTROL Analisar JSON] e que a estrutura de dados esteja definida corretamente. Para obter mais informações, consulte [Transformação de registros de dados em JSON](#transforming-data-records-to-json) neste artigo.

### O módulo falha ao usar declarações condicionais em JSON

Ao usar declarações condicionais como `if` no JSON, coloque as aspas fora da declaração condicional.

>[!INFO]
>
**Exemplo:**
>
![](assets/quotes-in-json-350x120.png)
