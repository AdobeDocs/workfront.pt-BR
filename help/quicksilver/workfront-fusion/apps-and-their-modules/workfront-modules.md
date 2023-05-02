---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: conector
navigation-topic: apps-and-their-modules
title: Módulos Adobe Workfront
description: Você pode usar o conector Adobe Workfront Fusion Adobe Workfront para automatizar seus processos no Workfront. Se você tiver uma licença Workfront Fusion for Work Automation and Integration , também poderá usá-la para se conectar a aplicativos e serviços de terceiros.
author: Becky
feature: Workfront Fusion, Workfront Integrations and Apps
exl-id: b84d2d41-a983-4ea3-b331-0302bfcf8a2b
source-git-commit: 852d6acb4363e1926c20a64ada381a114bfe11ee
workflow-type: tm+mt
source-wordcount: '5345'
ht-degree: 3%

---

# [!DNL Adobe Workfront] módulos

Você pode usar o [!DNL Adobe Workfront Fusion] [!DNL Adobe Workfront] para automatizar seus processos no [!DNL Workfront]. Se você tiver uma [!UICONTROL [!DNL Workfront Fusion] para automação e integração de trabalho] , você também pode usá-lo para se conectar a aplicativos e serviços de terceiros.

O [!DNL Workfront] O conector não conta em relação ao número de aplicativos ativos disponíveis para sua organização. Todos os cenários, mesmo que eles usem somente a variável [!DNL Workfront] aplicativo, faça a contagem em relação à contagem total de cenários de sua organização.

Para obter mais informações sobre os aplicativos e cenários disponíveis em sua organização, consulte [Organizações](../../workfront-fusion/organizations/organizations-and-teams.md#organiza2) em [[!DNL Adobe Workfront Fusion] organizações e equipes](../../workfront-fusion/organizations/organizations-and-teams.md).

Se precisar de instruções para criar um cenário, consulte [Crie um cenário em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md). Para obter informações sobre módulos, consulte [Módulos em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] para automação e integração de trabalho] </p>  <p>[!UICONTROL [!DNL Workfront Fusion] para Automação de Trabalho]</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produto</td> 
   <td>Sua organização deve comprar [!DNL Adobe Workfront Fusion] bem como [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo.</td> 
  </tr> 
 </tbody> 
</table>


Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com seu [!DNL Workfront] administrador.

Para obter informações sobre [!DNL Adobe Workfront Fusion] licenças, consulte [[!DNL Adobe Workfront Fusion] licenças](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Connect [!DNL Workfront] para [!DNL Workfront Fusion]

O [!DNL Workfront] O conector usa o OAuth 2.0 para se conectar [!DNL Workfront].

Você pode criar uma conexão com o [!DNL Workfront] conta diretamente de dentro de uma [!DNL Workfront Fusion] módulo.

1. Em qualquer [!DNL Workfront] módulo do aplicativo, clique em **[!UICONTROL Adicionar]** ao lado do [!UICONTROL Conexão] caixa.
1. Insira o nome da sua instância no URL. Exemplo: `https://<your instance>.my.workfront.com`.
1. Clique em **[!UICONTROL Próximo]**.
1. Clique em **[!UICONTROL Logon do SAML]** para criar a conexão e retornar ao módulo .

   Ou

   Digite seu nome de usuário e senha e clique em **[!UICONTROL Fazer logon]** para criar a conexão e retornar ao módulo .

   >[!NOTE]
   >
   >* Se você não vir um botão de logon SAML, sua organização não ativou o Logon único (SSO). Você pode fazer logon com seu Nome de usuário e Senha.
      >   
      >   Para obter mais informações sobre SSO, consulte [Visão geral do logon único [!DNL Adobe Workfront]](../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md)
   >   
   >* Conexões OAuth 2.0 para o [!DNL Workfront] A API não depende mais das chaves da API.


## [!DNL Workfront] módulos e seus campos

Ao configurar [!DNL Workfront] módulos, [!DNL Workfront Fusion] exibe os campos listados abaixo. Junto com esses, [!DNL Workfront] podem ser exibidos, dependendo de fatores como seu nível de acesso no aplicativo ou serviço. Um título em negrito em um módulo indica um campo obrigatório.

Se o botão de mapa for exibido acima de um campo ou função, é possível usá-lo para definir variáveis e funções para esse campo. Para obter mais informações, consulte [Mapear informações de um módulo para outro no [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Triggers](#triggers)
* [Ações](#actions)
* [Pesquisas](#searches)

### Triggers

<!--
* [Watch Events](#watch-events) 
* [Watch Record](#watch-record) 
* [Watch Field](#watch-field)
-->

+++ **[!UICONTROL Eventos de observação]**

Esse módulo de acionador executa um cenário em tempo real quando objetos de um tipo específico são adicionados, atualizados ou excluídos no Workfront

O módulo retorna quaisquer campos padrão associados ao registro, juntamente com quaisquer campos e valores personalizados que a conexão acessa. Você pode mapear essas informações em módulos subsequentes do cenário.

1. Clique em **[!UICONTROL Adicionar]** à direita do **Webhook** caixa.

1. Configure o webhook no **[!UICONTROL Adicionar um gancho]** que é exibida.

   Ao configurar esse módulo, os seguintes campos são exibidos.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td>[!UICONTROL Nome do Webhook]</td> 
      <td>(Opcional) Digite um novo nome para o webhook</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Connection]</td> 
      <td> <p>Para obter instruções sobre como conectar seu [!DNL Workfront] aplicativo para [!DNL Workfront Fusion], consulte <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Connect [!DNL Workfront] para [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Tipo de registro]</td> 
      <td>Selecione o tipo de [!DNL Workfront] registre que você deseja que o módulo assista.</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Estado]</td> 
      <td>Selecione se deseja observar o estado antigo ou o novo.<ul><li><p><b>[!UICONTROL Novo estado]</b></p><p>Acionar um cenário quando o registro for alterado <b>para</b> um determinado valor.</p><p>Por exemplo, se o estado estiver definido como [!UICONTROL Novo Estado] e o filtro estiver definido como [!UICONTROL Status] [!UICONTROL Igual] [!UICONTROL Em Andamento], o webhook acionará um cenário quando o [!UICONTROL Status] for alterado para [!UICONTROL Em Andamento], independentemente do status anterior. </p></li><li><p><b>[!UICONTROL Estado antigo]</b></p><p>Acionar um cenário quando o registro for alterado <b>from</b> um determinado valor.</p><p>Por exemplo, se o estado estiver definido como [!UICONTROL Estado Antigo] e o filtro estiver definido como [!UICONTROL Status] [!UICONTROL Igual] [!UICONTROL Em Andamento], o webhook acionará um cenário quando um [!UICONTROL Status] que está atualmente [!UICONTROL Em Andamento] for alterado para outro status. </p></li></ul></td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td> <p>[!UICONTROL Events filters]</p> </td> 
      <td> <p>Você pode definir filtros para monitorar somente registros que atendam aos critérios selecionados.</p> <p>Para cada filtro, insira o campo que o filtro deve avaliar, o operador e o valor que você deseja que o filtro permita. Você pode usar mais de um filtro adicionando regras AND.</p> <p>Observação: Não é possível editar filtros em [!DNL Workfront] webhooks. Para configurar filtros diferentes para [!DNL Workfront] assinaturas de evento, remova o webhook atual e crie um novo.</p> <p>Para obter mais informações sobre filtros de evento, consulte <a href="#event-subscription-filters-in-the-workfront-watch-events-modules" class="MCXref xref">Os filtros de assinatura de evento na [!DNL Workfront] &gt; [!UICONTROL Eventos de observação] módulos</a> neste artigo.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td>Excluir eventos feitos por esta conexão</td> 
      <td>Ative essa opção para excluir eventos criados ou atualizados usando o mesmo conector que esse módulo de acionador usa. Isso pode evitar situações em que um cenário pode se acionar, fazendo com que ele se repita em um loop infinito.</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Origem do registro]</td> 
      <td> <p>Escolha se deseja que o cenário seja monitorado <strong>[!UICONTROL Novos registros somente]</strong>, <strong>[!UICONTROL Somente Registros Atualizados]</strong>, <strong>[!UICONTROL Registros novos e atualizados]</strong>ou <strong>[!DNL Deleted Records Only]</strong>.</p> <p>Observação: Se você escolher <strong>[!UICONTROL Registros novos e atualizados]</strong>, a criação do webhook cria 2 assinaturas de evento (para o mesmo endereço do webhook).</p> </td> 
     </tr> 
    </tbody> 
   </table>

Após a criação do webhook, você pode exibir o endereço do endpoint para o qual os eventos são enviados.

Para obter mais informações, consulte a seção [Exemplos de cargas de evento](../../wf-api/general/event-subs-api.md#examples-of-event-payloads) no [!DNL Workfront] Artigo de ajuda [API de assinatura de evento](../../wf-api/general/event-subs-api.md).

Veja uma lista de [!DNL Workfront] tipos de objetos para os quais você pode usar este módulo em [[!DNL Workfront] object types available for each [!DNL Workfront] módulo](#workfront-object-types-available-for-each-workfront-module).

+++

+++ **[!UICONTROL Campo de observação]**

Esse módulo de acionador executa um cenário quando um campo especificado é atualizado. O módulo retorna o valor antigo e o novo do campo especificado. Você pode mapear essas informações em módulos subsequentes do cenário.

Ao configurar esse módulo, os seguintes campos são exibidos.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Workfront] aplicativo para [!DNL Workfront Fusion], consulte <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Connect [!DNL Workfront] para [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipo de registro]</td> 
   <td> <p>Selecione o tipo de [!DNL Workfront] registre que você deseja que o módulo assista.</p> <p>Por exemplo, selecione [!UICONTROL Tarefa] se desejar começar a executar o cenário sempre que um campo de registro for atualizado em uma tarefa.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Campo]</td> 
   <td>Selecione o campo que o módulo deve procurar por atualizações. Esses campos refletem os campos que [!DNL Workfront] O administrador configurou para rastreamento.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Saídas]</td> 
   <td>Selecione as informações que deseja incluir no pacote de saída deste módulo.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Limite]</td> 
   <td> <p>Insira ou mapeie o número máximo de registros que você deseja que o módulo retorne durante cada ciclo de execução de cenário.</p> </td> 
  </tr> 
 </tbody> 
</table>

Veja uma lista de [!DNL Workfront] tipos de objetos para os quais você pode usar este módulo em [[!DNL Workfront] object types available for each [!DNL Workfront] módulo](#workfront-object-types-available-for-each-workfront-module).

+++

+++ **[!UICONTROL Registro de monitoramento]**

Esse módulo de acionador executa um cenário quando objetos de um tipo específico são adicionados, atualizados ou ambos. O módulo retorna todos os campos padrão associados ao registro ou registros, juntamente com quaisquer campos e valores personalizados que a conexão acessa. Você pode mapear essas informações em módulos subsequentes do cenário. Na saída, o módulo indica se cada registro é novo ou atualizado.

Os registros que foram adicionados e atualizados em um determinado período são retornados como novos registros.

Ao configurar esse módulo, os seguintes campos são exibidos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Workfront] aplicativo para [!DNL Workfront Fusion], consulte <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Connect [!DNL Workfront] para [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filtro]</td> 
   <td> <p>Escolha se deseja que o cenário seja monitorado <strong>[!UICONTROL Novos registros somente]</strong>, <strong>[!UICONTROL Somente Registros Atualizados]</strong>ou <strong>[!UICONTROL Registros novos e atualizados]</strong>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de registro]</td> 
   <td> <p>(É exibido depois que você escolhe uma <strong>Filtro</strong>.) Selecione o tipo de [!DNL Workfront] registre que você deseja que o módulo assista.</p> <p>Por exemplo, se você quiser iniciar o cenário sempre que um novo Projeto for criado, selecione [!UICONTROL Projeto]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Saídas]</td> 
   <td> <p>Selecione as informações que deseja incluir no pacote de saída deste módulo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filtro opcional]</td> 
   <td> <p>(Avançado) Digite uma string de código de API para definir quaisquer parâmetros ou códigos adicionais que refinarão seus critérios. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limite]</td> 
   <td> <p>Insira ou mapeie o número máximo de registros que você deseja que o módulo retorne durante cada ciclo de execução de cenário.</p> </td> 
  </tr> 
 </tbody> 
</table>

Veja uma lista de [!DNL Workfront] tipos de objetos para os quais você pode usar este módulo em [[!DNL Workfront] object types available for each [!DNL Workfront] módulo](#workfront-object-types-available-for-each-workfront-module).

+++


### Ações

<!--
* [Convert object](#convert-object) 
* [Create a record (attaching custom forms)](#create-a-record-attaching-custom-forms) 
* [Create a record](#create-a-record) 
* [Custom API Call](#custom-api-call) 
* [Delete Record](#delete-record) 
* [Download Document](#download-document) 
* [Misc Action](#misc-action) 
* [Read a Record](#read-a-record) 
* [Update Record](#update-record) 
* [Upload Document](#upload-document)
-->

+++ **[!UICONTROL Converter objeto]**

Esse módulo de ação faz uma das seguintes conversões:

* Converter problema em projeto
* Converter problema em tarefa
* Converter tarefa em projeto

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Workfront] aplicativo para [!DNL Workfront Fusion], consulte <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Connect [!DNL Workfront] para [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Tipo de objeto]</td> 
   <td> <p>Selecione o tipo de objeto que deseja converter. Esse é o tipo que o objeto tem antes da conversão.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Converter em]</td> 
   <td>Selecione o objeto para o qual deseja convertê-lo. Esse é o tipo que o objeto tem após a conversão.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL &lt;object&gt; ID]</td> 
   <td> <p>Insira a ID do objeto. </p> <p>Observação: Ao inserir a ID de um objeto, você pode começar a digitar o nome do objeto e, em seguida, selecioná-lo na lista. O módulo insere a ID apropriada no campo .</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL ID do modelo]</td> 
   <td> <p>Se estiver convertendo em um projeto, selecione a ID de modelo que deseja usar para o projeto.</p> <p>Observação: Ao inserir a ID de um objeto, você pode começar a digitar o nome do objeto e, em seguida, selecioná-lo na lista. O módulo insere a ID apropriada no campo .</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Formulários personalizados]</td> 
   <td>Selecione todos os formulários personalizados que deseja adicionar ao objeto recém-convertido e insira valores para os campos do formulário personalizado.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Opções]</td> 
   <td> <p>Ative as opções desejadas ao converter o objeto. As opções estão disponíveis dependendo de qual objeto você está convertendo de ou para.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Criar um registro (anexar formulários personalizados)]**

Esse módulo de ação cria um objeto, como um projeto, uma tarefa ou um problema em [!DNL Workfront]e permite adicionar um formulário personalizado ao novo objeto. O módulo permite selecionar quais campos do objeto estão disponíveis no módulo .

Especifique a ID do registro.

O módulo retorna a ID do registro e quaisquer campos associados, juntamente com quaisquer campos e valores personalizados que a conexão acessa. Você pode mapear essas informações em módulos subsequentes do cenário.

Você pode usar esse módulo, por exemplo, para criar uma tarefa em [!DNL Workfront] quando um cliente adiciona uma nova linha em um [!DNL Google Sheets] lista de tarefas que precisam ser realizadas.

Ao configurar esse módulo, os seguintes campos são exibidos.

Certifique-se de fornecer o número mínimo de campos de entrada. Por exemplo, para criar um problema, é necessário fornecer uma ID de projeto pai válida no campo ID do projeto para indicar onde o problema deve estar no Workfront. Você pode usar o painel de mapeamento para mapear essas informações de outro módulo em seu cenário, ou pode inseri-las manualmente digitando o nome e depois selecionando-o na lista.

<table style="table-layout:auto">
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Workfront] aplicativo para [!DNL Workfront Fusion], consulte <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Connect [!DNL Workfront] para [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipo de registro]</td> 
   <td> <p>Selecione o tipo de [!DNL Workfront] registre que deseja que o módulo crie.</p> <p>Por exemplo, se você deseja criar um Projeto, selecione [!UICONTROL Projeto] na lista suspensa e verifique se você tem acesso aos dados (dos módulos anteriores na situação) que preencherão o projeto.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Selecionar campos a serem mapeados]</td> 
   <td> <p>Selecione os campos que deseja disponibilizar para entrada de dados. Isso permite usar esses campos sem precisar rolar pelos campos que não são necessários.</p> <p>Para campos em formulários personalizados, use o <b>[!UICONTROL Anexar formulário personalizado]</b> campo.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Anexar formulário personalizado]</td> 
   <td>Selecione todos os formulários personalizados que deseja adicionar ao novo objeto e insira valores para esses campos.</td> 
  </tr> 
 </tbody> 
</table>

Veja uma lista de [!DNL Workfront] tipos de objetos para os quais você pode usar este módulo em [[!DNL Workfront] object types available for each [!DNL Workfront] módulo](#workfront-object-types-available-for-each-workfront-module).

>[!NOTE]
>
>* Ao inserir a ID de um objeto, você pode começar a digitar o nome do objeto e, em seguida, selecioná-lo na lista. O módulo insere a ID apropriada no campo .
>* Ao inserir o texto para um campo personalizado ou um [!UICONTROL Observação] objeto (Comentário ou resposta), é possível usar tags HTML no [!UICONTROL Texto da nota] para criar rich text, como negrito ou itálico.
>
>  Para obter mais informações sobre rich text em atualizações, consulte [Adicionar uma atualização a um item de trabalho](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#add) em [Atualizar trabalho](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

+++

+++ **[!UICONTROL Criar registro]**

Esse módulo de ação cria um objeto, como um projeto, uma tarefa ou um problema no Workfront. O módulo permite selecionar quais campos do objeto estão disponíveis no módulo .

Especifique a ID do registro.

O módulo retorna a ID do registro e quaisquer campos associados, juntamente com quaisquer campos e valores personalizados que a conexão acessa. Você pode mapear essas informações em módulos subsequentes do cenário.

Você pode usar esse módulo, por exemplo, para criar uma tarefa em [!DNL Workfront] quando um cliente adiciona uma nova linha em uma lista de planilhas Google de tarefas que precisam ser realizadas.

Ao configurar esse módulo, os seguintes campos são exibidos.

Certifique-se de fornecer o número mínimo de campos de entrada. Por exemplo, para criar um problema, é necessário fornecer uma ID de projeto pai válida no campo ID do projeto para indicar onde o problema deve estar no Workfront. Você pode usar o painel de mapeamento para mapear essas informações de outro módulo em seu cenário, ou pode inseri-las manualmente digitando o nome e depois selecionando-o na lista.

<table style="table-layout:auto">
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Workfront] aplicativo para [!DNL Workfront Fusion], consulte <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Connect [!DNL Workfront] para [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipo de registro]</td> 
   <td> <p>Selecione o tipo de [!DNL Workfront] registre que deseja que o módulo crie.</p> <p>Por exemplo, se você deseja criar um Projeto, selecione [!UICONTROL Projeto] na lista suspensa e verifique se você tem acesso aos dados (dos módulos anteriores na situação) que preencherão o projeto.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Selecionar campos a serem mapeados]</td> 
   <td>Selecione os campos que deseja disponibilizar para entrada de dados. Isso permite usar esses campos sem precisar rolar pelos campos que não são necessários.</td> 
  </tr> 
 </tbody> 
</table>

Veja uma lista de [!DNL Workfront] tipos de objetos para os quais você pode usar este módulo em [[!DNL Workfront] object types available for each [!DNL Workfront] módulo](#workfront-object-types-available-for-each-workfront-module).

>[!NOTE]
>
>* Ao inserir a ID de um objeto, você pode começar a digitar o nome do objeto e, em seguida, selecioná-lo na lista. O módulo insere a ID apropriada no campo .
>* Ao inserir o texto para um campo personalizado ou um [!UICONTROL Observação] objeto (Comentário ou resposta), é possível usar tags HTML no [!UICONTROL Texto da nota] para criar rich text, como negrito ou itálico.
>
>  Para obter mais informações sobre rich text em atualizações, consulte [Adicionar uma atualização a um item de trabalho](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#add) em [Atualizar trabalho](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

+++

+++ **[!UICONTROL Chamada da API personalizada]**

Esse módulo de ação permite que você faça uma chamada autenticada personalizada para o [!DNL Workfront] API. Dessa forma, você pode criar uma automação de fluxo de dados que não pode ser realizada pela outra [!DNL Workfront] módulos.

O módulo retorna as seguintes informações:

* **[!UICONTROL Código de status]** (número): Isso indica o sucesso ou a falha de sua solicitação HTTP. Estes são códigos padrão que você pode pesquisar na Internet.
* **[!UICONTROL Cabeçalhos]** (objeto): Um contexto mais detalhado para o código de resposta/status que não está relacionado ao corpo da saída. Nem todos os cabeçalhos exibidos em um cabeçalho de resposta são cabeçalhos de resposta, portanto alguns podem não ser úteis para você.

   Os cabeçalhos de resposta dependem da solicitação HTTP que você escolheu ao configurar o módulo.

* **[!UICONTROL Corpo]** (objeto): Dependendo da solicitação HTTP escolhida ao configurar o módulo, você poderá receber alguns dados de volta. Esses dados, como os dados de uma solicitação do GET, estão contidos nesse objeto.

Você pode mapear essas informações em módulos subsequentes do cenário.

Ao configurar esse módulo, os seguintes campos são exibidos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Workfront] aplicativo para [!DNL Workfront Fusion], consulte <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Connect [!DNL Workfront] para [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">URL</td> 
   <td> <p>Insira um caminho relativo a<code> https://&lt;WORKFRONT_DOMAIN&gt;/attask/api/&lt;API_VERSION&gt;/</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Versão da API]</td> 
   <td>Selecione a versão do [!DNL Workfront] API que você deseja que o módulo use.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Método]</td> 
   td&gt; <p>Selecione o método de solicitação HTTP que você precisa configurar a chamada da API. Para obter mais informações, consulte <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">Métodos de solicitação HTTP em [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cabeçalhos]</td> 
   <td> <p>Adicione os cabeçalhos da solicitação no formato de um objeto JSON padrão. Isso determina o tipo de conteúdo da solicitação.</p> <p>Por exemplo,<code> {"Content-type":"application/json"}</code></p> <p>Observação: Se você estiver recebendo erros e for difícil determinar sua origem, considere modificar cabeçalhos com base no [!DNL Workfront] documentação. Se a sua chamada à API personalizada retornar um erro de solicitação HTTP 422, tente usar um <code>"Content-Type":"text/plain"</code> cabeçalho.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sequência de consulta]</td> 
   <td> <p>Adicione a query para a chamada de API no formato de um objeto JSON padrão.</p> <p>Por exemplo: <code>{"name":"something-urgent"}</code></p> <p>Dica: Recomendamos enviar informações por meio do corpo JSON, em vez de como parâmetros de consulta.</p> </td> 
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

Veja uma lista de [!DNL Workfront] tipos de objetos para os quais você pode usar este módulo em [[!DNL Workfront] object types available for each [!DNL Workfront] módulo](#workfront-object-types-available-for-each-workfront-module).

+++

+++ **[!UICONTROL Excluir registro]**

Esse módulo de ação exclui um objeto, como um projeto, uma tarefa ou um problema no Workfront.

Especifique a ID do registro.

O módulo retorna a ID do registro e quaisquer campos associados, juntamente com quaisquer campos e valores personalizados que a conexão acessa. Você pode mapear essas informações em módulos subsequentes do cenário.

Ao configurar esse módulo, os seguintes campos são exibidos.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Workfront] aplicativo para [!DNL Workfront Fusion], consulte <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Connect [!DNL Workfront] para [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Forçar exclusão]</td> 
   <td>Ative essa opção para garantir que o registro seja excluído, mesmo que a função [!DNL Workfront] A interface solicitaria a confirmação da exclusão.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>ID</td> 
   <td> <p>Insira o [!DNL Workfront] ID do registro que você deseja que o módulo exclua.</p> <p>Para obter a ID, abra o [!DNL Workfront] no navegador e copie o texto no final do URL após "ID=". Por exemplo: https://my.workfront.com/project/view?ID=<i>5e43010c03286a2a555e1d0a75d6a86e</i></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipo de registro]</td> 
   <td>Selecione o tipo de [!DNL Workfront] registre que deseja que o módulo exclua.</td> 
  </tr> 
 </tbody> 
</table>

Veja uma lista de [!DNL Workfront] tipos de objetos para os quais você pode usar este módulo em [[!DNL Workfront] object types available for each [!DNL Workfront] módulo](#workfront-object-types-available-for-each-workfront-module).

+++

+++ **[!UICONTROL Baixar Documento]**

Este módulo de ação baixa um documento do Workfront.

Especifique a ID do registro.

O módulo retorna o conteúdo, o nome do arquivo, a extensão de arquivo e o tamanho do arquivo do documento. Você pode mapear essas informações em módulos subsequentes do cenário.

Ao configurar esse módulo, os seguintes campos são exibidos.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Workfront] aplicativo para [!DNL Workfront Fusion], consulte <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Connect [!DNL Workfront] para [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID do documento]</td> 
   <td> <p>Mapear ou inserir manualmente o [!DNL Workfront] ID do documento que você deseja que o módulo baixe.</p> <p>Para obter a ID, abra o [!DNL Workfront] no navegador e copie o texto no final do URL após "ID=". Por exemplo: https://my.workfront.com/project/view?ID=<i>5e43010c03286a2a555e1d0a75d6a86e</i></p> </td> 
  </tr> 
 </tbody> 
</table>

Veja uma lista de [!DNL Workfront] tipos de objetos para os quais você pode usar este módulo em [[!DNL Workfront] object types available for each [!DNL Workfront] módulo](#workfront-object-types-available-for-each-workfront-module).

+++

+++ **[!UICONTROL Ação Diversa]**

Esse módulo de ação permite executar ações em relação à API.

Ao configurar esse módulo, os seguintes campos são exibidos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Workfront] aplicativo para [!DNL Workfront Fusion], consulte <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Connect [!DNL Workfront] para [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Tipo de registro]</td> 
   <td> <p>Selecione o tipo de [!DNL Workfront] gravar com o qual você deseja que o módulo interaja.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Ação]</td> 
   <td> <p>Selecione a ação que deseja que o módulo execute.</p> <p>Talvez seja necessário preencher campos adicionais, dependendo do [!UICONTROL Tipo de registro] e da [!UICONTROL Ação] que você escolher. Algumas combinações dessas duas configurações podem exigir apenas uma ID de registro, enquanto outras (como Projeto para a variável <strong>[!UICONTROL Tipo de registro]</strong> e [!UICONTROL Anexar modelo] para o <strong>[!UICONTROL Ação]</strong>) exigem informações adicionais (como uma ID de objeto e uma ID de modelo).</p> <p>Para obter detalhes sobre campos individuais, consulte o <a href="http://developer.workfront.com/">Documentação do desenvolvedor do Workfront</a>. </p> 
    <ol> 
     <li value="1"> <p>Selecione o tipo de registro no menu de navegação esquerdo [!DNL Workfront] página de documentação do desenvolvedor. Os seguintes tipos têm suas próprias páginas:</p> 
      <ul> 
       <li> <p>[!UICONTROL Projetos]</p> </li> 
       <li> <p>[!UICONTROL Tarefas]</p> </li> 
       <li> <p>[!UICONTROL Problemas]</p> </li> 
       <li> <p>[!UICONTROL Usuários]</p> </li> 
       <li> <p>[!UICONTROL Documentos]</p> </li> 
      </ul> <p>Para todos os outros tipos de registro, selecione <b>[!UICONTROL Outros objetos e pontos de extremidade]</b>e localize o tipo de registro nas páginas classificadas alfabeticamente.</p> </li> 
     <li value="2"> <p>Na página do tipo de registro apropriado, pesquise a ação (Ctrl-F ou Cmd-F).</p> </li> 
     <li value="3"> <p>Exiba descrições de campos disponíveis na ação selecionada.</p> </li> 
    </ol> <p>Nota:  <p>Ao criar uma prova por meio do [!DNL Workfront] Módulo [!UICONTROL Misc Action], a prática recomendada é criar uma prova sem opções avançadas e, em seguida, atualizar a prova usando o [!DNL Workfront Proof] API SOAP.</p> <p>Para obter mais informações sobre como criar uma prova com a variável [!DNL Workfront] API (que esse módulo usa), consulte <a href="../../wf-api/tips-tricks-and-troubleshooting/api-create-proof-options-json.md" class="MCXref xref">Adicione opções avançadas de prova ao criar uma prova por meio do [!DNL Adobe Workfront] API</a></p> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL ID]</td> 
   <td>Insira ou mapeie a [!DNL Workfront] ID do registro com o qual você deseja que o módulo interaja.<p>Para obter a ID, abra o [!DNL Workfront] no navegador e copie o texto no final do URL após "ID=". Por exemplo: https://my.workfront.com/project/view?ID=<i>5e43010c03286a2a555e1d0a75d6a86e</i></p></td> 
  </tr> 
 </tbody> 
</table>

Veja uma lista de [!DNL Workfront] tipos de objetos para os quais você pode usar este módulo em [[!DNL Workfront] object types available for each [!DNL Workfront] módulo](#workfront-object-types-available-for-each-workfront-module).

+++

+++ **[!UICONTROL Ler um registro]**

Esse módulo de ação recupera dados de um único registro.

Especifique a ID do registro. Você também pode especificar quais registros relacionados deseja que o módulo leia.

Por exemplo, se o registro que o módulo está lendo for um projeto, você pode especificar que deseja que as tarefas do projeto sejam lidas.

O módulo retorna uma matriz de dados dos campos padrão para a saída especificada.

Ao configurar esse módulo, os seguintes campos são exibidos.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td>[!UICONTROL Connection]</td>

<td> <p>Para obter instruções sobre como conectar seu [!DNL Workfront] aplicativo para [!DNL Workfront Fusion], consulte <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Connect [!DNL Workfront] para [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
    <td>[!UICONTROL Tipo de registro]</td>

<td>Escolha a [!DNL Workfront] tipo de objeto que você deseja que o módulo leia.</td> 
  </tr> 
  <tr> 
    <td>[!UICONTROL Saídas]</td>

<td> <p>Selecione as informações que deseja incluir no pacote de saída deste módulo.</p> </td> 
  </tr> 
  <tr> 
    <td>[!UICONTROL Referências]</td>
   <td>Selecione quaisquer campos de referência que deseja incluir na saída.</td> 
  </tr> 
  <tr> 
    <td>[!UICONTROL Coleções]</td>
   <td>Selecione quaisquer campos de referência que deseja incluir na saída.</td> 
  </tr> 
  <tr> 
    <td>[!UICONTROL ID]</td>
   <td> <p>Insira o [!DNL Workfront] ID do registro que você deseja que o módulo leia.</p> <p>Para obter a ID, abra o [!DNL Workfront] no navegador e copie o texto no final do URL após "ID=". Por exemplo: https://my.workfront.com/project/view?ID=<i>5e43010c03286a2a555e1d0a75d6a86e</i></p> </td> 
  </tr> 
 </tbody> 
</table>

Veja uma lista de [!DNL Workfront] tipos de objetos para os quais você pode usar este módulo em [[!DNL Workfront] object types available for each [!DNL Workfront] módulo](#workfront-object-types-available-for-each-workfront-module).

+++

+++ **[!UICONTROL Atualizar registro]**

Esse módulo de ação atualiza um objeto, como um projeto, uma tarefa ou um problema. O módulo permite selecionar quais campos do objeto estão disponíveis no módulo .

Especifique a ID do registro.

O módulo retorna a ID do objeto e quaisquer campos associados, juntamente com quaisquer campos e valores personalizados que a conexão acessa. Você pode mapear essas informações em módulos subsequentes do cenário.

Ao configurar esse módulo, os seguintes campos são exibidos.

<table style="table-layout:auto">
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Workfront] aplicativo para [!DNL Workfront Fusion], consulte <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Connect [!DNL Workfront] para [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL ID]</td> 
   <td> <p>Insira o [!DNL Workfront] ID do registro que você deseja que o módulo atualize.</p> <p>Para obter a ID, abra o [!DNL Workfront] no navegador e copie o texto no final do URL após "ID=". Por exemplo: https://my.workfront.com/project/view?ID=<i>5e43010c03286a2a555e1d0a75d6a86e</i></p> </td> 
  </tr> 
  <tr> 
   <td>[!DNL Record Type]</td> 
   <td> <p>Selecione o tipo de [!DNL Workfront] registre que deseja que o módulo seja atualizado.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!DNL Select fields to map]</td> 
   <td>Selecione os campos que deseja disponibilizar para entrada de dados. Isso permite usar esses campos sem precisar rolar pelos campos que não são necessários.</td> 
  </tr> 
 </tbody> 
</table>

Veja uma lista de [!DNL Workfront] tipos de objetos para os quais você pode usar este módulo em [[!DNL Workfront] object types available for each [!DNL Workfront] módulo](#workfront-object-types-available-for-each-workfront-module).

>[!NOTE]
>
>* Ao inserir a ID de um objeto, você pode começar a digitar o nome do objeto e, em seguida, selecioná-lo na lista. O módulo insere a ID apropriada no campo .
>* Ao inserir o texto para um campo personalizado ou um [!UICONTROL Observação] objeto (Comentário ou resposta), é possível usar tags HTML no [!UICONTROL Texto da nota] para criar rich text, como negrito ou itálico.
>
>  Para obter mais informações sobre rich text em atualizações, consulte [Adicionar uma atualização a um item de trabalho](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#add) em [Atualizar trabalho](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

+++

+++ **[!UICONTROL Fazer upload do documento]**

Este módulo de ação carrega um documento em um [!DNL Workfront] objeto, como projeto, tarefa ou problema.

Especifique o local do documento, o arquivo que deseja carregar e um novo nome opcional para o arquivo.

O módulo retorna a ID do documento e quaisquer campos associados, juntamente com quaisquer campos e valores personalizados que a conexão acessa. Você pode mapear essas informações em módulos subsequentes do cenário.

Ao configurar esse módulo, os seguintes campos são exibidos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Workfront] aplicativo para [!DNL Workfront Fusion], consulte <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Connect [!DNL Workfront] para [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL ID de registro relacionado]</td> 
   <td>Insira o [!DNL Workfront] ID do registro para o qual você deseja fazer upload do documento.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipo de registro relacionado]</td> 
   <td>Selecione o tipo de [!DNL Workfront] registre onde deseja que o módulo carregue o documento.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Arquivo de origem]</td> 
   <td> <p>Selecione um arquivo de origem de um módulo anterior ou mapeie o nome e os dados do arquivo de origem.</p> </td> 
  </tr> 
 </tbody> 
</table>

Veja uma lista de [!DNL Workfront] tipos de objetos para os quais você pode usar este módulo em [[!DNL Workfront] object types available for each [!DNL Workfront] módulo](#workfront-object-types-available-for-each-workfront-module).

+++

### Pesquisas

<!--
* [Read Related Records](#read-related-records) 
* [Search](#search)
-->

+++ **[!UICONTROL Ler registros relacionados]**

Esse módulo de pesquisa lê registros que correspondem à consulta de pesquisa especificada, em um objeto pai específico.

Especifique quais campos você deseja incluir na saída. Você pode mapear essas informações em módulos subsequentes do cenário.

Ao configurar esse módulo, os seguintes campos são exibidos.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Workfront] aplicativo para [!DNL Workfront Fusion], consulte <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Connect [!DNL Workfront] para [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Tipo de registro]</td> 
   <td> <p>Selecione o tipo de registro pai (objeto Workfront) cujos registros associados você deseja ler.</p> <p>Veja uma lista de [!DNL Workfront] tipos de objetos para os quais você pode usar este módulo em <a href="#object-types-available-for-each-workfront-search-module" class="MCXref xref">[!DNL Workfront] tipos de objetos disponíveis para cada [!DNL Workfront] módulo</a> neste artigo.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL ID de registro pai]</td> 
   <td> <p>Insira ou mapeie a ID do registro pai cujos registros associados você deseja ler.</p> <p>Para obter a ID, abra o [!DNL Workfront] no navegador e copie o texto no final do URL após "ID=". Por exemplo: https://my.workfront.com/project/view?ID=<i>5e43010c03286a2a555e1d0a75d6a86e</i></p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Coleções]</td> 
   <td>Selecione ou mapeie o tipo de registro filho que você deseja que o módulo leia.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Saídas]</td> 
   <td> <p>Selecione as informações que deseja incluir no pacote de saída deste módulo.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Pesquisar]**

Este módulo de pesquisa procura registros em um objeto em [!DNL Workfront] que correspondem à consulta de pesquisa especificada.

Você pode mapear essas informações em módulos subsequentes do cenário.

Ao configurar esse módulo, os seguintes campos são exibidos.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Workfront] aplicativo para [!DNL Workfront Fusion], consulte <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Connect [!DNL Workfront] para [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipo de registro]</td> 
   <td> <p>Selecione o tipo de [!DNL Workfront] registre que deseja que o módulo procure.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Conjunto de resultados]</td> 
   <td>Selecione uma opção para especificar se deseja que o módulo obtenha o primeiro resultado que corresponda aos seus critérios de pesquisa ou a todos os resultados que correspondem a ele.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Máximo]</td> 
   <td> <p>Insira ou mapeie o número máximo de registros que você deseja que o módulo retorne durante cada ciclo de execução de cenário.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Critérios de pesquisa]</td> 
   <td> <p>Insira o campo que deseja pesquisar, o operador que deseja usar na query e o valor que está procurando no campo .</p> <p>Observação: Não utilizar <code>username </code>em seus critérios de pesquisa. Incluindo <code>username </code>em uma consulta de API para [!DNL Workfront] registra o usuário no Workfront e a pesquisa não será bem-sucedida.</p> <p>Observação: <code>In</code> e <code>NotIn</code>trabalhe com arrays. As entradas devem estar no formato de matriz.</p></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Saídas]</td> 
   <td> <p>Selecione os campos que deseja incluir na saída deste módulo.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Referências]</td> 
   <td>Selecione quaisquer campos de referência que deseja incluir na pesquisa.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Coleções]</td> 
   <td>Selecione quaisquer coleções que deseja adicionar à pesquisa.</td> 
  </tr> 
 </tbody> 
</table>

Veja uma lista de [!DNL Workfront] tipos de objetos para os quais você pode usar este módulo em [[!DNL Workfront] object types available for each [!DNL Workfront] módulo](#workfront-object-types-available-for-each-workfront-module).

+++

## [!DNL Workfront] tipos de objetos disponíveis para cada [!DNL Workfront] módulo

<!-- [Object types available for each Workfront trigger module](#object-types-available-for-each-workfront-trigger-module) 
* [Object types available for each Workfront action module](#object-types-available-for-each-workfront-action-module) 
* [Object types available for each Workfront search module](#object-types-available-for-each-workfront-search-module)-->

+++**Tipos de objeto disponíveis para cada [!DNL Workfront] módulo de acionamento**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> </th> 
   <th>[!UICONTROL Registro de monitoramento]</th> 
   <th>[!UICONTROL Campo de observação]</th> 
   <th>[!UICONTROL Eventos de monitoramento]</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Processo de aprovação</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Atribuição</td> 
   <td> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Linha de base</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> Registro de Cobrança </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Preço</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Empresa</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Painel de Controle</td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Documento</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Pasta de documento</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Solicitação de documento</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Versão do Documento</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Despesa</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Tipo de Despesa</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Grupo</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Hora</td> 
   <td> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Tipo de hora</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Problema</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Iteração</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Função de trabalho</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Entrada no Relatório</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Etapa</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Caminho de Etapas</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Nota</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Etiqueta de nota</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Portfólio</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Programa</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Projeto</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Usuário de Projeto</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Hora reservada* </td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Relatório</td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Risco</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Tipo de Risco</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Aprovador de etapa</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Tarefa</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Equipe</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Modelo</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Modelo de Tarefa</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Planilha de horas</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Usuário</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Atualizar</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++**Tipos de objeto disponíveis para cada [!DNL Workfront] módulo de ação**

>[!NOTE]
>
>O [!UICONTROL Baixar documento] não está incluído nesta tabela porque [!DNL Workfront] os tipos de objetos não fazem parte de sua configuração.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> </th> 
   <th>[!UICONTROL Criar um registro]</th> 
   <th>[!UICONTROL Atualizar um registro]</th> 
   <th>[!UICONTROL Excluir um registro]</th> 
   <th>[!UICONTROL Upload Document]</th> 
   <th>[!UICONTROL Ler um registro]</th> 
   <th>[!UICONTROL Chamada da API personalizada]</th> 
   <th>[!UICONTROL Misc Action]</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Processo de aprovação</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Atribuição</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Registro de Cobrança</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Preço</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Empresa</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Documento</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Pasta de documento</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Versão do Documento</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Despesa</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Tipo de Despesa</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Grupo</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Hora</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Tipo de hora</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Problema</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Iteração</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Função de trabalho</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Entrada no Relatório</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Etapa</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Caminho de Etapas</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Nota</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Etiqueta de nota</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Portfólio</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Programa</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Projeto</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Usuário de Projeto</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Hora reservada* </td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Risco</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Tipo de Risco</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Aprovador de etapa</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Tarefa</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Equipe</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Modelo</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Modelo de Tarefa</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Planilha de horas</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Usuário</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Atualizar</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> <p> </p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++**Tipos de objeto disponíveis para cada [!DNL Workfront] módulo de pesquisa**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> </th> 
   <th>[!UICONTROL Search]</th> 
   <th>[!UICONTROL Ler registros relacionados]</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Processo de aprovação</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Atribuição</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Registro de Cobrança</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Preço</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Empresa</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Documento</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Pasta de documento</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Versão do Documento</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Despesa</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Tipo de Despesa</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Grupo</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Hora</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Tipo de hora</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Problema</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Iteração</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Função de trabalho</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Entrada no Relatório</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Etapa</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Caminho de Etapas</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Nota</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Etiqueta de nota</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Portfólio</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Programa</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Projeto</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Usuário de Projeto</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Hora reservada* </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Risco</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Tipo de Risco</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Aprovador de etapa</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Tarefa</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Equipe</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Modelo</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Modelo de Tarefa</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Planilha de horas</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Usuário</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Delegação de usuários</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

Recomendamos que você verifique novamente para garantir que isso funcione da maneira desejada.

+++

## Os filtros de assinatura de evento na [!DNL Workfront] > [!UICONTROL Eventos de observação] módulos

>[!NOTE]
>
>É altamente recomendável usar filtros de assinatura de evento em seu [!UICONTROL Eventos de observação] módulos.

O [!DNL Workfront] [!UICONTROL Eventos de observação] O módulo aciona cenários com base em um webhook que cria uma assinatura de evento no [!DNL Workfront] API. A assinatura do evento é um conjunto de dados que determina quais eventos são enviados para o webhook. Por exemplo, se você configurar uma [!UICONTROL Eventos de observação] que está observando problemas, a assinatura do evento envia somente eventos relacionados a problemas.

Ao usar filtros de assinatura de evento, os usuários do Fusion podem criar assinaturas de evento que são mais adequadas para seus casos de uso. Por exemplo, você pode configurar uma assinatura de evento no [!DNL Workfront] API para enviar somente problemas que estejam em um projeto específico para o webhook, garantindo que a função [!UICONTROL Eventos de observação] só acionará problemas nesse projeto. A capacidade de criar acionadores mais estreitos melhora o design de cenário, ao reduzir o número de acionadores irrelevantes.

Isso é diferente de configurar um filtro na variável [!DNL Workfront Fusion] . Sem um filtro de assinatura de evento, o webhook recebe todos os eventos relacionados ao tipo de objeto selecionado. A maioria desses eventos seria irrelevante para o cenário e deve ser filtrada para que o cenário possa continuar.

Os seguintes operadores estão disponíveis no filtro Workfront > Watch events :

* Igual
* Não é igual
* Maior que
* Menor que
* Maior que ou igual a
* Menor que ou igual a
* Contém
* Existe
* Não existe
* Alterado

>[!NOTE]
>
> * O `Exists`, `Does not exist`e `Changed` Os operadores não exigem um valor e o campo de valor está ausente dessas opções.
> * O `Changed` ignora o campo State .


>[!IMPORTANT]
>
>Não é possível editar filtros em [!DNL Workfront] webhooks. Para configurar filtros diferentes para [!DNL Workfront] assinaturas de evento, remova o webhook atual e crie um novo.

>[!INFO]
>
>**Exemplo:** Considere um cenário que processa novos problemas atribuídos a um usuário específico, a Ana.
>
>### Filtrar eventos usando um filtro de assinatura de evento (recomendado)
>
>Usando o filtro de evento, você pode configurar o webhook para acionar o cenário quando um problema é atribuído à Ana quando o problema é criado. Ana possui a userID b378489d8f7cd3cee0539260720a84b7.
>
>![](assets/event-filter-watch-events-350x277.png)
>
>Se 100 problemas forem criados em um dia, mas apenas dois deles forem atribuídos à Ana, o cenário seria executado duas vezes.
>
>### Filtrar eventos dentro do cenário (não recomendado)
>
>Para filtrar eventos para que somente os problemas atribuídos à Ana sejam processados, você pode criar um filtro após a [!UICONTROL Eventos de observação] módulo.
>
>![](assets/watch-events-non-event-filter-350x206.png)
>
>Se 100 problemas forem criados em um dia, mas apenas dois deles forem atribuídos à Ana, o cenário será executado 100 vezes. 98 das execuções seriam interrompidas no filtro, mas o módulo acionador ainda está consumindo dados e executando operações em todas as execuções.

Para obter mais informações sobre assinaturas de eventos, consulte [Perguntas frequentes - Assinaturas de eventos](../../wf-api/general/event-subs-faq.md).

Para obter mais informações sobre webhooks, consulte [Acionadores instantâneos (webhooks) em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/webhooks/instant-triggers-webhooks.md)

Para obter mais informações sobre filtros em cenários, consulte [Adicione um filtro a um cenário em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/add-a-filter-to-a-scenario.md).
