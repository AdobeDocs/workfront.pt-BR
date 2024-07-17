---
content-type: api
navigation-topic: api-navigation-topic
title: Novidades da API versão 12
description: O Workfront lançou a API versão 12 em 12 de novembro de 2020. A API versão 12 apresenta as seguintes alterações da versão 11
author: Becky
feature: Workfront API
role: Developer
exl-id: 1ffba3b5-ab24-4ca2-a1ef-f7e5b77e776c
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '2475'
ht-degree: 1%

---

# Novidades da API versão 12

O Workfront lançou a API versão 12 em 12 de novembro de 2020. A API versão 12 apresenta as seguintes alterações da versão 11

## Recursos adicionados

Os seguintes recursos são novos na API do Workfront versão 12.

* [BreadCrumb](#breadcrumb)
* [RichTextParameterValue](#richtextparametervalue)

### BreadCrumb {#breadcrumb}

Um objeto BreadCrumb representa um elemento na hierarquia pai/filho de um item de trabalho do Adobe Workfront. As navegações estruturais indicam como um item de trabalho se encaixa na estrutura maior de Portfolio, Projetos, Projetos e Tarefas.

Para obter mais informações sobre navegações estruturais no Workfront, consulte [Visão geral sobre navegações estruturais na nova experiência do Adobe Workfront](../../workfront-basics/the-new-workfront-experience/breadcrumb-overview.md)

<table style="table-layout:auto"> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> 
 <tbody> 
  <tr> 
   <td>Ação</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">getObjectHierarchy</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### RichTextParameterValue {#richtextparametervalue}

Os campos de rich text agora estão disponíveis em mais objetos. O objeto RichTextParameterValue foi adicionado ao Workfront para oferecer suporte a essa disponibilidade.

Para obter mais informações, consulte [Campos de rich text na API do Adobe Workfront](../../wf-api/general/rich-text-field-api.md).

<table style="table-layout:auto"> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> 
 <tbody> 
  <tr> 
   <td>Campos diretos</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">ID</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Campos principais</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">ID</li> 
     <li style="font-weight: bold;">objCode</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Recursos removidos

Nenhum recurso foi removido para a API versão 12.

## Recursos modificados

Os recursos a seguir foram modificados para a API do Workfront versão 12.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> 
    <ul> 
     <li> <p><a href="#accesslevel" class="MCXref xref">NívelDeAcesso</a> </p> </li> 
     <li> <p><a href="#accesslevelpermissions" class="MCXref xref">PermissõesDeNívelDeAcesso</a> </p> </li> 
     <li> <p><a href="#accessrequest" class="MCXref xref">SolicitaçãoDeAcesso</a> </p> </li> 
     <li> <p><a href="#accessrule" class="MCXref xref">RegraDeAcesso</a> </p> </li> 
     <li> <p><a href="#activitylog" class="MCXref xref">LogAtividade</a> </p> </li> 
     <li> <p><a href="#announcementattachment" class="MCXref xref">AnúncioAnexo</a> </p> </li> 
     <li> <p><a href="#approval" class="MCXref xref">Aprovação</a> </p> </li> 
     <li> <p><a href="#calendarsection" class="MCXref xref">SeçãoCalendário</a> </p> </li> 
     <li> <p><a href="#company" class="MCXref xref">Empresa</a> </p> </li> 
     <li> <p><a href="#customer" class="MCXref xref">Cliente</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p><a href="#customerpreferences" class="MCXref xref">PreferênciasDoCliente</a> </p> </li> 
     <li> <p><a href="#document" class="MCXref xref">Documento</a> </p> </li> 
     <li> <p><a href="#documentversion" class="MCXref xref">VersãoDocumento</a> </p> </li> 
     <li> <p><a href="#group" class="MCXref xref">Grupo </a> </p> </li> 
     <li> <p><a href="#linkedfolder" class="MCXref xref">PastaVinculada</a> </p> </li> 
     <li> <p><a href="#optask" class="MCXref xref">TarefaOp</a> </p> </li> 
     <li> <p><a href="#parameter" class="MCXref xref">Parâmetro</a> </p> </li> 
     <li> <p><a href="#portfolio" class="MCXref xref">Portfolio</a> </p> </li> 
     <li> <p><a href="#program" class="MCXref xref">Programa</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p><a href="#queuedef" class="MCXref xref">DefiniçãoDaFila</a> </p> </li> 
     <li> <p><a href="#scheduledreport" class="MCXref xref">RelatórioAgendado</a> </p> </li> 
     <li> <p><a href="#scorecardquestion" class="MCXref xref">ScoreCardQuestion</a> </p> </li> 
     <li> <p><a href="#task" class="MCXref xref">Tarefa</a> </p> </li> 
     <li> <p><a href="#team" class="MCXref xref">Equipe</a> </p> </li> 
     <li> <p><a href="#templatetask" class="MCXref xref">TarefaModelo</a> </p> </li> 
     <li> <p><a href="#timesheet" class="MCXref xref">Planilha de horas</a> </p> </li> 
     <li> <p><a href="#user" class="MCXref xref">Usuário</a> </p> </li> 
     <li> <p><a href="#work" class="MCXref xref">Trabalho </a> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

 

### NívelDeAcesso {#accesslevel}

Um objeto AccessLevel está associado a usuários e descreve o conjunto de AccessLevelPermissions que determinam o que o usuário pode acessar.

Para obter mais informações sobre níveis de acesso, consulte [Como os níveis de acesso funcionam](../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels.md).

<table style="table-layout:auto"> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> 
 <tbody> 
  <tr> <!--
    <td data-mc-conditions="QuicksilverOrClassic.Draft mode">Direct Fields</td>
   --> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <!--
       <p data-mc-conditions="QuicksilverOrClassic.Draft mode">fieldAccessPrivileges</p>
      --> <!--
       <p style="font-weight: normal;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Added the possible value CPJ (Copy). This allows Users with Planner Access Level to copy Projects.</p>
      --> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### PermissõesDeNívelDeAcesso {#accesslevelpermissions}

Um objeto AccessLevelPermissions representa uma permissão específica para acessar, criar ou modificar um objeto Workfront. Essas permissões podem ser associadas a um Nível de acesso.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campos diretos</td> 
   <td> 
    <ul> 
     <li> <p><strong>coreAction</strong> </p> <p>Foram adicionados os seguintes valores possíveis:</p> 
      <ul> 
       <li> <p>PLANNED_HOURS_CONTORNING </p> <p>Um usuário com um nível de acesso que inclui essa permissão pode atualizar horas planejadas no Balanceador de carga de trabalho.</p> <p>Para obter mais informações, consulte <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md#update" class="MCXref xref">Atualizar horas planejadas da tarefa ao gerenciar alocações de usuário</a> em <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md" class="MCXref xref">Gerenciar alocações de usuário no Balanceador de carga de trabalho</a>.</p> </li> 
       <li> <p>ADD_TO_CUSTOM_FORMS </p> <p>Um usuário com um nível de acesso que inclui essa permissão pode adicionar campos a formulários personalizados.</p> <p>Para obter mais informações, consulte <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md#add2" class="MCXref xref"></a> em <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">Criar ou editar um formulário personalizado</a>.</p> </li> 
       <li> <p>EDIT_SYSTEMWIDE </p> <p>Um usuário com um nível de acesso que inclui essa permissão pode compartilhar um sistema de campos personalizados com acesso de exclusão.</p> <p>Para obter mais informações, consulte <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/configure-sharing-for-a-custom-field.md" class="MCXref xref">Configurar compartilhamento para campos e widgets personalizados</a>.</p> </li> 
      </ul> </li> 
     <li> <p><strong>açõesProibidas</strong> </p> <p>Foram adicionados os seguintes valores possíveis:</p> 
      <ul> 
       <li> <p>PLANNED_HOURS_CONTORNING </p> </li> 
       <li> <p>ADD_TO_CUSTOM_FORMS </p> </li> 
       <li> <p>EDIT_SYSTEMWIDE </p> </li> 
      </ul> </li> 
     <li> <p><strong>açõesSecundárias</strong> </p> <p>Foram adicionados os seguintes valores possíveis:</p> 
      <ul> 
       <li> <p>PLANNED_HOURS_CONTORNING </p> </li> 
       <li> <p>ADD_TO_CUSTOM_FORMS </p> </li> 
       <li> <p>EDIT_SYSTEMWIDE </p> </li> 
      </ul> </li> 
    </ul> <!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">OR</p>
    --> <!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">The following fields added the possible value PLANNED_HOURS_CONTOURING, which allows a user to update planned hours in the Workload Balancer</p>
    --> 
    <ul> 
     <li> <!--
       <p data-mc-conditions="QuicksilverOrClassic.Draft mode">coreAction</p>
      --> </li> 
     <li> <!--
       <p data-mc-conditions="QuicksilverOrClassic.Draft mode">forbiddenActions</p>
      --> </li> 
     <li> <!--
       <p data-mc-conditions="QuicksilverOrClassic.Draft mode">secondaryActions</p>
      --> </li> 
    </ul> <!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">The following fields added the possible value ADD_TO_CUSTOM_FORMS, which allows a user to add fields to custom forms.</p>
    --> 
    <ul> 
     <li> <!--
       <p data-mc-conditions="QuicksilverOrClassic.Draft mode">coreAction</p>
      --> </li> 
     <li> <!--
       <p data-mc-conditions="QuicksilverOrClassic.Draft mode">forbiddenActions</p>
      --> </li> 
     <li> <!--
       <p data-mc-conditions="QuicksilverOrClassic.Draft mode">secondaryActions</p>
      --> </li> 
    </ul> <!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">The following fields added the possible value EDIT_SYSTEMWIDE, which allows a user to share a custom field system-wide with Delete access. </p>
    --> <!--
     <ul data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
      <li> <p>coreAction</p> </li> 
      <li> <p>forbiddenActions</p> </li> 
      <li> <p>secondaryActions</p> </li> 
     </ul>
    --> </td> 
  </tr> 
 </tbody> 
</table>

### Solicitação de acesso {#accessrequest}

Se um usuário não tiver acesso a um objeto no Workfront necessário, ele poderá solicitar acesso a esse objeto. O objeto AccessRequest representa essa solicitação.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campos diretos</td> 
   <td> 
    <ul> 
     <li> <p style="font-weight: bold;">ação</p> <p>Foram adicionados os seguintes valores possíveis:</p> 
      <ul> 
       <li> <p>PLANNED_HOURS_CONTORNING </p> <p>Um usuário com um nível de acesso que inclui essa permissão pode atualizar horas planejadas no Balanceador de carga de trabalho.</p> <p>Para obter mais informações, consulte <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md#update" class="MCXref xref">Atualizar horas planejadas da tarefa ao gerenciar alocações de usuário</a> em <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md" class="MCXref xref">Gerenciar alocações de usuário no Balanceador de carga de trabalho</a>.</p> </li> 
       <li> <p>ADD_TO_CUSTOM_FORMS </p> <p>Um usuário com um nível de acesso que inclui essa permissão pode adicionar campos a formulários personalizados.</p> <p>Para obter mais informações, consulte <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md#add2" class="MCXref xref"></a> em <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">Criar ou editar um formulário personalizado</a>.</p> </li> 
       <li> <p>EDIT_SYSTEMWIDE </p> <p>Um usuário com um nível de acesso que inclui essa permissão pode compartilhar um sistema de campos personalizados com acesso de exclusão.</p> <p>Para obter mais informações, consulte <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/configure-sharing-for-a-custom-field.md" class="MCXref xref">Configurar compartilhamento para campos e widgets personalizados</a>.</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Regra de acesso {#accessrule}

Um objeto AccessRule representa um conjunto de regras em níveis de acesso personalizados que determina como os usuários podem compartilhar projetos criados por eles.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campos diretos</td> 
   <td> 
    <ul> 
     <li><strong>coreAction</strong> <p>Foram adicionados os seguintes valores possíveis:</p> 
      <ul> 
       <li> <p>PLANNED_HOURS_CONTORNING </p> <p>Um usuário com um nível de acesso que inclui essa permissão pode atualizar horas planejadas no Balanceador de carga de trabalho.</p> <p>Para obter mais informações, consulte <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md#update" class="MCXref xref">Atualizar horas planejadas da tarefa ao gerenciar alocações de usuário</a> em <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md" class="MCXref xref">Gerenciar alocações de usuário no Balanceador de carga de trabalho</a>.</p> </li> 
       <li> <p>ADD_TO_CUSTOM_FORMS </p> <p>Um usuário com um nível de acesso que inclui essa permissão pode adicionar campos a formulários personalizados.</p> <p>Para obter mais informações, consulte <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md#add2" class="MCXref xref"></a> em <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">Criar ou editar um formulário personalizado</a>.</p> </li> 
       <li> <p>EDIT_SYSTEMWIDE </p> <p>Um usuário com um nível de acesso que inclui essa permissão pode compartilhar um sistema de campos personalizados com acesso de exclusão.</p> <p>Para obter mais informações, consulte <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/configure-sharing-for-a-custom-field.md" class="MCXref xref">Configurar compartilhamento para campos e widgets personalizados</a>.</p> </li> 
      </ul> </li> 
     <li> <p><strong>açõesProibidas</strong> </p> <p>Foram adicionados os seguintes valores possíveis:</p> 
      <ul> 
       <li> <p>PLANNED_HOURS_CONTORNING </p> </li> 
       <li> <p>ADD_TO_CUSTOM_FORMS </p> </li> 
       <li> <p>EDIT_SYSTEMWIDE </p> </li> 
      </ul> </li> 
     <li> <p><strong>açõesSecundárias</strong> </p> <p>Foram adicionados os seguintes valores possíveis:</p> 
      <ul> 
       <li> <p>PLANNED_HOURS_CONTORNING </p> </li> 
       <li> <p>ADD_TO_CUSTOM_FORMS </p> </li> 
       <li> <p>EDIT_SYSTEMWIDE </p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### ActivityLog {#activitylog}

Um objeto ActivityLog é uma lista completa de todas as atividades que ocorreram em uma determinada conta do Workfront Proof.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>Operações</p> </td> 
   <td> <p>A operação a seguir foi removida do objeto ActivityLog:</p> 
    <ul> 
     <li> <p><strong>ADICIONAR</strong> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### AnúncioAnexo {#announcementattachment}

Um objeto AnnouncementAttachment representa um arquivo que foi anexado a um anúncio do Workfront.

Para obter mais informações sobre anexos de comunicado, consulte [Enviar avisos](../../administration-and-setup/get-started-wf-administration/view-send-announcements.md)

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>Campos diretos</p> </td> 
   <td> 
    <ul> 
     <li> <p><strong>fileExtension</strong> </p> <p>Valores possíveis adicionados:</p> 
      <ul> 
       <li> <p>qdoc (enum.fileextension.qdoc)</p> </li> 
       <li> <p>qslides (enum.fileextension.qslides)</p> </li> 
       <li> <p>qsheet (enum.fileextension.qsheet)</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Aprovação {#approval}

Um determinado item de trabalho, como uma tarefa, um documento ou uma folha de horas, pode exigir que um supervisor ou outro usuário faça logoff no item de trabalho. Um objeto de Aprovação representa a ação de desconectar em um item de trabalho.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campos diretos</td> 
   <td> 
    <ul> 
     <li> <p><strong>ordemListaDePendências</strong> </p> <p>Os seguintes sinalizadores foram removidos:</p> 
      <ul> 
       <li> <p>DINÂMICO,</p> </li> 
       <li> <p>LAZY_READ,</p> </li> 
       <li> <p>NOT_GROUPABLE</p> </li> 
      </ul> </li> 
     <li> <p><strong>groupID</strong> </p> <p>Adição dos seguintes sinalizadores</p> 
      <ul> 
       <li> <p>AUTO_LOAD,</p> </li> 
       <li> <p>DINÂMICO,</p> </li> 
       <li> <p>READ_ONLY</p> </li> 
      </ul> </li> 
     <li> <p><strong>esforçoTrabalho</strong> </p> <p>Este campo foi adicionado e representa se um usuário precisa de uma pequena, média ou grande quantidade de esforço diário para concluir uma tarefa. Os valores possíveis são:</p> 
      <ul> 
       <li> <p>1 (Pequeno)</p> </li> 
       <li> <p>2 (Medium)</p> </li> 
       <li> <p>3 (Grande)</p> </li> 
      </ul> <p>Para obter mais informações sobre o Esforço de trabalho no Workfront, consulte <a href="../../manage-work/tasks/task-information/work-effort.md" class="MCXref xref">Visão geral do Esforço de trabalho</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### SeçãoCalendário {#calendarsection}

Uma Seção de calendário é um relatório de calendário.

Para obter mais informações sobre relatórios de calendário, consulte [Visão geral dos relatórios de calendário](../../reports-and-dashboards/reports/calendars/calendar-reports-overview.md).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campos diretos</td> 
   <td> <p style="font-weight: normal;">Os campos a seguir foram adicionados ao objeto CalendarSection para oferecer suporte à nova funcionalidade de usar datas personalizadas nos relatórios de calendário. </p> <p style="font-weight: normal;">Para obter mais informações, consulte <a href="../../reports-and-dashboards/reports/calendars/use-custom-dates.md" class="MCXref xref">Usar campos de data personalizados em um relatório de calendário</a>.</p> 
    <ul> 
     <li> <p style="font-weight: normal;">customDate</p> </li> 
     <li> <p style="font-weight: normal;">customEndDateParameterID</p> </li> 
     <li> <p style="font-weight: normal;">customStartDateParameterID</p> </li> 
     <li> <p style="font-weight: normal;">ignoreAtualDates</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Empresa {#company}

Um objeto Company representa uma organização que consiste em uma coleção de pessoas.

Para obter mais informações, consulte [Criar e editar empresas](../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campos diretos</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>groupID</p> <p style="font-weight: normal;">A ID do grupo ao qual a empresa está associada.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Campos de referência</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>grupo</p> <p style="font-weight: normal;">O grupo ao qual a empresa está associada. Associar uma empresa a um grupo permite que o administrador do grupo estenda o acesso e as permissões do grupo à empresa.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Cliente {#customer}

Um objeto Customer representa uma organização que usa uma instância do Workfront.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Ações</td> 
   <td> 
    <ul> 
     <li> <p style="font-weight: normal;"><strong>productEnabled</strong> </p> <p style="font-weight: normal;">Essa ação usa um argumento CustomerProductTypeEnum e retorna um booleano que informa se esse cliente tem uma conta para esse produto. </p> </li> 
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
       <li style="font-weight: normal;">password:zoomIntegrationEnabled (Habilita a integração do Zoom no fluxo de atualizações)</li> 
       <li style="font-weight: normal;"> senha:quipIntegrationEnabled (config.general.quip.enabled)  </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Documento {#document}

Um objeto Documento representa um arquivo (como material escrito, imagens ou outras formas de informação).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Ações</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>createLinkedProofVersion</p> <p style="font-weight: normal;">Adicionado</p> </li> 
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
   <td>Campos diretos</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>externalIntegrationType</p> <p style="font-weight: normal;">Valor possível removido:</p> 
      <ul> 
       <li style="font-weight: normal;">QUIP (Quip)</li> 
      </ul> </li> 
    </ul> 
    <ul> 
     <li> <p style="font-weight: normal;"><strong>proofDecision</strong> </p> <p>Adicionado</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Ações</td> 
   <td> <p>As ações a seguir foram adicionadas ao objeto Documento.</p> 
    <ul> 
     <li> <p style="font-weight: bold;">getDocumentReviewerDecision</p> <p style="font-weight: normal;">Essa ação pega o argumento documentVersionID (string) e retorna um mapa que indica a decisão do revisor.</p> </li> 
     <li style="font-weight: bold;"> <p>setDocumentReviewerDecision</p> <p style="font-weight: normal;">Essa ação aceita os seguintes argumentos:</p> 
      <ul style="font-weight: normal;"> 
       <li> <p>documentVersionID (sequência de caracteres)</p> </li> 
       <li> <p>reviewerDecision (sequência de caracteres)</p> </li> 
       <li> <p>comentário (sequência de caracteres)</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Grupo  {#group}

Um objeto Grupo representa um conjunto de usuários e equipes. Os grupos geralmente representam a estrutura departamental.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campos diretos</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>businessLeaderID</p> <p style="font-weight: normal;">A ID do Líder de negócios atribuído ao grupo.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Campos de referência</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>líder de negócios</p> <p style="font-weight: normal;">O Líder de negócios atribuído ao grupo. Um Líder de negócios é alguém que toma decisões de negócios para o grupo.</p> <p style="font-weight: normal;">Para obter mais informações sobre líderes de negócios, consulte <a href="../../administration-and-setup/manage-groups/group-roles/business-leader-overview.md" class="MCXref xref">Visão geral sobre Líderes de negócios</a>.<br></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Ações</td> 
   <td> 
    <ul> 
     <li> <p><strong>atribuirMúltiplo</strong> </p> <p>Essa ação aceita os seguintes argumentos:</p> 
      <ul> 
       <li> <p>userIDs (string[])</p> </li> 
       <li> <p>roleIDs (string[])</p> </li> 
       <li> <p>teamID (string)</p> </li> 
      </ul> </li> 
     <li> <p><strong>getGroupMembers</strong> </p> </li> 
     <li> <p><strong>updateMembersList</strong> </p> <p>Essa ação aceita os seguintes argumentos:</p> 
      <ul> 
       <li> <p>newMemberIDs (string[])</p> </li> 
       <li> <p>removedMemberDs (string[])</p> </li> 
      </ul> </li> 
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
     <li style="font-weight: bold;"> <p>externalIntegrationType</p> <p style="font-weight: normal;">Valor possível removido:</p> 
      <ul> 
       <li style="font-weight: normal;">QUIP (Quip)</li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### OpTask {#optask}

Um objeto OpTask é comumente conhecido como um Problema. Um problema é um item de trabalho que geralmente indica que há um problema que impede a conclusão de uma tarefa ou projeto. Um problema também pode ser uma solicitação de Help Desk. Pedidos de alteração, solicitações e bugs também são problemas.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Campos diretos</p> </td> 
   <td> 
    <ul> 
     <li> <p><strong>ordemListaDePendências</strong> </p> <p>A ordem indica a posição de uma tarefa ou história no backlog Agile.</p> <p>Esse campo removeu os seguintes sinalizadores:
       <ul>
        <li>DINÂMICO,</li>
        <li>LAZY_READ,</li>
        <li>NOT_GROUPABLE:</li>
       </ul></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Ações</td> 
   <td> <p>Essas ações adicionaram o status do argumento para suportar a nova funcionalidade do botão Iniciar, que altera o status de um item de trabalho quando um usuário clica no botão para indicar que começou a trabalhar no item.</p> <p>Para obter mais informações, consulte <a href="../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md" class="MCXref xref">Substituir o botão Trabalhar na tarefa por um botão Iniciar</a>.</p> 
    <ul> 
     <li> <p><strong>acceptWork</strong> </p> </li> 
     <li> <p><strong>cancelarTrabalho</strong> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Parâmetro {#parameter}

Um objeto Parameter é um campo personalizado.

O recurso Parameter adicionou o sinalizador SHARABLE.

Para obter mais informações sobre campos personalizados, consulte [Criar ou editar um formulário personalizado](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md#create) em [Criar ou editar um formulário personalizado](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Campos diretos</td> 
   <td> 
    <ul> 
     <li> <p><strong>dataType</strong> </p> <p>Valor adicionado possível:</p> 
      <ul> 
       <li> <p>RICO (Rich Text)</p> <p>Para obter mais informações, consulte <a href="../../wf-api/general/rich-text-field-api.md" class="MCXref xref">Campos de rich text na API do Adobe Workfront</a>.</p> </li> 
      </ul> </li> 
     <li> <p><strong>displayType</strong> </p> <p>Valor adicionado possível:</p> 
      <ul> 
       <li> <p>RICH (Campo de texto com formatação)</p> <p>Para obter mais informações, consulte <a href="../../wf-api/general/rich-text-field-api.md" class="MCXref xref">Campos de rich text na API do Adobe Workfront</a>.</p> </li> 
      </ul> </li> 
     <li> <p><strong>rótulo</strong> </p> <p>Adicionado</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Campos de coleção</td> 
   <td> 
    <ul> 
     <li> <p><strong>accessRules</strong> </p> <p>Adicionado</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Campos padrão</td> 
   <td> 
    <ul> 
     <li> <p class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray"><strong>rótulo</strong> </p> <p>Adicionado</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Portfólio {#portfolio}

Um objeto Portfolio é uma coleção de projetos que competem pelos mesmos recursos, normalmente dinheiro ou pessoas para concluí-los.

Para obter mais informações sobre portfólios, consulte [visão geral de Portfolio no Adobe Workfront](../../manage-work/portfolios/portfolios-overview/portfolio-overview.md).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campos diretos</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>groupID</p> <p style="font-weight: normal;">A ID do grupo ao qual o portfólio está associado.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Campos de referência</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>grupo</p> <p style="font-weight: normal;">O grupo ao qual o portfólio está associado. </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Programa {#program}

Um objeto Programa é um subconjunto de projetos em um portfólio, em que projetos semelhantes podem ser agrupados.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campos diretos</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>groupID</p> <p style="font-weight: normal;">A ID do grupo ao qual o programa está associado.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Campos de referência</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>grupo</p> <p style="font-weight: normal;">O grupo ao qual o programa está associado. </p> </li> 
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
     <li><strong>solicitanteCoreAction</strong> <p>Foram adicionados os seguintes valores possíveis:</p> 
      <ul> 
       <li> <p>PLANNED_HOURS_CONTORNING </p> <p>Um usuário com um nível de acesso que inclui essa permissão pode atualizar horas planejadas no Balanceador de carga de trabalho.</p> <p>Para obter mais informações, consulte <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md#update" class="MCXref xref">Atualizar horas planejadas da tarefa ao gerenciar alocações de usuário</a> em <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md" class="MCXref xref">Gerenciar alocações de usuário no Balanceador de carga de trabalho</a>.</p> </li> 
       <li> <p>ADD_TO_CUSTOM_FORMS </p> <p>Um usuário com um nível de acesso que inclui essa permissão pode adicionar campos a formulários personalizados.</p> <p>Para obter mais informações, consulte <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md#add2" class="MCXref xref"></a> em <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">Criar ou editar um formulário personalizado</a>.</p> </li> 
       <li> <p>EDIT_SYSTEMWIDE </p> <p>Um usuário com um nível de acesso que inclui essa permissão pode compartilhar um sistema de campos personalizados com acesso de exclusão.</p> <p>Para obter mais informações, consulte <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/configure-sharing-for-a-custom-field.md" class="MCXref xref">Configurar compartilhamento para campos e widgets personalizados</a></p> </li> 
      </ul> <li> <p><strong>solicitanteForbiddenActions</strong> </p> <p>Foram adicionados os seguintes valores possíveis:</p> 
       <ul> 
        <li> <p>PLANNED_HOURS_CONTORNING </p> </li> 
        <li> <p>ADD_TO_CUSTOM_FORMS </p> </li> 
        <li> <p>EDIT_SYSTEMWIDE </p> </li> 
       </ul> </li> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### RelatórioAgendado {#scheduledreport}

Um objeto ScheduledReport representa um relatório que foi configurado para ser agendado para entrega.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Campos diretos</td> 
   <td> 
    <ul> 
     <li> <p><strong>formato</strong> </p> <p>Valores possíveis adicionados:</p> 
      <ul> 
       <li> <p>qdoc (enum.fileextension.qdoc)</p> </li> 
       <li> <p>qslides (enum.fileextension.qslides)</p> </li> 
       <li> <p>qsheet (enum.fileextension.qsheet)</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### ScoreCardQuestion {#scorecardquestion}

Um objeto ScoreCardQuestion representa uma pergunta que foi adicionada a um Scorecard. Essas perguntas geralmente são determinadas pelo gerente de Portfolio, e suas respostas permitem que o gerente entenda como um projeto se alinha com as metas do portfólio.

Para obter mais informações sobre Perguntas do Scorecard, consulte [Criar um scorecard](../../administration-and-setup/set-up-workfront/configure-system-defaults/create-scorecard.md).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campos diretos</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>displayType</p> <p style="font-weight: normal;">Adição do valor possível RICH (Campo de texto com formatação) </p> <p style="font-weight: normal;">Para obter mais informações, consulte <a href="../../wf-api/general/rich-text-field-api.md" class="MCXref xref">Campos de rich text na API do Adobe Workfront</a>.  </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Tarefa {#task}

Um objeto Tarefa representa um item de trabalho que deve ser executado como uma etapa para atingir uma meta final (concluir um Projeto).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Campos diretos</td> 
   <td> 
    <ul> 
     <li> <p><strong>esforçoTrabalho</strong> </p> <p>Este campo foi adicionado e representa se um usuário precisa de uma pequena, média ou grande quantidade de esforço diário para concluir uma tarefa. Os valores possíveis são:</p> 
      <ul> 
       <li> <p>1 (Pequeno)</p> </li> 
       <li> <p>2 (Medium)</p> </li> 
       <li> <p>3 (Grande)</p> </li> 
      </ul> <p>Para obter mais informações sobre o Esforço de trabalho no Workfront, consulte <a href="../../manage-work/tasks/task-information/work-effort.md" class="MCXref xref">Visão geral do Esforço de trabalho</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Ações</td> 
   <td> <p>Essas ações adicionaram o status do argumento para suportar a nova funcionalidade do botão Iniciar, que altera o status de um item de trabalho quando um usuário clica no botão para indicar que começou a trabalhar no item.</p> <p>Para obter mais informações, consulte <a href="../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md" class="MCXref xref">Substituir o botão Trabalhar na tarefa por um botão Iniciar</a>.</p> 
    <ul> 
     <li> <p><strong>acceptWork</strong> </p> </li> 
     <li> <p><strong>cancelarTrabalho</strong> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Equipe {#team}

Um objeto Equipe é uma coleção de Usuários que pode ser atribuída a um item de trabalho.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Campos diretos</td> 
   <td> <p>Os seguintes campos foram adicionados ao recurso Equipe:</p> 
    <ul> 
     <li> <p><strong>completeDaysOnKanbanBoard</strong> </p> <p>Esse campo representa o número de dias que um cartão concluído permanece no quadro Kanban.</p> <!--
       <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For more information, see <a href="../../agile/get-started-with-agile-in-workfront/configure-kanban.md" class="MCXref xref">Configure Kanban</a>.</p>
      --> </li> 
     <li> <p><strong>groupID</strong> </p> <p>Este campo associa uma equipe a um grupo. Isso identifica a equipe como parte do grupo e permite que o Administrador do grupo gerencie as equipes.</p> </li> 
     <li> <p><strong>workOnItStatusChange</strong> </p> <p>Este é um parâmetro booleano que indica se o botão Trabalhar na equipe foi configurado como um botão Iniciar. Quando um membro da equipe clica em um botão Iniciar para começar a trabalhar em um item de trabalho, o status do item muda de Novo para um status configurado nas configurações da equipe.</p> </li> 
     <li> <p>Os campos a seguir permitem especificar status personalizados para o botão Iniciar nos itens de trabalho individuais.</p> 
      <ul> 
       <li> <p><strong>workOnItOpTaskBugReportStatuses</strong> </p> </li> 
       <li> <p><strong>workOnItOpTaskChangeOrderStatuses</strong> </p> </li> 
       <li> <p><strong>workOnItOpTaskIssueStatuses</strong> </p> </li> 
       <li> <p><strong>workOnItOpTaskRequestStatuses</strong> </p> <p><strong>workOnItTaskStatuses</strong> </p> </li> 
      </ul> <p>Para obter mais informações sobre o botão Iniciar, consulte <a href="../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md" class="MCXref xref">Substituir o botão Trabalhar na tarefa por um botão Iniciar</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Campos de referência</td> 
   <td> <p>O seguinte campo foi adicionado ao recurso Equipe:</p> 
    <ul> 
     <li> <p><strong>grupo</strong> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### TarefaModelo {#templatetask}

Um objeto TemplateTask representa uma Tarefa que faz parte de um Template. Modelos de Tarefa se tornam Tarefas no Projeto onde o Modelo é usado.

Para obter mais informações sobre Modelos de Tarefa, consulte [Editar uma tarefa de modelo](../../manage-work/projects/create-and-manage-templates/edit-template-task.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Campos diretos</td> 
   <td> 
    <ul> 
     <li> <p><strong>esforçoTrabalho</strong> </p> <p>Este campo foi adicionado e representa se um usuário precisa de uma pequena, média ou grande quantidade de esforço diário para concluir uma tarefa. Os valores possíveis são:</p> 
      <ul> 
       <li> <p>1 (Pequeno)</p> </li> 
       <li> <p>2 (Medium)</p> </li> 
       <li> <p>3 (Grande)</p> </li> 
      </ul> <p>Para obter mais informações sobre o Esforço de trabalho no Workfront, consulte <a href="../../manage-work/tasks/task-information/work-effort.md" class="MCXref xref">Visão geral do Esforço de trabalho</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Planilha de horas {#timesheet}

Um objeto de Planilha de Horas representa um cartão de ponto virtual que permite aos Usuários inserir as horas reais trabalhadas para Tarefas, Projetos e Tipos de Horas Gerais.

Para obter mais informações sobre Folhas de horas, consulte [Visão geral sobre Folhas de horas](../../timesheets/timesheets/timesheets-overview.md)

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Campos principais</td> 
   <td> <p>O campo a seguir foi removido do recurso Quadro de horários:</p> 
    <ul> 
     <li> <p><strong>objcode</strong> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Atualizar

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Campos diretos</td> 
   <td> 
    <ul> 
     <li> <p><strong>updateType</strong> </p> <p>Foram adicionados os seguintes valores possíveis:</p> 
      <ul> 
       <li> <p>initiativeAdd (enum.updatetypeenum.initiativeadd)</p> </li> 
       <li> <p>initiativeEdit (enum.updatetypeenum.initiativeedit)</p> </li> 
      </ul> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Para obter mais informações sobre iniciativas, consulte <a href="../../scenario-planner/initiatives-overview.md" class="MCXref xref">Visão geral das iniciativas no Planejador de cenários</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Usuário {#user}

Um objeto Usuário representa uma pessoa com uma conta no Workfront que pode fazer logon e interagir com o sistema.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Campos diretos</td> 
   <td> <p>Os seguintes campos foram adicionados ao recurso Usuário:</p> 
    <ul> 
     <li> <p><strong>atualDeactivationDate</strong> </p> <p>Representa a data e a hora em que um usuário foi desativado.</p> <p>Para obter mais informações sobre Usuários desativados, consulte <a href="../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">Desativar ou reativar um usuário</a>.</p> </li> 
     <li> <p><strong>alignAccessType</strong> </p> <p>Este campo mostra o acesso do usuário às Metas do Workfront. Os valores possíveis são:</p> 
      <ul> 
       <li> <p>Sem acesso</p> </li> 
       <li> <p>Exibir</p> </li> 
       <li> <p>Editar</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Ações</td> 
   <td> <p>A seguinte ação foi adicionada ao recurso Usuário:</p> 
    <ul> 
     <li> <p><strong>getUserAccessPermissionsByObjCode</strong> </p> <p>Esta ação aceita os seguintes argumentos</p> 
      <ul> 
       <li> <p>ids (sequência de caracteres)</p> </li> 
       <li> <p>objCode (string)</p> </li> 
      </ul> </li> 
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
   <td>Campos diretos</td> 
   <td> 
    <ul> 
     <li> <p><strong>ordemListaDePendências</strong> </p> <p>A ordem indica a posição de uma tarefa ou história no backlog Agile.</p> <p>Esse campo removeu os seguintes sinalizadores:</p> 
      <ul> 
       <li> <p>DINÂMICO,</p> </li> 
       <li> <p>LAZY_READ,</p> </li> 
       <li> <p>NOT_GROUPABLE</p> </li> 
      </ul> </li> 
     <li> <p><strong>groupID</strong> </p> <p>Esse campo adicionou os seguintes sinalizadores:</p> 
      <ul> 
       <li> <p>AUTO_LOAD,</p> </li> 
       <li> <p>DINÂMICO,</p> </li> 
       <li> <p>READ_ONLY</p> </li> 
      </ul> </li> 
     <li> <p><strong>esforçoTrabalho</strong> </p> <p>Este campo foi adicionado e representa se um usuário precisa de uma pequena, média ou grande quantidade de esforço diário para concluir uma tarefa. Os valores possíveis são:</p> 
      <ul> 
       <li> <p>1 (Pequeno)</p> </li> 
       <li> <p>2 (Medium)</p> </li> 
       <li> <p>3 (Grande)</p> </li> 
      </ul> <p>Para obter mais informações sobre o Esforço de trabalho no Workfront, consulte <a href="../../manage-work/tasks/task-information/work-effort.md" class="MCXref xref">Visão geral do Esforço de trabalho</a>.</p> </li> 
    </ul> <p style="font-weight: normal;">  </p> </td> 
  </tr> 
 </tbody> 
</table>
