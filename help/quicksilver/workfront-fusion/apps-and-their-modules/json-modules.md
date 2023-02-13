---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Módulos JSON
description: O aplicativo Adobe Workfront Fusion JSON fornece módulos para processar dados no formato JSON, de modo que o Adobe Workfront Fusion possa trabalhar ainda mais com o conteúdo de dados ou criar novo conteúdo JSON.
author: Becky
feature: Workfront Fusion
exl-id: 60540608-9d2e-4e10-9fb2-5388dda64784
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1157'
ht-degree: 0%

---

# [!UICONTROL JSON] módulos

O [!DNL Adobe Workfront Fusion] [!UICONTROL JSON] o aplicativo fornece módulos para processar dados no formato JSON, de modo que [!DNL Adobe Workfront Fusion] pode trabalhar ainda mais com o conteúdo de dados ou criar novo conteúdo JSON.

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] para automação e integração de trabalho] </p> <p>[!UICONTROL [!DNL Workfront Fusion] para Automação de Trabalho] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produto</td> 
   <td>Sua organização deve comprar [!DNL Adobe Workfront Fusion] bem como [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo.</td> 
  </tr> 
 </tbody> 
</table>

Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com seu [!DNL Workfront] administrador.

Para obter informações sobre [!DNL Adobe Workfront Fusion] licenças, consulte [[!DNL Adobe Workfront Fusion] licenças](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Analisar JSON

* [Estrutura de dados](#data-structure)
* [Coleção versus Matriz](#collection-vs-array)

### Estrutura de dados

A estrutura de dados descreve como os dados JSON são organizados e permite o mapeamento de itens JSON individuais para outros módulos em seu cenário. Se você não fornecer a estrutura de dados, poderá executar manualmente o módulo e [!DNL Workfront Fusion] criará a estrutura do JSON fornecido:

1. Adicione o [!UICONTROL Analisar JSON] para um cenário.
1. No **[!UICONTROL String JSON]** , insira o JSON do qual deseja criar uma estrutura de dados.
1. Não conecte outros módulos à [!UICONTROL Analisar JSON] módulo ainda. Porque [!DNL Workfront Fusion] ainda não conhece a estrutura dos dados JSON, ainda não é possível mapear dados do [!UICONTROL Analisar JSON] para outros módulos em seu cenário.
1. Execute o cenário manualmente. Isso permite que a variável [!UICONTROL Analisar JSON] para identificar a estrutura JSON do JSON fornecido.
1. Agora você pode conectar os seguintes módulos. Os itens do módulo JSON de análise agora estão disponíveis para mapeamento.

Para obter mais informações, consulte [Estruturas de dados em [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/modules/data-structures.md).

### Coleção versus Matriz

Se o campo da cadeia JSON contiver uma coleção `{ ... }`, A saída é um único pacote contendo os itens da coleção.

>[!INFO]
>
>**Exemplo:**
>
>
```
>{
>       "name" : "Peter",
>
>    
   "ID" : 1
>}
>```
>
>![](assets/json-collection.png)

Se o campo da string JSON contiver uma matriz `[ ... ]`, a saída é uma série de pacotes. cada pacote contém um elemento da matriz.

>[!INFO]
>
>**Exemplo:**
>
>
```
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

Ao configurar [!DNL JSON] módulos, [!DNL Workfront Fusion] exibe os campos listados abaixo. Juntamente com eles, campos JSON adicionais podem ser exibidos, dependendo de fatores como seu nível de acesso no aplicativo ou serviço. Um título em negrito em um módulo indica um campo obrigatório.

Se o botão de mapa for exibido acima de um campo ou função, é possível usá-lo para definir variáveis e funções para esse campo. Para obter mais informações, consulte [Mapear informações de um módulo para outro no [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Agregar ao JSON](#aggregate-to-json)
* [Converter JSON em XML](#convert-json-to-xml)
* [Analisar JSON](#parse-json)
* [Criar JSON](#create-json)
* [Transformar JSON](#transform-json)

### [!UICONTROL Agregar ao JSON]

Este módulo agregador agrega a saída de um módulo anterior no JSON.

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
   <td> <p>Selecione a estrutura de dados que deseja usar para criar o JSON. A estrutura de dados determina quais outros campos estão disponíveis nesse módulo. Para obter mais informações, consulte <a href="#data-structure" class="MCXref xref">Estrutura de dados</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Indentação]</td> 
   <td> <p> Selecione se deseja recuar o JSON usando guias, dois espaços ou quatro espaços.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Agrupar por]</td> 
   <td>Defina uma expressão pela qual deseja agrupar a saída agregada. Essa expressão pode conter um ou mais itens mapeados. Os dados agregados são então separados em grupos usando o valor dessa expressão. Cada grupo é gerado como um pacote separado com uma chave (a expressão avaliada) e um valor (o texto agregado). Você pode usar a chave como filtro em módulos subsequentes.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Parar o processamento após uma agregação vazia]</td> 
   <td>Ative essa opção para interromper o cenário quando não houver resultados.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Converter JSON em XML]

Esse módulo de ação converte uma string JSON em XML.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL JSON string] </td> 
   <td> <p>Insira ou mapeie o JSON que deseja converter em XML.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Analisar JSON]

Esse módulo de ação analisa uma string JSON em uma estrutura de dados, que permite acessar os dados dentro da string JSON.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Estrutura de dados]</td> 
   <td> <p>Selecione a estrutura de dados que deseja usar para criar o JSON. Para obter mais informações, consulte <a href="#data-structure" class="MCXref xref">Estrutura de dados</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL JSON string] </td> 
   <td> <p>Insira ou mapeie o JSON que deseja analisar.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Criar JSON]

Esse módulo de ação cria o JSON de uma estrutura de dados.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">Estrutura de dados</td> 
   <td> <p>Selecione a estrutura de dados que deseja usar para criar o JSON. Para obter mais informações, consulte <a href="#data-structure" class="MCXref xref">Estrutura de dados</a> neste artigo.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Transformar JSON]

Esse módulo de ação transforma um objeto em uma string json.

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

## Transformando registros de dados em JSON

>[!INFO]
>
>**Exemplo:** O exemplo a seguir mostra como transformar registros de dados de [!DNL Google Sheets] para o formato JSON:
>
>1. Coloque o [!DNL Google Sheets] > [!UICONTROL Selecionar linhas] no seu cenário para buscar os dados. Configurar o módulo para recuperar linhas de seu [!DNL Google] planilha. Defina o &#x200B;**[!UICONTROL Número máximo de linhas retornadas]** para um número pequeno, mas maior que um para fins de teste (exemplo, três). Execute o [!DNL Google Sheets] clicando com o botão direito do mouse e escolhendo &quot;**[!UICONTROL Executar este módulo somente]**.&quot; Verifique a saída do módulo.
1. Conecte o [!UICONTROL Agregador de matriz] após a [!DNL Google Sheets] módulo. Na configuração do módulo, escolha [!DNL Google Sheets] no **[!UICONTROL Nó de origem]** campo. Deixe os outros campos como estão no momento.
1. Connect [!UICONTROL JSON] > [!UICONTROL Criar JSON] após a [!UICONTROL Agregador de matriz] módulo. A configuração do módulo requer uma estrutura de dados que descreve o formato JSON. Clique em **[!UICONTROL Adicionar]** para abrir a configuração da estrutura de dados. A maneira mais fácil de criar essa estrutura de dados é gerá-la automaticamente a partir de uma amostra JSON. Clique em **[!UICONTROL Gerador]** e cole sua amostra do JSON no **[!UICONTROL Dados de exemplo]** campo :

   **Exemplo:**
   ```
   {
   
   "books": [
   
   {
   
   "id": "ID",
   
   "title": "Title",
   
   "author": "Author"
   
   }
   
   ]
   
   }
   ```
1. Clique em **[!UICONTROL Salvar]**. O [!UICONTROL Especificação] no campo Data structure agora contém a estrutura gerada.
1. Altere o nome da sua estrutura de dados para algo mais específico e clique em **[!UICONTROL Salvar]**. Um campo correspondente ao atributo da matriz raiz é exibido como um campo mapeável na configuração do módulo JSON.
1. Clique no botão **[!UICONTROL Mapa]** ao lado do campo e mapeie a variável `Array[]` item da saída do agregador de matriz para ele.
1. Clique em **[!UICONTROL OK]** para fechar o [!UICONTROL JSON] configuração do módulo.
1. Abra a configuração do [!UICONTROL Agregador de matriz] módulo. Altere o **[!UICONTROL Estrutura do Target]** from [!UICONTROL Personalizado] para [!UICONTROL JSON] campo do módulo correspondente ao atributo da matriz raiz. Mapear itens do [!DNL Google Sheets] aos campos apropriados.
1. Clique em **[!UICONTROL OK]** para fechar o [!UICONTROL Agregador de matriz] configuração do módulo.
1. Execute o cenário.
   O [!UICONTROL JSON] O módulo gera o formato JSON correto.
1. Abra a configuração do [!DNL Google Sheets] e aumente o [!UICONTROL Número máximo de linhas retornadas] número para ser maior que o número de linhas na planilha para processar todos os dados.


## Solução de problemas

### Não é possível mapear dados do [!UICONTROL Analisar JSON] módulo

Certifique-se de que o conteúdo JSON esteja mapeado corretamente na variável [!UICONTROL Analisar JSON] e que a estrutura de dados está definida corretamente. Para obter mais informações, consulte [Transformando registros de dados em JSON](#transforming-data-records-to-json) neste artigo.

### O módulo falha ao usar declarações condicionais no JSON

Ao usar declarações condicionais como `if` no JSON, coloque as aspas fora da declaração condicional.

>[!INFO]
**Exemplo:**
![](assets/quotes-in-json-350x120.png)
