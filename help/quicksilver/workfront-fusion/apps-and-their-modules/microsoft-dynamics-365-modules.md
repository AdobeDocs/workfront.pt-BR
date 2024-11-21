---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: conector
navigation-topic: apps-and-their-modules
title: Módulos do Microsoft Dynamics 365
description: Em um cenário  [!DNL Adobe Workfront Fusion] , você pode automatizar fluxos de trabalho que usam o Microsoft Dynamics 365, bem como conectá-lo a vários aplicativos e serviços de terceiros.
author: Becky
feature: Workfront Fusion
exl-id: 116df088-20a7-40a8-8880-9f422dc37632
source-git-commit: 55485da1ea650121b5537a3f19d8102623ed4f43
workflow-type: tm+mt
source-wordcount: '1724'
ht-degree: 0%

---

# [!DNL Microsoft Dynamics 365 modules]

Em um cenário [!DNL Adobe Workfront Fusion], você pode automatizar fluxos de trabalho que usam [!DNL Microsoft Dynamics 365], bem como conectá-los a vários aplicativos e serviços de terceiros.

>[!NOTE]
>
>O conector [!DNL Microsoft Dynamics 365] não dá suporte a [!DNL Dynamics Finance and Operations].

Se você precisar de instruções sobre como criar um cenário, consulte [Criar um cenário [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

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
   <td>
   <p>Requisito de licença atual: nenhum requisito de licença [!DNL Workfront Fusion].</p>
   <p>Ou</p>
   <p>Requisito de licença herdada: [!UICONTROL [!DNL Workfront Fusion] para Automação e Integração do Trabalho] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produto</td> 
   <td>
   <p>Requisito atual do produto: se você tiver o plano [!UICONTROL Select] ou [!UICONTROL Prime] [!DNL Adobe Workfront], sua organização deve comprar [!DNL Adobe Workfront Fusion] e [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo. [!DNL Workfront Fusion] está incluído no plano [!DNL Workfront] do [!UICONTROL Ultimate].</p>
   <p>Ou</p>
   <p>Requisito de produto herdado: sua organização deve comprar o [!DNL Adobe Workfront Fusion] e o [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo.</p>
   </td> 
  </tr>
 </tbody> 
</table>

Para saber que plano, tipo de licença ou acesso você tem, contate o administrador do [!DNL Workfront].

Para obter informações sobre [!DNL Adobe Workfront Fusion] licenças, consulte [[!DNL Adobe Workfront Fusion] licenças](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Pré-requisitos

Para usar o [!DNL Microsoft Dynamics] 365, você deve ter uma conta [!DNL Microsoft Dynamics 365].

## Conectar o Microsoft Dynamics 365 ao Workfront Fusion

Você pode criar uma conexão com sua conta do [!DNL Microsoft Dynamics 365] diretamente de dentro de um módulo [!DNL Microsoft Dynamics 365].

>[!NOTE]
>
>Alguns aplicativos do Microsoft usam a mesma conexão, que está vinculada a permissões de usuário individuais. Portanto, ao criar uma conexão, a tela de consentimento de permissões exibe todas as permissões que foram concedidas anteriormente à conexão deste usuário, além de todas as novas permissões necessárias para o aplicativo atual.
>
>Por exemplo, se um usuário tiver permissões de &quot;Tabela de leitura&quot; concedidas por meio do conector do Excel e criar uma conexão no conector do Outlook para ler emails, a tela de consentimento de permissões mostrará a permissão &quot;Tabela de leitura&quot; já concedida e a permissão &quot;Gravar email&quot; recém-necessária.

1. Em qualquer módulo [!DNL Microsoft Dynamics 365], clique em **[!UICONTROL Adicionar]** ao lado do campo [!UICONTROL Conexão].
1. Insira um nome para a conexão.
1. No campo **[!UICONTROL Recurso]**, digite o endereço da sua conta do [!DNL Dynamics 365], sem `https://`.
1. Clique em **[!UICONTROL Continuar]** para criar a conexão e voltar para o módulo.

>[!NOTE]
>
>Ao registrar [!DNL Workfront Fusion] no portal [!DNL Microsoft Azure], use o seguinte URI de redirecionamento:
>
>* `https://app.workfrontfusion.com/oauth/cb/workfront-microsoft-dynamics2`


## [!DNL Microsoft Dynamics 365] módulos e seus campos

Ao configurar módulos do [!DNL Microsoft Dynamics 365], o [!DNL Workfront Fusion] exibe os campos listados abaixo. Junto com esses, campos [!DNL Microsoft Dynamics 365] adicionais podem ser exibidos, dependendo de fatores como seu nível de acesso no aplicativo ou serviço. Um título em negrito em um módulo indica um campo obrigatório.

Se você vir o botão de mapa acima de um campo ou função, poderá usá-lo para definir variáveis e funções para esse campo. Para obter mais informações, consulte [Mapear informações de um módulo para outro em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [[!UICONTROL Registros de Inspeção (Agendados)]](#watch-records-scheduled)
* [[!UICONTROL Registros de Inspeção (Tempo Real)]](#watch-records-real-time)
* [[!UICONTROL Criar Registro]](#create-record)
* [[!UICONTROL Fazer uma chamada de API]](#make-an-api-call)
* [[!UICONTROL Excluir Registro]](#delete-record)
* [[!UICONTROL Ler Registros]](#read-records)
* [[!UICONTROL Atualizar Registro]](#update-record)
* [[!UICONTROL Pesquisar Registros]](#search-records)

### [!UICONTROL Registros de Inspeção (Agendados)]

Este módulo de gatilho agendado executa um cenário quando um registro no objeto especificado é criado ou atualizado após a última execução agendada em [!DNL Dynamics 365].

A saída do módulo indica se o registro encontrado é novo ou atualizado (se foi adicionado e atualizado no período, é marcado como novo). Você pode mapear essas informações em módulos subsequentes no cenário.

Isso acontece em um intervalo programado regularmente especificado por você.

Ao configurar esse módulo, os campos a seguir são exibidos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão]</td> 
  <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Microsoft Dynamics 365] ao [!DNL Workfront Fusion], consulte <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Microsoft Dynamics 365] ao [!DNL Workfront Fusion]</a> neste artigo. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Incluir]</td> 
   <td>Selecione se deseja que o módulo assista <strong>[!UICONTROL Somente novos registros]</strong>, <strong>[!UICONTROL Somente registros atualizados]</strong> ou <strong>[!UICONTROL Novos registros e todas as alterações]</strong>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de Entidade]</td> 
   <td>Escolha o tipo de registro [!UICONTROL Microsoft Dynamics 365] que você deseja que o cenário assista.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Saídas]</td> 
   <td> <p>Selecione as informações que deseja incluir no pacote de saída deste módulo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Máximo de Registros]</td> 
   <td> <p>Insira ou mapeie o número máximo de registros que deseja que o módulo retorne durante cada ciclo de execução de cenário.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Registros de Inspeção (Tempo Real)]

Esse módulo de acionador instantâneo executa um cenário quando um registro (objeto) especificado é criado ou atualizado em [!DNL Dynamics 365].

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
     <li value="2"> <p>No campo de nome <strong>[!UICONTROL Webhook]</strong>, digite um nome descritivo para o webhook.</p> </li> 
     <li value="3"> <p>No campo <strong>[!UICONTROL Conexão]</strong>, selecione a Conexão que deseja usar selecionada</p> <p>Para obter instruções sobre como conectar sua conta do [!DNL Microsoft Dynamics 365] ao [!DNL Workfront Fusion], consulte <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Microsoft Dynamics 365] ao [!DNL Workfront Fusion]</a> neste artigo. </p> </li> 
     <li value="4"> <p>Clique em <strong>[!UICONTROL Salvar]</strong> para salvar seu webhook e retornar ao módulo.</p> </li> 
    </ol> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Criar Registro]

Este módulo de ação cria uma entidade, como um compromisso ou tarefa.

Especifique informações sobre a entidade que deseja criar.

O módulo retorna a ID da nova entidade e quaisquer campos associados, juntamente com quaisquer campos e valores personalizados que a conexão acesse. Você pode mapear essas informações em módulos subsequentes no cenário.

Ao configurar esse módulo, os campos a seguir são exibidos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão]</td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Microsoft Dynamics 365] ao [!DNL Workfront Fusion], consulte <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Microsoft Dynamics 365] ao [!DNL Workfront Fusion]</a> neste artigo. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de Entidade]</td> 
   <td>Selecione o tipo de entidade que você deseja que o módulo crie.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Selecionar campos para mapear]</td> 
   <td>Selecione os campos para os quais deseja incluir valores quando o registro for criado. Os campos disponíveis dependem do tipo de entidade.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Campos de propriedade]</td> 
   <td> Esses são os campos selecionados. Insira o valor que você deseja que o registro tenha para uma determinada propriedade. </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Fazer uma chamada de API]

Este módulo de ação permite fazer uma chamada autenticada personalizada para a API [!DNL Microsoft Dynamics 365]. Dessa forma, você pode criar uma automação de fluxo de dados que não pode ser realizada pelos outros módulos do [!DNL Microsoft Dynamics 365].

O módulo retorna informações sobre o código de status, cabeçalhos e corpo. Você pode mapear essas informações em módulos subsequentes no cenário.

Para saber mais, consulte a documentação do [!DNL Microsoft] sobre o uso do [!DNL Dynamics 365 Customer Engagement Web API].

Ao configurar esse módulo, os campos a seguir são exibidos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão]</td> 
  <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Microsoft Dynamics 365] ao [!DNL Workfront Fusion], consulte <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Microsoft Dynamics 365] ao [!DNL Workfront Fusion]</a> neste artigo. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td> <p>Insira um caminho relativo para <code>&lt;Instance URL>/api/data/v9.1/</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Método]</td> 
   <td> <p>Selecione o método de solicitação HTTP necessário para configurar a chamada de API. Para obter mais informações, consulte <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">Métodos de solicitação HTTP em [!DNL Adobe Workfront Fusion]</a>.</p> <p>Para obter mais informações em</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cabeçalhos]</td> 
   <td> <p>Adicione os cabeçalhos da solicitação no formulário de um objeto JSON padrão.</p> <p>Por exemplo, <code>{"Content-type":"application/json"}</code></p> <p>[!DNL Workfront Fusion] O adiciona os cabeçalhos de autorização para você.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cadeia de Consulta]</td> 
   <td> <p>Adicione a consulta da chamada à API na forma de um objeto JSON padrão.</p> <p>Por exemplo: <code>{"name":"something-urgent"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Corpo]</td> 
   <td> <p>Adicione o conteúdo do corpo para a chamada à API na forma de um objeto JSON padrão.</p> <p>Nota:  <p>Ao usar instruções condicionais como <code>if</code> em seu JSON, coloque as aspas fora da instrução condicional.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Excluir Registro]

Este módulo de ação exclui uma entidade.

Você especifica a ID da entidade.

O módulo retorna a ID da entidade e quaisquer campos associados, juntamente com quaisquer campos e valores personalizados que a conexão acessa. Você pode mapear essas informações em módulos subsequentes no cenário.

Ao configurar esse módulo, os campos a seguir são exibidos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão]</td> 
  <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Microsoft Dynamics 365] ao [!DNL Workfront Fusion], consulte <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Microsoft Dynamics 365] ao [!DNL Workfront Fusion]</a> neste artigo. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de Entidade]</td> 
   <td> <p>Selecione o tipo de entidade que você deseja que o módulo exclua.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td> <p>Insira ou mapeie a ID [!DNL Microsoft Dynamics 365] exclusiva do registro que você deseja que o módulo exclua.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Ler Registros]

Este módulo de ação lê os dados de uma única entidade em [!DNL Microsoft Dynamics 365].

Você especifica a ID da entidade.

O módulo retorna a ID da entidade e quaisquer campos associados, juntamente com quaisquer campos e valores personalizados que a conexão acessa. Você pode mapear essas informações em módulos subsequentes no cenário.

Ao configurar esse módulo, os campos a seguir são exibidos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão]</td> 
  <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Microsoft Dynamics 365] ao [!DNL Workfront Fusion], consulte <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Microsoft Dynamics 365] ao [!DNL Workfront Fusion]</a> neste artigo. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de Entidade]</td> 
   <td>Selecione o tipo de entidade que você deseja que o módulo leia.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Saídas]</td> 
   <td> <p>Selecione as informações que deseja incluir no pacote de saída deste módulo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>Insira ou mapeie a ID [!DNL Microsoft Dynamics 365] exclusiva do registro que você deseja que o módulo leia.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Atualizar Registro]

Este módulo de ação atualiza uma entidade.

Você especifica a ID da entidade.

O módulo retorna a ID do registro atualizado e quaisquer campos associados, juntamente com quaisquer campos e valores personalizados que a conexão acessa. Você pode mapear essas informações em módulos subsequentes no cenário.

Ao configurar esse módulo, os campos a seguir são exibidos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão]</td> 
  <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Microsoft Dynamics 365] ao [!DNL Workfront Fusion], consulte <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Microsoft Dynamics 365] ao [!DNL Workfront Fusion]</a> neste artigo. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Tipo de Entidade]</td> 
   <td>Selecione o tipo de entidade que você deseja que o módulo atualize.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Selecionar campos para mapear]</td> 
   <td>Selecione os campos para os quais deseja incluir valores quando o registro for criado. Os campos disponíveis dependem do tipo de entidade.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Campos de propriedade]</td> 
   <td>Esses são os campos que você selecionou. Insira o valor que você deseja que o registro tenha para uma determinada propriedade.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>Insira ou mapeie a ID exclusiva [!DNL Microsoft Dynamics] 365 do registro que você deseja que o módulo atualize.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Pesquisar Registros]

Este módulo de pesquisa procura registros em um objeto em [!DNL Microsoft Dynamics 365] que correspondam à consulta de pesquisa especificada. Você pode mapear essas informações em módulos subsequentes no cenário.

Ao configurar esse módulo, os campos a seguir são exibidos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão]</td> 
  <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Microsoft Dynamics 365] ao [!DNL Workfront Fusion], consulte <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Microsoft Dynamics 365] ao [!DNL Workfront Fusion]</a> neste artigo. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de Entidade]</td> 
   <td>Selecione o tipo de entidade que você deseja que o módulo atualize.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filtros]</td> 
   <td> <p>Selecione o filtro que deseja usar para esta pesquisa.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Filtros Padrão]</strong> </p> <p>Configure o filtro selecionando um campo e operador e inserindo ou mapeando o valor que deseja pesquisar. Você pode usar as regras AND ou OR para filtrar.</p> </li> 
     <li> <p><strong>[!UICONTROL Consultar Funções]</strong> </p> <p>Insira a função de consulta da API da Web [!DNL Dynamics 365] que você deseja usar para pesquisar. </p> <p>Para obter mais informações sobre funções de consulta, consulte a <a href="https://docs.microsoft.com/en-us/dynamics365/customer-engagement/web-api/queryfunctions?view=dynamics-ce-odata-9">Referência da Função de Consulta da API da Web</a> na documentação [!DNL Microsoft].</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Classificar]</td> 
   <td> <p>Especificar a ordem de devolução dos itens. É possível adicionar várias classificações.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Campo]</strong> </p> <p>Especifique o campo pelo qual deseja classificar os resultados.</p> </li> 
     <li> <p><strong>[!UICONTROL Direção]</strong> </p> <p>Especifique a direção da classificação (crescente ou decrescente).</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Máximo de Registros]</td> 
   <td> <p>Insira ou mapeie o número máximo de registros que deseja que o módulo retorne durante cada ciclo de execução de cenário.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Saídas]</td> 
   <td> <p>Selecione as informações que deseja incluir no pacote de saída deste módulo.</p> </td> 
  </tr> 
 </tbody> 
</table>
