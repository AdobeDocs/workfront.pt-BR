---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: conector
navigation-topic: apps-and-their-modules
title: Módulos do Adobe Workfront
description: Você pode usar o conector do Adobe Workfront Fusion Adobe Workfront para automatizar seus processos no Workfront. Se você tiver uma licença do Workfront Fusion for Work Automation and Integration, também poderá usá-la para se conectar a aplicativos e serviços de terceiros.
author: Becky
feature: Workfront Fusion, Workfront Integrations and Apps
exl-id: b84d2d41-a983-4ea3-b331-0302bfcf8a2b
source-git-commit: 879d2ec0c8f3909a5dd385c77bd2de81120d40fa
workflow-type: tm+mt
source-wordcount: '5825'
ht-degree: 2%

---

# [!DNL Adobe Workfront] módulos

Você pode usar o [!DNL Adobe Workfront Fusion] [!DNL Adobe Workfront] conector para automatizar os processos no [!DNL Workfront]. Se você tiver uma [!UICONTROL [!DNL Workfront Fusion] para Automação e integração do trabalho] licença, você também pode usá-la para se conectar a aplicativos e serviços de terceiros.

A variável [!DNL Workfront] O conector do não é contabilizado em relação ao número de aplicativos ativos disponíveis para sua organização. Todos os cenários, mesmo que usem apenas o [!DNL Workfront] , não contem com a contagem total de cenários de sua organização.

Para obter mais informações sobre os aplicativos e cenários disponíveis em sua organização, consulte [Organizações](../../workfront-fusion/organizations/organizations-and-teams.md#organiza2) in [[!DNL Adobe Workfront Fusion] organizações e equipes](../../workfront-fusion/organizations/organizations-and-teams.md).

Se precisar de instruções sobre como criar um cenário, consulte [Criar um cenário no [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md). Para obter informações sobre módulos, consulte [Módulos no [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

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

## Conectar [!DNL Workfront] para [!DNL Workfront Fusion]

A variável [!DNL Workfront] O conector usa o OAuth 2.0 para se conectar a [!DNL Workfront].

Você pode criar uma conexão com o seu [!DNL Workfront] conta diretamente de dentro de um [!DNL Workfront Fusion] módulo.

1. Em qualquer [!DNL Workfront] módulo de aplicativo, clique em **[!UICONTROL Adicionar]** ao lado da [!UICONTROL Conexão] caixa.
1. Insira o nome da sua instância no URL. Exemplo: `https://<your instance>.my.workfront.com`.
1. Clique em **[!UICONTROL Próxima]**.
1. Clique em **[!UICONTROL Login do SAML]** para criar a conexão e voltar ao módulo.

   Ou

   Digite seu nome de usuário e senha e clique em **[!UICONTROL Fazer logon]** para criar a conexão e voltar ao módulo.

   >[!NOTE]
   >
   >* Se você não vir um botão de logon SAML, sua organização não habilitou o Logon único (SSO). Você pode fazer logon com seu Nome de usuário e Senha.
   >   
   >   Para obter mais informações sobre SSO, consulte [Visão geral do logon único no [!DNL Adobe Workfront]](../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md)
   >   
   >* Conexões OAuth 2.0 com o [!DNL Workfront] A API não depende mais das chaves de API.

## [!DNL Workfront] módulos e seus campos

Ao configurar [!DNL Workfront] módulos, [!DNL Workfront Fusion] exibe os campos listados abaixo. Junto com esses, [!DNL Workfront] Os campos podem ser exibidos, dependendo de fatores como seu nível de acesso no aplicativo ou serviço. Um título em negrito em um módulo indica um campo obrigatório.

Se você vir o botão de mapa acima de um campo ou função, poderá usá-lo para definir variáveis e funções para esse campo. Para obter mais informações, consulte [Mapear informações de um módulo para outro no [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

>[!NOTE]
>
>Se você não vir os campos mais atualizados em um módulo do Workfront, isso pode ser devido a problemas de cache. Aguarde uma hora e tente novamente.

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

+++ **[!UICONTROL Assistir a eventos]**

Esse módulo de acionador executa um cenário em tempo real quando objetos de um tipo específico são adicionados, atualizados ou excluídos no Workfront

O módulo retorna quaisquer campos padrão associados ao registro, juntamente com quaisquer campos e valores personalizados que a conexão acessa. Você pode mapear essas informações em módulos subsequentes no cenário.

1. Clique em **[!UICONTROL Adicionar]** à direita do **Webhook** caixa.

1. Configure o webhook no **[!UICONTROL Adicionar um gancho]** que é exibida.

   Ao configurar esse módulo, os campos a seguir são exibidos.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td>[!UICONTROL Nome do Webhook]</td> 
      <td>(Opcional) Digite um novo nome para o webhook</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Conexão]</td> 
      <td> <p>Para obter instruções sobre como conectar seu [!DNL Workfront] aplicativo para [!DNL Workfront Fusion], consulte <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Workfront] para [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Tipo de Registro]</td> 
      <td>Selecione o tipo de [!DNL Workfront] registre que você deseja que o módulo assista.</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Estado]</td> 
      <td>Selecione se deseja observar o estado antigo ou o novo estado.<ul><li><p><b>[!UICONTROL Novo estado]</b></p><p>Acionar um cenário quando o registro for alterado <b>para</b> um determinado valor.</p><p>Por exemplo, se o estado estiver definido como [!UICONTROL Novo Estado] e o filtro estiver definido como [!UICONTROL Status] [!UICONTROL Igual a] [!UICONTROL Em Andamento], o webhook acionará um cenário quando o [!UICONTROL Status] for alterado para [!UICONTROL Em Andamento], independentemente do status anterior. </p></li><li><p><b>[!UICONTROL Estado antigo]</b></p><p>Acionar um cenário quando o registro for alterado <b>de</b> um determinado valor.</p><p>Por exemplo, se o estado estiver definido como [!UICONTROL Estado Antigo] e o filtro estiver definido como [!UICONTROL Status] [!UICONTROL Igual a] [!UICONTROL Em Andamento], o webhook acionará um cenário quando um [!UICONTROL Status] atual [!UICONTROL Em Andamento] for alterado para outro status. </p></li></ul></td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td> <p>[!UICONTROL Eventos filtros]</p> </td> 
      <td> <p>É possível definir filtros para observar apenas os registros que atendem aos critérios selecionados.</p> <p>Para cada filtro, insira o campo que deseja que o filtro avalie, o operador e o valor que deseja que o filtro permita. Você pode usar mais de um filtro adicionando regras AND.</p> <p>Observação: não é possível editar filtros no existente [!DNL Workfront] webhooks. Para configurar filtros diferentes para [!DNL Workfront] assinaturas de evento, remova o webhook atual e crie um novo.</p> <p>Para obter mais informações sobre filtros de evento, consulte <a href="#event-subscription-filters-in-the-workfront-watch-events-modules" class="MCXref xref">Filtros de assinatura de evento na [!DNL Workfront] &gt; módulos [!UICONTROL Watch Events]</a> neste artigo.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td>Excluir eventos feitos por esta conexão</td> 
      <td>Habilite essa opção para excluir eventos criados ou atualizados usando o mesmo conector que esse módulo de acionador usa. Isso pode evitar situações em que um cenário pode ser acionado, fazendo com que ele se repita em um loop infinito.</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Origem do Registro]</td> 
      <td> <p>Escolha se deseja que o cenário assista <strong>[!UICONTROL Somente Novos Registros]</strong>, <strong>[!UICONTROL Atualizou Somente Registros]</strong>, <strong>[!UICONTROL Registros Novos e Atualizados]</strong>ou <strong>[!DNL Deleted Records Only]</strong>.</p> <p>Observação: se você escolher <strong>[!UICONTROL Registros Novos e Atualizados]</strong>, a criação do webhook cria 2 assinaturas de evento (para o mesmo endereço de webhook).</p> </td> 
     </tr> 
    </tbody> 
   </table>

Depois que o webhook for criado, você poderá exibir o endereço do endpoint para o qual os eventos são enviados.

Para obter mais informações, consulte a seção [Exemplos de payloads de evento](../../wf-api/general/event-subs-api.md#examples-of-event-payloads) no [!DNL Workfront] Artigo de ajuda [API de assinatura de evento](../../wf-api/general/event-subs-api.md).

Veja uma lista dos [!DNL Workfront] tipos de objeto para os quais você pode usar este módulo em [[!DNL Workfront] tipos de objeto disponíveis para cada [!DNL Workfront] módulo](#workfront-object-types-available-for-each-workfront-module).

+++

+++ **[!UICONTROL Campo de observação]**

Esse módulo de acionamento executa um cenário quando um campo especificado é atualizado. O módulo retorna o valor antigo e o novo do campo especificado. Você pode mapear essas informações em módulos subsequentes no cenário.

Ao configurar esse módulo, os campos a seguir são exibidos.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexão]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Workfront] aplicativo para [!DNL Workfront Fusion], consulte <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Workfront] para [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipo de Registro]</td> 
   <td> <p>Selecione o tipo de [!DNL Workfront] registre que você deseja que o módulo assista.</p> <p>Por exemplo, selecione [!UICONTROL Tarefa] se desejar começar a executar o cenário sempre que um campo de registro for atualizado em uma tarefa.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Campo]</td> 
   <td>Selecione o campo que você deseja que o módulo veja por atualizações. Esses campos refletem os campos que [!DNL Workfront] O administrador configurou o para rastreamento.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Saídas]</td> 
   <td>Selecione as informações que deseja incluir no pacote de saída deste módulo.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Limite]</td> 
   <td> <p>Insira ou mapeie o número máximo de registros que deseja que o módulo retorne durante cada ciclo de execução de cenário.</p> </td> 
  </tr> 
 </tbody> 
</table>

Veja uma lista dos [!DNL Workfront] tipos de objeto para os quais você pode usar este módulo em [[!DNL Workfront] tipos de objeto disponíveis para cada [!DNL Workfront] módulo](#workfront-object-types-available-for-each-workfront-module).

+++

+++ **[!UICONTROL Assistir ao registro]**

Esse módulo de acionamento executa um cenário quando objetos de um tipo específico são adicionados, atualizados ou ambos. O módulo retorna todos os campos padrão associados ao registro ou aos registros, juntamente com quaisquer campos e valores personalizados que a conexão acesse. Você pode mapear essas informações em módulos subsequentes no cenário. Na saída, o módulo indica se cada registro é novo ou atualizado.

Os registros que foram adicionados e atualizados no período determinado são retornados como novos registros.

Ao configurar esse módulo, os campos a seguir são exibidos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Workfront] aplicativo para [!DNL Workfront Fusion], consulte <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Workfront] para [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filtro]</td> 
   <td> <p>Escolha se deseja que o cenário assista <strong>[!UICONTROL Somente Novos Registros]</strong>, <strong>[!UICONTROL Atualizou Somente Registros]</strong>ou <strong>[!UICONTROL Registros Novos e Atualizados]</strong>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de Registro]</td> 
   <td> <p>(É exibido depois que você escolhe um <strong>Filtro</strong>.) Selecione o tipo de [!DNL Workfront] registre que você deseja que o módulo assista.</p> <p>Por exemplo, se você deseja iniciar o cenário sempre que um novo projeto for criado, selecione [!UICONTROL Projeto]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Saídas]</td> 
   <td> <p>Selecione as informações que deseja incluir no pacote de saída deste módulo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filtro Opcional]</td> 
   <td> <p>(Avançado) Digite uma string de código da API para definir parâmetros ou códigos adicionais que refinarão seus critérios. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limite]</td> 
   <td> <p>Insira ou mapeie o número máximo de registros que deseja que o módulo retorne durante cada ciclo de execução de cenário.</p> </td> 
  </tr> 
 </tbody> 
</table>

Veja uma lista dos [!DNL Workfront] tipos de objeto para os quais você pode usar este módulo em [[!DNL Workfront] tipos de objeto disponíveis para cada [!DNL Workfront] módulo](#workfront-object-types-available-for-each-workfront-module).

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

* Converter Problema em Projeto
* Converter problema em tarefa
* Converter Tarefa em Projeto

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexão]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Workfront] aplicativo para [!DNL Workfront Fusion], consulte <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Workfront] para [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Tipo de objeto]</td> 
   <td> <p>Selecione o tipo de objeto que deseja converter. Esse é o tipo que o objeto tem antes da conversão.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Converter em]</td> 
   <td>Selecione o objeto para o qual você deseja convertê-lo. Esse é o tipo que o objeto tem após a conversão.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL &lt;object&gt; ID]</td> 
   <td> <p>Insira a ID do objeto. </p> <p>Observação: Ao informar o ID de um objeto, você pode começar a digitar o nome do objeto e, em seguida, selecioná-lo na lista. O módulo insere a ID apropriada no campo.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL ID de Modelo]</td> 
   <td> <p>Se estiver convertendo em um projeto, selecione a ID do modelo que deseja usar para o projeto.</p> <p>Observação: Ao informar o ID de um objeto, você pode começar a digitar o nome do objeto e, em seguida, selecioná-lo na lista. O módulo insere a ID apropriada no campo.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Formulários personalizados]</td> 
   <td>Selecione os formulários personalizados que deseja adicionar ao objeto recém-convertido e insira valores para os campos do formulário personalizado.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Opções]</td> 
   <td> <p>Ative as opções desejadas ao converter o objeto. As opções estão disponíveis dependendo do objeto para o qual você está convertendo ou a partir do.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Criar um registro (anexar formulários personalizados)]**

Este módulo de ação cria um objeto, como um projeto, tarefa ou problema no [!DNL Workfront]e permite adicionar um formulário personalizado ao novo objeto. O módulo permite selecionar quais dos campos do objeto estão disponíveis no módulo.

Especifique a ID do registro.

O módulo retorna a ID do registro e quaisquer campos associados, juntamente com quaisquer campos e valores personalizados que a conexão acessa. Você pode mapear essas informações em módulos subsequentes no cenário.

Você pode usar esse módulo, por exemplo, para criar uma tarefa no [!DNL Workfront] quando um cliente adiciona uma nova linha em um [!DNL Google Sheets] lista de tarefas que precisam ser feitas.

Ao configurar esse módulo, os campos a seguir são exibidos.

Forneça o número mínimo de campos de entrada. Por exemplo, se você deseja criar um problema, é necessário fornecer uma ID de projeto principal válida no campo ID do projeto para indicar onde o problema deve residir na Workfront. Você pode usar o painel de mapeamento para mapear essas informações de outro módulo em seu cenário ou pode inseri-las manualmente digitando o nome e selecionando-o na lista.

<table style="table-layout:auto">
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexão]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Workfront] aplicativo para [!DNL Workfront Fusion], consulte <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Workfront] para [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipo de Registro]</td> 
   <td> <p>Selecione o tipo de [!DNL Workfront] registro que você deseja que o módulo crie.</p> <p>Por exemplo, se você deseja criar um Projeto, selecione [!UICONTROL Project] na lista suspensa e verifique se você tem acesso aos dados (dos módulos anteriores no cenário) que preencherão o projeto.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Selecionar campos a serem mapeados]</td> 
   <td> <p>Selecione os campos que deseja disponibilizar para entrada de dados. Isso permite usar esses campos sem precisar percorrer os que não são necessários.</p> <p>Para campos em formulários personalizados, use o <b>[!UICONTROL Anexar Formulário Personalizado]</b> campo.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Anexar Formulário Personalizado]</td> 
   <td>Selecione quaisquer formulários personalizados que deseja adicionar ao novo objeto e insira valores para esses campos.</td> 
  </tr> 
 </tbody> 
</table>

Veja uma lista dos [!DNL Workfront] tipos de objeto para os quais você pode usar este módulo em [[!DNL Workfront] tipos de objeto disponíveis para cada [!DNL Workfront] módulo](#workfront-object-types-available-for-each-workfront-module).

>[!NOTE]
>
>* Ao inserir a ID de um objeto, você pode começar a digitar o nome do objeto e, em seguida, selecioná-lo na lista. O módulo insere a ID apropriada no campo.
>* Ao inserir o texto para um campo personalizado ou uma [!UICONTROL Nota] (Comentário ou resposta), você pode usar tags HTML na variável [!UICONTROL Texto da Nota] para criar rich text, como negrito ou itálico.
>
>  Para obter mais informações sobre rich text em atualizações, consulte [Adicionar uma atualização a um item de trabalho](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#add) in [Atualizar trabalho](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).
>

+++

+++ **[!UICONTROL Criar registro]**

Esse módulo de ação cria um objeto, como um projeto, tarefa ou problema no Workfront. O módulo permite selecionar quais dos campos do objeto estão disponíveis no módulo.

Especifique a ID do registro.

O módulo retorna a ID do registro e quaisquer campos associados, juntamente com quaisquer campos e valores personalizados que a conexão acessa. Você pode mapear essas informações em módulos subsequentes no cenário.

Você pode usar esse módulo, por exemplo, para criar uma tarefa no [!DNL Workfront] quando um cliente adiciona uma nova linha em uma lista de tarefas do Google Sheets que precisam ser feitas.

Ao configurar esse módulo, os campos a seguir são exibidos.

Forneça o número mínimo de campos de entrada. Por exemplo, se você deseja criar um problema, é necessário fornecer uma ID de projeto principal válida no campo ID do projeto para indicar onde o problema deve residir na Workfront. Você pode usar o painel de mapeamento para mapear essas informações de outro módulo em seu cenário ou pode inseri-las manualmente digitando o nome e selecionando-o na lista.

<table style="table-layout:auto">
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexão]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Workfront] aplicativo para [!DNL Workfront Fusion], consulte <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Workfront] para [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipo de Registro]</td> 
   <td> <p>Selecione o tipo de [!DNL Workfront] registro que você deseja que o módulo crie.</p> <p>Por exemplo, se você deseja criar um Projeto, selecione [!UICONTROL Project] na lista suspensa e verifique se você tem acesso aos dados (dos módulos anteriores no cenário) que preencherão o projeto.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Selecionar campos a serem mapeados]</td> 
   <td>Selecione os campos que deseja disponibilizar para entrada de dados. Isso permite usar esses campos sem precisar percorrer os que não são necessários.</td> 
  </tr> 
 </tbody> 
</table>

Veja uma lista dos [!DNL Workfront] tipos de objeto para os quais você pode usar este módulo em [[!DNL Workfront] tipos de objeto disponíveis para cada [!DNL Workfront] módulo](#workfront-object-types-available-for-each-workfront-module).

>[!NOTE]
>
>* Ao inserir a ID de um objeto, você pode começar a digitar o nome do objeto e, em seguida, selecioná-lo na lista. O módulo insere a ID apropriada no campo.
>* Ao inserir o texto para um campo personalizado ou uma [!UICONTROL Nota] (Comentário ou resposta), você pode usar tags HTML na variável [!UICONTROL Texto da Nota] para criar rich text, como negrito ou itálico.
>
>  Para obter mais informações sobre rich text em atualizações, consulte [Adicionar uma atualização a um item de trabalho](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#add) in [Atualizar trabalho](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).
>

+++

+++ **[!UICONTROL Chamada de API personalizada]**

Esse módulo de ação permite fazer uma chamada autenticada personalizada para o [!DNL Workfront] API. Dessa forma, você pode criar uma automação de fluxo de dados que não pode ser realizada pelo outro [!DNL Workfront] módulos.

O módulo retorna as seguintes informações:

* **[!UICONTROL Código de status]** (número): isso indica o sucesso ou a falha de sua solicitação HTTP. Esses são códigos padrão que você pode pesquisar na Internet.
* **[!UICONTROL Cabeçalhos]** (objeto): um contexto mais detalhado para o código de resposta/status que não está relacionado ao corpo de saída. Nem todos os cabeçalhos que aparecem em um cabeçalho de resposta são cabeçalhos de resposta, portanto, alguns podem não ser úteis para você.

  Os cabeçalhos de resposta dependem da solicitação HTTP escolhida ao configurar o módulo.

* **[!UICONTROL Corpo]** (objeto): dependendo da solicitação HTTP escolhida ao configurar o módulo, talvez você receba alguns dados de volta. Esses dados, como os dados de uma solicitação GET, estão contidos neste objeto.

Você pode mapear essas informações em módulos subsequentes no cenário.

Ao configurar esse módulo, os campos a seguir são exibidos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Workfront] aplicativo para [!DNL Workfront Fusion], consulte <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Workfront] para [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
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
   td&gt; <p>Selecione o método de solicitação HTTP necessário para configurar a chamada de API. Para obter mais informações, consulte <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">Métodos de solicitação HTTP em [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cabeçalhos]</td> 
   <td> <p>Adicione os cabeçalhos da solicitação no formulário de um objeto JSON padrão. Isso determina o tipo de conteúdo da solicitação.</p> <p>Por exemplo,<code> {"Content-type":"application/json"}</code></p> <p>Observação: se você estiver recebendo erros e for difícil determinar sua origem, considere modificar cabeçalhos com base na [!DNL Workfront] documentação. Se sua chamada de API personalizada retornar um erro de solicitação HTTP 422, tente usar um <code>"Content-Type":"text/plain"</code> cabeçalho.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cadeia de Consulta]</td> 
   <td> <p>Adicione a consulta da chamada à API na forma de um objeto JSON padrão.</p> <p>Por exemplo: <code>{"name":"something-urgent"}</code></p> <p>Dica: recomendamos que você envie informações por meio do corpo JSON, em vez de como parâmetros de consulta.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Corpo]</td> 
   <td> <p>Adicione o conteúdo do corpo para a chamada à API na forma de um objeto JSON padrão.</p> <p>Nota:  <p>Ao usar declarações condicionais como <code>if</code> no JSON, coloque as aspas fora da declaração condicional.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

Veja uma lista dos [!DNL Workfront] tipos de objeto para os quais você pode usar este módulo em [[!DNL Workfront] tipos de objeto disponíveis para cada [!DNL Workfront] módulo](#workfront-object-types-available-for-each-workfront-module).

+++

+++ **[!UICONTROL Excluir registro]**

Esse módulo de ação exclui um objeto, como um projeto, tarefa ou problema no Workfront.

Especifique a ID do registro.

O módulo retorna a ID do registro e quaisquer campos associados, juntamente com quaisquer campos e valores personalizados que a conexão acessa. Você pode mapear essas informações em módulos subsequentes no cenário.

Ao configurar esse módulo, os campos a seguir são exibidos.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexão]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Workfront] aplicativo para [!DNL Workfront Fusion], consulte <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Workfront] para [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Forçar exclusão]</td> 
   <td>Habilite essa opção para garantir que o registro seja excluído, mesmo que a variável [!DNL Workfront] A interface do solicitaria a confirmação da exclusão.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>ID</td> 
   <td> <p>Insira o único [!DNL Workfront] ID do registro que você deseja que o módulo exclua.</p> <p>Para obter a ID, abra o [!DNL Workfront] no navegador e copie o texto no final do URL após "ID=". Por exemplo: https://my.workfront.com/project/view?ID=<i>5e43010c03286a2a555e1d0a75d6a86e</i></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipo de Registro]</td> 
   <td>Selecione o tipo de [!DNL Workfront] registro que você deseja que o módulo exclua.</td> 
  </tr> 
 </tbody> 
</table>

Veja uma lista dos [!DNL Workfront] tipos de objeto para os quais você pode usar este módulo em [[!DNL Workfront] tipos de objeto disponíveis para cada [!DNL Workfront] módulo](#workfront-object-types-available-for-each-workfront-module).

>[!NOTE]
>
>Recomendamos a configuração do cenário a seguir para evitar a possibilidade de registros não serem excluídos devido a operações assíncronas.
>
>1. Excluir o registro de forma síncrona.
>1. Adicione a manipulação de erros ao módulo Delete Record para Ignorar o erro causado pelo tempo limite de 40 segundos.


+++

+++ **[!UICONTROL Baixar documento]**

Este módulo de ação baixa um documento do Workfront.

Especifique a ID do registro.

O módulo retorna o conteúdo do documento, o nome do arquivo, a extensão do arquivo e o tamanho do arquivo. Você pode mapear essas informações em módulos subsequentes no cenário.

Ao configurar esse módulo, os campos a seguir são exibidos.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexão]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Workfront] aplicativo para [!DNL Workfront Fusion], consulte <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Workfront] para [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID de Documento]</td> 
   <td> <p>Mapeie ou insira manualmente o [!DNL Workfront] ID do documento que você deseja que o módulo baixe.</p> <p>Para obter a ID, abra o [!DNL Workfront] no navegador e copie o texto no final do URL após "ID=". Por exemplo: https://my.workfront.com/project/view?ID=<i>5e43010c03286a2a555e1d0a75d6a86e</i></p> </td> 
  </tr> 
 </tbody> 
</table>

Veja uma lista dos [!DNL Workfront] tipos de objeto para os quais você pode usar este módulo em [[!DNL Workfront] tipos de objeto disponíveis para cada [!DNL Workfront] módulo](#workfront-object-types-available-for-each-workfront-module).

+++

+++ **[!UICONTROL Ação Diversa]**

Esse módulo de ação permite executar ações na API.

Ao configurar esse módulo, os campos a seguir são exibidos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexão]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Workfront] aplicativo para [!DNL Workfront Fusion], consulte <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Workfront] para [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Tipo de Registro]</td> 
   <td> <p>Selecione o tipo de [!DNL Workfront] registro com o qual você deseja que o módulo interaja.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Ação]</td> 
   <td> <p>Selecione a ação que deseja que o módulo execute.</p> <p>Talvez seja necessário preencher campos adicionais, dependendo do [!UICONTROL Record Type] e da [!UICONTROL Action] escolhidos. Algumas combinações dessas duas configurações podem exigir apenas uma ID de registro, enquanto outras (como Project para o <strong>[!UICONTROL Tipo de Registro]</strong> e [!UICONTROL Anexar Modelo] para o <strong>[!UICONTROL Ação]</strong>) exigem informações adicionais (como uma ID de objeto e uma ID de modelo).</p> <p>Para obter detalhes sobre campos individuais, consulte a <a href="http://developer.workfront.com/">Documentação do desenvolvedor do Workfront</a>. <p><strong>Nota</strong>: o site de documentação do desenvolvedor inclui informações somente por meio da API versão 14, mas ainda contém informações valiosas para chamadas de API. </p> 
    <ol> 
     <li value="1"> <p>Selecione o tipo de registro na navegação à esquerda no [!DNL Workfront] página da documentação do desenvolvedor. Os seguintes tipos têm suas próprias páginas:</p> 
      <ul> 
       <li> <p>[!UICONTROL Projetos]</p> </li> 
       <li> <p>[!UICONTROL Tarefas]</p> </li> 
       <li> <p>[!UICONTROL Problemas]</p> </li> 
       <li> <p>[!UICONTROL Usuários]</p> </li> 
       <li> <p>[!UICONTROL Documentos]</p> </li> 
      </ul> <p>Para todos os outros tipos de registro, selecione <b>[!UICONTROL Outros objetos e pontos de extremidade]</b>e localize o tipo de registro nas páginas classificadas alfabeticamente.</p> </li> 
     <li value="2"> <p>Na página do tipo de registro apropriado, pesquise (Ctrl-F ou Cmd-F) a ação.</p> </li> 
     <li value="3"> <p>Exibir descrições para campos disponíveis sob a ação selecionada.</p> </li> 
    </ol> <p>Nota:  <p>Ao criar uma prova por meio da [!DNL Workfront] Módulo [!UICONTROL Misc Action], a prática recomendada é criar uma prova sem nenhuma opção avançada e, em seguida, atualizar a prova usando o [!DNL Workfront Proof] API SOAP.</p> <p>Para obter mais informações sobre como criar uma prova com o [!DNL Workfront] API (que este módulo usa), consulte <a href="../../wf-api/tips-tricks-and-troubleshooting/api-create-proof-options-json.md" class="MCXref xref">Adicionar opções de prova avançada ao criar uma prova por meio da [!DNL Adobe Workfront] API</a></p> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL ID]</td> 
   <td>Insira ou mapeie o [!DNL Workfront] ID do registro com o qual você deseja que o módulo interaja.<p>Para obter a ID, abra o [!DNL Workfront] no navegador e copie o texto no final do URL após "ID=". Por exemplo: https://my.workfront.com/project/view?ID=<i>5e43010c03286a2a555e1d0a75d6a86e</i></p></td> 
  </tr> 
 </tbody> 
</table>

Veja uma lista dos [!DNL Workfront] tipos de objeto para os quais você pode usar este módulo em [[!DNL Workfront] tipos de objeto disponíveis para cada [!DNL Workfront] módulo](#workfront-object-types-available-for-each-workfront-module).

+++

+++ **[!UICONTROL Ler um Registro]**

Este módulo de ação recupera dados de um único registro.

Especifique a ID do registro. Você também pode especificar quais registros relacionados deseja que o módulo leia.

Por exemplo, se o registro que o módulo está lendo for um projeto, você pode especificar que deseja ler as tarefas do projeto.

O módulo retorna uma matriz de dados dos campos padrão para a saída especificada.

Ao configurar esse módulo, os campos a seguir são exibidos.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td>[!UICONTROL Conexão]</td>

<td> <p>Para obter instruções sobre como conectar seu [!DNL Workfront] aplicativo para [!DNL Workfront Fusion], consulte <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Workfront] para [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
    <td>[!UICONTROL Tipo de Registro]</td>

<td>Escolha o [!DNL Workfront] tipo de objeto que você deseja que o módulo leia.</td> 
  </tr> 
  <tr> 
    <td>[!UICONTROL Saídas]</td>

<td> <p>Selecione as informações que deseja incluir no pacote de saída deste módulo.</p> </td> 
  </tr> 
  <tr> 
    <td>[!UICONTROL Referências]</td>
   <td>Selecione os campos de referência que deseja incluir na saída.</td> 
  </tr> 
  <tr> 
    <td>[!UICONTROL Coleções]</td>
   <td>Selecione os campos de referência que deseja incluir na saída.</td> 
  </tr> 
  <tr> 
    <td>[!UICONTROL ID]</td>
   <td> <p>Insira o único [!DNL Workfront] ID do registro que você deseja que o módulo leia.</p> <p>Para obter a ID, abra o [!DNL Workfront] no navegador e copie o texto no final do URL após "ID=". Por exemplo: https://my.workfront.com/project/view?ID=<i>5e43010c03286a2a555e1d0a75d6a86e</i></p> </td> 
  </tr> 
 </tbody> 
</table>

Veja uma lista dos [!DNL Workfront] tipos de objeto para os quais você pode usar este módulo em [[!DNL Workfront] tipos de objeto disponíveis para cada [!DNL Workfront] módulo](#workfront-object-types-available-for-each-workfront-module).

+++

+++ **[!UICONTROL Atualizar registro]**

Esse módulo de ação atualiza um objeto, como um projeto, tarefa ou problema. O módulo permite selecionar quais dos campos do objeto estão disponíveis no módulo.

Especifique a ID do registro.

O módulo retorna a ID do objeto e quaisquer campos associados, juntamente com quaisquer campos e valores personalizados que a conexão acessa. Você pode mapear essas informações em módulos subsequentes no cenário.

Ao configurar esse módulo, os campos a seguir são exibidos.

<table style="table-layout:auto">
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexão]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Workfront] aplicativo para [!DNL Workfront Fusion], consulte <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Workfront] para [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL ID]</td> 
   <td> <p>Insira o único [!DNL Workfront] ID do registro que você deseja que o módulo atualize.</p> <p>Para obter a ID, abra o [!DNL Workfront] no navegador e copie o texto no final do URL após "ID=". Por exemplo: https://my.workfront.com/project/view?ID=<i>5e43010c03286a2a555e1d0a75d6a86e</i></p> </td> 
  </tr> 
  <tr> 
   <td>[!DNL Record Type]</td> 
   <td> <p>Selecione o tipo de [!DNL Workfront] registro que você deseja que o módulo atualize.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!DNL Select fields to map]</td> 
   <td>Selecione os campos que deseja disponibilizar para entrada de dados. Isso permite usar esses campos sem precisar percorrer os que não são necessários.</td> 
  </tr> 
 </tbody> 
</table>

Veja uma lista dos [!DNL Workfront] tipos de objeto para os quais você pode usar este módulo em [[!DNL Workfront] tipos de objeto disponíveis para cada [!DNL Workfront] módulo](#workfront-object-types-available-for-each-workfront-module).

>[!NOTE]
>
>* Ao inserir a ID de um objeto, você pode começar a digitar o nome do objeto e, em seguida, selecioná-lo na lista. O módulo insere a ID apropriada no campo.
>* Ao inserir o texto para um campo personalizado ou uma [!UICONTROL Nota] (Comentário ou resposta), você pode usar tags HTML na variável [!UICONTROL Texto da Nota] para criar rich text, como negrito ou itálico.
>
>  Para obter mais informações sobre rich text em atualizações, consulte [Adicionar uma atualização a um item de trabalho](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#add) in [Atualizar trabalho](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).
>

+++

+++ **[!UICONTROL Carregar documento]**

Esse módulo de ação faz upload de um documento em um [!DNL Workfront] como um projeto, tarefa ou problema.

Especifique o local do documento, o arquivo que deseja fazer upload e um novo nome opcional para o arquivo.

O módulo retorna a ID do documento e quaisquer campos associados, juntamente com quaisquer campos e valores personalizados que a conexão acessa. Você pode mapear essas informações em módulos subsequentes no cenário.

Ao configurar esse módulo, os campos a seguir são exibidos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexão]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Workfront] aplicativo para [!DNL Workfront Fusion], consulte <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Workfront] para [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL ID de Registro Relacionado]</td> 
   <td>Insira o único [!DNL Workfront] ID do registro no qual você deseja fazer upload do documento.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipo de Registro Relacionado]</td> 
   <td>Selecione o tipo de [!DNL Workfront] registre onde deseja que o módulo carregue o documento.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Arquivo de origem]</td> 
   <td> <p>Selecione um arquivo de origem de um módulo anterior ou mapeie o nome e os dados do arquivo de origem.</p> </td> 
  </tr> 
 </tbody> 
</table>

Veja uma lista dos [!DNL Workfront] tipos de objeto para os quais você pode usar este módulo em [[!DNL Workfront] tipos de objeto disponíveis para cada [!DNL Workfront] módulo](#workfront-object-types-available-for-each-workfront-module).

+++

### Pesquisas

<!--
* [Read Related Records](#read-related-records) 
* [Search](#search)
-->

+++ **[!UICONTROL Ler registros relacionados]**

Esse módulo de pesquisa lê registros que correspondem à consulta de pesquisa especificada em um determinado objeto pai.

Você especifica quais campos deseja incluir na saída. Você pode mapear essas informações em módulos subsequentes no cenário.

Ao configurar esse módulo, os campos a seguir são exibidos.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexão]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Workfront] aplicativo para [!DNL Workfront Fusion], consulte <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Workfront] para [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Tipo de Registro]</td> 
   <td> <p>Selecione o tipo do registro pai (objeto Workfront) cujos registros associados você deseja ler.</p> <p>Veja uma lista dos [!DNL Workfront] tipos de objeto para os quais você pode usar este módulo em <a href="#object-types-available-for-each-workfront-search-module" class="MCXref xref">[!DNL Workfront] tipos de objeto disponíveis para cada [!DNL Workfront] módulo</a> neste artigo.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL ID de Registro Pai]</td> 
   <td> <p>Informe ou mapeie o ID do registro-pai cujos registros associados você deseja ler.</p> <p>Para obter a ID, abra o [!DNL Workfront] no navegador e copie o texto no final do URL após "ID=". Por exemplo: https://my.workfront.com/project/view?ID=<i>5e43010c03286a2a555e1d0a75d6a86e</i></p> </td> 
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

+++ **[!UICONTROL Pesquisa]**

Este módulo de pesquisa procura registros em um objeto no [!DNL Workfront] que correspondam à consulta de pesquisa especificada.

Você pode mapear essas informações em módulos subsequentes no cenário.

Ao configurar esse módulo, os campos a seguir são exibidos.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexão]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Workfront] aplicativo para [!DNL Workfront Fusion], consulte <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Workfront] para [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipo de Registro]</td> 
   <td> <p>Selecione o tipo de [!DNL Workfront] registro que você deseja que o módulo procure.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Conjunto de Resultados]</td> 
   <td>Selecione uma opção para especificar se você deseja que o módulo obtenha o primeiro resultado que corresponda aos seus critérios de pesquisa ou todos os resultados que correspondam a ele.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Máximo]</td> 
   <td> <p>Insira ou mapeie o número máximo de registros que deseja que o módulo retorne durante cada ciclo de execução de cenário.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Pesquisar critérios]</td> 
   <td> <p>Digite o campo pelo qual deseja pesquisar, o operador que deseja usar na consulta e o valor que está procurando no campo.</p> <p>Observação: não use <code>username </code>em seus critérios de pesquisa. Incluindo <code>username </code>em uma consulta de API para [!DNL Workfront] O conecta o usuário no Workfront e a pesquisa não será bem-sucedida.</p> <p>Nota: <code>In</code> e <code>NotIn</code>trabalhar com arrays. As entradas devem estar em formato de matriz.</p></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Saídas]</td> 
   <td> <p>Selecione os campos que deseja incluir na saída deste módulo.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Referências]</td> 
   <td>Selecione os campos de referência que deseja incluir na pesquisa.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Coleções]</td> 
   <td>Selecione todas as coleções que deseja adicionar à pesquisa.</td> 
  </tr> 
 </tbody> 
</table>

Veja uma lista dos [!DNL Workfront] tipos de objeto para os quais você pode usar este módulo em [[!DNL Workfront] tipos de objeto disponíveis para cada [!DNL Workfront] módulo](#workfront-object-types-available-for-each-workfront-module).

+++

## [!DNL Workfront] tipos de objeto disponíveis para cada [!DNL Workfront] módulo

<!-- [Object types available for each Workfront trigger module](#object-types-available-for-each-workfront-trigger-module) 
* [Object types available for each Workfront action module](#object-types-available-for-each-workfront-action-module) 
* [Object types available for each Workfront search module](#object-types-available-for-each-workfront-search-module)-->

+++**Tipos de objeto disponíveis para cada [!DNL Workfront] módulo acionador**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> </th> 
   <th>[!UICONTROL Observar Registro]</th> 
   <th>[!UICONTROL Campo de Observação]</th> 
   <th>[!UICONTROL Observar Eventos]</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Processo de aprovação</td> 
   <td> </td> 
   <td>✓ µ</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Atribuição</td> 
   <td> </td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
  </tr> 
  <tr> 
   <td>Linha de base</td> 
   <td>✓ µ</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> Registro de Cobrança </td> 
   <td>✓ µ</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Taxa de faturamento</td> 
   <td> </td> 
   <td>✓ µ</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Empresa</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
  </tr> 
  <tr> 
   <td>Painel</td> 
   <td> </td> 
   <td> </td> 
   <td>✓ µ</td> 
  </tr> 
  <tr> 
   <td>Documento</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
  </tr> 
  <tr> 
   <td>Pasta de documento</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Solicitação de documento</td> 
   <td>✓ µ</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Versão do Documento</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Despesa</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
  </tr> 
  <tr> 
   <td>Tipo de Despesa</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Grupo</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Hora</td> 
   <td> </td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
  </tr> 
  <tr> 
   <td>Tipo de hora</td> 
   <td> </td> 
   <td>✓ µ</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Problema</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
  </tr> 
  <tr> 
   <td>Iteração</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Função no trabalho</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Entrada no Relatório</td> 
   <td>✓ µ</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Etapa</td> 
   <td> </td> 
   <td>✓ µ</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Caminho de Etapas</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Nota</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
  </tr> 
  <tr> 
   <td>Etiqueta de nota</td> 
   <td> </td> 
   <td>✓ µ</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Portfólio</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
  </tr> 
  <tr> 
   <td>Programa</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
  </tr> 
  <tr> 
   <td>Projeto</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
  </tr> 
  <tr> 
   <td>Usuário de Projeto</td> 
   <td> </td> 
   <td>✓ µ</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Aprovação da revisão</td> 
   <td> </td> 
   <td> </td> 
   <td>✓ µ</td> 
  </tr> 
  <tr> 
   <td>Tempo reservado* </td> 
   <td> </td> 
   <td>✓ µ</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Relatório</td> 
   <td> </td> 
   <td> </td> 
   <td>✓ µ</td> 
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
   <td>Aprovador da etapa</td> 
   <td> </td> 
   <td>✓ µ</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Tarefa</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
  </tr> 
  <tr> 
   <td>Equipe</td> 
   <td> </td> 
   <td>✓ µ</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Modelo</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
  </tr> 
  <tr> 
   <td>Modelo de Tarefa</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Planilha de horas</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
  </tr> 
  <tr> 
   <td>Usuário</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
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
>A variável [!UICONTROL Baixar documento] O módulo não está incluído nesta tabela porque [!DNL Workfront] tipos de objeto não fazem parte de sua configuração.

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
   <th>[!UICONTROL Carregar Documento]</th> 
   <th>[!UICONTROL Ler um registro]</th> 
   <th>[!UICONTROL Chamada de API Personalizada]</th> 
   <th>[!UICONTROL Ação Diversa]</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Processo de aprovação</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
  </tr> 
  <tr> 
   <td>Atribuição</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td> </td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
  </tr> 
  <tr> 
   <td>Registro de Cobrança</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td> </td> 
   <td>✓ µ</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Taxa de faturamento</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Empresa</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
  </tr> 
  <tr> 
   <td>Documento</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
  </tr> 
  <tr> 
   <td>Pasta de documento</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
  </tr> 
  <tr> 
   <td>Versão do Documento</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
  </tr> 
  <tr> 
   <td>Despesa</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
  </tr> 
  <tr> 
   <td>Tipo de Despesa</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td> </td> 
   <td>✓ µ</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Grupo</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
  </tr> 
  <tr> 
   <td>Hora</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Tipo de hora</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td> </td> 
   <td>✓ µ</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Problema</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
  </tr> 
  <tr> 
   <td>Iteração</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Função no trabalho</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Entrada no Relatório</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td> </td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
  </tr> 
  <tr> 
   <td>Etapa</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Caminho de Etapas</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Nota</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
  </tr> 
  <tr> 
   <td>Etiqueta de nota</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Portfólio</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
  </tr> 
  <tr> 
   <td>Programa</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
  </tr> 
  <tr> 
   <td>Projeto</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
  </tr> 
  <tr> 
   <td>Usuário de Projeto</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Tempo reservado* </td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Risco</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Tipo de Risco</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td> </td> 
   <td>✓ µ</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Aprovador da etapa</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Tarefa</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
  </tr> 
  <tr> 
   <td>Equipe</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Modelo</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Modelo de Tarefa</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
  </tr> 
  <tr> 
   <td>Planilha de horas</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Usuário</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
  </tr> 
  <tr> 
   <td>Atualizar</td> 
   <td> </td> 
   <td>✓ µ</td> 
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
   <th>[!UICONTROL Pesquisar]</th> 
   <th>[!UICONTROL Ler registros relacionados]</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Processo de aprovação</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
  </tr> 
  <tr> 
   <td>Atribuição</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
  </tr> 
  <tr> 
   <td>Registro de Cobrança</td> 
   <td>✓ µ</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Taxa de faturamento</td> 
   <td>✓ µ</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Empresa</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
  </tr> 
  <tr> 
   <td>Documento</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
  </tr> 
  <tr> 
   <td>Pasta de documento</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
  </tr> 
  <tr> 
   <td>Versão do Documento</td> 
   <td>✓ µ</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Despesa</td> 
   <td>✓ µ</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Tipo de Despesa</td> 
   <td>✓ µ</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Grupo</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
  </tr> 
  <tr> 
   <td>Hora</td> 
   <td>✓ µ</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Tipo de hora</td> 
   <td>✓ µ</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Problema</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
  </tr> 
  <tr> 
   <td>Iteração</td> 
   <td>✓ µ</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Função no trabalho</td> 
   <td>✓ µ</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Entrada no Relatório</td> 
   <td>✓ µ</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Etapa</td> 
   <td>✓ µ</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Caminho de Etapas</td> 
   <td>✓ µ</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Nota</td> 
   <td>✓ µ</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Etiqueta de nota</td> 
   <td>✓ µ</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Portfólio</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
  </tr> 
  <tr> 
   <td>Programa</td> 
   <td>✓ µ</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Projeto</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
  </tr> 
  <tr> 
   <td>Usuário de Projeto</td> 
   <td>✓ µ</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Tempo reservado* </td> 
   <td>✓ µ</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Risco</td> 
   <td>✓ µ</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Tipo de Risco</td> 
   <td>✓ µ</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Aprovador da etapa</td> 
   <td>✓ µ</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Tarefa</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
  </tr> 
  <tr> 
   <td>Equipe</td> 
   <td>✓ µ</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Modelo</td> 
   <td>✓ µ</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Modelo de Tarefa</td> 
   <td>✓ µ</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Planilha de horas</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
  </tr> 
  <tr> 
   <td>Usuário</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
  </tr> 
  <tr> 
   <td>Delegação de usuários</td> 
   <td>✓ µ</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

Recomendamos que você verifique novamente para garantir que isso funcione da maneira esperada.

+++

## Filtros de assinatura de evento na [!DNL Workfront] > [!UICONTROL Assistir a eventos] módulos

>[!NOTE]
>
>É altamente recomendável usar os filtros de assinatura de evento na [!UICONTROL Assistir a eventos] módulos.

A variável [!DNL Workfront] [!UICONTROL Assistir a eventos] O módulo aciona cenários com base em um webhook que cria uma assinatura de evento no [!DNL Workfront] API. A assinatura do evento é um conjunto de dados que determina quais eventos são enviados para o webhook. Por exemplo, se você configurar um [!UICONTROL Assistir a eventos] que está observando problemas, a assinatura do evento envia somente eventos relacionados a problemas.

Ao usar filtros de subscrição de eventos, os usuários do Fusion podem criar subscrições de eventos que são mais adequadas para seus casos de uso. Por exemplo, você pode configurar uma assinatura de evento na variável [!DNL Workfront] API para enviar ao webhook somente problemas que estão em um projeto específico, garantindo que o [!UICONTROL Assistir a eventos] O módulo do acionará somente para problemas nesse projeto. A capacidade de criar acionadores mais estreitos melhora o design do cenário ao reduzir o número de acionadores irrelevantes.

Isso é diferente da configuração de um filtro no [!DNL Workfront Fusion] cenário. Sem um filtro de inscrição de evento, seu webhook recebe todos os eventos relacionados ao tipo de objeto selecionado. A maioria desses eventos seria irrelevante para o cenário e deve ser filtrada para que o cenário possa continuar.

Os seguintes operadores estão disponíveis no filtro Workfront > Eventos de observação:

* Igual
* Não é igual
* Maior que
* Menor que
* Maior que ou igual a
* Menor que ou igual a
* Contém
* Existe
   * Esse operador não requer um valor e o campo de valor está ausente.
* Não existe
   * Esse operador não requer um valor e o campo de valor está ausente.
* Alterado
   * Esse operador não requer um valor e o campo de valor está ausente.
   * Este operador ignora o campo Estado.
   * Ao usar `Changed`, selecione **Somente eventos atualizados** no **Origem do Registro** campo.

>[!IMPORTANT]
>
>Não é possível editar filtros em [!DNL Workfront] webhooks. Para configurar filtros diferentes para [!DNL Workfront] assinaturas de evento, remova o webhook atual e crie um novo.

>[!INFO]
>
>**Exemplo:** Considere um cenário que processa novos problemas atribuídos a um usuário específico, Ana.
>
>### Filtrar eventos usando um filtro de assinatura de evento (recomendado)
>
>Usando o filtro de eventos, você pode configurar o webhook para acionar o cenário quando um problema for atribuído a Ana quando o problema for criado. Ana tem a ID de usuário b378489d8f7cd3cee0539260720a84b7.
>
>![](assets/event-filter-watch-events-350x277.png)
>
>Se forem criados 100 problemas em um dia, mas apenas dois deles forem atribuídos a Ana, o cenário seria executado duas vezes.
>
>### Filtrar eventos dentro do cenário (não recomendado)
>
>Para filtrar eventos de modo que somente problemas atribuídos a Ana sejam processados, você pode criar um filtro após o [!UICONTROL Assistir a eventos] módulo.
>
>![](assets/watch-events-non-event-filter-350x206.png)
>
>Se 100 edições forem criadas em um dia, mas apenas duas delas forem atribuídas a Ana, o cenário seria executado 100 vezes. 98 das execuções parariam no filtro, mas o módulo de acionamento ainda está consumindo dados e executando operações em todas as execuções.

Para obter mais informações sobre assinaturas de evento, consulte [Perguntas frequentes - Assinaturas de eventos](../../wf-api/general/event-subs-faq.md).

Para obter mais informações sobre webhooks, consulte [Acionadores instantâneos (webhooks) no [!DNL Adobe Workfront Fusion]](../../workfront-fusion/webhooks/instant-triggers-webhooks.md)

Para obter mais informações sobre filtros em cenários, consulte [Adicionar um filtro a um cenário no [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/add-a-filter-to-a-scenario.md).

