---
content-type: reference
product-area: reports and dashboards
navigation-topic: data lake
title: Dicionário de dados Data Lake
description: Esta página contém informações sobre a estrutura e o conteúdo dos dados no data lake da Workfront.
author: Nolan
feature: Reports and Dashboards
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: c82f70c78bc23f69bed2351a67c2e0d0bac9e973
workflow-type: tm+mt
source-wordcount: '456'
ht-degree: 8%

---

# Dicionário de dados do Workfront data lake

Esta página contém informações sobre a estrutura e o conteúdo dos dados no data lake da Workfront.

>[!NOTE]
>
>Os dados no data lake da Workfront são atualizados a cada quatro horas, portanto, alterações recentes podem não ser refletidas imediatamente.

## Tipos de tabela

Há vários tipos de tabelas que você pode utilizar para visualizar os dados do Workfront de uma maneira que forneça o maior insight.

### Tabela atual

A tabela Atual reflete os dados de forma semelhante a como eles existem no Workfront, em cada objeto e em seu estado atual. No entanto, ela pode ser navegada com latência muito mais baixa do que no Workfront.

### Tabela de eventos

A tabela Evento rastreia cada registro de alteração no Workfront: ou seja, sempre que um objeto muda de estado, um registro é criado para mostrar quando a alteração aconteceu, quem fez a alteração e o que foi alterado. Portanto, essa tabela é útil para comparações point-in-time. Esta tabela inclui apenas registros dos últimos três anos.

### Tabela Histórico diário

A tabela Histórico Diário oferece uma versão abreviada da tabela Evento, na medida em que mostra o estado de cada objeto diariamente em vez de quando cada evento individual ocorreu. Dessa forma, essa tabela é útil para a análise de tendências.

<!-- Custom table -->

## Tabela de relacionamento de entidade

A tabela a seguir correlaciona os nomes de objetos no Workfront (bem como seus nomes na interface e na API) com seu nome equivalente no data lake.

<table>
<thead>
  <tr>
    <th>Nome da entidade Workfront</th>
    <th>Referências da interface</th>
    <th>Referência da API | Rótulo</th>
    <th>Tabelas Data Lake</th>
    <th>Notas</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Atribuição</td>
    <td>Atribuição</td>
    <td>ATRIBUIR | Atribuição</td>
    <td>ATRIBUIÇÕES_ATUAIS<br>     ASSIGNMENTS_DAILY_HISTORY<br>     EVENTO_DE_ATRIBUIÇÕES</td>
    <td></td>
  </tr>
  <tr>
    <td>CustomEnum</td>
    <td>Condição, Prioridade, Severidade, Status</td>
    <td>CSTEM | Enumerado Personalizado</td>
    <td>CUSTOMENUMS_CURRENT<br>     CUSTOMENUMS_DAILY_HISTORY<br>     CUSTOMENUMS_EVENT</td>
    <td>O tipo de registro é identificado por meio da propriedade "enumClass". Veja a seguir os tipos esperados:<br>     CONDITION_OPTASK<br>     CONDITION_PROJ<br>     CONDITION_TASK<br>     PRIORITY_OPTASK<br>     PRIORITY_PROJ<br>     PRIORITY_TASK<br>     SEVERITY_OPTASK<br>     STATUS_OPTASK<br>     STATUS_PROJ<br>     STATUS_TASK</td>
  </tr>
  <tr>
    <td>Documento</td>
    <td>Documento</td>
    <td>DOCU | Documento</td>
    <td>DOCUMENTS_CURRENT<br>     DOCUMENTS_DAILY_HISTORY<br>     DOCUMENTS_EVENT<br>     <br>     DOCUMENTS_CUSTOM_VALUE_CURRENT<br>     DOCUMENTS_CUSTOM_VALUE_DAILY_HISTORY<br>     DOCUMENTS_CUSTOM_VALUE_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>VersãoDocumento</td>
    <td>Versão do Documento</td>
    <td>DOCV | Versão do documento</td>
    <td>DOCUMENTVERSIONS_CURRENT<br>     DOCUMENTVERSIONS_DAILY_HISTORY<br>     DOCUMENTVERSIONS_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>Grupo</td>
    <td>Grupo</td>
    <td>GRUPO | Grupo</td>
    <td>GROUPS_CURRENT<br>     GROUPS_DAILY_HISTORY<br>     GROUPS_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>Hora</td>
    <td>Hora</td>
    <td>HORA | Hora</td>
    <td>HOURS_CURRENT<br>     HOURS_DAILY_HISTORY<br>     HOURS_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>Tipo de hora</td>
    <td>Tipo de hora</td>
    <td>HORA | Tipo de Hora</td>
    <td>HOURTYPES_CURRENT</td>
    <td></td>
  </tr>
  <tr>
    <td>Etapa</td>
    <td>Etapa</td>
    <td>MILHA | Etapa</td>
    <td>MARCOS_ATUAIS<br>     MARCOS_HISTÓRICO_DIÁRIO<br>     MARCOS_EVENTO</td>
    <td></td>
  </tr>
  <tr>
    <td>CaminhoEtapas</td>
    <td>Caminho de Etapas</td>
    <td>MPATH | Caminho de Etapas</td>
    <td>MILESTONEPATHS_CURRENT<br>     MILESTONEPATHS_DAILY_HISTORY<br>     MILESTONEPATHS_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>Nota</td>
    <td>Nota</td>
    <td>NOTA | Nota</td>
    <td>NOTAS_ATUAIS<br>     NOTES_DAILY_HISTORY<br>     NOTES_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>OpTask</td>
    <td>Problema, Solicitação</td>
    <td>OPTASK | Problema</td>
    <td>OPTASKS_CURRENT<br>     OPTASKS_DAILY_HISTORY<br>     OPTASKS_EVENT<br>     <br>     OPTASKS_CUSTOM_VALUE_CURRENT<br>     OPTASKS_CUSTOM_VALUE_DAILY_HISTORY<br>     OPTASKS_CUSTOM_VALUE_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>Portfólio</td>
    <td>Portfólio</td>
    <td>PORTA | Portfolio</td>
    <td>PORTFOLIO_CURRENT<br>     PORTFOLIO_DAILY_HISTORY<br>     PORTFOLIO_EVENT<br>     <br>     PORTFOLIO_CUSTOM_VALUE_CURRENT<br>     PORTFOLIO_CUSTOM_VALUE_DAILY_HISTORY<br>     PORTFOLIO_CUSTOM_VALUE_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>Programa</td>
    <td>Programa</td>
    <td>PRGM | Programa</td>
    <td>PROGRAMAS_ATUAIS<br>     PROGRAMS_DAILY_HISTORY<br>     PROGRAMS_EVENT<br>     <br>     PROGRAMS_CUSTOM_VALUE_CURRENT<br>     PROGRAMS_CUSTOM_VALUE_DAILY_HISTORY<br>     PROGRAMS_CUSTOM_VALUE_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>Projeto</td>
    <td>Projeto</td>
    <td>PROJ | Projeto</td>
    <td>PROJETOS_ATUAIS<br>     PROJECTS_DAILY_HISTORY<br>     PROJECTS_EVENT<br>     <br>     PROJECTS_CUSTOM_VALUE_CURRENT<br>     PROJECTS_CUSTOM_VALUE_DAILY_HISTORY<br>     PROJECTS_CUSTOM_VALUE_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>Função</td>
    <td>Função no trabalho</td>
    <td>FUNÇÃO | Função de trabalho</td>
    <td>FUNÇÕES_ATUAIS<br>     ROLES_DAILY_HISTORY<br>     ROLES_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>Agendar</td>
    <td>Agendar</td>
    <td>SCHED | Agendar</td>
    <td>SCHEDULES_CURRENT<br>     SCHEDULES_DAILY_HISTORY<br>     SCHEDULES_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>Tarefa</td>
    <td>Tarefa</td>
    <td>TAREFA | Tarefa</td>
    <td>TAREFAS_ATUAIS<br>     TASKS_DAILY_HISTORY<br>     TASKS_EVENT<br>     <br>     TASKS_CUSTOM_VALUE_CURRENT<br>     TASKS_CUSTOM_VALUE_DAILY_HISTORY<br>     TASKS_CUSTOM_VALUE_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>Equipe</td>
    <td>Equipe</td>
    <td>TEAMOB | Equipe</td>
    <td>TEAMS_CURRENT<br>     TEAMS_DAILY_HISTORY<br>     TEAMS_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>Planilha de horas</td>
    <td>Planilha de horas</td>
    <td>FOLHA | Planilha de horas</td>
    <td>PLANILHA_DE_HORAS_ATUAL<br>     TIMESHEETS_DAILY_HISTORY<br>     TIMESHEETS_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>Usuário</td>
    <td>Usuário</td>
    <td>USUÁRIO | Usuário</td>
    <td>USERS_CURRENT<br>     USERS_DAILY_HISTORY<br>     USERS_EVENT<br>     <br>     USERS_CUSTOM_VALUE_CURRENT<br>     USERS_CUSTOM_VALUE_DAILY_HISTORY<br>     USERS_CUSTOM_VALUE_EVENT</td>
    <td></td>
  </tr>
</tbody>
</table>