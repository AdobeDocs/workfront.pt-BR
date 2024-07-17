---
content-type: reference
product-area: reports and dashboards
navigation-topic: data lake
title: Dicionário de dados Data Lake
description: Esta página contém informações sobre a estrutura e o conteúdo dos dados no data lake da Workfront.
author: Nolan
feature: Reports and Dashboards
recommendations: noDisplay, noCatalog
exl-id: 57985404-554e-4289-b871-b02d3427aa5c
source-git-commit: 81f8477dd26b828c4255c678b36d98789cd81ff8
workflow-type: tm+mt
source-wordcount: '725'
ht-degree: 5%

---

# Dicionário de dados do Workfront data lake

Esta página contém informações sobre a estrutura e o conteúdo dos dados no data lake da Workfront.

>[!NOTE]
>
>Os dados no data lake da Workfront são atualizados a cada quatro horas, portanto, alterações recentes podem não ser refletidas imediatamente.

## Tipos de tabela

Há vários tipos de tabelas que você pode utilizar para visualizar os dados do Workfront de uma maneira que forneça o maior insight.

* **Tabela atual**

  A tabela Atual reflete os dados de forma semelhante a como eles existem no Workfront, em cada objeto e em seu estado atual. No entanto, ela pode ser navegada com latência muito mais baixa do que no Workfront.

* **Tabela de eventos**

  A tabela Evento rastreia cada registro de alteração no Workfront: ou seja, sempre que um objeto muda de estado, um registro é criado para mostrar quando a alteração aconteceu, quem fez a alteração e o que foi alterado. Portanto, essa tabela é útil para comparações point-in-time. Esta tabela inclui apenas registros dos últimos três anos.

* **Tabela de Histórico Diário**

  A tabela Histórico Diário oferece uma versão abreviada da tabela Evento, na medida em que mostra o estado de cada objeto diariamente em vez de quando cada evento individual ocorreu. Dessa forma, essa tabela é útil para a análise de tendências.

<!-- Custom table -->

## Diagrama de relacionamento de entidade

Os objetos no Workfront (e, portanto, no data lake) são definidos não apenas por seus valores individuais, mas por suas relações com outros objetos. O diagrama de relacionamento de entidade abaixo fornece um mapeamento de alto nível de relacionamentos de objetos no data lake da Workfront. O diagrama pode ser visualizado e baixado por meio do seguinte link:

[Diagrama de relacionamento de entidade do data lake da Workfront](/help/quicksilver/reports-and-dashboards/data-lake/assets/Workfront-data-lake_entity-relationship-diagram.pdf)

>[!IMPORTANT]
>
>O diagrama de relacionamento de entidade é um trabalho em andamento, sendo assim, ele serve apenas para fins de referência e está sujeito a alterações.

## Tipos de data

Há vários objetos de data que fornecem informações sobre quando eventos específicos ocorrem.

* `DL_LOAD_TIMESTAMP`: essa data é usada para referência interna e reflete quando os dados foram carregados na tabela Histórico Atual, de Eventos ou Diário. Essa data não deve ser usada para análise de dados e deve ser removida durante a fase beta do data lake da Workfront.
* `CALENDAR_DATE`: esta data está presente apenas na tabela Histórico Diário. Esta tabela fornece um registro de como foram os dados às 11h59 UTC para cada data especificada em `CALENDAR_DATE`.
* `BEGIN_EFFECTIVE_TIMESTAMP`: esta data está presente nas tabelas Evento e Histórico Diário e registra exatamente quando um registro mudou _para_ o valor que tem na linha atual.
* `END_EFFECTIVE_TIMESTAMP`: Essa data está presente nas tabelas Evento e Histórico Diário e registra exatamente quando um registro alterou _de_ o valor na linha atual para um valor em uma linha diferente. Para permitir entre consultas em `BEGIN_EFFECTIVE_TIMESTAMP` e `END_EFFECTIVE_TIMESTAMP`, esse valor nunca é nulo, mesmo que não haja um novo valor. Caso um registro ainda seja válido (isto é, o valor não tenha sido alterado), `END_EFFECTIVE_TIMESTAMP` terá um valor 2300-01-01.

## Tabela de terminologia

A tabela a seguir correlaciona nomes de objetos no Workfront (bem como seus nomes na interface e na API) com seus nomes equivalentes no data lake.

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
    <td>ASSIGNMENTS_CURRENT<br>ASSIGNMENTS_DAILY_HISTORY<br>ASSIGNMENTS_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>CustomEnum</td>
    <td>Condição, Prioridade, Severidade, Status</td>
    <td>CSTEM | Enumerado Personalizado</td>
    <td>CUSTOMENUMS_CURRENT<br>CUSTOMENUMS_DAILY_HISTORY<br>CUSTOMENUMS_EVENT</td>
    <td>O tipo de registro é identificado por meio da propriedade "enumClass". Estes são os tipos esperados:<br>CONDITION_OPTASK<br>CONDITION_PROJ<br>CONDITION_TASK<br>PRIORITY_OPTASK<br>PRIORITY_PROJ<br>PRIORITY_TASK<br>SEVERITY_OPTASK<br>STATUS_OPTASK<br>STATUS_PROJ<br>STATUS_TASK</td>
  </tr>
  <tr>
    <td>Documento</td>
    <td>Documento</td>
    <td>DOCU | Documento</td>
    <td>DOCUMENTS_CURRENT<br>DOCUMENTS_DAILY_HISTORY<br>DOCUMENTS_EVENT<br><br>DOCUMENTS_CUSTOM_VALUE_CURRENT<br>DOCUMENTS_CUSTOM_VALUE_DAILY_HISTORY<br>DOCUMENTS_CUSTOM_VALUE_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>VersãoDocumento</td>
    <td>Versão do Documento</td>
    <td>DOCV | Versão do documento</td>
    <td>DOCUMENTVERSIONS_CURRENT<br>DOCUMENTVERSIONS_DAILY_HISTORY<br>DOCUMENTVERSIONS_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>Grupo</td>
    <td>Grupo</td>
    <td>GRUPO | Grupo</td>
    <td>GROUPS_CURRENT<br>GROUPS_DAILY_HISTORY<br>GROUPS_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>Hora</td>
    <td>Hora</td>
    <td>HORA | Hora</td>
    <td>HOURS_CURRENT<br>HOURS_DAILY_HISTORY<br>HOURS_EVENT</td>
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
    <td>MARCOS_ATUAIS<br>MARCOS_HISTÓRICO_DIÁRIO<br>MARCOS_EVENTO</td>
    <td></td>
  </tr>
  <tr>
    <td>CaminhoEtapas</td>
    <td>Caminho de Etapas</td>
    <td>MPATH | Caminho de Etapas</td>
    <td>MILESTONEPATHS_CURRENT<br>MILESTONEPATHS_DAILY_HISTORY<br>MILESTONEPATHS_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>Nota</td>
    <td>Nota</td>
    <td>NOTA | Nota</td>
    <td>NOTES_CURRENT<br>NOTES_DAILY_HISTORY<br>NOTES_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>OpTask</td>
    <td>Problema, Solicitação</td>
    <td>OPTASK | Problema</td>
    <td>OPTASKS_CURRENT<br>OPTASKS_DAILY_HISTORY<br>OPTASKS_EVENT<br><br>OPTASKS_CUSTOM_VALUE_CURRENT<br>OPTASKS_CUSTOM_VALUE_DAILY_HISTORY<br>OPTASKS_CUSTOM_VALUE_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>Portfólio</td>
    <td>Portfólio</td>
    <td>PORTA | Portfolio</td>
    <td>PORTFOLIO_CURRENT<br>PORTFOLIO_DAILY_HISTORY<br>PORTFOLIO_EVENT<br><br>PORTFOLIO_CUSTOM_VALUE_CURRENT<br>PORTFOLIO_CUSTOM_VALUE_DAILY_HISTORY<br>PORTFOLIO_CUSTOM_VALUE_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>Programa</td>
    <td>Programa</td>
    <td>PRGM | Programa</td>
    <td>PROGRAMS_CURRENT<br>PROGRAMS_DAILY_HISTORY<br>PROGRAMS_EVENT<br><br>PROGRAMS_CUSTOM_VALUE_CURRENT<br>PROGRAMS_CUSTOM_VALUE_DAILY_HISTORY<br>PROGRAMS_CUSTOM_VALUE_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>Projeto</td>
    <td>Projeto</td>
    <td>PROJ | Projeto</td>
    <td>PROJECTS_CURRENT<br>PROJECTS_DAILY_HISTORY<br>PROJECTS_EVENT<br><br>PROJECTS_CUSTOM_VALUE_CURRENT<br>PROJECTS_CUSTOM_VALUE_DAILY_HISTORY<br>PROJECTS_CUSTOM_VALUE_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>Função</td>
    <td>Função no trabalho</td>
    <td>FUNÇÃO | Função de trabalho</td>
    <td>ROLES_CURRENT<br>HISTÓRICO_DIÁRIO_DE_FUNÇÕES<br>EVENTO_DE_FUNÇÕES</td>
    <td></td>
  </tr>
  <tr>
    <td>Agendar</td>
    <td>Agendar</td>
    <td>SCHED | Agendar</td>
    <td>SCHEDULES_CURRENT<br>SCHEDULES_DAILY_HISTORY<br>SCHEDULES_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>Tarefa</td>
    <td>Tarefa</td>
    <td>TAREFA | Tarefa</td>
    <td>TASKS_CURRENT<br>TASKS_DAILY_HISTORY<br>TASKS_EVENT<br><br>TASKS_CUSTOM_VALUE_CURRENT<br>TASKS_CUSTOM_VALUE_DAILY_HISTORY<br>TASKS_CUSTOM_VALUE_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>Equipe</td>
    <td>Equipe</td>
    <td>TEAMOB | Equipe</td>
    <td>TEAMS_CURRENT<br>TEAMS_DAILY_HISTORY<br>TEAMS_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>Planilha de horas</td>
    <td>Planilha de horas</td>
    <td>FOLHA | Planilha de horas</td>
    <td>FOLHAS_DE_HORAS_ATUAIS<br>FOLHAS_DE_HORAS_DIÁRIAS_HISTÓRICO<br>FOLHAS_DE_HORAS_EVENTO</td>
    <td></td>
  </tr>
  <tr>
    <td>Usuário</td>
    <td>Usuário</td>
    <td>USUÁRIO | Usuário</td>
    <td>USERS_CURRENT<br>USERS_DAILY_HISTORY<br>USERS_EVENT<br><br>USERS_CUSTOM_VALUE_CURRENT<br>USERS_CUSTOM_VALUE_DAILY_HISTORY<br>USERS_CUSTOM_VALUE_EVENT</td>
    <td></td>
  </tr>
</tbody>
</table>
