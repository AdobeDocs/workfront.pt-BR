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
source-git-commit: 2682c027b2cd248b2674cebe8f0a0b8d1006257b
workflow-type: tm+mt
source-wordcount: '6797'
ht-degree: 2%

---

# [!DNL Adobe Workfront] módulos

Você pode usar o conector [!DNL Adobe Workfront Fusion] [!DNL Adobe Workfront] para automatizar seus processos no [!DNL Workfront]. Se você tiver uma licença do [!UICONTROL [!DNL Workfront Fusion] para Automação e Integração do Trabalho], também poderá usá-la para se conectar a aplicativos e serviços de terceiros.

O conector [!DNL Workfront] não conta com o número de aplicativos ativos disponíveis para a sua organização. Todos os cenários, mesmo que usem apenas o aplicativo [!DNL Workfront], contam com a contagem total de cenários de sua organização.

Para obter mais informações sobre os aplicativos e cenários disponíveis em sua organização, consulte [Organizações](../../workfront-fusion/organizations/organizations-and-teams.md#organiza2) em [[!DNL Adobe Workfront Fusion] organizações e equipes](../../workfront-fusion/organizations/organizations-and-teams.md).

Se você precisar de instruções sobre como criar um cenário, consulte [Criar um cenário [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md). Para obter informações sobre módulos, consulte [Módulos em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

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
   <p>Requisito de licença herdada: [!UICONTROL [!DNL Workfront Fusion] para Automação e Integração do Trabalho], [!UICONTROL [!DNL Workfront Fusion] para Automação do Trabalho]</p>
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

## Conectar [!DNL Workfront] a [!DNL Workfront Fusion]

O conector [!DNL Workfront] usa OAuth 2.0 para se conectar a [!DNL Workfront].

Você pode criar uma conexão com sua conta do [!DNL Workfront] diretamente de dentro de um módulo do [!DNL Workfront Fusion].

1. Em qualquer módulo do Adobe Workfront, clique em **Adicionar** ao lado do campo Conexão.
1. Preencha os seguintes campos:

   <table style="table-layout:auto"> 
    <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1">
    </col>
    <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">
    </col>
    <tbody>
      <tr>
        <td role="rowheader">[!UICONTROL Nome da Conexão]</td>
        <td>
          <p>Insira um nome para a nova conexão.</p>
        </td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Ambiente]</td>
        <td>
          <p>Selecione se estão se conectando a um ambiente de produção ou não produção.</p>
        </td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Tipo de conexão]</td>
        <td>
          <p>Selecione se você está se conectando a uma conta de serviço ou a uma conta pessoal.</p>
        </td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL ID do Cliente]</td>
        <td>Insira sua ID de cliente do [!DNL Workfront]. Isso pode ser encontrado na área Aplicativos OAuth2 da área Configuração no Workfront. Abra o aplicativo específico ao qual você está se conectando para ver a ID do cliente.</td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Segredo do Cliente]</td>
        <td>Insira sua ID de cliente do [!DNL Workfront]. Isso pode ser encontrado na área Aplicativos OAuth2 da área Configuração no Workfront. Abra o aplicativo específico ao qual você está se conectando para ver a ID do cliente.</td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL URL de Autenticação]</td>
        <td>Isso pode permanecer como o valor padrão, ou você pode inserir a URL da sua instância do Workfront, seguida por <code>/integrations/oauth2</code>. <p>Exemplo: <code>https://mydomain.my.workfront.com/integrations/oauth2</code></p></td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Prefixo de host]</td>
        <td>Na maioria dos casos, esse valor deve ser <code>origin</code>.
      </tr>
    </tbody>
    </table>

1. Clique em **[!UICONTROL Continuar]** para salvar a conexão e retornar ao módulo.




<!--1. Enter the name of your instance into the URL. Example: `https://<your instance>.my.workfront.com`.
1. Click **[!UICONTROL Next]**.
1. Click **[!UICONTROL SAML log in]** to create the connection and go back to the module.

   Or

   Enter your Username and Password, then click **[!UICONTROL Log in]** to create the connection and go back to the module.-->

>[!NOTE]
>
>* Se você não vir um botão de logon SAML, sua organização não habilitou o Logon único (SSO). Você pode fazer logon com seu Nome de usuário e Senha.
>   
>   Para obter mais informações sobre SSO, consulte [Visão geral do logon único em [!DNL Adobe Workfront]](../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md)
>   
>* As conexões OAuth 2.0 para a API [!DNL Workfront] não dependem mais das chaves de API.
>* Para criar uma conexão com um ambiente de sandbox da Workfront, você deve criar um aplicativo OAuth2 nesse ambiente e usar a ID do cliente e o Segredo do cliente gerados por esse aplicativo em sua conexão.
>
>   Para obter instruções sobre como criar um aplicativo OAuth2 no Workfront, consulte [Criar um aplicativo OAuth2 usando credenciais de usuário (Fluxo de código de autorização)](/help/quicksilver/administration-and-setup/configure-integrations/create-oauth-application.md#create-an-oauth2-application-using-user-credentials-authorization-code-flow) no artigo Criar aplicativos OAuth2 para integrações do Workfront.

## [!DNL Workfront] módulos e seus campos

Ao configurar módulos do [!DNL Workfront], o [!DNL Workfront Fusion] exibe os campos listados abaixo. Junto com esses, campos [!DNL Workfront] adicionais podem ser exibidos, dependendo de fatores como seu nível de acesso no aplicativo ou serviço. Um título em negrito em um módulo indica um campo obrigatório.

Se você vir o botão de mapa acima de um campo ou função, poderá usá-lo para definir variáveis e funções para esse campo. Para obter mais informações, consulte [Mapear informações de um módulo para outro em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).


![](assets/map-toggle-350x74.png)

>[!NOTE]
>
>* Se você não vir os campos mais atualizados em um módulo do Workfront, isso pode ser devido a problemas de cache. Aguarde uma hora e tente novamente.
>* Os códigos de status HTTP 429 do Adobe Workfront não devem causar desativações, mas acionar uma pausa de execução curta no cenário.

* [Acionadores](#triggers)
* [Ações](#actions)
* [Pesquisas](#searches)

### Triggers

<!--
* [Watch Events](#watch-events) 
* [Watch Record](#watch-record) 
* [Watch Field](#watch-field)
-->

+++ **[!UICONTROL Assistir a Eventos]**

Esse módulo de acionador executa um cenário em tempo real quando objetos de um tipo específico são adicionados, atualizados ou excluídos no Workfront

O módulo retorna quaisquer campos padrão associados ao registro, juntamente com quaisquer campos e valores personalizados que a conexão acessa. Você pode mapear essas informações em módulos subsequentes no cenário.

1. Clique em **[!UICONTROL Adicionar]** à direita da caixa **Webhook**.

1. Configure o webhook na caixa **[!UICONTROL Adicionar um gancho]** que é exibida.

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
      <td> <p>Para obter instruções sobre como conectar seu aplicativo [!DNL Workfront] ao [!DNL Workfront Fusion], consulte <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Workfront] ao [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Tipo de Registro]</td> 
      <td>Selecione o tipo de registro [!DNL Workfront] que você deseja que o módulo assista.</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Estado]</td> 
      <td>Selecione se deseja observar o estado antigo ou o novo estado.<ul><li><p><b>[!UICONTROL Novo estado]</b></p><p>Acione um cenário quando o registro alterar <b>para</b> um determinado valor.</p><p>Por exemplo, se o estado estiver definido como [!UICONTROL Novo Estado] e o filtro estiver definido como [!UICONTROL Status] [!UICONTROL Igual a] [!UICONTROL Em Andamento], o webhook acionará um cenário quando o [!UICONTROL Status] for alterado para [!UICONTROL Em Andamento], independentemente do status anterior. </p></li><li><p><b>[!UICONTROL Estado antigo]</b></p><p>Acione um cenário quando o registro alterar <b>de</b> um determinado valor.</p><p>Por exemplo, se o estado estiver definido como [!UICONTROL Estado Antigo] e o filtro estiver definido como [!UICONTROL Status] [!UICONTROL Igual a] [!UICONTROL Em Andamento], o webhook acionará um cenário quando um [!UICONTROL Status] atual [!UICONTROL Em Andamento] for alterado para outro status. </p></li></ul></td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td> <p>[!UICONTROL Eventos filtros]</p> </td> 
      <td> <p>É possível definir filtros para observar apenas os registros que atendem aos critérios selecionados.</p> <p>Para cada filtro, insira o campo que deseja que o filtro avalie, o operador e o valor que deseja que o filtro permita. Você pode usar mais de um filtro adicionando regras AND.</p> <p>Observação: não é possível editar filtros em webhooks [!DNL Workfront] existentes. Para configurar filtros diferentes para assinaturas de evento [!DNL Workfront], remova o webhook atual e crie um novo.</p> <p>Para obter mais informações sobre filtros de evento, consulte <a href="#event-subscription-filters-in-the-workfront-watch-events-modules" class="MCXref xref">Filtros de assinatura de evento nos módulos [!DNL Workfront] &gt; [!UICONTROL Watch Events]</a> neste artigo.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td>Excluir eventos feitos por esta conexão</td> 
      <td>Habilite essa opção para excluir eventos criados ou atualizados usando o mesmo conector que esse módulo de acionador usa. Isso pode evitar situações em que um cenário pode ser acionado, fazendo com que ele se repita em um loop infinito.<p><b>OBSERVAÇÃO</b>O tipo de registro Atribuição não inclui essa opção.</p></td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Origem do Registro]</td> 
      <td> <p>Escolha se deseja que o cenário assista a <strong>[!UICONTROL Novos Registros Somente]</strong>, <strong>[!UICONTROL Registros Atualizados Somente]</strong>, <strong>[!UICONTROL Registros Novos e Atualizados]</strong> ou <strong>[!DNL Deleted Records Only]</strong>.</p> <p>Observação: se você escolher <strong>[!UICONTROL Registros novos e atualizados]</strong>, a criação do webhook criará 2 assinaturas de evento (para o mesmo endereço do webhook).</p> </td> 
     </tr> 
    </tbody> 
   </table>

Depois que o webhook for criado, você poderá exibir o endereço do endpoint para o qual os eventos são enviados.

Para obter mais informações, consulte a seção [Exemplos de cargas de evento](../../wf-api/general/event-subs-api.md#examples-of-event-payloads) no [!DNL Workfront] artigo de ajuda [API de assinatura de evento](../../wf-api/general/event-subs-api.md).

Veja uma lista dos [!DNL Workfront] tipos de objetos para os quais você pode usar este módulo em [[!DNL Workfront] tipos de objetos disponíveis para cada [!DNL Workfront] módulo](#workfront-object-types-available-for-each-workfront-module).

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
   <td> <p>Para obter instruções sobre como conectar seu aplicativo [!DNL Workfront] ao [!DNL Workfront Fusion], consulte <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Workfront] ao [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipo de Registro]</td> 
   <td> <p>Selecione o tipo de registro [!DNL Workfront] que você deseja que o módulo assista.</p> <p>Por exemplo, selecione [!UICONTROL Tarefa] se desejar começar a executar o cenário sempre que um campo de registro for atualizado em uma tarefa.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Campo]</td> 
   <td>Selecione o campo que você deseja que o módulo veja por atualizações. Esses campos refletem os campos que o administrador do [!DNL Workfront] configurou para rastreamento.</td> 
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

Veja uma lista dos [!DNL Workfront] tipos de objetos para os quais você pode usar este módulo em [[!DNL Workfront] tipos de objetos disponíveis para cada [!DNL Workfront] módulo](#workfront-object-types-available-for-each-workfront-module).

+++

+++ **[!UICONTROL Assistir ao Registro]**

Esse módulo de acionamento executa um cenário quando objetos de um tipo específico são adicionados, atualizados ou ambos. O módulo retorna todos os campos padrão associados ao registro ou aos registros, juntamente com quaisquer campos e valores personalizados que a conexão acesse. Você pode mapear essas informações em módulos subsequentes no cenário. Na saída, o módulo indica se cada registro é novo ou atualizado.

Os registros que foram adicionados e atualizados no período determinado são retornados como novos registros.

Ao configurar esse módulo, os campos a seguir são exibidos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão]</td> 
   <td> <p>Para obter instruções sobre como conectar seu aplicativo [!DNL Workfront] ao [!DNL Workfront Fusion], consulte <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Workfront] ao [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filtro]</td> 
   <td> <p>Escolha se deseja que o cenário assista a <strong>[!UICONTROL Novos Registros Somente]</strong>, <strong>[!UICONTROL Registros Atualizados Somente]</strong> ou <strong>[!UICONTROL Registros Novos e Atualizados]</strong>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de Registro]</td> 
   <td> <p>(Exibido depois que você escolhe um <strong>Filtro</strong>.) Selecione o tipo de registro [!DNL Workfront] que deseja que o módulo assista.</p> <p>Por exemplo, se você deseja iniciar o cenário sempre que um novo projeto for criado, selecione [!UICONTROL Projeto]</p> </td> 
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

Veja uma lista dos [!DNL Workfront] tipos de objetos para os quais você pode usar este módulo em [[!DNL Workfront] tipos de objetos disponíveis para cada [!DNL Workfront] módulo](#workfront-object-types-available-for-each-workfront-module).

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

>[!NOTE]
>
>A partir de julho de 2024, formulários personalizados poderão ser incluídos ao converter um objeto.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexão]</td> 
   <td> <p>Para obter instruções sobre como conectar seu aplicativo [!DNL Workfront] ao [!DNL Workfront Fusion], consulte <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Workfront] ao [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
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
   <td>[!UICONTROL &lt;Objeto&gt; ID]</td> 
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
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Copiar campos nativos]</td> 
   <td> <p>Ative esta opção para copiar quaisquer campos nativos do objeto original para o novo objeto.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Copiar formulários personalizados]</td> 
   <td> <p>Ative esta opção para copiar quaisquer campos nativos do objeto original para o novo objeto.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Criar um registro (anexar formulários personalizados)]**

Este módulo de ação cria um objeto, como um projeto, tarefa ou problema no [!DNL Workfront], e permite que você adicione um formulário personalizado ao novo objeto. O módulo permite selecionar quais dos campos do objeto estão disponíveis no módulo.

Especifique a ID do registro.

O módulo retorna a ID do registro e quaisquer campos associados, juntamente com quaisquer campos e valores personalizados que a conexão acessa. Você pode mapear essas informações em módulos subsequentes no cenário.

Você poderia usar este módulo, por exemplo, para criar uma tarefa em [!DNL Workfront] quando um cliente adiciona uma nova linha em uma lista [!DNL Google Sheets] de tarefas que precisam ser feitas.

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
   <td> <p>Para obter instruções sobre como conectar seu aplicativo [!DNL Workfront] ao [!DNL Workfront Fusion], consulte <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Workfront] ao [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipo de Registro]</td> 
   <td> <p>Selecione o tipo de registro [!DNL Workfront] que você deseja que o módulo crie.</p> <p>Por exemplo, se você deseja criar um Projeto, selecione [!UICONTROL Project] na lista suspensa e verifique se você tem acesso aos dados (dos módulos anteriores no cenário) que preencherão o projeto.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Selecionar campos a serem mapeados]</td> 
   <td> <p>Selecione os campos que deseja disponibilizar para entrada de dados. Isso permite usar esses campos sem precisar percorrer os que não são necessários.</p> <p>Para campos em formulários personalizados, use o campo <b>[!UICONTROL Anexar Formulário Personalizado]</b>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Anexar Formulário Personalizado]</td> 
   <td>Selecione quaisquer formulários personalizados que deseja adicionar ao novo objeto e insira valores para esses campos.</td> 
  </tr> 
 </tbody> 
</table>

Veja uma lista dos [!DNL Workfront] tipos de objetos para os quais você pode usar este módulo em [[!DNL Workfront] tipos de objetos disponíveis para cada [!DNL Workfront] módulo](#workfront-object-types-available-for-each-workfront-module).

>[!NOTE]
>
>* Ao inserir a ID de um objeto, você pode começar a digitar o nome do objeto e, em seguida, selecioná-lo na lista. O módulo insere a ID apropriada no campo.
>* Ao inserir o texto para um campo personalizado ou um objeto [!UICONTROL Nota] (Comentário ou resposta), você pode usar as marcas HTML no campo [!UICONTROL Texto da Nota] para criar rich text, como negrito ou itálico.
>
>  Para obter mais informações sobre rich text em atualizações, consulte [Adicionar uma atualização a um item de trabalho](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#add) em [Atualizar trabalho](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).
>

+++

+++ **[!UICONTROL Criar Registro]**

Esse módulo de ação cria um objeto, como um projeto, tarefa ou problema no Workfront. O módulo permite selecionar quais dos campos do objeto estão disponíveis no módulo.

Especifique a ID do registro.

O módulo retorna a ID do registro e quaisquer campos associados, juntamente com quaisquer campos e valores personalizados que a conexão acessa. Você pode mapear essas informações em módulos subsequentes no cenário.

Você poderia usar este módulo, por exemplo, para criar uma tarefa no [!DNL Workfront] quando um cliente adiciona uma nova linha em uma lista de tarefas do Google Sheets que precisam ser feitas.

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
   <td> <p>Para obter instruções sobre como conectar seu aplicativo [!DNL Workfront] ao [!DNL Workfront Fusion], consulte <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Workfront] ao [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipo de Registro]</td> 
   <td> <p>Selecione o tipo de registro [!DNL Workfront] que você deseja que o módulo crie.</p> <p>Por exemplo, se você deseja criar um Projeto, selecione [!UICONTROL Project] na lista suspensa e verifique se você tem acesso aos dados (dos módulos anteriores no cenário) que preencherão o projeto.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Selecionar campos a serem mapeados]</td> 
   <td>Selecione os campos que deseja disponibilizar para entrada de dados. Isso permite usar esses campos sem precisar percorrer os que não são necessários.</td> 
  </tr> 
 </tbody> 
</table>

Veja uma lista dos [!DNL Workfront] tipos de objetos para os quais você pode usar este módulo em [[!DNL Workfront] tipos de objetos disponíveis para cada [!DNL Workfront] módulo](#workfront-object-types-available-for-each-workfront-module).

>[!NOTE]
>
>* Ao inserir a ID de um objeto, você pode começar a digitar o nome do objeto e, em seguida, selecioná-lo na lista. O módulo insere a ID apropriada no campo.
>* Ao inserir o texto para um campo personalizado ou um objeto [!UICONTROL Nota] (Comentário ou resposta), você pode usar as marcas HTML no campo [!UICONTROL Texto da Nota] para criar rich text, como negrito ou itálico.
>
>  Para obter mais informações sobre rich text em atualizações, consulte [Adicionar uma atualização a um item de trabalho](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#add) em [Atualizar trabalho](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).
>

+++

+++ **[!UICONTROL Chamada de API personalizada]**

Este módulo de ação permite fazer uma chamada autenticada personalizada para a API [!DNL Workfront]. Dessa forma, você pode criar uma automação de fluxo de dados que não pode ser realizada pelos outros módulos do [!DNL Workfront].

O módulo retorna as seguintes informações:

* **[!UICONTROL Código de Status]** (número): indica o sucesso ou a falha da sua solicitação HTTP. Esses são códigos padrão que você pode pesquisar na Internet.
* **[!UICONTROL Cabeçalhos]** (objeto): um contexto mais detalhado para o código de resposta/status que não está relacionado ao corpo de saída. Nem todos os cabeçalhos que aparecem em um cabeçalho de resposta são cabeçalhos de resposta, portanto, alguns podem não ser úteis para você.

  Os cabeçalhos de resposta dependem da solicitação HTTP escolhida ao configurar o módulo.

* **[!UICONTROL Corpo]** (objeto): dependendo da solicitação HTTP escolhida ao configurar o módulo, você poderá receber alguns dados de volta. Esses dados, como os dados de uma solicitação GET, estão contidos neste objeto.

Você pode mapear essas informações em módulos subsequentes no cenário.

Ao configurar esse módulo, os campos a seguir são exibidos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão]</td> 
   <td> <p>Para obter instruções sobre como conectar seu aplicativo [!DNL Workfront] ao [!DNL Workfront Fusion], consulte <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Workfront] ao [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">URL</td> 
   <td> <p>Insira um caminho relativo a <code> https://&lt;WORKFRONT_DOMAIN&gt;/attask/api/&lt;API_VERSION&gt;/</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Versão da API]</td> 
   <td>Selecione a versão da API [!DNL Workfront] que você deseja que o módulo use.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Método]</td> 
   <td> <p>Selecione o método de solicitação HTTP necessário para configurar a chamada de API. Para obter mais informações, consulte <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">Métodos de solicitação HTTP em [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cabeçalhos]</td> 
   <td> <p>Adicione os cabeçalhos da solicitação no formulário de um objeto JSON padrão. Isso determina o tipo de conteúdo da solicitação.</p> <p>Por exemplo,<code> {"Content-type":"application/json"}</code></p> <p>Observação: se você estiver recebendo erros e for difícil determinar sua origem, considere modificar cabeçalhos com base na documentação [!DNL Workfront]. Se sua Chamada de API personalizada retornar um Erro de solicitação HTTP 422, tente usar um cabeçalho <code>"Content-Type":"text/plain"</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cadeia de Consulta]</td> 
   <td> <p>Adicione a consulta da chamada à API na forma de um objeto JSON padrão.</p> <p>Por exemplo: <code>{"name":"something-urgent"}</code></p> <p>Dica: recomendamos que você envie informações por meio do corpo JSON, em vez de como parâmetros de consulta.</p> </td> 
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

Veja uma lista dos [!DNL Workfront] tipos de objetos para os quais você pode usar este módulo em [[!DNL Workfront] tipos de objetos disponíveis para cada [!DNL Workfront] módulo](#workfront-object-types-available-for-each-workfront-module).

+++

+++ **[!UICONTROL Excluir Registro]**

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
   <td> <p>Para obter instruções sobre como conectar seu aplicativo [!DNL Workfront] ao [!DNL Workfront Fusion], consulte <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Workfront] ao [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Forçar exclusão]</td> 
   <td>Habilite esta opção para garantir que o registro seja excluído, mesmo que a interface do usuário do [!DNL Workfront] solicite confirmação da exclusão.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>ID</td> 
   <td> <p>Insira a ID [!DNL Workfront] exclusiva do registro que você deseja que o módulo exclua.</p> <p>Para obter a ID, abra o objeto [!DNL Workfront] no navegador e copie o texto no final da URL após "ID=". Por exemplo: https://my.workfront.com/project/view?ID=<i>5e43010c03286a2a555e1d0a75d6a86e</i></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipo de Registro]</td> 
   <td>Selecione o tipo de registro [!DNL Workfront] que você deseja que o módulo exclua.</td> 
  </tr> 
 </tbody> 
</table>

Veja uma lista dos [!DNL Workfront] tipos de objetos para os quais você pode usar este módulo em [[!DNL Workfront] tipos de objetos disponíveis para cada [!DNL Workfront] módulo](#workfront-object-types-available-for-each-workfront-module).

>[!NOTE]
>
>Recomendamos a configuração do cenário a seguir para evitar a possibilidade de registros não serem excluídos devido a operações assíncronas.
>
>1. Excluir o registro de forma síncrona.
>1. Adicione a manipulação de erros ao módulo Delete Record para Ignorar o erro causado pelo tempo limite de 40 segundos.


+++

+++ **[!UICONTROL Baixar Documento]**

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
   <td> <p>Para obter instruções sobre como conectar seu aplicativo [!DNL Workfront] ao [!DNL Workfront Fusion], consulte <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Workfront] ao [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID de Documento]</td> 
   <td> <p>Mapeie ou insira manualmente a ID [!DNL Workfront] exclusiva do documento que você deseja que o módulo baixe.</p> <p>Para obter a ID, abra o objeto [!DNL Workfront] no navegador e copie o texto no final da URL após "ID=". Por exemplo: https://my.workfront.com/project/view?ID=<i>5e43010c03286a2a555e1d0a75d6a86e</i></p> </td> 
  </tr> 
 </tbody> 
</table>

Veja uma lista dos [!DNL Workfront] tipos de objetos para os quais você pode usar este módulo em [[!DNL Workfront] tipos de objetos disponíveis para cada [!DNL Workfront] módulo](#workfront-object-types-available-for-each-workfront-module).

+++

+++ **[!UICONTROL Ações diversas]**

Esse módulo de ação permite executar ações na API.

>[!NOTE]
>
>A partir de julho de 2024, a ação `convertToProject` inclui o campo `copyCategories`. Quando definido como `TRUE`, todos os formulários personalizados serão incluídos no projeto para o qual o problema é convertido.

Ao configurar esse módulo, os campos a seguir são exibidos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexão]</td> 
   <td> <p>Para obter instruções sobre como conectar seu aplicativo [!DNL Workfront] ao [!DNL Workfront Fusion], consulte <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Workfront] ao [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Tipo de Registro]</td> 
   <td> <p>Selecione o tipo de registro [!DNL Workfront] com o qual você deseja que o módulo interaja.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Ação]</td> 
   <td> <p>Selecione a ação que deseja que o módulo execute.</p> <p>Talvez seja necessário preencher campos adicionais, dependendo do [!UICONTROL Record Type] e da [!UICONTROL Action] escolhidos. Algumas combinações dessas duas configurações podem exigir apenas uma ID de registro, enquanto outras (como Projeto para o <strong>[!UICONTROL Tipo de Registro]</strong> e [!UICONTROL Anexar Modelo] para a <strong>[!UICONTROL Ação]</strong>) exigem informações adicionais (como uma ID de Objeto e uma ID de Modelo).</p><p>Para opções disponíveis para algumas ações, consulte <a href="#misc-action-options" class="MCXref xref">Opções de ações diversas</a> neste artigo.</p> <p>Para obter detalhes sobre campos individuais, consulte a <a href="http://developer.workfront.com/">documentação para desenvolvedor do Workfront</a>. <p><strong>Observação</strong>: o site de documentação do desenvolvedor inclui informações somente da API versão 14, mas ainda contém informações valiosas para chamadas de API. </p> 
    <ol> 
     <li value="1"> <p>Selecione o tipo de registro na navegação à esquerda na página de documentação do desenvolvedor [!DNL Workfront]. Os seguintes tipos têm suas próprias páginas:</p> 
      <ul> 
       <li> <p>[!UICONTROL Projetos]</p> </li> 
       <li> <p>[!UICONTROL Tarefas]</p> </li> 
       <li> <p>[!UICONTROL Problemas]</p> </li> 
       <li> <p>[!UICONTROL Usuários]</p> </li> 
       <li> <p>[!UICONTROL Documentos]</p> </li> 
      </ul> <p>Para todos os outros tipos de registro, selecione <b>[!UICONTROL Outros objetos e pontos de extremidade]</b> e localize o tipo de registro nas páginas classificadas alfabeticamente.</p> </li> 
     <li value="2"> <p>Na página do tipo de registro apropriado, pesquise (Ctrl-F ou Cmd-F) a ação.</p> </li> 
     <li value="3"> <p>Exibir descrições para campos disponíveis sob a ação selecionada.</p> </li> 
    </ol> <p>Nota:  <p>Ao criar uma prova por meio do módulo [!DNL Workfront] [!UICONTROL Misc Action], a prática recomendada é criar uma prova sem nenhuma opção avançada e, em seguida, atualizar a prova usando a API SOAP [!DNL Workfront Proof].</p> <p>Para obter mais informações sobre como criar uma prova com a API [!DNL Workfront] (que este módulo usa), consulte <a href="../../wf-api/tips-tricks-and-troubleshooting/api-create-proof-options-json.md" class="MCXref xref">Adicionar opções de prova avançada ao criar uma prova por meio da API [!DNL Adobe Workfront]</a></p> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL ID]</td> 
   <td>Insira ou mapeie a ID exclusiva [!DNL Workfront] do registro com a qual você deseja que o módulo interaja.<p>Para obter a ID, abra o objeto [!DNL Workfront] no navegador e copie o texto no final da URL após "ID=". Por exemplo: https://my.workfront.com/project/view?ID=<i>5e43010c03286a2a555e1d0a75d6a86e</i></p></td> 
  </tr> 
 </tbody> 
</table>

Veja uma lista dos [!DNL Workfront] tipos de objetos para os quais você pode usar este módulo em [[!DNL Workfront] tipos de objetos disponíveis para cada [!DNL Workfront] módulo](#workfront-object-types-available-for-each-workfront-module).

#### Opções de ação diversas

##### Tarefa

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <th>Ação</th> 
   <th>Opções</th> 
  </tr> 
  <tr> 
   <td>Copiar</td> 
   <td>
   <ul>
   <li>clearApprovers</li>
   <li>clearAssignments</li>
   <li>clearConstraints</li>
   <li>clearCustomData</li>
   <li>clearDocuments</li>
   <li>clearExpenses</li>
   <li>clearFinancials<p>Limpa dados financeiros</p></li>
   <li>clearPermissions</li>
   <li>clearPredecessors</li>
   <li>clearProgress</li>
   <li>clearTimedNotifications<p>Limpa as notificações de lembrete</p></li>
   </ul>
   </td> 
  </tr> 
  <tr> 
   <td>Mover</td> 
   <td>
   <ul>
   <li>clearApprovers</li>
   <li>clearAssignments</li>
   <li>clearDocuments</li>
   <li>clearConstraints</li>
   <li>clearExpenses</li>
   <li>clearFinancials<p>Limpa dados financeiros</p></li>
   <li>clearPermissions</li>
   <li>clearPredecessors</li>
   <li>clearProgress</li>
   <li>clearTimedNotifications<p>Limpa as notificações de lembrete</p></li>
   </ul>
   </td> 
  </tr> 
 </tbody> 
</table>

##### Problema

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <th>Ação</th> 
   <th>Opções</th> 
  </tr> 
  <tr> 
   <td>Copiar</td> 
   <td>
   <ul>
   <li>clearApprovers</li>
   <li>clearAssignments</li>
   <li>clearCustomData</li>
   <li>clearDocuments</li>
   <li>clearPermissions</li>
   <li>clearProgress</li>
   </ul>
   </td> 
  </tr> 
  <tr> 
   <td>Converter em tarefa</td> 
   <td>
   <ul>
   <li>preserveIssue<p>Conservar o problema original e vincular a sua resolução a esta tarefa</p></li>
   <li>preservePrimaryContact<p>Permitir que o contato primário do problema acesse esta tarefa</p></li>
   <li>preserveCompletionDate<p>Manter a data de conclusão planejada do problema</p></li>
   </ul>
   </td> 
  </tr> 
  <tr> 
   <td>Converter em projeto</td> 
   <td>
   <ul>
   <li>preserveIssue<p>Conservar o problema original e vincular a sua resolução a esta tarefa</p></li>
   <li>preservePrimaryContact<p>Permitir que o contato primário do problema acesse esta tarefa</p></li>
   </ul>
   </td> 
  </tr> 
 </tbody> 
</table>



##### Projeto

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <th>Ação</th> 
   <th>Opções</th> 
  </tr> 
  <tr> 
   <td>Copiar</td> 
   <td>
   <ul>
   <li>clearApprovers</li>
   <li>clearAssignments</li>
   <li>clearCustomData</li>
   <li>clearDocuments</li>
   <li>clearExpenses</li>
   <li>clearFinancials<p>Limpa dados financeiros</p></li>
   <li>clearPermissions</li>
   <li>clearPredecessors</li>
   <li>clearProgress</li>
   <li>clearTimedNotifications<p>Limpa as notificações de lembrete</p></li>
   </ul>
   </td> 
  </tr> 
  <tr> 
   <td>Anexar modelo / Salvar como modelo</td> 
   <td>
   <ul>
   <li>clearApprovers</li>
   <li>clearAssignments</li>
   <li>clearBillingRates</li>
   <li>clearConstraints</li>
   <li>clearDeliverables<p>Limpa metas</p></li>
   <li>clearDocuments</li>
   <li>clearExpenses</li>
   <li>clearFinancials<p>Limpa dados financeiros</p></li>
   <li>clearHourTypes</li>
   <li>clearIssueSetup<p>Limpa as propriedades da fila e a configuração de problemas</p></li>
   <li>clearPredecessors</li>
   <li>clearRisks</li>
   <li>clearSharingOptions</li>
   <li>clearTimedNotifications<p>Limpa as notificações de lembrete</p></li>
   </ul>
   </td> 
  </tr> 
 </tbody> 
</table>



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
    <td> <p>Para obter instruções sobre como conectar seu aplicativo [!DNL Workfront] ao [!DNL Workfront Fusion], consulte <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Workfront] ao [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
    <td>[!UICONTROL Tipo de Registro]</td>
     <td>Escolha o tipo de objeto [!DNL Workfront] que você deseja que o módulo leia.</td> 
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
   <td> <p>Insira a ID [!DNL Workfront] exclusiva do registro que você deseja que o módulo leia.</p> <p>Para obter a ID, abra o objeto [!DNL Workfront] no navegador e copie o texto no final da URL após "ID=". Por exemplo: https://my.workfront.com/project/view?ID=<i>5e43010c03286a2a555e1d0a75d6a86e</i></p> </td> 
  </tr> 
 </tbody> 
</table>

Veja uma lista dos [!DNL Workfront] tipos de objetos para os quais você pode usar este módulo em [[!DNL Workfront] tipos de objetos disponíveis para cada [!DNL Workfront] módulo](#workfront-object-types-available-for-each-workfront-module).

+++

+++ **[!UICONTROL Atualizar Registro]**

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
   <td> <p>Para obter instruções sobre como conectar seu aplicativo [!DNL Workfront] ao [!DNL Workfront Fusion], consulte <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Workfront] ao [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL ID]</td> 
   <td> <p>Insira a ID [!DNL Workfront] exclusiva do registro que você deseja que o módulo atualize.</p> <p>Para obter a ID, abra o objeto [!DNL Workfront] no navegador e copie o texto no final da URL após "ID=". Por exemplo: https://my.workfront.com/project/view?ID=<i>5e43010c03286a2a555e1d0a75d6a86e</i></p> </td> 
  </tr> 
  <tr> 
   <td>[!DNL Record Type]</td> 
   <td> <p>Selecione o tipo de registro [!DNL Workfront] que você deseja que o módulo atualize.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!DNL Select fields to map]</td> 
   <td>Selecione os campos que deseja disponibilizar para entrada de dados. Isso permite usar esses campos sem precisar percorrer os que não são necessários.</td> 
  </tr> 
 </tbody> 
</table>

Veja uma lista dos [!DNL Workfront] tipos de objetos para os quais você pode usar este módulo em [[!DNL Workfront] tipos de objetos disponíveis para cada [!DNL Workfront] módulo](#workfront-object-types-available-for-each-workfront-module).

>[!NOTE]
>
>* Ao inserir a ID de um objeto, você pode começar a digitar o nome do objeto e, em seguida, selecioná-lo na lista. O módulo insere a ID apropriada no campo.
>* Ao inserir o texto para um campo personalizado ou um objeto [!UICONTROL Nota] (Comentário ou resposta), você pode usar as marcas HTML no campo [!UICONTROL Texto da Nota] para criar rich text, como negrito ou itálico.
>
>  Para obter mais informações sobre rich text em atualizações, consulte [Adicionar uma atualização a um item de trabalho](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#add) em [Atualizar trabalho](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).
>

+++

+++ **[!UICONTROL Carregar documento]**

Este módulo de ação carrega um documento para um objeto [!DNL Workfront], como um projeto, tarefa ou problema. Esse módulo carrega o documento em partes, o que torna o processo de upload mais suave para o Workfront.

Especifique o local do documento, o arquivo que deseja fazer upload e um novo nome opcional para o arquivo.

O módulo retorna a ID do documento e quaisquer campos associados, juntamente com quaisquer campos e valores personalizados que a conexão acessa. Você pode mapear essas informações em módulos subsequentes no cenário.

Ao configurar esse módulo, os campos a seguir são exibidos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexão]</td> 
   <td> <p>Para obter instruções sobre como conectar seu aplicativo [!DNL Workfront] ao [!DNL Workfront Fusion], consulte <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Workfront] ao [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL ID de Registro Relacionado]</td> 
   <td>Insira a ID [!DNL Workfront] exclusiva do registro para o qual você deseja carregar o documento.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipo de Registro Relacionado]</td> 
   <td>Selecione o tipo de registro [!DNL Workfront] no qual você deseja que o módulo carregue o documento.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID da Pasta]</td> 
   <td>Dependendo do tipo de registro relacionado, talvez seja necessário inserir ou mapear uma ID de pasta.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL arquivo Source]</td> 
   <td> <p>Selecione um arquivo de origem de um módulo anterior ou mapeie o nome e os dados do arquivo de origem.</p> </td> 
  </tr> 
 </tbody> 
</table>

Veja uma lista dos [!DNL Workfront] tipos de objetos para os quais você pode usar este módulo em [[!DNL Workfront] tipos de objetos disponíveis para cada [!DNL Workfront] módulo](#workfront-object-types-available-for-each-workfront-module).

+++

+++ **[!UICONTROL Carregar Documento (Herdado)]**

Este módulo de ação carrega um documento para um objeto [!DNL Workfront], como um projeto, tarefa ou problema. Ele carrega o documento inteiro de uma só vez.

Especifique o local do documento, o arquivo que deseja fazer upload e um novo nome opcional para o arquivo.

O módulo retorna a ID do documento e quaisquer campos associados, juntamente com quaisquer campos e valores personalizados que a conexão acessa. Você pode mapear essas informações em módulos subsequentes no cenário.

Ao configurar esse módulo, os campos a seguir são exibidos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexão]</td> 
   <td> <p>Para obter instruções sobre como conectar seu aplicativo [!DNL Workfront] ao [!DNL Workfront Fusion], consulte <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Workfront] ao [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL ID de Registro Relacionado]</td> 
   <td>Insira a ID [!DNL Workfront] exclusiva do registro para o qual você deseja carregar o documento.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipo de Registro Relacionado]</td> 
   <td>Selecione o tipo de registro [!DNL Workfront] no qual você deseja que o módulo carregue o documento.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID da Pasta]</td> 
   <td>Dependendo do tipo de registro relacionado, talvez seja necessário inserir ou mapear uma ID de pasta.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL arquivo Source]</td> 
   <td> <p>Selecione um arquivo de origem de um módulo anterior ou mapeie o nome e os dados do arquivo de origem.</p> </td> 
  </tr> 
 </tbody> 
</table>

Veja uma lista dos [!DNL Workfront] tipos de objetos para os quais você pode usar este módulo em [[!DNL Workfront] tipos de objetos disponíveis para cada [!DNL Workfront] módulo](#workfront-object-types-available-for-each-workfront-module).

+++

### Pesquisas

<!--
* [Read Related Records](#read-related-records) 
* [Search](#search)
-->

+++ **[!UICONTROL Ler Registros Relacionados]**

Esse módulo de pesquisa lê registros que correspondem à consulta de pesquisa especificada em um determinado objeto pai.

Você especifica quais campos deseja incluir na saída. Você pode mapear essas informações em módulos subsequentes no cenário.

Ao configurar esse módulo, os campos a seguir são exibidos.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexão]</td> 
   <td> <p>Para obter instruções sobre como conectar seu aplicativo [!DNL Workfront] ao [!DNL Workfront Fusion], consulte <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Workfront] ao [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Tipo de Registro]</td> 
   <td> <p>Selecione o tipo do registro pai (objeto Workfront) cujos registros associados você deseja ler.</p> <p>Consulte uma lista dos [!DNL Workfront] tipos de objetos para os quais você pode usar este módulo em <a href="#object-types-available-for-each-workfront-search-module" class="MCXref xref">[!DNL Workfront] tipos de objetos disponíveis para cada [!DNL Workfront] módulo</a> neste artigo.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL ID de Registro Pai]</td> 
   <td> <p>Informe ou mapeie o ID do registro-pai cujos registros associados você deseja ler.</p> <p>Para obter a ID, abra o objeto [!DNL Workfront] no navegador e copie o texto no final da URL após "ID=". Por exemplo: https://my.workfront.com/project/view?ID=<i>5e43010c03286a2a555e1d0a75d6a86e</i></p> </td> 
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

Este módulo de pesquisa procura registros em um objeto em [!DNL Workfront] que correspondam à consulta de pesquisa especificada.

Você pode mapear essas informações em módulos subsequentes no cenário.

Ao configurar esse módulo, os campos a seguir são exibidos.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexão]</td> 
   <td> <p>Para obter instruções sobre como conectar seu aplicativo [!DNL Workfront] ao [!DNL Workfront Fusion], consulte <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Workfront] ao [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipo de Registro]</td> 
   <td> <p>Selecione o tipo de registro [!DNL Workfront] que você deseja que o módulo procure.</p> </td> 
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
   <td>[!UICONTROL Pesquisar campos de critérios]</td> 
   <td> <p>Selecione os campos que deseja usar com os critérios de pesquisa. Esses campos estarão disponíveis na lista suspensa Search criteria.</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Pesquisar critérios]</td> 
   <td> <p>Digite o campo pelo qual deseja pesquisar, o operador que deseja usar na consulta e o valor que está procurando no campo.</p> <p>Observação: não use <code>username </code> nos seus critérios de pesquisa. A inclusão de <code>username </code> em uma consulta de API para [!DNL Workfront] faz com que o usuário entre no Workfront e a pesquisa não será bem-sucedida.</p> <p>Observação: <code>In</code> e <code>NotIn</code>funcionam com matrizes. As entradas devem estar em formato de matriz.</p></td> 
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

+++

+++ **[!UICONTROL Pesquisar (Herdado)]**

Este módulo de pesquisa procura registros em um objeto em [!DNL Workfront] que correspondam à consulta de pesquisa especificada.

Você pode mapear essas informações em módulos subsequentes no cenário.

Ao configurar esse módulo, os campos a seguir são exibidos.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexão]</td> 
   <td> <p>Para obter instruções sobre como conectar seu aplicativo [!DNL Workfront] ao [!DNL Workfront Fusion], consulte <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Workfront] ao [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipo de Registro]</td> 
   <td> <p>Selecione o tipo de registro [!DNL Workfront] que você deseja que o módulo procure.</p> </td> 
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
   <td> <p>Digite o campo pelo qual deseja pesquisar, o operador que deseja usar na consulta e o valor que está procurando no campo.</p> <p>Observação: não use <code>username </code> nos seus critérios de pesquisa. A inclusão de <code>username </code> em uma consulta de API para [!DNL Workfront] faz com que o usuário entre no Workfront e a pesquisa não será bem-sucedida.</p> <p>Observação: <code>In</code> e <code>NotIn</code>funcionam com matrizes. As entradas devem estar em formato de matriz.</p></td> 
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

Veja uma lista dos [!DNL Workfront] tipos de objetos para os quais você pode usar este módulo em [[!DNL Workfront] tipos de objetos disponíveis para cada [!DNL Workfront] módulo](#workfront-object-types-available-for-each-workfront-module).

+++

## [!DNL Workfront] tipos de objetos disponíveis para cada módulo [!DNL Workfront]

<!-- [Object types available for each Workfront trigger module](#object-types-available-for-each-workfront-trigger-module) 
* [Object types available for each Workfront action module](#object-types-available-for-each-workfront-action-module) 
* [Object types available for each Workfront search module](#object-types-available-for-each-workfront-search-module)-->

+++**Tipos de objeto disponíveis para cada módulo de gatilho [!DNL Workfront]**

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
   <td>Marco</td> 
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

+++**Tipos de objeto disponíveis para cada módulo de ação [!DNL Workfront]**

>[!NOTE]
>
>O módulo [!UICONTROL Baixar Documento] não está incluído nesta tabela porque os tipos de objeto [!DNL Workfront] não fazem parte de sua configuração.

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
   <td>Linha de base</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td> </td> 
   <td>✓ µ</td> 
   <td> </td> 
   <td> </td> 
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
   <td> </td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
  </tr> 
  <tr> 
   <td>Taxa de câmbio</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td> </td> 
   <td>✓ µ</td> 
   <td> </td> 
   <td> </td> 
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
   <td>Documento externo</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td>✓ µ</td> 
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
   <td>Marco</td> 
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
   <td> </td> 
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
   <td>Marco</td> 
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

## Filtros de assinatura de evento no módulo [!DNL Workfront] > [!UICONTROL Eventos de observação]

>[!NOTE]
>
>É altamente recomendável usar filtros de assinatura de evento em seus módulos [!UICONTROL Assistir Eventos].

O módulo [!DNL Workfront] [!UICONTROL Assistir Eventos] aciona cenários com base em um webhook que cria uma assinatura de evento na API [!DNL Workfront]. A assinatura do evento é um conjunto de dados que determina quais eventos são enviados para o webhook. Por exemplo, se você configurar um módulo [!UICONTROL Eventos de observação] que esteja observando problemas, a assinatura do evento enviará somente eventos relacionados a problemas.

Ao usar filtros de subscrição de eventos, os usuários do Fusion podem criar subscrições de eventos que são mais adequadas para seus casos de uso. Por exemplo, você pode configurar uma assinatura de evento na API [!DNL Workfront] para enviar ao webhook somente problemas que estão em um projeto específico, garantindo que o módulo [!UICONTROL Assistir Eventos] acionará problemas somente nesse projeto. A capacidade de criar acionadores mais estreitos melhora o design do cenário ao reduzir o número de acionadores irrelevantes.

Isso é diferente da configuração de um filtro no cenário [!DNL Workfront Fusion]. Sem um filtro de inscrição de evento, seu webhook recebe todos os eventos relacionados ao tipo de objeto selecionado. A maioria desses eventos seria irrelevante para o cenário e deve ser filtrada para que o cenário possa continuar.

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
   * Ao usar `Changed`, selecione **Somente Eventos Atualizados** no campo **Origem do Registro**.

>[!IMPORTANT]
>
>Não é possível editar filtros em webhooks [!DNL Workfront] existentes. Para configurar filtros diferentes para assinaturas de evento [!DNL Workfront], remova o webhook atual e crie um novo.

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
>Para filtrar eventos de modo que somente problemas atribuídos a Ana sejam processados, você pode criar um filtro após o módulo [!UICONTROL Assistir Eventos].
>
>![](assets/watch-events-non-event-filter-350x206.png)
>
>Se 100 edições forem criadas em um dia, mas apenas duas delas forem atribuídas a Ana, o cenário seria executado 100 vezes. 98 das execuções parariam no filtro, mas o módulo de acionamento ainda está consumindo dados e executando operações em todas as execuções.

Para obter mais informações sobre assinaturas de eventos, consulte [Perguntas frequentes - Assinaturas de Eventos](../../wf-api/general/event-subs-faq.md).

Para obter mais informações sobre webhooks, consulte [Acionadores instantâneos (webhooks) em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/webhooks/instant-triggers-webhooks.md)

Para obter mais informações sobre filtros em cenários, consulte [Adicionar um filtro a um cenário em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/add-a-filter-to-a-scenario.md).

