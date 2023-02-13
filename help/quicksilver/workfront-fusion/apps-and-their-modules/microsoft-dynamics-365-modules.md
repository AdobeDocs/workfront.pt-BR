---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: conector
navigation-topic: apps-and-their-modules
title: Módulos do Microsoft Dynamics 365
description: Em um [!DNL Adobe Workfront Fusion] você pode automatizar fluxos de trabalho que usam o Microsoft Dynamics 365, bem como conectá-lo a vários aplicativos e serviços de terceiros.
author: Becky
feature: Workfront Fusion
exl-id: 116df088-20a7-40a8-8880-9f422dc37632
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1541'
ht-degree: 0%

---

# [!DNL Microsoft Dynamics 365 modules]

Em um [!DNL Adobe Workfront Fusion] , é possível automatizar workflows que usam [!DNL Microsoft Dynamics 365], bem como conectá-lo a vários aplicativos e serviços de terceiros.

>[!NOTE]
>
>O [!DNL Microsoft Dynamics 365] o conector não é compatível [!DNL Dynamics Finance and Operations].

Se precisar de instruções para criar um cenário, consulte [Crie um cenário em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

Para obter informações sobre módulos, consulte [Módulos em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] para automação e integração de trabalho] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produto</td> 
   <td>Sua organização deve comprar [!DNL Adobe Workfront Fusion] bem como [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo.</td> 
  </tr>
 </tbody> 
</table>

Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com seu [!DNL Workfront] administrador.

Para obter informações sobre [!DNL Adobe Workfront Fusion] licenças, consulte [[!DNL Adobe Workfront Fusion] licenças](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Pré-requisitos

Para usar [!DNL Microsoft Dynamics] 365, você deve ter um [!DNL Microsoft Dynamics 365] conta.

## Conecte o Microsoft Dynamics 365 ao Workfront Fusion

Você pode criar uma conexão com o [!DNL Microsoft Dynamics 365] conta diretamente de dentro de uma [!DNL Microsoft Dynamics 365] módulo.

1. Em qualquer [!DNL Microsoft Dynamics 365] módulo, clique em **[!UICONTROL Adicionar]** ao lado do [!UICONTROL Conexão] campo.
1. Digite um nome para a conexão.
1. No **[!UICONTROL Recurso]** , insira o endereço de sua [!DNL Dynamics 365] conta, sem `https://`.
1. Clique em **[!UICONTROL Continuar]** para criar a conexão e retornar ao módulo .

>[!NOTE]
>
>Ao registrar [!DNL Workfront Fusion] em seu [!DNL Microsoft Azure] portal, use o seguinte URI de redirecionamento:
>
>* `https://app.workfrontfusion.com/oauth/cb/workfront-microsoft-dynamics2`



## [!DNL Microsoft Dynamics 365] módulos e seus campos

Ao configurar [!DNL Microsoft Dynamics 365] módulos, [!DNL Workfront Fusion] exibe os campos listados abaixo. Junto com esses, [!DNL Microsoft Dynamics 365] podem ser exibidos, dependendo de fatores como seu nível de acesso no aplicativo ou serviço. Um título em negrito em um módulo indica um campo obrigatório.

Se o botão de mapa for exibido acima de um campo ou função, é possível usá-lo para definir variáveis e funções para esse campo. Para obter mais informações, consulte [Mapear informações de um módulo para outro no [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [[!UICONTROL Registros de monitoramento (agendados)]](#watch-records-scheduled)
* [[!UICONTROL Registros de monitoramento (Tempo real)]](#watch-records-real-time)
* [[!UICONTROL Criar registro]](#create-record)
* [[!UICONTROL Faça uma chamada de API]](#make-an-api-call)
* [[!UICONTROL Excluir registro]](#delete-record)
* [[!UICONTROL Ler registros]](#read-records)
* [[!UICONTROL Atualizar registro]](#update-record)
* [[!UICONTROL Pesquisar registros]](#search-records)

### [!UICONTROL Registros de monitoramento (agendados)]

Esse módulo de acionador agendado executa um cenário quando um registro no objeto especificado por você é criado ou atualizado após a última execução agendada em [!DNL Dynamics 365].

A saída do módulo indica se o registro encontrado é novo ou atualizado (se ele foi adicionado e atualizado no período, ele é marcado como novo). Você pode mapear essas informações em módulos subsequentes do cenário.

Isso acontece em um intervalo agendado regularmente e especificado por você.

Ao configurar esse módulo, os seguintes campos são exibidos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
  <td> <p>Para obter instruções sobre como conectar seu [!DNL Microsoft Dynamics 365] para [!DNL Workfront Fusion], consulte <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">Connect [!DNL Microsoft Dynamics 365] para [!DNL Workfront Fusion]</a> neste artigo. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Include]</td> 
   <td>Selecione se deseja que o módulo assista <strong>[!UICONTROL Somente novos registros]</strong>, <strong>[!UICONTROL Somente registros atualizados]</strong>ou <strong>[!UICONTROL Novos registros e todas as alterações]</strong>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de entidade]</td> 
   <td>Escolha o tipo de registro [!UICONTROL Microsoft Dynamics 365] que deseja que o cenário assista.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Saídas]</td> 
   <td> <p>Selecione as informações que deseja incluir no pacote de saída deste módulo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Máximo de registros]</td> 
   <td> <p>Insira ou mapeie o número máximo de registros que você deseja que o módulo retorne durante cada ciclo de execução de cenário.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Registros de monitoramento (Tempo real)]

Esse módulo de acionador instantâneo executa um cenário quando um registro (objeto) especificado por você é criado ou atualizado em [!DNL Dynamics 365].

Um webhook é necessário neste módulo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td> <p>Selecione o webhook que deseja usar para este módulo. </p> <p>Para adicionar um novo webhook:</p> 
    <ol> 
     <li value="1"> <p>Clique em <strong>[!UICONTROL Adicionar]</strong> à direita do campo Webhook</p> </li> 
     <li value="2"> <p>No <strong>[!UICONTROL Webhook]</strong> campo de nome, digite um nome descritivo para o webhook.</p> </li> 
     <li value="3"> <p>No <strong>[!UICONTROL Connection]</strong> , selecione a Conexão que deseja usar selecionada</p> <p>Para obter instruções sobre como conectar seu [!DNL Microsoft Dynamics 365] para [!DNL Workfront Fusion], consulte <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">Connect [!DNL Microsoft Dynamics 365] para [!DNL Workfront Fusion]</a> neste artigo. </p> </li> 
     <li value="4"> <p>Clique em <strong>[!UICONTROL Salvar]</strong> para salvar seu webhook e retornar ao módulo .</p> </li> 
    </ol> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Criar registro]

Esse módulo de ação cria uma entidade, como um compromisso ou tarefa.

Especifique as informações sobre a entidade que deseja criar.

O módulo retorna a ID da nova entidade e quaisquer campos associados, juntamente com quaisquer campos e valores personalizados que a conexão acessa. Você pode mapear essas informações em módulos subsequentes do cenário.

Ao configurar esse módulo, os seguintes campos são exibidos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Microsoft Dynamics 365] para [!DNL Workfront Fusion], consulte <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">Connect [!DNL Microsoft Dynamics 365] para [!DNL Workfront Fusion]</a> neste artigo. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de entidade]</td> 
   <td>Selecione o tipo de entidade que deseja que o módulo crie.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Campos de propriedade]</td> 
   <td>Nesses campos, insira o valor que você deseja que o item de trabalho tenha para uma determinada propriedade. Os campos disponíveis dependem do tipo de entidade.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Faça uma chamada de API]

Esse módulo de ação permite que você faça uma chamada autenticada personalizada para o [!DNL Microsoft Dynamics 365] API. Dessa forma, você pode criar uma automação de fluxo de dados que não pode ser realizada pela outra [!DNL Microsoft Dynamics 365] módulos.

O módulo retorna informações sobre o código de status, cabeçalhos e corpo. Você pode mapear essas informações em módulos subsequentes do cenário.

Para saber mais, consulte a [!DNL Microsoft] documentação sobre o uso da variável [!DNL Dynamics 365 Customer Engagement Web API].

Ao configurar esse módulo, os seguintes campos são exibidos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
  <td> <p>Para obter instruções sobre como conectar seu [!DNL Microsoft Dynamics 365] para [!DNL Workfront Fusion], consulte <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">Connect [!DNL Microsoft Dynamics 365] para [!DNL Workfront Fusion]</a> neste artigo. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td> <p>Insira um caminho relativo a <code>&lt;Instance URL>/api/data/v9.1/</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Método]</td> 
   <td> <p>Selecione o método de solicitação HTTP que você precisa configurar a chamada da API. Para obter mais informações, consulte <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">Métodos de solicitação HTTP em [!DNL Adobe Workfront Fusion]</a>.</p> <p>Para obter mais informações</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cabeçalhos]</td> 
   <td> <p>Adicione os cabeçalhos da solicitação no formato de um objeto JSON padrão.</p> <p>Por exemplo, <code>{"Content-type":"application/json"}</code></p> <p>[!DNL Workfront Fusion] adiciona os cabeçalhos de autorização para você.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sequência de consulta]</td> 
   <td> <p>Adicione a query para a chamada de API no formato de um objeto JSON padrão.</p> <p>Por exemplo: <code>{"name":"something-urgent"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Corpo]</td> 
   <td> <p>Adicione o conteúdo do corpo para a chamada da API no formato de um objeto JSON padrão.</p> <p>Nota:  <p>Ao usar declarações condicionais como <code>if</code> no JSON, coloque as aspas fora da declaração condicional.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Excluir registro]

Esse módulo de ação exclui uma entidade.

Especifique a ID da entidade.

O módulo retorna a ID da entidade e quaisquer campos associados, juntamente com quaisquer campos e valores personalizados que a conexão acessa. Você pode mapear essas informações em módulos subsequentes do cenário.

Ao configurar esse módulo, os seguintes campos são exibidos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
  <td> <p>Para obter instruções sobre como conectar seu [!DNL Microsoft Dynamics 365] para [!DNL Workfront Fusion], consulte <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">Connect [!DNL Microsoft Dynamics 365] para [!DNL Workfront Fusion]</a> neste artigo. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de entidade]</td> 
   <td> <p>Selecione o tipo de entidade que deseja que o módulo exclua.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td> <p>Insira ou mapeie a [!DNL Microsoft Dynamics 365] ID do registro que você deseja que o módulo exclua.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Ler registros]

Este módulo de ação lê dados de uma única entidade em [!DNL Microsoft Dynamics 365].

Especifique a ID da entidade.

O módulo retorna a ID da entidade e quaisquer campos associados, juntamente com quaisquer campos e valores personalizados que a conexão acessa. Você pode mapear essas informações em módulos subsequentes do cenário.

Ao configurar esse módulo, os seguintes campos são exibidos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
  <td> <p>Para obter instruções sobre como conectar seu [!DNL Microsoft Dynamics 365] para [!DNL Workfront Fusion], consulte <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">Connect [!DNL Microsoft Dynamics 365] para [!DNL Workfront Fusion]</a> neste artigo. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de entidade]</td> 
   <td>Selecione o tipo de entidade que deseja que o módulo leia.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Saídas]</td> 
   <td> <p>Selecione as informações que deseja incluir no pacote de saída deste módulo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>Insira ou mapeie a [!DNL Microsoft Dynamics 365] ID do registro que você deseja que o módulo leia.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Atualizar registro]

Este módulo de ação atualiza uma entidade.

Especifique a ID da entidade.

O módulo retorna a ID do registro atualizado e quaisquer campos associados, juntamente com quaisquer campos e valores personalizados que a conexão acessa. Você pode mapear essas informações em módulos subsequentes do cenário.

Ao configurar esse módulo, os seguintes campos são exibidos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
  <td> <p>Para obter instruções sobre como conectar seu [!DNL Microsoft Dynamics 365] para [!DNL Workfront Fusion], consulte <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">Connect [!DNL Microsoft Dynamics 365] para [!DNL Workfront Fusion]</a> neste artigo. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Tipo de entidade]</td> 
   <td>Selecione o tipo de entidade que deseja que o módulo atualize.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Campos de propriedade]</td> 
   <td>Nesses campos, insira o valor que você deseja que o item de trabalho tenha para uma determinada propriedade. Os campos disponíveis dependem do tipo de entidade.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>Insira ou mapeie a [!DNL Microsoft Dynamics] 365 ID do registro que você deseja que o módulo atualize.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Pesquisar registros]

Este módulo de pesquisa procura registros em um objeto em [!DNL Microsoft Dynamics 365] que correspondem à consulta de pesquisa especificada. Você pode mapear essas informações em módulos subsequentes do cenário.

Ao configurar esse módulo, os seguintes campos são exibidos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
  <td> <p>Para obter instruções sobre como conectar seu [!DNL Microsoft Dynamics 365] para [!DNL Workfront Fusion], consulte <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">Connect [!DNL Microsoft Dynamics 365] para [!DNL Workfront Fusion]</a> neste artigo. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de entidade]</td> 
   <td>Selecione o tipo de entidade que deseja que o módulo atualize.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filtros]</td> 
   <td> <p>Selecione o filtro que deseja usar para essa pesquisa.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Filtros padrão]</strong> </p> <p>Configure o filtro selecionando um campo e um operador e digitando ou mapeando o valor que deseja pesquisar. Você pode usar regras AND ou OR no filtro.</p> </li> 
     <li> <p><strong>[!UICONTROL Funções de consulta]</strong> </p> <p>Insira o [!DNL Dynamics 365] função de consulta da API da Web que você deseja usar para pesquisar. </p> <p>Para obter mais informações sobre funções de consulta, consulte <a href="https://docs.microsoft.com/en-us/dynamics365/customer-engagement/web-api/queryfunctions?view=dynamics-ce-odata-9">Referência da função de consulta da API da Web</a> no [!DNL Microsoft] documentação.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Classificar]</td> 
   <td> <p>Especifique a ordem em que os itens são retornados. Você pode adicionar vários tipos.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Campo]</strong> </p> <p>Especifique o campo pelo qual deseja classificar os resultados.</p> </li> 
     <li> <p><strong>[!UICONTROL Direção]</strong> </p> <p>Especifique a direção da classificação (crescente ou decrescente).</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Máximo de registros]</td> 
   <td> <p>Insira ou mapeie o número máximo de registros que você deseja que o módulo retorne durante cada ciclo de execução de cenário.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Saídas]</td> 
   <td> <p>Selecione as informações que deseja incluir no pacote de saída deste módulo.</p> </td> 
  </tr> 
 </tbody> 
</table>
