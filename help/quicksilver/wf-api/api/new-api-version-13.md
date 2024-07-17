---
content-type: api
navigation-topic: api-navigation-topic
title: Novidades da API versão 13
description: O Adobe Workfront lançou a API versão 13 em 22 de abril de 2021. A API versão 13 apresenta as seguintes alterações da versão 12.
author: Becky
feature: Workfront API
role: Developer
exl-id: afbc986e-8b5c-40bc-9120-e8d34e0f7004
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '1072'
ht-degree: 2%

---

# Novidades da API versão 13

O Adobe Workfront lançou a API versão 13 em 22 de abril de 2021. A API versão 13 apresenta as seguintes alterações da versão 12.

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
     <li> <p><a href="#accesslevel" class="MCXref xref">NívelDeAcesso</a> </p> </li> 
     <li> <p><a href="#breadcrumb" class="MCXref xref">BreadCrumb</a> </p> </li> 
     <li> <p><a href="#burndownevent" class="MCXref xref">BurndownEvent</a> </p> </li> 
     <li> <p><a href="#customerpreferences" class="MCXref xref">PreferênciasDoCliente</a> </p> </li> 
     <li> <p><a href="#documentversion" class="MCXref xref">VersãoDocumento</a> </p> </li> 
     <li> <p><a href="#group" class="MCXref xref">Grupo </a> </p> </li> 
     <li> <p><a href="#journalentry" class="MCXref xref">EntradaDiário</a> </p> </li> 
     <li> <p><a href="#layouttemplate" class="MCXref xref">ModeloDeLayout</a> </p> </li> 
     <li> <p><a href="#linkedfolder" class="MCXref xref">PastaVinculada</a> </p> </li> 
     <li> <p><a href="#optask" class="MCXref xref">TarefaOp</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p><a href="#project" class="MCXref xref">Projeto</a> </p> </li> 
     <li> <p><a href="#proofapproval" class="MCXref xref">AprovaçãoDeProva</a> </p> </li> 
     <li> <p><a href="#queuedef" class="MCXref xref">DefiniçãoDaFila</a> </p> </li> 
     <li> <p><a href="#task" class="MCXref xref">Tarefa</a> </p> </li> 
     <li> <p><a href="#team" class="MCXref xref">Equipe</a> </p> </li> 
     <li> <p><a href="#timesheet" class="MCXref xref">Planilha de horas</a> </p> </li> 
     <li> <p><a href="#timesheetprofile" class="MCXref xref">PerfilPlanilhaDeHoras</a> </p> </li> 
     <li> <p><a href="#uitemplate" class="MCXref xref">UITemplate</a> </p> </li> 
     <li> <p><a href="#userdelegation" class="MCXref xref">DelegaçãodeUsuários</a> </p> </li> 
     <li> <p><a href="#work" class="MCXref xref">Trabalho </a> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### NívelDeAcesso {#accesslevel}

Um objeto AccessLevel está associado a usuários e descreve o conjunto de AccessLevelPermissions que determinam o que o usuário pode acessar.

Para obter mais informações sobre níveis de acesso, consulte [Como os níveis de acesso funcionam](../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels.md).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>Campos diretos</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>Descrição</b> </p> <p>Adição do validador MAX_LENGTH, que especifica que o comprimento da descrição não é superior a 4000 caracteres.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### BreadCrumb {#breadcrumb}

Um objeto BreadCrumb representa um elemento na hierarquia pai/filho de um item de trabalho do Workfront. As navegações estruturais indicam como um item de trabalho se encaixa na estrutura maior de Portfolio, Projetos, Projetos e Tarefas.

Para obter mais informações sobre navegação estrutural, consulte [Visão geral sobre navegação estrutural na nova experiência do Adobe Workfront](../../workfront-basics/the-new-workfront-experience/breadcrumb-overview.md)

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>Campos diretos</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>objCode</b> </p> <p>Códigos de objeto podem ser encontrados no <a href="../../wf-api/general/api-explorer.md" class="MCXref xref">API Explorer</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### BurndownEvent {#burndownevent}

Um objeto BurndownEvent representa um objeto que altera o bundown de uma iteração.

Para obter mais informações sobre burndown, consulte [Burndown](../../agile/use-scrum-in-an-agile-team/burndown/burndown.md).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>Campos diretos</p> </td> 
   <td> <p>Os seguintes campos removeram o sinalizador NOT_GROUPABLE </p> 
    <ul> 
     <li> <p>applyDate</p> </li> 
     <li> <p>entryDate</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### PreferênciasDoCliente {#customerpreferences}

Um objeto CustomerPreferences representa o conjunto de preferências que um cliente definiu para sua instância do Workfront.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campos diretos</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>name</p> <p style="font-weight: normal;">Valores possíveis adicionados:</p> 
      <ul> 
       <li style="font-weight: normal;">senha:aemAPIKey (config.general.aem.apikey)</li> 
       <li style="font-weight: normal;"> senha:aemAADomain (config.general.aem.aadomain) </li> 
       <li style="font-weight: normal;">senha:aemIntegrationEnabled (config.general.aem.enabled)</li> 
       <li style="font-weight: normal;">senha:aemHost (config.general.aem.host)</li> 
       <li style="font-weight: normal;">folha de horas:padrão.folha de horas.restringir.folha de horas.editar.proprietários.administradores (config.folha de horas.restringir.folha de horas.editar.proprietários.administradores)</li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Ações</td> 
   <td> <p>As ações a seguir foram adicionadas ao recurso Preferências do cliente.</p> 
    <ul> 
     <li> <p><b>getTimesheetPreferences</b> </p> </li> 
     <li> <p><b>setTimesheetPreferences</b> </p> <p>Assume o argumento:</p> 
      <ul> 
       <li> <p>preferências (mapa)</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### VersãoDocumento {#documentversion}

Um objeto DocumentVersion representa uma versão específica de um arquivo (como material escrito, imagens ou outras formas de informação).

Para obter mais informações sobre versões de documentos, consulte [Carregar uma nova versão de um documento](../../documents/managing-documents/upload-new-document-version.md).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>Campos diretos</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>externalIntegrationType</b> </p> <p>Valor adicionado possível:</p> 
      <ul> 
       <li> <p>AEM (Adobe Experience Manager)</p> </li> 
      </ul> </li> 
    </ul> 
    <ul> 
     <li> <p><b>proofID</b> </p> <p>Adicionado sinalizador NOT_FILTERABLE</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Grupo  {#group}

Um objeto Grupo representa um conjunto de usuários e equipes. Os grupos geralmente representam a estrutura departamental.

Para obter mais informações sobre grupos, consulte [Grupos versus equipes no Adobe Workfront](../../people-teams-and-groups/work-with-groups-and-teams/understanding-differences-and-similarities-between-groups-and-teams.md).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>Ações</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>getParents</b> </p> <p>Esta ação retorna uma matriz dos grupos principais do grupo (grupos dos quais o grupo fornecido é um subgrupo).</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### EntradaDiário {#journalentry}

O objeto JournalEntry pode ser configurado para registrar informações sobre campos de objeto específicos sempre que esses campos forem modificados. Quando um campo é configurado para ser registrado como parte do objeto de Entrada de diário, uma Entrada de diário correspondente será criada toda vez que o campo for modificado.

O recurso JournalEntry adicionou o sinalizador REPORTABLE.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>Campos diretos</p> </td> 
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

Os administradores do Adobe Workfront ou de grupo podem criar modelos para personalizar os elementos de layout no Adobe Workfront. O objeto LayoutTemplate é específico do Adobe Workfront Classic.

Para o objeto que representa modelos de layout na nova experiência do Adobe Workfront, consulte [UITemplate](#uitemplate)

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>Campos diretos</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>Descrição</b> </p> <p>Adição do validador MAX_LENGTH, que especifica que o comprimento da descrição não é superior a 4000 caracteres.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### LinkedFolder {#linkedfolder}

Um objeto LinkedFolder representa uma pasta vinculada de um provedor de documentos externo, como Google Drive ou Dropbox.

Para obter mais informações sobre Pastas Vinculadas, consulte [Vincular documentos de aplicativos externos](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>Campos diretos</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>externalIntegrationType</b> </p> <p>Valor adicionado possível:</p> 
      <ul> 
       <li> <p>AEM (Adobe Experience Manager)</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### OpTask {#optask}

Um objeto OpTask é comumente conhecido como um Problema. Um problema é um item de trabalho que geralmente indica que há um problema que impede a conclusão de uma tarefa ou projeto. Um problema também pode ser uma solicitação de Help Desk. Pedidos de alteração, solicitações e bugs também são problemas.

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

Os projetos são itens de trabalho no Workfront e um elemento principal da maneira como o Workfront ajuda as pessoas a trabalhar. Um objeto Projeto representa um grupo de tarefas com uma meta comum e específica.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>Campos diretos</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>convertedOpTaskOriginatorID</b> </p> <!--
       <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Removed flag NOT&nbsp;FILTERABLE</p>
      --> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### AprovaçãoDaProva {#proofapproval}

Um objeto ProofApproval representa uma aprovação que está diretamente conectada a uma prova.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>Campos diretos</p> </td> 
   <td> <p>Os campos a seguir foram adicionados ao recurso Aprovação de prova.</p> 
    <ul> 
     <li> <p><b>approverStage</b> </p> </li> 
     <li> <p><b>DataDecisão</b> </p> </li> 
     <li> <p><b>modeloDeFluxoDeTrabalho</b> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### QueueDef {#queuedef}

Um objeto QueueDef representa uma Fila, que é um Projeto publicado na área Help Desk para permitir que os usuários enviem Problemas a ele.

Para obter mais informações sobre Filas de solicitações, consulte [Criar uma fila de solicitações](../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Campos diretos</td> 
   <td> 
    <ul> 
     <li> <p><b>documentPosition</b> </p> <p>Adição de. Os valores possíveis são:</p> 
      <ul> 
       <li> <p>0 (Após formulários personalizados)</p> </li> 
       <li> <p>1 (Antes dos formulários personalizados)</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Tarefa {#task}

Um objeto Tarefa representa um item de trabalho que deve ser executado como uma etapa para atingir uma meta final (concluir um Projeto).

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
   <td>Campos diretos</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">Este campo foi adicionado e é um parâmetro booleano que tem um valor true se um objeto estiver ativo e false se não for. Os objetos definidos como Ativos aparecem em menus suspensos e campos de digitação antecipada e podem ser anexados a outros objetos. Objetos não definidos como Ativos não são visíveis em menus suspensos e campos de digitação antecipada para anexar a outros objetos.  </p> </li> 
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

Um objeto de Planilha de Horas representa um cartão de ponto virtual que permite aos Usuários inserir as horas reais trabalhadas para Tarefas, Projetos e Tipos de Horas Gerais.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campos diretos</td> 
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

### PerfilPlanilhaDeHoras {#timesheetprofile}

Um objeto de Planilha de Horas representa um cartão de ponto virtual que permite aos Usuários inserir as horas reais trabalhadas para Tarefas, Projetos e Tipos de Horas Gerais.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campos diretos</td> 
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

### Modelo UIT {#uitemplate}

Os administradores do Adobe Workfront ou de grupo podem criar modelos para personalizar os elementos de layout no Adobe Workfront. O objeto UITemplate é específico para a nova experiência do Adobe Workfront.

Para o objeto que representa modelos de layout no Adobe Workfront Classic, consulte [LayoutTemplate](#layouttemplate).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Ações</td> 
   <td> <p>As ações a seguir foram adicionadas ao recurso UITemplate.</p> 
    <ul> 
     <li> <p><b>migrateCustomersAllLayoutTemplates</b> </p> <p>Assume o argumento:</p> 
      <ul> 
       <li> <p>overrideIfExists (booleano)</p> </li> 
      </ul> </li> 
     <li> <p><b>migrateLayoutTemplates</b> </p> <p>Pega os argumentos:</p> 
      <ul> 
       <li> <p>layoutTemplateIDs (string[])</p> </li> 
       <li> <p>overrideIfExists (booleano)</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### UserDelegation {#userdelegation}

Um objeto UserDelegation representa o ato de delegar trabalho de um usuário para outro por um período específico de tempo.

O objeto UserDelegation adicionou o sinalizador REPORTABLE.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Campos diretos</td> 
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

Um objeto Trabalho é uma interface comum que tanto Tarefa quanto OpTask herdam e compartilha código comum entre os dois.

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
