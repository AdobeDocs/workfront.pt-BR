---
content-type: api
navigation-topic: api-navigation-topic
title: Novidades da API versão 13
description: A Adobe Workfront lançou a API versão 13 em 22 de abril de 2021. A API versão 13 apresenta as seguintes alterações da versão 12.
author: John
feature: Workfront API
exl-id: afbc986e-8b5c-40bc-9120-e8d34e0f7004
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '1064'
ht-degree: 2%

---

# Novidades da API versão 13

A Adobe Workfront lançou a API versão 13 em 22 de abril de 2021. A API versão 13 apresenta as seguintes alterações da versão 12.

## Recursos adicionados

Nenhum recurso foi adicionado para a API versão 13.

## Recursos removidos

Nenhum recurso foi removido para a API versão 13.

## Recursos modificados

Os recursos a seguir foram modificados para a API versão 13.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> 
    <ul> 
     <li> <p><a href="#accesslevel" class="MCXref xref">AccessLevel</a> </p> </li> 
     <li> <p><a href="#breadcrumb" class="MCXref xref">BreadCrumb</a> </p> </li> 
     <li> <p><a href="#burndownevent" class="MCXref xref">BurndownEvent</a> </p> </li> 
     <li> <p><a href="#customerpreferences" class="MCXref xref">CustomerPreferences</a> </p> </li> 
     <li> <p><a href="#documentversion" class="MCXref xref">DocumentVersion</a> </p> </li> 
     <li> <p><a href="#group" class="MCXref xref">Grupo </a> </p> </li> 
     <li> <p><a href="#journalentry" class="MCXref xref">JournalEntry</a> </p> </li> 
     <li> <p><a href="#layouttemplate" class="MCXref xref">LayoutTemplate</a> </p> </li> 
     <li> <p><a href="#linkedfolder" class="MCXref xref">LinkedFolder</a> </p> </li> 
     <li> <p><a href="#optask" class="MCXref xref">OpTask</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p><a href="#project" class="MCXref xref">Projeto</a> </p> </li> 
     <li> <p><a href="#proofapproval" class="MCXref xref">AprovaçãoDeProva</a> </p> </li> 
     <li> <p><a href="#queuedef" class="MCXref xref">QueueDef</a> </p> </li> 
     <li> <p><a href="#task" class="MCXref xref">Tarefa</a> </p> </li> 
     <li> <p><a href="#team" class="MCXref xref">Equipe</a> </p> </li> 
     <li> <p><a href="#timesheet" class="MCXref xref">Planilha de horas</a> </p> </li> 
     <li> <p><a href="#timesheetprofile" class="MCXref xref">TimesheetProfile</a> </p> </li> 
     <li> <p><a href="#uitemplate" class="MCXref xref">UITemplate</a> </p> </li> 
     <li> <p><a href="#userdelegation" class="MCXref xref">UserDelegate</a> </p> </li> 
     <li> <p><a href="#work" class="MCXref xref">Trabalho </a> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### AccessLevel {#accesslevel}

Um objeto AccessLevel é associado a usuários e descreve o conjunto de AccessLevelPermissions que determina o que o usuário pode acessar.

Para obter mais informações sobre níveis de acesso, consulte [Como os níveis de acesso funcionam](../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels.md).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>Campos Diretos</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>Descrição</b> </p> <p>Adição do validador MAX_LENGTH, que especifica que o comprimento da descrição não é superior a 4000 caracteres.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### BreadCrumb {#breadcrumb}

Um objeto BreadCrumb representa um elemento na hierarquia pai/filho de um item de trabalho do Workfront. As navegações estruturais indicam como um item de trabalho se encaixa na maior estrutura de Portfolio, Projetos, Projetos e Tarefas.

Para obter mais informações sobre navegação estrutural, consulte [Visão geral das navegações estruturais na nova experiência do Adobe Workfront](../../workfront-basics/the-new-workfront-experience/breadcrumb-overview.md)

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>Campos Diretos</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>objCode</b> </p> <p>Os códigos de objeto podem ser encontrados no <a href="../../wf-api/general/api-explorer.md" class="MCXref xref">API Explorer</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### BurndownEvent {#burndownevent}

Um objeto BurndownEvent representa um objeto que altera o pacote de uma iteração.

Para obter mais informações sobre o detalhamento, consulte [Interrupção](../../agile/use-scrum-in-an-agile-team/burndown/burndown.md).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>Campos Diretos</p> </td> 
   <td> <p>Os seguintes campos removeram o sinalizador NOT_GROUPABLE </p> 
    <ul> 
     <li> <p>applyDate</p> </li> 
     <li> <p>entryDate</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### CustomerPreferences {#customerpreferences}

Um objeto CustomerPreferences representa o conjunto de preferências que um cliente definiu para sua instância do Workfront.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campos Diretos</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>name</p> <p style="font-weight: normal;">Valores possíveis adicionados:</p> 
      <ul> 
       <li style="font-weight: normal;">senha:aemAPIKey (config.general.aem.apikey)</li> 
       <li style="font-weight: normal;"> senha:aemAADomain (config.general.aem.adomain) </li> 
       <li style="font-weight: normal;">senha:aemIntegrationEnabled (config.general.aem.enabled)</li> 
       <li style="font-weight: normal;">senha:aemHost (config.general.aem.host)</li> 
       <li style="font-weight: normal;">folha de ponto:default.timesheet.restrict.timesheet.edit.proprietários.admins (config.timesheet.restrict.timesheet.edit.proprietários.admins)</li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Ações</td> 
   <td> <p>As seguintes ações foram adicionadas ao recurso CustomerPreferences.</p> 
    <ul> 
     <li> <p><b>getTimesheetPreferences</b> </p> </li> 
     <li> <p><b>setTimesheetPreferences</b> </p> <p>Pega o argumento :</p> 
      <ul> 
       <li> <p>preferências (mapa)</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### DocumentVersion {#documentversion}

Um objeto DocumentVersion representa uma versão específica de um arquivo (como material gravado, imagens ou outras formas de informações).

Para obter mais informações sobre versões de documentos, consulte [Fazer upload de uma nova versão de um documento](../../documents/managing-documents/upload-new-document-version.md).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>Campos Diretos</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>externalIntegrationType</b> </p> <p>Valor possível adicionado:</p> 
      <ul> 
       <li> <p>AEM (Adobe Experience Manager)</p> </li> 
      </ul> </li> 
    </ul> 
    <ul> 
     <li> <p><b>proofID</b> </p> <p>Adição do sinalizador NOT_FILTERABLE</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Grupo  {#group}

Um objeto Group representa um conjunto de usuários e equipes. Os grupos geralmente representam a estrutura departamental.

Para obter mais informações sobre grupos, consulte [Grupos versus equipes no Adobe Workfront](../../people-teams-and-groups/work-with-groups-and-teams/understanding-differences-and-similarities-between-groups-and-teams.md).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>Ações</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>getParents</b> </p> <p>Essa ação retorna uma matriz dos grupos pai do grupo (grupos dos quais o grupo em questão é um subgrupo).</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### JournalEntry {#journalentry}

O objeto JournalEntry pode ser configurado para registrar informações sobre campos de objeto específicos sempre que esses campos forem modificados. Quando um campo é configurado para ser registrado como parte do objeto Entrada de diário, uma Entrada de diário correspondente é criada toda vez que esse campo é modificado.

O recurso JournalEntry adicionou o sinalizador REPORTABLE.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>Campos Diretos</p> </td> 
   <td> <p>Os seguintes campos removeram o sinalizador NOT_GROUPABLE:</p> 
    <ul> 
     <li> <p><b>changeType</b> </p> </li> 
     <li> <p><b>entryDate</b> </p> </li> 
     <li> <p><b>fieldName</b> </p> </li> 
     <li> <p><b>objObjCode</b> </p> </li> 
    </ul> <p>Os seguintes campos adicionaram o sinalizador NOT_FILTERABLE:</p> 
    <ul> 
     <li> <p><b>subObjCode</b> </p> </li> 
     <li> <p><b>subObjID</b> </p> </li> 
     <li> <p><b>topObjCode</b> </p> </li> 
     <li> <p><b>topObjID</b> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### LayoutTemplate {#layouttemplate}

Os administradores do Adobe Workfront ou administradores de grupo podem criar modelos para personalizar os elementos de layout no Adobe Workfront. O objeto LayoutTemplate é específico do Adobe Workfront Classic.

Para o objeto que representa modelos de layout na nova experiência do Adobe Workfront, consulte [UITemplate](#uitemplate)

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>Campos Diretos</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>Descrição</b> </p> <p>Adição do validador MAX_LENGTH, que especifica que o comprimento da descrição não é superior a 4000 caracteres.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### LinkedFolder {#linkedfolder}

Um objeto LinkedFolder representa uma pasta vinculada a um provedor de documento externo, como Google Drive ou Dropbox.

Para obter mais informações sobre Pastas vinculadas, consulte [Vincular documentos de aplicativos externos](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>Campos Diretos</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>externalIntegrationType</b> </p> <p>Valor possível adicionado:</p> 
      <ul> 
       <li> <p>AEM (Adobe Experience Manager)</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### OpTask {#optask}

Um objeto OpTask é normalmente conhecido como um problema. Um problema é um item de trabalho que geralmente indica que há um problema que impede a conclusão de uma tarefa ou projeto. Um problema também pode ser uma solicitação de suporte técnico. Pedidos de alteração, solicitações e bugs também são problemas.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>Campos de Busca</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>favoritedByUsersMM</b> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Projeto {#project}

Os projetos são itens de trabalho no Workfront e são um elemento essencial na maneira como o Workfront ajuda as pessoas a trabalhar. Um objeto Project representa um grupo de tarefas com um objetivo comum e específico.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>Campos Diretos</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>convertedOpTaskOriginatorID</b> </p> <!--
       <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Removed flag NOT&nbsp;FILTERABLE</p>
      --> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### AprovaçãoDeProva {#proofapproval}

Um objeto ProofApproval representa uma aprovação que está diretamente ligada a uma prova.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>Campos Diretos</p> </td> 
   <td> <p>Os seguintes campos foram adicionados ao recurso ProofApproval .</p> 
    <ul> 
     <li> <p><b>aproverStage</b> </p> </li> 
     <li> <p><b>DataDecisão</b> </p> </li> 
     <li> <p><b>workflowTemplate</b> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### QueueDef {#queuedef}

Um objeto QueueDef representa uma Fila, que é um Projeto que foi publicado na área Help Desk para permitir que os usuários enviem Problemas a ele.

Para obter mais informações sobre as filas de solicitações, consulte [Criar uma fila de solicitações](../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Campos Diretos</td> 
   <td> 
    <ul> 
     <li> <p><b>documentPosition</b> </p> <p>Adicionado. Os valores possíveis são:</p> 
      <ul> 
       <li> <p>0 (Após formulários personalizados)</p> </li> 
       <li> <p>1 (Antes de formulários personalizados)</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Tarefa {#task}

Um objeto Task representa um item de trabalho que deve ser executado como uma etapa para atingir uma meta final (conclusão de um projeto).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>Campos de Busca</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>favoritedByUsersMM</b> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Equipe {#team}

Um objeto Equipe é uma coleção de Usuários que pode ser atribuída a um item de trabalho.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campos Diretos</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">Este campo foi adicionado e é um parâmetro booleano que tem um valor true se um objeto estiver ativo e false se não estiver ativo. Os objetos definidos como Ativo são exibidos nos menus suspensos e nos campos do tipo avançar e podem ser anexados a outros objetos. Os objetos não definidos como Ativo não são visíveis nos menus suspensos e nos campos do tipo avançar para anexar a outros objetos.  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Campos padrão</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">Adicionado</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Planilha de horas {#timesheet}

Um objeto de Folha de Horas representa um cartão de ponto virtual que permite que os usuários insiram horas reais trabalhadas para Tarefas, Projetos e Tipos de Horário de Custo.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campos Diretos</td> 
   <td> 
    <ul> 
     <li> <p><b>isOvertimeDisabled</b> </p> <p>Adicionado</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Campos principais</td> 
   <td> 
    <ul> 
     <li> <p><b>objCode</b> </p> <p>Removido</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### TimesheetProfile {#timesheetprofile}

Um objeto de Folha de Horas representa um cartão de ponto virtual que permite que os usuários insiram horas reais trabalhadas para Tarefas, Projetos e Tipos de Horário de Custo.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campos Diretos</td> 
   <td> 
    <ul> 
     <li> <p><b>isOvertimeDisabled</b> </p> <p>Adicionado</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Campos padrão</td> 
   <td> 
    <ul> 
     <li> <p><b>isOvertimeDisabled</b> </p> <p>Adicionado</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### UITemplate {#uitemplate}

Os administradores do Adobe Workfront ou administradores de grupo podem criar modelos para personalizar os elementos de layout no Adobe Workfront. O objeto LayoutTemplate é específico para a nova experiência do Adobe Workfront.

Para o objeto que representa modelos de layout no Adobe Workfront Classic, consulte [LayoutTemplate](#layouttemplate).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Ações</td> 
   <td> <p>As seguintes ações foram adicionadas ao recurso UITemplate .</p> 
    <ul> 
     <li> <p><b>migrarCustomersAllLayoutTemplates</b> </p> <p>Pega o argumento :</p> 
      <ul> 
       <li> <p>overrideIfExists (booleano)</p> </li> 
      </ul> </li> 
     <li> <p><b>migrarLayoutModelos</b> </p> <p>Pega os argumentos:</p> 
      <ul> 
       <li> <p>layoutTemplateIDs (string[])</p> </li> 
       <li> <p>overrideIfExists (booleano)</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### UserDelegate {#userdelegation}

Um objeto UserDelegate representa o ato de delegar trabalho de um usuário a outro por um período específico.

O objeto UserDelegate adicionou o sinalizador REPORTABLE.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Campos Diretos</td> 
   <td> <p>Os seguintes campos removeram o sinalizador NOT_GROUPABLE</p> 
    <ul> 
     <li> <p><b>endDate</b> </p> </li> 
     <li> <p><b>startDate</b> </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Campos padrão</td> 
   <td> <p>Os seguintes campos foram adicionados:</p> 
    <ul> 
     <li> <p><b>endDate</b> </p> </li> 
     <li> <p><b>startDate</b> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Trabalho  {#work}

Um objeto de trabalho é uma interface comum que Tarefa e OpTask herdam e compartilha um código comum entre os dois.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>Campos de Busca</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>favoritedByUsersMM</b> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>
