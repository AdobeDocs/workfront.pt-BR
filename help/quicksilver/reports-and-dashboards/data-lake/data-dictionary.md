---
content-type: reference
product-area: reports and dashboards
navigation-topic: data connect
title: Dicionário de dados da Workfront Data Connect
description: Esta página contém informações sobre a estrutura e o conteúdo dos dados no Workfront Data Connect.
author: Nolan
feature: Reports and Dashboards
recommendations: noDisplay, noCatalog
exl-id: 57985404-554e-4289-b871-b02d3427aa5c
source-git-commit: 57c08a06a57bebfaa81035e4fe801f3077e6a829
workflow-type: tm+mt
source-wordcount: '4295'
ht-degree: 4%

---

# Dicionário de dados da Workfront Data Connect

Esta página contém informações sobre a estrutura e o conteúdo dos dados no Workfront Data Connect.

>[!NOTE]
>
>Os dados no Data Connect são atualizados a cada quatro horas, portanto, alterações recentes podem não ser refletidas imediatamente.

## Tipos de tabela

Há vários tipos de tabela que você pode utilizar no Data Connect para exibir seus dados do Workfront de uma maneira que forneça mais insight.

* **Tabela atual**

  A tabela Atual reflete os dados de forma semelhante a como eles existem no Workfront, em cada objeto e em seu estado atual. No entanto, ela pode ser navegada com latência muito mais baixa do que no Workfront.

* **Tabela de eventos**

  A tabela Evento rastreia cada registro de alteração no Workfront: ou seja, sempre que um objeto muda de estado, um registro é criado para mostrar quando a alteração aconteceu, quem fez a alteração e o que foi alterado. Portanto, essa tabela é útil para comparações point-in-time. Esta tabela inclui apenas registros dos últimos três anos.

* **Tabela de Histórico Diário**

  A tabela Histórico Diário oferece uma versão abreviada da tabela Evento, na medida em que mostra o estado de cada objeto diariamente em vez de quando cada evento individual ocorreu. Dessa forma, essa tabela é útil para a análise de tendências.

<!-- Custom table -->

## Diagrama de relacionamento de entidade

Os objetos no Workfront (e, portanto, no data lake da Data Connect) são definidos não apenas por seus valores individuais, mas por suas relações com outros objetos. O diagrama de relacionamento de entidade abaixo fornece um mapeamento de alto nível de relacionamentos de objetos no Data Connect. O diagrama pode ser visualizado e baixado por meio do seguinte link:

[Diagrama de relacionamento da entidade Conexão de Dados](/help/quicksilver/reports-and-dashboards/data-lake/assets/Workfront-data-lake_entity-relationship-diagram.pdf)

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

A tabela a seguir correlaciona nomes de objetos no Workfront (bem como seus nomes na interface e na API) com seus nomes equivalentes no Data Connect.

<table>
  <thead>
    <tr>
        <th>Nome da entidade Workfront</th>
        <th>Referências da interface</th>
        <th>Referência da API | Rótulo</th>
        <th>Tabelas Data Lake</th>
        <th>Opções</th>
        <th>Campo de relacionamentos</th>
        <th>Tabela e campo do relacionamento</th>
    </tr>
  </thead>
  <tbody>
    <tr>
        <td>Nível de acesso</td>
        <td>Nível de acesso</td>
        <td>ACSLVL | Nível de acesso</td>
        <td>ACCESSLEVELS_CURRENT<br>ACCESSLEVELS_DAILY_HISTORY<br>ACCESSLEVELS_EVENT</td>
        <td></td>
        <td>ACCESSLEVELID (self)<br>APPGLOBALID<br>LASTUPDATEDBYID<br>LEGACYACCESSLEVELID<br>OBJID<br>SYSID</td>
        <td>Self<br>Not uma relação; usado para fins internos do aplicativo<br>USER_CURRENT | USERID<br>Não é uma relação; usada para fins de aplicativo interno<br>A ID do objeto identificado no campo OBJCODE<br>Não é uma relação; usada para fins de aplicativo interno</td>
    </tr>
    <tr>
        <td>Regra de acesso</td>
        <td>Compartilhar</td>
        <td>ACSRUL | Compartilhar</td>
        <td>ACCESSRULES_CURRENT<br>ACCESSRULES_DAILY_HISTORY<br>ACCESSRULES_EVENT</td>
        <td></td>
        <td>ACCESSORID <br>ACCESSRULEID (self) <br>ANCESTORID <br>LASTUPDATEDBYID <br>SECURITYOBJID <br>SYSID</td>
        <td>A ID do objeto identificado no campo ACCESSOROBJCODE<br>Self<br>A ID do objeto identificado no campo ANCESTOROBJCODE<br>USERS_CURRENT | USERID<br>A ID do objeto identificado no campo SECURITYOBJCODE<br>Não é uma relação; usada para fins de aplicativo interno</td>
    </tr>
    <tr>
        <td>Caminho de aprovação</td>
        <td>Caminho de aprovação</td>
        <td>ARVPTH | Aprovação</td>
        <td><br>APPROVALPATHS_EVENT do APPROVALPATHS_DAILY_HISTORY de APPROVALPATHS_CURRENT<br></td>
        <td></td>
        <td>APPROVALPATHID (self) <br>APPROVALPROCESSID  <br>ENTEREDBYID  <br>GLOBALPATHID  <br>LASTUPDATEDBYID <br>SYSID</td>
        <td>Self<br>APPROVALPROCESSES_CURRENT | APPROVALPROCESSID<br>USERS_CURRENT | USERID<br>Não é uma relação; usada para fins de aplicativo interno<br>USERS_CURRENT | USERID<br>Não é uma relação; usada para fins de aplicativo interno</td>
    </tr>
    <tr>
        <td>Processo de aprovação</td>
        <td>Processo de aprovação</td>
        <td>ARVPRC | Processo de aprovação</td>
        <td>APPROVALPROCESSES_CURRENT<br>APPROVALPROCESSES_DAILY_HISTORY<br>APPROVALPROCESSES_EVENT</td>
        <td></td>
        <td>APPROVALPROCESSID (auto) <br>ENTEREDBYID <br>LASTUPDATEDBYID<br>SYSID</td>
        <td>Self<br>USERS_CURRENT | USERID<br>USERS_CURRENT | USERID<br>Não é uma relação; usada para fins de aplicativo interno</td>
    </tr>
    <tr>
        <td>Etapa de aprovação</td>
        <td>Etapa de aprovação</td>
        <td>ARVSTP | Estágio de aprovação</td>
        <td>APPROVALSTEPS_CURRENT<br>APPROVALSTEPS_DAILY_HISTORY<br>APPROVALSTEPS_EVENT</td>
        <td></td>
        <td>APPROVALPATHID <br>APPROVALSTEPID (self) <br>SYSID</td>
        <td>APPROVALPATHS_CURRENT | APPROVALPATHID<br>Self<br>Não é uma relação; usada para fins de aplicativo interno</td>
    </tr>
    <tr>
        <td>Status do aprovador</td>
        <td>Status do aprovador</td>
        <td>ARVSTS | Status do aprovador</td>
        <td>APPROVERSTATUSES_CURRENT<br>APPROVERSTATUSES_DAILY_HISTORY<br>APPROVERSTATUSES_EVENT</td>
        <td></td>
        <td>APPROVERSTATUSID (self)<br>APPROVABLEOBJID<br>APPROVALSTEPID<br>APPROVEDBYID <br>DELEGATEUSERID<br>LASTUPDATEDBYID <br>OPTASKID<br>OVERRIDDENUSERID<br>PROJECTID<br>STEPAPPROVERID<br>SYSID<br>TASKID<br>WILDCARDUSERID</td>
        <td>Self<br>A ID do objeto identificado no campo APPROVABLEOBJCODE<br>APPROVALSTEPS_CURRENT | APPROVALSTEPID<br>USERS_CURRENT | USERID <br>USERS_CURRENT | USERID<br>USERS_CURRENT | USERID <br>OPTASKS_CURRENT | OPTASKID<br>USUÁRIOS_ATUAIS | USERID<br>PROJECTS_CURRENT | PROJECTID<br>USERS_CURRENT | USERID<br>Não é uma relação; usada para fins de aplicativo interno<br>TASKS_CURRENT | TASKID<br>USERS_CURRENT | USERID</td>
    </tr>
    <tr>
        <td>Atribuição</td>
        <td>Atribuição</td>
        <td>ATRIBUIR | Atribuição</td>
        <td>ASSIGNMENTS_CURRENT<br>ASSIGNMENTS_DAILY_HISTORY<br>ASSIGNMENTS_EVENT</td>
        <td></td>
        <td>ASSIGNEDBYID<br>ASSIGNEDTOID<br>ASSIGNMENTID (self)<br>CATEGORYID<br>CLASSIFIERID<br>OPTASKID<br>PRIVATERATECARDID<br>PROJECTID<br>ROLEID<br>TASKID<br>TEAMID</td>
        <td>USER_CURRENT | USERID<br>USER_CURRENT | ID DE USUÁRIO<br>Self<br>CATEGORIES_CURRENT | Atualmente, não há suporte para a tabela de classificadores CATEGORYID<br>OPTASK_CURRENT | OPTASKID<br>RATECARD_CURRENT | RATECARDID<br>PROJECT_CURRENT | PROJECTID<br>ROLE_CURRENT | ROLEID<br>TASK_CURRENT | TASKID<br>EQUIPE_ATUAL | TEAMID<br></td>
    </tr>
    <tr>
        <td>Aguardando aprovações</td>
        <td>Aguardando aprovações</td>
        <td>AWAPVL | Aguardando aprovação</td>
        <td>AWAITINGAPPROVALS_CURRENT<br>AWAITINGAPPROVALS_DAILY_HISTORY<br>AWAITINGAPPROVALS_EVENT</td>
        <td></td>
        <td>ACCESSREQUESTID<br>APPROVABLEID <br>APPROVERID <br>AWAITINGAPPROVALID (self) <br>DOCUMENTID <br>DOCUMENTVERSIONID<br>OPTASKID <br>PROJECTID <br>ROLEID <br>SUBMITTEDBYID <br>SYSID<br>TASKID <br>TEAMID <br>TIMESHEETID<br>USERID</td>
        <td>Atualmente, não há suporte para a tabela de Solicitação de Acesso<br>Não é uma relação; usada para fins internos do aplicativo<br>USERS_CURRENT | USERID<br>Self<br>DOCUMENTS_CURRENT | DOCUMENTID<br>DOCUMENTVERSIONS_CURRENT | DOCUMENTVERSIONID<br>OPTASKS_CURRENT | OPTASKID<br>PROJETOS_ATUAIS | PROJECTID<br>FUNÇÕES_ATUAIS | ROLEID<br>USUÁRIOS_ATUAIS | USERID<br>Não é uma relação; usada para fins de aplicativo interno<br>TASKS_CURRENT | TASKID<br>TEAMS_CURRENT | TEAMID<br>PLANILHAS_DE_HORAS_ATUAIS | TIMESHEETID<br>USERS_CURRENT | USERID</td>
    </tr>
    <tr>
        <td>Linha de base</td>
        <td>Linha de base</td>
        <td>BLIN | Linha de base</td>
        <td>LINHAS_BASE_CURRENT<br>LINHAS_BASE_DAILY_HISTORY<br>LINHAS_BASE_EVENT</td>
        <td></td>
        <td>BASELINEID (self)<br>EXCHANGERATEID <br>PROJECTID <br>SYSID</td>
        <td>Self<br>EXCHANGERATES_CURRENT | EXCHANGERATEID<br>PROJECTS_CURRENT | PROJECTID<br>Não é uma relação; usada para fins de aplicativo interno</td>
    </tr>
    <tr>
        <td>Tarefa da Linha de Base</td>
        <td>Tarefa da Linha de Base</td>
        <td>BSTSK | Tarefa da Linha de Base</td>
        <td>BASELINETASKS_CURRENT<br>BASELINETASKS_DAILY_HISTORY<br>BASELINETASKS_EVENT</td>
        <td></td>
        <td>BASELINEID<br>BASELINETASKID (self) <br>EXCHANGERATEID <br>PROJECTID <br>SYSID<br>TASKID</td>
        <td>LINHAS_DE_BASE_ATUAIS | BASELINEID<br>Self<br>EXCHANGERATES_CURRENT | EXCHANGERATEID<br>PROJECTS_CURRENT | PROJECTID<br>Não é uma relação; usada para fins de aplicativo interno<br>TASKS_CURRENT | TASKID</td>
    </tr>
    <tr>
        <td>Taxa de faturamento</td>
        <td>Taxa ou Taxa de Sobreposição</td>
        <td>TAXA | Taxa de cobrança</td>
        <td>RATES_CURRENT<br>RATES_DAILY_HISTORY<br>RATES_EVENT</td>
        <td></td>
        <td>ASSIGNMENTID<br>CLASSIFIERID<br>EXCHANGERATEID<br>NLBRCATEGORYID<br>NONLABORRESOURCEID<br>OBJID<br>PROJECTID <br>RATECARDID<br>RATEID (self)<br>ROLEID <br>SOURCERATECARDID <br>SYSID <br>TEMPLATEID<br>USERID</td>
        <td>ATRIBUIÇÕES_ATUAIS | A tabela ASSIGNMENTID<br>Classifier não tem suporte atualmente<br>EXCHANGERATES_CURRENT | EXCHANGERATEID<br>Tabela de Categoria de Recursos Não Mão-de-Obra não suportada atualmente<br>NONLABORRESOURCES_CURRENT | NONLABORRESOURCEID<br>A ID do objeto identificado no campo OBJCODE<br>PROJECTS_CURRENT | PROJECTID <br>RATECARD_CURRENT | RATECARDID<br>Self<br>ROLES_CURRENT | ROLEID <br>RATECARD_CURRENT | RATECARDID <br>Não é uma relação; usada para fins de aplicativo interno <br>TEMPLATES_CURRNT | TEMPLATEID<br>USERS_CURRENT | USERID</td>
    </tr>
    <tr>
        <td>Registro de Cobrança</td>
        <td>Registro de Cobrança</td>
        <td>FATURA | Registro de Cobrança</td>
        <td>BILLINGRECORDS_CURRENT<br>BILLINGRECORDS_DAILY_HISTORY<br>BILLINGRECORDS_EVENT</td>
        <td></td>
        <td>BILLINGRECORDID (self)<br>CATEGORYID<br>EXCHANGERATEID <br>INVOICEID <br>LASTUPDATEDBYID <br>PROJECTID <br>SYSID</td>
        <td>Auto<br>CATEGORIES_CURRENT | CATEGORYID<br>EXCHANGERATES_CURRENT | Atualmente, a tabela de faturas <br>EXCHANGERATEID não tem suporte <br>USERS_CURRENT | ID DE USUÁRIO <br>PROJECTS_CURRENT | PROJECTID   <br>Não é uma relação; usada para fins de aplicativo interno</td>
    </tr>
    <tr>
        <td>Reserva</td>
        <td>Reserva</td>
        <td>BOOKNG | Reserva</td>
        <td><br>BOOKINGS_EVENT do BOOKINGS_CURRENT BOOKINGS_DAILY_HISTORY<br></td>
        <td></td>
        <td>BOOKINGID (self)<br>ENTEREDBYID<br>LASTUPDATEDBYID<br>NLBRCATEGORYID<br>NONLABORRESOURCEID<br>OBJID<br>PROJECTID<br>SYSID<br>TASKID TEMPLATEID<br><br>TEMPLATETASKID<br>TOPOBJID</td>
        <td>Auto-USERS_CURRENT<br>| USERS_CURRENT USERID<br>| Tabela de Categoria de recursos não trabalhistas USERID<br>não suportada atualmente<br>NONLABORRESOURCES_CURRENT | NONLABORRESOURCEID<br>A ID do objeto identificado no campo<br>OBJOBJCODE PROJECTS_CURRENT | PROJECTID <br>Não é um relacionamento; usado para fins<br>internos de aplicativo TASKS_CURRENT | TEMPLATES_CURRENT TASKID     <br>| TEMPLATETASKS_CURRENT TEMPLATEID<br>| TEMPLATETASKID<br>A ID do objeto identificado no campo TOPOBJCODE</td>
    </tr>
    <tr>
        <td>Categoria</td>
        <td>Formulário personalizado</td>
        <td>CTGY | Categoria</td>
        <td>CATEGORIES_CURRENT<br>CATEGORIES_DAILY_HISTORY<br>CATEGORIES_EVENT</td>
        <td></td>
        <td>CATEGORYID (self)<br>ENTEREDBYID<br>GROUPID <br>LASTUPDATEDBYID <br>SYSID</td>
        <td>Self<br>USERS_CURRENT | USERID<br>GROUPS_CURRENT | GROUPID <br>USERS_CURRENT | USERID <br>Não é uma relação; usada para fins de aplicativo interno</td>
    </tr>
    <tr>
        <td>Parâmetro da Categoria</td>
        <td>Campos de formulário personalizados</td>
        <td>CTGYPA | Parâmetro da categoria</td>
        <td>CATEGORIESPARAMETERS_CURRENT<br>CATEGORIESPARAMETERS_DAILY_HISTORY<br>CATEGORIESPARAMETERS_EVENT</td>
        <td></td>
        <td>CATEGORIESPARAMETERID (self)<br>CATEGORYID<br>PARAMETERGROUPID<br>PARAMETERID    <br>SYSID</td>
        <td>Auto<br>CATEGORIES_CURRENT | No momento, não há suporte para a tabela CATEGORYID<br>Grupo de Parâmetros<br>PARAMETERS_CURRENT | PARAMETERID    <br>Não é uma relação; usada para fins de aplicativo interno</td>
    </tr>
    <tr>
        <td>Empresa</td>
        <td>Empresa</td>
        <td>COMPY | Empresa</td>
        <td>COMPANIES_CURRENT<br>COMPANIES_DAILY_HISTORY<br>COMPANHIAS_EVENT</td>
        <td></td>
        <td>CATEGORYID<br>COMPANYID (self)<br>ENTEREDBYID<br>GROUPID<br>LASTUPDATEDBYID<br>PRIVATERATECARDID<br>SYSID</td>
        <td>CATEGORIES_CURRENT | CATEGORYID<br>Self<br>USERS_CURRENT | USERID <br>GROUPS_CURRENT | GROUPID<br>USERS_CURRENT | ID DE USUÁRIO <br>RATECARD_CURRENT | RATECARDID<br>Não é uma relação; usada para fins de aplicativo interno</td>
    </tr>
    <tr>
        <td>Trimestre personalizado</td>
        <td>Trimestre personalizado</td>
        <td>CSTQRT | Trimestre personalizado</td>
        <td>CUSTOMQUARTERS_CURRENT<br>CUSTOMQUARTERS_DAILY_HISTORY<br>CUSTOMQUARTERS_EVENT</td>
        <td></td>
        <td>CUSTOMQUARTERID (self) <br>SYSID</td>
        <td>Self<br>Not uma relação; usada para fins de aplicativo interno</td>
    </tr>
    <tr>
        <td>CustomEnum</td>
        <td>Condição, Prioridade, Severidade, Status</td>
        <td>CSTEM | Enumerado Personalizado</td>
        <td>CUSTOMENUMS_CURRENT<br>CUSTOMENUMS_DAILY_HISTORY<br>CUSTOMENUMS_EVENT</td>
        <td>O tipo de registro é identificado por meio da propriedade "enumClass". Estes são os tipos esperados:<br>CONDITION_OPTASK<br>CONDITION_PROJ<br>CONDITION_TASK<br>PRIORITY_OPTASK<br>PRIORITY_PROJ<br>PRIORITY_TASK<br>SEVERITY_OPTASK<br>STATUS_OPTASK<br>STATUS_PROJ<br>STATUS_TASK</td>
        <td>ENTEREDBYID<br>GROUPID</td>
        <td>USER_CURRENT | USERID<br>GROUP_CURRENT | GROUPID</td>
    </tr>
    <tr>
        <td>Documento</td>
        <td>Documento</td>
        <td>DOCU | Documento</td>
        <td>DOCUMENTS_CURRENT<br>DOCUMENTS_DAILY_HISTORY<br>DOCUMENTS_EVENT<br>DOCUMENTS_CUSTOM_VALUE_CURRENT<br>DOCUMENTS_CUSTOM_VALUE_DAILY_HISTORY<br>DOCUMENTS_CUSTOM_VALUE_EVENT</td>
        <td></td>
        <td>CATEGORYID<br>CHECKEDOUTBYID<br>DOCUMENTREQUESTID<br>DOCUMENTREQUESTID<br>EXCHANGERATEID<br>ITERATIONID<br>LASTNOTEID<br>LASTUPDATEDBYID<br>NOTEID<br>OBJID<br>OPTASKID<br>OWNERID<br>PORTFOLIOID<br>PROGRAMID<br>PROJECTID<br>RELEASEVERSIONID<br>TASKID<br>TEMPLATEID<br>TEMPLATETASKID<br>TOPOBJID<br>USERID</td>
        <td>CATEGORIES_CURRENT | CATEGORYID<br>USER_CURRENT | Atualmente, não há suporte para a tabela USERID<br>Self<br>Document Request<br>EXCHANGERATES_CURRENT | EXCHANGERATEID<br>ITERATIONS_CURRENT | ITERATIONID<br>NOTA_ATUAL | NOTEID<br>USER_CURRENT | ID DE USUÁRIO<br>NOTA_ATUAL | NOTEID<br>Variável dependendo do valor de DOCOBJCODE<br>OPTASK_CURRENT | OPTASKID<br>USER_CURRENT | USERID<br>PORTFOLIO_CURRENT | PORTFOLIOID<br>PROGRAMA_ATUAL | PROGRAMID<br>PROJECT_CURRENT | PROJECTID<br>Não há suporte para a tabela de versão no momento<br>TASK_CURRENT | TASKID<br>MODELOS_ATUAIS | TEMPLATEID<br>TEMPLATETASKS_CURRENT | TEMPLATETASKID<br>Variável dependendo do valor TOPOBJCODE<br>USER_CURRENT | USERID</td>
    </tr>
    <tr>
        <td>Aprovação de documento</td>
        <td>Aprovação de documento</td>
        <td>DOCAPL | Aprovação de documento</td>
        <td>DOCAPPROVALS_CURRENT<br>DOCAPPROVALS_DAILY_HISTORY<br>DOCAPPROVALS_EVENT</td>
        <td></td>
        <td>APPROVERID<br>DOCAPPROVALID (self)<br>DOCUMENTID<br>NOTEID<br>REQUESTORID<br>SYSID</td>
        <td>USERS_CURRENT | USERID <br>Self<br>DOCUMENTS_CURRENT | DOCUMENTID<br>NOTES_CURRENT | NOTEID<br>USERS_CURRENT | USERID <br>Não é uma relação; usada para fins de aplicativo interno</td>
    </tr>
    <tr>
        <td>Pasta de documento</td>
        <td>Pasta de documento</td>
        <td>DOCFLD | DocsFolders</td>
        <td>DOCFOLDERS_CURRENT<br>DOCFOLDERS_DAILY_HISTORY<br>DOCFOLDERS_EVENT</td>
        <td></td>
        <td>DOCFOLDERID (self)<br>ENTEREDBYID<br>ISSUEID<br>ITERATIONID    <br>LINKEDFOLDERID<br>PARENTID<br>PORTFOLIOID <br>PROGRAMID    <br>ID DO PROJETO<br>ID DO SISTEMA<br>ID DA TAREFA     <br>TEMPLATEID<br>TEMPLATETASKID<br>USERID</td>
        <td>Self<br>USERS_CURRENT | USERID<br>OPTASKS_CURRENT | OPTASKID<br>ITERATIONS_CURRENT | ITERATIONID<br>LINKEDFOLDERS_CURRENT | LINKEDFOLDERID<br>DOCFOLDERS_CURRENT | DOCFOLDERID<br>PORTFOLIO_CURRENT | PORTFOLIOID <br>PROGRAMA_ATUAL | PROGRAMID    <br>PROJETOS_ATUAIS | PROJECTID <br>Não é uma relação; usada para fins de aplicativo interno<br>TASKS_CURRENT | TASKID     <br>MODELOS_ATUAIS | TEMPLATEID<br>TEMPLATETASKS_CURRENT | TEMPLATETASKID<br>USERS_CURRENT | USERID</td>
    </tr>
    <tr>
        <td>DocumentProvideMetadata</td>
        <td>Metadados de fornecimento de documento</td>
        <td>DOCMET | MetadadosDoProvedorDeDocumentos</td>
        <td>DOCPROVIDERMETA_CURRENT<br>DOCPROVIDERMETA_DAILY_HISTORY<br>DOCPROVIDERMETA_EVENT</td>
        <td></td>
        <td>DOCPROVIDERMETAID (self) <br>SYSID</td>
        <td>Self<br>Not uma relação; usada para fins de aplicativo interno</td>
    </tr>
    <tr>
        <td>DocumentProvider</td>
        <td>Provedor do Documento</td>
        <td>DOCPRO | Provedor de documento</td>
        <td><br>DOCPROVIDERS_EVENT do DOCPROVIDERS_DAILY_HISTORY de DOCPROVIDERS_CURRENT<br></td>
        <td></td>
        <td>DOCPROVIDERCONFIGID<br>DOCPROVIDERID (self)<br>OWNERID    <br>SYSID</td>
        <td>DOCPROVIDERCONFIG_CURRENT | DOCPROVIDERCONFIGID<br>Self<br>USERS_CURRENT | USERID    <br>Não é uma relação; usada para fins de aplicativo interno</td>
    </tr>
    <tr>
        <td>DocumentProviderConfig</td>
        <td>Configuração do provedor de documentos</td>
        <td>DOCCFG | DocumentProviderConfig</td>
        <td>DOCPROVIDERCONFIG_CURRENT<br>DOCPROVIDERCONFIG_DAILY_HISTORY<br>DOCPROVIDERCONFIG_EVENT</td>
        <td></td>
        <td>DOCPROVIDERCONFIGID (self)<br>SYSID</td>
        <td>Self<br>Not uma relação; usada para fins de aplicativo interno</td>
    </tr>
    <tr>
        <td>VersãoDocumento</td>
        <td>Versão do Documento</td>
        <td>DOCV | Versão do documento</td>
        <td>DOCUMENTVERSIONS_CURRENT<br>DOCUMENTVERSIONS_DAILY_HISTORY<br>DOCUMENTVERSIONS_EVENT</td>
        <td></td>
        <td>DOCUMENTID<br>DOCUMENTPROVIDERID<br>DOCUMENTVERSIONID<br>ENTEREDBYID<br>EXTERNALSTORAGEID<br>PROOFAPPROVALSTATUSID<br>PROOFEDBYUSERID<br>PROOFID<br>PROOFOWNERID<br>PROOFSTAGEID</td>
        <td>DOCUMENT_CURRENT | DOCUMENTID<br>DOCPROVIDERS_CURRENT | DOCUMENTPROVIDERID<br>Self<br>USER_CURRENT | USERID<br>ID externa<br>Tabela de status de aprovação de prova não suportada atualmente<br>USER_CURRENT | USERID<br>Tabela de prova não suportada atualmente<br>USER_CURRENT | Atualmente, a tabela USERID<br>Preparo de prova não é suportada</td>
    </tr>
    <tr>
        <td>Taxa de câmbio</td>
        <td>Taxa de câmbio</td>
        <td>EXTRAIR | Taxa de câmbio</td>
        <td>EXCHANGERATES_CURRENT<br>EXCHANGERATES_DAILY_HISTORY<br>EXCHANGERATES_EVENT</td>
        <td></td>
        <td>EXCHANGERATEID (self)<br>PROJECTID<br>SYSID <br>TEMPLATEID  </td>
        <td>Self<br>PROJECTS_CURRENT | PROJECTID <br>Não é uma relação; usada para fins de aplicativo interno <br>TEMPLATES_CURRENT | TEMPLATEID  </td>
    </tr>
    <tr>
        <td>Despesa</td>
        <td>Despesa</td>
        <td>EXPNS | Despesa</td>
        <td>EXPENSES_CURRENT<br>EXPENSES_DAILY_HISTORY<br>EXPENSES_EVENT</td>
        <td></td>
        <td>BILLINGRECORDID<br>CATEGORYID<br>ENTEREDBYID<br>EXCHANGERATEID <br>EXPENSEID (self) <br>EXPENSETYPEID <br>LASTUPDATEDBYID <br>OBJID <br>PROJECTID<br>SYSID<br>TASKID<br>TEMPLATEID<br>TEMPLATETASKID<br>TOPOBJID</td>
        <td>BILLINGRECORDS_CURRENT | BILLINGRECORDID<br>CATEGORIES_CURRENT | CATEGORYID<br>USERS_CURRENT | USERID<br>EXCHANGERATES_CURRENT | EXCHANGERATEID <br>Self <br>EXPENSETYPES_CURRENT | EXPENSETYPEID <br>USERS_CURRENT | USERID <br>A ID do objeto identificado no campo OBJCODE <br>PROJECTS_CURRENT | PROJECTID <br>Não é uma relação; usada para fins de aplicativo interno<br>TASKS_CURRENT | TASKID<br>MODELOS_ATUAIS | TEMPLATEID<br>TEMPLATETASKS_CURRENT | TEMPLATETASKID<br>A ID do objeto identificado no campo TOPOBJCODE</td>
    </tr>
    <tr>
        <td>Tipo de Despesa</td>
        <td>Tipo de Despesa</td>
        <td>EXPTYP | Tipo de Despesa</td>
        <td>EXPENSETYPES_CURRENT<br>EXPENSETYPES_DAILY_HISTORY<br>EXPENSETYPES_EVENT</td>
        <td></td>
        <td>APPGLOBALID<br>EXPENSETYPEID (self)<br>OBJID  <br>SYSID  </td>
        <td>Não é uma relação; usada para fins de aplicativo interno<br>Self<br>A ID do objeto identificado no campo OBJCODE <br>Não é uma relação; usada para fins de aplicativo interno  </td>
    </tr>
    <tr>
        <td>Grupo</td>
        <td>Grupo</td>
        <td>GRUPO | Grupo</td>
        <td>GROUPS_CURRENT<br>GROUPS_DAILY_HISTORY<br>GROUPS_EVENT</td>
        <td></td>
        <td>BUSINESSLEADERID<br>CATEGORYID<br>ENTEREDBYID<br>GROUPID<br>LAYOUTTEMPLATEID<br>PARENTID<br>ROOTID<br>UITEMPLATEID</td>
        <td>USER_CURRENT | ID DE USUÁRIO<br>CATEGORIES_CURRENT | CATEGORYID<br>USER_CURRENT | A tabela USERID<br>Self<br>Modelo de Layout não terá suporte<br>GROUP_CURRENT | GROUPID<br>GROUP_CURRENT | GROUPID<br>UITEMPLATES_CURRENT | UITEMPLATEID</td>
    </tr>
    <tr>
        <td>Hora</td>
        <td>Hora</td>
        <td>HORA | Hora</td>
        <td>HOURS_CURRENT<br>HOURS_DAILY_HISTORY<br>HOURS_EVENT</td>
        <td></td>
        <td>APPROVEDBYID<br>BILLINGRECORDID<br>CATEGORYID<br>CLASSIFIERID<br>DUPID<br>EXCHANGERATEID<br>EXTERNALTIMESHEETID<br>HOURID<br>HOURTYPEID<br>LASTUPDATEDBYID<br>OPTASKID<br>OWNERID<br>PROJECTID<br>PROJECTOVERHEADID<br>}ID DA FUNÇÃO<br>ID DA TAREFA<br>ID DA PLANILHA DE HORAS</td>
        <td>USER_CURRENT | USERID<br>BILLINGRECORDS_CURRENT | BILLINGRECORDID<br>CATEGORIES_CURRENT | CATEGORYID<br>Não há suporte para a tabela de classificador no momento<br>Não é uma relação; usada para fins de aplicativo interno<br>EXCHANGERATES_CURRENT | EXCHANGERATEID<br>Não é uma relação Workfront; usado para integração a sistemas externos<br>Self<br>HOURTYPE_CURRENT | HOURTYPEID<br>USER_CURRENT | USERID<br>OPTASK_CURRENT | OPTASKID<br>USER_CURRENT | USERID<br>PROJECT_CURRENT | PROJECTID<br>Não é uma relação; usado para fins de aplicativo interno<br>ROLE_CURRENT | ROLEID<br>TASK_CURRENT | TASKID<br>PLANILHA_DE_HORAS_ATUAL | TIMESHEETID</td>
    </tr>
    <tr>
        <td>Tipo de hora</td>
        <td>Tipo de hora</td>
        <td>HORA | Tipo de Hora</td>
        <td>HOURTYPES_CURRENT</td>
        <td></td>
        <td>APPGLOBALID<br>HOURTYPEID<br>OBJID</td>
        <td>Não é uma relação; usada para fins de aplicativo interno<br>Self<br>Não é uma relação; usada para fins de aplicativo interno</td>
    </tr>
    <tr>
        <td>Iteração</td>
        <td>Iteração</td>
        <td>ITRN | Iteração</td>
        <td>ITERATIONS_CURRENT<br>ITERATIONS_DAILY_HISTORY<br>ITERATIONS_EVENT</td>
        <td></td>
        <td>CATEGORYID<br>ENTEREDBYID<br>ITERATIONID (self)<br>LASTUPDATEDBYID<br>OWNERID<br>SYSID<br>TEAMID</td>
        <td>CATEGORIES_CURRENT | CATEGORYID<br>USERS_CURRENT | ID DE USUÁRIO <br>Self<br>USERS_CURRENT | USERID <br>USERS_CURRENT | USERID <br>Não é uma relação; usada para fins de aplicativo interno<br>TEAMS_CURRENT | TEAMID</td>
    </tr>
    <tr>
        <td>Entrada no Relatório</td>
        <td>Entrada no Relatório</td>
        <td>JRNLE | Entrada do diário</td>
        <td><br>JOURNALENTRIES_EVENT de JOURNALENTRIES_DAILY_HISTORY de JOURNALENTRIES_CURRENT<br></td>
        <td></td>
        <td>APPROVERSTATUSID<br>ASSIGNMENTID<br>AUDITRECORDID<br>BASELINEID <br>BILLINGRECORDID<br>COMPANYID <br>DOCUMENTID <br>DOCUMENTSHAREID <br>EDITEDBYID<br>EXPENSEID<br>HOURID INITIATIVEID<br><br>JOURNALENTRIEID (self)<br>OBJID OPTASKID<br>PORTFOLIOID PROGRAMID<br>PROJECTID<br><br>SUBOBJID<br>SUBSCRIBEID<br>SYSID TASKID<br><br>TIMESHEETID<br><br>TOPBJID<br><br>USERID</td>
        <td>APPROVERSTATUSES_CURRENT | APPROVERSTATUSID<br>ASSIGNMENTS_CURRENT | A tabela de registro ASSIGNMENTID<br>de auditoria não tem suporte atualmente<br>BASELINES_CURRENT | BASELINEID <br>BILLINGRECORDS_CURRENT | BILLINGRECORDID<br>COMPANIES_CURRENT | COMPANYID <br>DOCUMENTS_CURRENT | A tabela de Compartilhamento de Documentos <br>DOCUMENTID não tem suporte atualmente <br>USERS_CURRENT | USERID<br>EXPENSES_CURRENT | EXPENSEID<br>HOURS_CURRENT | HOURID<br>Tabela de iniciativa sem suporte atualmente<br>Self<br>A ID do objeto identificado no campo OBJCODE<br>OPTASKS_CURRENT | OPTASKID<br>PORTFOLIO_CURRENT | PORTFOLIOID<br>PROGRAMA_ATUAL | PROGRAMID<br>PROJECTS_CURRENT | PROJECTID <br>A ID do objeto identificado no campo SUBOBJCODE<br>Não há suporte para a tabela de inscrição no momento<br>Não é uma relação; usada para fins de aplicativo interno<br>TASKS_CURRENT | TASKID<br>MODELOS_ATUAIS | TEMPLATEID<br>TIMESHEETS_CURRENT | TIMESHEETID<br>A ID do objeto identificado no campo TOPOBJCODE<br>USERS_CURRENT | USERID</td>
    </tr>
    <tr>
        <td>LinkedFolder</td>
        <td>LinkedFolder</td>
        <td>LNKFDR | LinkedFolder</td>
        <td>LINKEDFOLDERS_CURRENT<br>LINKEDFOLDERS_DAILY_HISTORY<br>LINKEDFOLDERS_EVENT</td>
        <td></td>
        <td>DOCUMENTPROVIDERID<br>EXTERNALSTORAGEID<br>FOLDERID<br>LINKEDBYID<br>LINKEDFOLDERID (self)<br>SYSID</td>
        <td>DOCPROVIDERS_CURRENT | DOCPROVIDERID<br>ID Externa<br>DOCFOLDERS_CURRENT | DOCFOLDERID<br>USERS_CURRENT | USERID <br>Self<br>Não é uma relação; usada para fins de aplicativo interno  </td>
    </tr>
    <tr>
        <td>Marco</td>
        <td>Marco</td>
        <td>MILHA | Etapa</td>
        <td>MARCOS_ATUAIS<br>MARCOS_HISTÓRICO_DIÁRIO<br>MARCOS_EVENTO</td>
        <td></td>
        <td>LASTUPDATEDBYID<br>MILESTONEID<br>MILESTONEPATHID</td>
        <td>USER_CURRENT | USERID<br>Self<br>MILESTONEPATH_CURRENT | MILESTONE ID</td>
    </tr>
    <tr>
        <td>CaminhoEtapas</td>
        <td>Caminho de Etapas</td>
        <td>MPATH | Caminho de Etapas</td>
        <td>MILESTONEPATHS_CURRENT<br>MILESTONEPATHS_DAILY_HISTORY<br>MILESTONEPATHS_EVENT</td>
        <td></td>
        <td>ENTEREDBYID<br>LASTUPDATEDBYID<br>MILESTONEPATHID</td>
        <td>USER_CURRENT | USERID<br>USER_CURRENT | ID DE USUÁRIO<br>Auto</td>
    </tr>
    <tr>
        <td>NonLaborResource</td>
        <td>Recurso não trabalhista</td>
        <td>NLBR | Recurso não mão de obra</td>
        <td>NONLABORRESOURCES_CURRENT<br>NONLABORRESOURCES_DAILY_HISTORY<br>NONLABORRESOURCES_EVENT</td>
        <td></td>
        <td>CATEGORYID<br>NONLABORRESOURCEID (self)<br>ENTEREDBYID<br>HOMEGROUPID<br>LASTUPDATEDBYID<br>NONLABORRESOURCECATEGORYID <br>SYSID  </td>
        <td>CATEGORIES_CURRENT | CATEGORYID<br>Self<br>USERS_CURRENT | USERID <br>GROUPS_CURRENT | GROUPID<br>USERS_CURRENT | USERID <br>Não há suporte para a tabela de Categoria de Recurso Não Mão-de-Obra no momento <br>Não é uma relação; usada para fins de aplicativo interno    </td>
    </tr>
    <tr>
        <td>Dia Não Útil</td>
        <td>Exceção de programação</td>
        <td>NONWKD | Dia Não Útil</td>
        <td>NONWORKDAYS_CURRENT<br>NONWORKDAYS_DAILY_HISTORY<br>NONWORKDAYS_EVENT</td>
        <td></td>
        <td>NONWORKDAYID (self)<br>OBJID  <br>SCHEDULEID  <br>SYSID  <br>USERID  </td>
        <td>Auto-ID<br>do objeto identificado no campo  <br>OBJCODE SCHEDULES_CURRENT | SCHEDULEID  <br>Não é um relacionamento; usado para fins  <br>internos de aplicativo USERS_CURRENT | ID DE USUÁRIO  </td>
    </tr>
    <tr>
        <td>Nota</td>
        <td>Nota</td>
        <td>NOTA | Nota</td>
        <td>NOTES_CURRENT<br>NOTES_DAILY_HISTORY<br>NOTES_EVENT</td>
        <td></td>
        <td>ATTACHDOCUMENTID<br>ATTACHOBJID<br>ATTACHOPTASKID<br>ATTACHWORKID<br>ATTACHWORKUSERID<br>AUDITRECORDID<br>COMPANYID<br>DOCUMENTID<br>EXTERNALSERVICEID<br>ITERATIONID<br>NOTEID<br>OBJID<br>OPTASKID<br>OWNERID<br>PARENTENDORSEMENTID<br> 4}PARENTJOURNALENTRYID<br>PARENTNOTEID<br>PORTFOLIOID<br>PROGRAMID<br>PROJECTID<br>PROOFACTIONID<br>PROOFID<br>RICHTEXTNOTEID<br>TASKID<br>TEMPLATEID<br>TEMPLATETASKID<br>THREADID<br>TIMESHEETID{22 7}TOPOBJID<br>USERID<br></td>
        <td>DOCUMENT_CURRENT | DOCUMENTID<br>Variável dependendo de ATTACHOBJCODE<br>OPTASK_CURRENT | OPTASKID<br>WORKITEMS_CURRENT<br>USER_CURRENT | No momento, não há suporte para a tabela de Registro de Auditoria USERID<br>COMPANIES_CURRENT | COMPANYID <br>DOCUMENT_CURRENT | DOCUMENTID<br>Não é um relacionamento Workfront; usado para integração a sistemas externos<br>ITERATIONS_CURRENT | ITERATIONID<br>Self<br>Variável dependendo de NOTEOBJCODE<br>OPTASK_CURRENT | OPTASKID<br>USER_CURRENT | USERID<br>Tabela de endosso sem suporte no momento<br>JOURNALENTRIES_CURRENT | JOURNALENTRYID<br>NOTA_ATUAL | NOTEID<br>PORTFOLIO_CURRENT | PORTFOLIOID<br>PROGRAMA_ATUAL | PROGRAMID<br>PROJECT_CURRENT | PROJECTID<br>Tabela de ação de prova sem suporte no momento<br>A tabela de prova não tem suporte no momento<br>RESERVEDTEXTNOTES_CURRENT | RICHTEXTNOTEID<br>TASK_CURRENT | TASKID<br>MODELOS_ATUAIS | TEMPLATEID<br>TEMPLATETASKS_CURRENT | TEMPLATETASKID<br>NOTA_ATUAL | NOTEID<br>PLANILHA_DE_HORAS_ATUAL | TIMESHEETID<br>Variável dependendo de TOPOBJCODE<br>USER_CURRENT | USERID<br></td>
    </tr>
    <tr>
        <td>Integração de objetos</td>
        <td>Integração de objetos</td>
        <td>OBJINT | ObjectIntegration</td>
        <td>OBJECTINTEGRATION_CURRENT<br>OBJECTINTEGRATION_DAILY_HISTORY<br>OBJECTINTEGRATION_EVENT</td>
        <td></td>
        <td>LINKEDOBJECTID<br>OBJECTINTEGRATIONID   (self)<br>OBJID <br>SYSID  </td>
        <td>A ID do objeto identificado no campo LINKEDOBJECTCODE <br>Self<br>A ID do objeto identificado no campo OBJCODE <br>Não é uma relação; usada para fins de aplicativo interno  </td>
    </tr>
    <tr>
        <td>Categoria de objetos</td>
        <td>Categorias de objeto</td>
        <td>OBJCAT | Categoria de objeto</td>
        <td>OBJECTSCATEGORIES_CURRENT<br>OBJECTSCATEGORIES_DAILY_HISTORY<br>OBJECTSCATEGORIES_EVENT</td>
        <td></td>
        <td>CATEGORYID<br>OBJECTSCATEGORYID (self)<br>OBJID <br>SYSID  </td>
        <td>CATEGORIES_CURRENT | CATEGORYID<br>Self<br>A ID do objeto identificado no campo OBJCODE <br>Não é uma relação; usada para fins de aplicativo interno  </td>
    </tr>
    <tr>
        <td>OpTask</td>
        <td>Problema, Solicitação</td>
        <td>OPTASK | Problema</td>
        <td>OPTASKS_CURRENT<br>OPTASKS_DAILY_HISTORY<br>OPTASKS_EVENT<br>OPTASKS_CUSTOM_VALUE_CURRENT<br>OPTASKS_CUSTOM_VALUE_DAILY_HISTORY<br>OPTASKS_CUSTOM_VALUE_EVENT</td>
        <td></td>
        <td>APPROVALPROCESSID<br>ASSIGNEDTOID<br>CATEGORYID<br>CURRENTAPPROVALSTEPID<br>ENTEREDBYID<br>EXCHANGERATEID<br>ITERATIONID<br>KANBANBOARDID<br>LASTCONDITIONNOTEID<br>LASTNOTEID<br>LASTUPDATEDBYID<br>OPTASKID<br>OWNERID<br>PROJECTID <br>QUEUEDEFID<br>QUEUETOPICID<br>RESOLVEOPTASKID<br>RESOLVEPROJECTID<br>RESOLVETASKID<br>RESOLVINGOBJID<br>ROLEID<br>SOURCEOBJID<br>SOURCETASKID<br>SUBMITTEDBYID<br>TEAMID</td>
        <td>APPROVALPROCESSES_CURRENT | APPROVALPROCESSID<br>USER_CURRENT | ID DE USUÁRIO<br>CATEGORIES_CURRENT | CATEGORYID<br>APPROVALSTEPS_CURRENT | APPROVALSTEPID<br>USER_CURRENT | USERID<br>EXCHANGERATES_CURRENT | EXCHANGERATEID<br>ITERATIONS_CURRENT | ITERATIONID<br>Não há suporte para a tabela de Quadro Kanban atualmente<br>NOTE_CURRENT | NOTEID<br>NOTA_ATUAL | NOTEID<br>USER_CURRENT | USERID<br>Self<br>USER_CURRENT | USERID<br>PROJECT_CURRENT | PROJECTID<br>Tabela de Definição de Fila sem suporte no momento<br>Tabela de Tópicos de Fila sem suporte no momento<br>OPTASK_CURRENT | OPTASKID<br>PROJETO_ATUAL | PROJECTID<br>TASK_CURRENT | TASKID<br>Variável dependendo de RESOLVINGOBJCODE<br>ROLE_CURRENT | ROLEID<br>Variável dependendo de SOURCEOBJCODE<br>TASK_CURRENT | TASKID<br>USER_CURRENT | ID DE USUÁRIO<br>EQUIPE_ATUAL | TEAMID</td>
    </tr>
    <tr>
        <td>Parâmetro</td>
        <td>Campo personalizado</td>
        <td>PARAM | Parâmetro</td>
        <td><br>PARAMETERS_EVENT PARAMETERS_CURRENT de PARAMETERS_DAILY_HISTORY<br></td>
        <td></td>
        <td>LASTUPDATEDBYID<br>PARAMETERFILTERID<br>PARAMETERID (self)<br>SYSID  </td>
        <td>USERS_CURRENT | Parâmetro USERID<br>Filtrar tabela não suportado no momento<br>Self<br>Not a relationship; usado para fins aplicativo internas  </td>
    </tr>
    <tr>
        <td>Opção de parâmetro</td>
        <td>Opção de parâmetro</td>
        <td>POPT | Opção de parâmetro</td>
        <td>PARAMETEROPTIONS_CURRENT<br>PARAMETEROPTIONS_DAILY_HISTORY<br>PARAMETEROPTIONS_EVENT</td>
        <td></td>
        <td>PARAMETERID<br>PARAMETEROPTIONID (self) <br>SYSID  </td>
        <td>PARAMETERS_CURRENT | PARAMETERID <br>Self <br>Não é uma relação; usada para fins de aplicativo interno  </td>
    </tr>
    <tr>
        <td>Seção do Portal</td>
        <td>Relatório</td>
        <td>PTLSEC | Relatório</td>
        <td>PORTALSECTIONS_CURRENT<br>PORTALSECTIONS_DAILY_HISTORY<br>PORTALSECTIONS_EVENT</td>
        <td></td>
        <td>APPGLOBALID<br>ENTEREDBYID<br>FILTERID<br>GROUPBYID<br>LASTUPDATEDBYID<br>LASTVIEWEDBYID<br>OBJID<br>PORTALSECTIONID (self)<br>PREFERENCEID<br>PUBLICRUNASUSERID<br>REPORTFOLDERID<br>RUNASUSERID<br>SCHEDULEDREPORTID<br>SYSID<br>3}VIEWID</td>
        <td>Não é uma relação; usada para fins de aplicativo interno <br>USERS_CURRENT | USERID <br>UIFILTERS_CURRENT | FILTERID<br>UIGROUPBYS_CURRENT | GROUPBYID<br>USERS_CURRENT | USERID <br>USERS_CURRENT | USERID <br>A ID do objeto identificado no campo OBJOBJCODE<br>Self<br>PREFERENCES_CURRENT | PREFERENCEID<br>USERS_CURRENT | USERID <br>REPORTFOLDERS_CURRENT | REPORTFOLDERID<br>USERS_CURRENT | USERID <br>A tabela de Relatórios Agendados não tem suporte no momento<br>Não é uma relação; usada para fins de aplicativo interno <br>UIVIEWS_CURRENT | VIEWID</td>
    </tr>
    <tr>
        <td>Guia Portal</td>
        <td>Painel</td>
        <td>PTLTAB | Painel</td>
        <td>PORTALTABS_CURRENT<br>PORTALTABS_DAILY_HISTORY<br>PORTALTABS_EVENT</td>
        <td></td>
        <td>DOCID<br>LASTUPDATEDBYID<br>PORTALPROFILEID<br>PORTALTABID (self)<br>SYSID<br>USERID</td>
        <td>Não é uma relação; usada para fins de aplicativo interno <br>USERS_CURRENT | A tabela de Perfil de Portal <br>USERID não terá suporte <br>Self<br>Not a relationship; usada para fins de aplicativo interno <br>USERS_CURRENT | USERID  </td>
    </tr>
    <tr>
        <td>Seção de Guias do Portal</td>
        <td>Seção do painel</td>
        <td>PRTBSC | Seção de Guias do Portal</td>
        <td>PORTALTABSPORTALSECTIONS_CURRENT<br>PORTALTABSPORTALSECTIONS_DAILY_HISTORY<br>PORTALTABSPORTALSECTIONS_EVENT</td>
        <td></td>
        <td>CALENDARPORTALSECTIONID<br>EXTERNALSECTIONID<br>INTERNALSECTIONID <br>PORTALSECTIONOBJID <br>PORTALTABID<br>PORTALTABSECTIONID (self)<br>SYSID</td>
        <td>Não há suporte para a Seção do Portal de Calendário no momento<br>A tabela Seções Externas não tem suporte no momento<br>PORTALSECTIONS_CURRENT | PORTALSECTIONID <br>A ID do objeto identificado no campo PORTALSECTIONOBJCODE<br>PORTALTABS_CURRENT | PORTALTABID<br>Self<br>Não é uma relação; usada para fins de aplicativo interno</td>
    </tr>
    <tr>
        <td>PortalSectionLastViewer</td>
        <td>Últimos visualizadores do relatório</td>
        <td>PLSLSV | PortalSectionLastViewer</td>
        <td>REPORTLASTVIEWERS_CURRENT<br>REPORTLASTVIEWERS_DAILY_HISTORY<br>REPORTLASTVIEWERS_EVENT</td>
        <td></td>
        <td>REPORTID<br>REPORTLASTVIEWERID (self)<br>SYSID<br>VIEWERID</td>
        <td>PORTALSECTIONS_CURRENT | PORTALSECTIONID <br>REPORTLASTVIEWERID (self)<br>Não é uma relação; usada para fins de aplicativo interno<br>USERS_CURRENT | USERID  </td>
    </tr>
    <tr>
        <td>Portfólio</td>
        <td>Portfólio</td>
        <td>PORTA | Portfolio</td>
        <td>PORTFOLIO_CURRENT<br>PORTFOLIO_DAILY_HISTORY<br>PORTFOLIO_EVENT<br>PORTFOLIO_CUSTOM_VALUE_CURRENT<br>PORTFOLIO_CUSTOM_VALUE_DAILY_HISTORY<br>PORTFOLIO_CUSTOM_VALUE_EVENT</td>
        <td></td>
        <td>ALIGNMENTSCORECARDID<br>CATEGORYID<br>ENTEREDBYID<br>GROUPID<br>LASTUPDATEDBYID<br>OWNERID<br>PORTFOLIOID</td>
        <td>Atualmente, não há suporte para a tabela de scorecard<br>CATEGORIES_CURRENT | CATEGORYID<br>USER_CURRENT | USERID<br>GROUP_CURRENT | GROUPID<br>USER_CURRENT | USERID<br>USER_CURRENT | ID DE USUÁRIO<br>Auto</td>
    </tr>
    <tr>
        <td>Preferência</td>
        <td>Exibir, Filtrar, Agrupar, Definição de Relatório</td>
        <td>PROSET | Preferência</td>
        <td>PREFERENCES_CURRENT<br>PREFERENCES_DAILY_HISTORY<br>PREFERENCES_EVENT</td>
        <td></td>
        <td>APPGLOBALID<br>PREFERENCEID (self) <br>SYSID  </td>
        <td>Não é uma relação; usada para fins de aplicativo interno<br>Self <br>Não é uma relação; usada para fins de aplicativo interno  </td>
    </tr>
    <tr>
        <td>Programa</td>
        <td>Programa</td>
        <td>PRGM | Programa</td>
        <td>PROGRAMS_CURRENT<br>PROGRAMS_DAILY_HISTORY<br>PROGRAMS_EVENT<br>PROGRAMS_CUSTOM_VALUE_CURRENT<br>PROGRAMS_CUSTOM_VALUE_DAILY_HISTORY<br>PROGRAMS_CUSTOM_VALUE_EVENT</td>
        <td></td>
        <td>CATEGORYID<br>ENTEREDBYID<br>GROUPID<br>LASTUPDATEDBYID<br>OWNERID<br>PORTFOLIOID<br>PROGRAMID</td>
        <td>CATEGORIES_CURRENT | CATEGORYID<br>USER_CURRENT | USERID<br>GROUP_CURRENT | GROUPID<br>USER_CURRENT | USERID<br>USER_CURRENT | ID DE USUÁRIO<br>PORTFOLIO_CURRENT | PORTFOLIOID<br>Self</td>
    </tr>
    <tr>
        <td>Projeto</td>
        <td>Projeto</td>
        <td>PROJ | Projeto</td>
        <td>PROJECTS_CURRENT<br>PROJECTS_DAILY_HISTORY<br>PROJECTS_EVENT<br>PROJECTS_CUSTOM_VALUE_CURRENT<br>PROJECTS_CUSTOM_VALUE_DAILY_HISTORY<br>PROJECTS_CUSTOM_VALUE_EVENT</td>
        <td></td>
        <td>AEMNATIVEFOLDERTREESREFID<br>ALIGNMENTSCORECARDID<br>APPROVALPROCESSID<br>ATTACHEDRATECARDID<br>CATEGORYID<br>COMPANYID<br>CONVERTEDOPTASKID<br>CONVERTEDOPTASKORIGINATORID<br>CURRENTAPPROVALSTEPID<br>DELIVERABLESCORECARDID<br>ENTEREDBYID<br>GROGROID PID<br>LASTCONDITIONNOTEID<br>LASTNOTEID<br>LASTUPDATEDBYID<br>MILESTONEPATHID<br>OWNERID<br>POPACCOUNTID<br>PORTFOLIOID<br>PRIVATERATECARDID<br>PROGRAMID<br>PROJECTID<br>QUEUEDEFID<br>REJECTIONISSUB ID<br>RESOURCEPOOLID<br>SCHEDULEID<br>SPONSORID<br>SUBMITTEDBYID<br>TEAMID<br>TEMPLATEID</td>
        <td>Não é uma relação Workfront; usada para integração a sistemas externos<br>Não há suporte para a tabela de scorecard atualmente<br>APPROVALPROCESSES_CURRENT | APPROVALPROCESSID<br>RATECARD_CURRENT | RATECARDID<br>CATEGORIES_CURRENT | CATEGORYID<br>COMPANIES_CURRENT | COMPANYID <br>OPTASK_CURRENT | OPTASKID<br>USER_CURRENT | ID DE USUÁRIO<br>APPROVALSTEPS_CURRENT | Atualmente, não há suporte para a tabela APPROVALSTEPID<br>Scorecard<br>USER_CURRENT | USERID<br>GROUP_CURRENT | GROUPID<br>NOTA_ATUAL | NOTEID<br>NOTA_ATUAL | NOTEID<br>USER_CURRENT | USERID<br>MILESTONEPATH_CURRENT | MILESTONEPATHID<br>USER_CURRENT | Atualmente, não há suporte para a tabela de conta POP USERID<br>PORTFOLIO_CURRENT | PORTFOLIOID<br>RATECARD_CURRENT | RATECARDID<br>PROGRAM_CURRENT | Tabela de Definição de Fila PROGRAMID<br>Self<br>sem suporte no momento<br>OPTASK_CURRENT | OPTASKID<br>POOLSDERECURSOS_ATUAIS | RESOURCEPOOLID<br>SCHEDULE_CURRENT | SCHEDULEID<br>USER_CURRENT | USERID<br>USER_CURRENT | ID DE USUÁRIO<br>EQUIPE_ATUAL | TEAMID<br>MODELOS_ATUAIS | TEMPLATEID<br></td>
    </tr>
    <tr>
        <td>RateCard</td>
        <td>Cartão de tarifa</td>
        <td>RTCRD |Cartão de tarifa</td>
        <td>RATECARD_CURRENT<br>RATECARD_DAILY_HISTORY<br>RATECARD_EVENT</td>
        <td></td>
        <td>CATEGORYID<br>ENTEREDBYID<br>LASTUPDATEDBYID <br>RATECARDID (self) <br>SECURITYROOTID <br>SOURCEID<br>SYSID</td>
        <td>CATEGORYID<br>USERS_CURRENT | USERID <br>USERS_CURRENT | USERID    <br>Self<br>A ID do objeto identificado no campo SECURITYOBJCODE <br>A ID do objeto identificado no campo SOURCEOBJCODE<br>Não é uma relação; usada para fins de aplicativo interno  </td>
    </tr>
    <tr>
        <td>Pasta de Relatório</td>
        <td>Pasta de Relatório</td>
        <td>RPTFDR | Pasta de Relatório</td>
        <td>REPORTFOLDERS_CURRENT<br>REPORTFOLDERS_DAILY_HISTORY<br>REPORTFOLDERS_EVENT</td>
        <td></td>
        <td>REPORTFOLDERID (self) <br>SYSID  </td>
        <td>Próprio <br>Não é uma relação; usado para fins de aplicativo interno  </td>
    </tr>
    <tr>
        <td>Tempo reservado</td>
        <td>Tempo livre (pessoal)</td>
        <td>RESVT | Folga</td>
        <td>RESERVEDTIMES_CURRENT<br>RESERVEDTIMES_DAILY_HISTORY<br>RESERVEDTIMES_EVENT</td>
        <td></td>
        <td>RESERVEDTIMEID (self) <br>SYSID<br>TASKID<br>USERID  </td>
        <td>Self<br>Not uma relação; usado para fins internos do aplicativo<br>TASKS_CURRENT | TASKID<br>USERS_CURRENT | USERID  </td>
    </tr>
    <tr>
        <td>Conjunto de Recursos</td>
        <td>Conjunto de Recursos</td>
        <td>RSPL | Conjunto de recursos</td>
        <td>RSRCPOOLS_CURRENT<br>RSRCPOOLS_DAILY_HISTORY<br>RSRCPOOLS_EVENT</td>
        <td></td>
        <td>ENTEREDBYID<br>LASTUPDATEDBYID <br>RESOURCEPOOLID (self)<br>SYSID  </td>
        <td>USERS_CURRENT | USERID <br>USERS_CURRENT | USERID <br>Self<br>Não é uma relação; usada para fins de aplicativo interno  </td>
    </tr>
    <tr>
        <td>Nota em Rich Text</td>
        <td>Nota em Rich Text</td>
        <td>RHNOTE | Nota em Rich Text</td>
        <td>RESERVEDTEXTNOTES_CURRENT<br>RESERVEDTEXTNOTES_DAILY_HISTORY<br>RESERVEDTEXTNOTES_EVENT</td>
        <td></td>
        <td>RICHTEXTNOTEID (self) <br>SYSID  </td>
        <td>Próprio <br>Não é uma relação; usado para fins de aplicativo interno  </td>
    </tr>
    <tr>
        <td>Valor do parâmetro Rich Text</td>
        <td>Valor do parâmetro Rich Text</td>
        <td>RCHVAL | RichTextParameterValue</td>
        <td>RICHTEXTPARAMETERVALUES_CURRENT<br>RICHTEXTPARAMETERVALUES_DAILY_HISTORY<br>RICHTEXTPARAMETERVALUES_EVENT</td>
        <td></td>
        <td>PARAMETERVALUEID<br>RICHTEXTPARAMETERVALUEID (self)  <br>SYSID  </td>
        <td>Parâmetro Valor tabela não suportado no<br>momento Auto-not  <br>uma relação; usado para fins internos aplicativo  </td>
    </tr>
    <tr>
        <td>Risco</td>
        <td>Risco</td>
        <td>RISCO | Risco</td>
        <td>RISKS_CURRENT<br>RISKS_DAILY_HISTORY<br>RISKS_EVENT</td>
        <td></td>
        <td>ENTEREDBYID<br>EXCHANGERATEID<br>LASTUPDATEDBYID <br>PROJECTID <br>RISKID (self)<br>RISKTYPEID<br>SYSID<br>TEMPLATEID</td>
        <td>USERS_CURRENT | USERID<br>EXCHANGERATES_CURRENT | EXCHANGERATEID<br>USERS_CURRENT | ID DE USUÁRIO <br>PROJECTS_CURRENT | PROJECTID   <br>Self<br>RISKTYPES_CURRENT | RISKTYPEID<br>Não é uma relação; usado para fins de aplicativo interno<br>TEMPLATES_CURRENT | TEMPLATEID</td>
    </tr>
    <tr>
        <td>Tipo de Risco</td>
        <td>Tipo de Risco</td>
        <td>RSKTYP | Tipo de Risco</td>
        <td>RISKTYPES_CURRENT<br>RISKTYPES_DAILY_HISTORY<br>RISKTYPES_EVENT</td>
        <td></td>
        <td>RISKTYPEID<br>SYSID</td>
        <td>Self<br>Not uma relação; usada para fins de aplicativo interno</td>
    </tr>
    <tr>
        <td>Função</td>
        <td>Função no trabalho</td>
        <td>FUNÇÃO | Função de trabalho</td>
        <td>ROLES_CURRENT<br>HISTÓRICO_DIÁRIO_DE_FUNÇÕES<br>EVENTO_DE_FUNÇÕES</td>
        <td></td>
        <td>ENTEREDBYID<br>LAYOUTTEMPLATEID<br>PRIVATERATECARDID<br>ROLEID<br>UITEMPLATEID</td>
        <td>USER_CURRENT | A tabela USERID<br>Modelo de Layout não terá suporte<br>RATECARD_CURRENT | RATECARDID<br>Self<br>UITEMPLATES_CURRENT |UITEMPLATEID</td>
    </tr>
    <tr>
        <td>Agendar</td>
        <td>Agendar</td>
        <td>SCHED | Agendar</td>
        <td>SCHEDULES_CURRENT<br>SCHEDULES_DAILY_HISTORY<br>SCHEDULES_EVENT</td>
        <td></td>
        <td>ENTEREDBYID<br>GROUPID<br>HOMEGROUPID<br>SCHEDULEID</td>
        <td>USER_CURRENT | USERID<br>GROUP_CURRENT | GROUPID<br>GROUP_CURRENT | GROUPID<br>Self</td>
    </tr>
    <tr>
        <td>Aprovador da etapa</td>
        <td>Aprovador da etapa</td>
        <td>SPAPVR | Aprovador de estágio</td>
        <td>STEPAPPROVERS_CURRENT<br>STEPAPPROVERS_DAILY_HISTORY<br>STEPAPPROVERS_EVENT</td>
        <td></td>
        <td>APPROVALSTEPID<br>ROLEID<br>STEPAPPROVERID (self)<br>SYSID <br>TEAMID<br>USERID</td>
        <td>APPROVALSTEPS_CURRENT | APPROVALSTEPID<br>FUNÇÕES_ATUAIS | ROLEID<br>Self<br>Não é uma relação; usada para fins de aplicativo interno <br>TEAMS_CURRENT | TEAMID<br>USUÁRIOS_ATUAIS | USERID</td>
    </tr>
    <tr>
        <td>Tarefa</td>
        <td>Tarefa</td>
        <td>TAREFA | Tarefa</td>
        <td>TASKS_CURRENT<br>TASKS_DAILY_HISTORY<br>TASKS_EVENT<br>TASKS_CUSTOM_VALUE_CURRENT<br>TASKS_CUSTOM_VALUE_DAILY_HISTORY<br>TASKS_CUSTOM_VALUE_EVENT</td>
        <td></td>
        <td>APPROVALPROCESSID<br>ASSIGNEDTOID<br>BILLINGRECORDID<br>CATEGORYID<br>CONVERTEDOPTASKID<br>CONVERTEDOPTASKORIGINATORID<br>CURRENTAPPROVALSTEPID<br>ENTEREDBYID<br>EXCHANGERATEID<br>GROUPID<br>ITERATIONID<br>KANBANBOARDID<br>LASTCONDITIONNOID<br>LASTNOTEID<br>LASTUPDATEDBYID<br>MILESTONEID<br>PARENTID<br>PROJECTID<br>RECURRENCERULEID<br>REJECTIONISSUEID<br>RESERVEDTIMEID<br>ROLEID<br>SUBMITTEDBYID<br>TASKID<br>TEAMID<br>TEMPLATEID SKID</td>
        <td>APPROVALPROCESSES_CURRENT | APPROVALPROCESSID<br>USER_CURRENT | USERID<br>BILLINGRECORDS_CURRENT | BILLINGRECORDID<br>CATEGORIES_CURRENT | CATEGORYID<br>OPTASK_CURRENT | OPTASKID<br>USER_CURRENT | ID DE USUÁRIO<br>APPROVALSTEPS_CURRENT | APPROVALSTEPID<br>USER_CURRENT | USERID<br>EXCHANGERATES_CURRENT | EXCHANGERATEID<br>GROUP_CURRENT | GROUPID<br>ITERATIONS_CURRENT | ITERATIONID<br>Tabela de Quadro Kanban não suportada atualmente<br>NOTE_CURRENT | NOTEID<br>NOTA_ATUAL | NOTEID<br>USER_CURRENT | ID DE USUÁRIO<br>MARCO_ATUAL | MILESTONEID<br>TASK_CURRENT | TASKID<br>PROJECT_CURRENT | PROJECTID<br>A tabela de Regras de Recorrência não tem suporte no momento<br>OPTASK_CURRENT | OPTASKID<br>RESERVEDTIMES_CURRENT | RESERVEDTIMEID<br>ROLE_CURRENT | ROLEID<br>USER_CURRENT | USERID<br>Self<br>TEAM_CURRENT | TEAMID<br>TEMPLATETASKS_CURRENT | TEMPLATETASKID</td>
    </tr>
    <tr>
        <td>Predecessora da Tarefa</td>
        <td>Predecessor</td>
        <td>PRED | Predecessora</td>
        <td>PREDECESSORS_CURRENT<br>PREDECESSORS_DAILY_HISTORY<br>PREDECESSORS_EVENT</td>
        <td></td>
        <td>ID (própria)<br>PREDECESSORID<br>SUCCESSORID <br>SYSID</td>
        <td>Self<br>TASKS_CURRENT | TASKID<br>TAREFAS_ATUAIS | TASKID <br>Não é uma relação; usada para fins de aplicativo interno</td>
    </tr>
    <tr>
        <td>Equipe</td>
        <td>Equipe</td>
        <td>TEAMOB | Equipe</td>
        <td>TEAMS_CURRENT<br>TEAMS_DAILY_HISTORY<br>TEAMS_EVENT</td>
        <td></td>
        <td>ENTEREDBYID<br>GROUPID<br>LAYOUTTEMPLATEID<br>MYWORKVIEWID<br>OWNERID<br>REQUESTSVIEWID<br>SCHEDULEID<br>TEAMID<br>UITEMPLATEID</td>
        <td>USER_CURRENT | USERID<br>GROUP_CURRENT | GROUPID<br>Não haverá suporte para a tabela de Modelo de Layout<br>UIVIEWS_CURRENT | UIVIEWID<br>USER_CURRENT | ID DE USUÁRIO<br>UIVIEWS_CURRENT | UIVIEWID<br>SCHEDULE_CURRENT | SCHEDULEID<br>Self<br>UITEMPLATES_CURRENT |UITEMPLATEID</td>
    </tr>
    <tr>
        <td>Integrante da Equipe</td>
        <td>Outras equipes, membro da equipe</td>
        <td>EQUIPE | Integrante da equipe</td>
        <td>TEAMMEMBERS_CURRENT<br>TEAMMEMBERS_DAILY_HISTORY<br>TEAMMEMBERS_EVENT</td>
        <td></td>
        <td>SYSID <br>TEAMID<br>TEAMMEMBERID (self)<br>USERID</td>
        <td>Não é uma relação; usada para fins de aplicativo interno <br>TEAMS_CURRENT | TEAMID<br>Self<br>USERS_CURRENT | USERID</td>
    </tr>
    <tr>
        <td>FunçãoIntegranteEquipe</td>
        <td>Função do Integrante da Equipe</td>
        <td>EQUIPE | Função do membro da equipe</td>
        <td>MEMBERROLES_CURRENT<br>MEMBERROLES_DAILY_HISTORY<br>MEMBERROLES_EVENT</td>
        <td></td>
        <td>ROLEID <br>TEAMID<br>TEAMMEMBERROLEID (self)<br>USERID</td>
        <td>ROLES_CURRENT | TEAMS_CURRENT ROLEID <br>| Auto-USERS_CURRENT<br>TEAMID<br>| ID DE USUÁRIO</td>
    </tr>
    <tr>
        <td>Modelo</td>
        <td>Modelo</td>
        <td>TMPL | Modelo</td>
        <td>TEMPLATES_CURRENT<br>TEMPLATES_DAILY_HISTORY<br>TEMPLATES_EVENT</td>
        <td></td>
        <td>APPROVALPROCESSID<br>CATEGORYID<br>COMPANYID <br>DELIVERABLESCORECARDID <br>ENTEREDBYID<br>GROUPID<br>LASTNOTEID<br>LASTUPDATEDBYID<br>MILESTONEPATHID <br>OWNERID <br>PRIVATERATECARDID<br>PROGRAMID<br>QUEUEDEFID<br>SCHEDULEID <br>3}SYSID <br>TEAMID<br>TEMPLATEID (própria)</td>
        <td>APPROVALPROCESSES_CURRENT | APPROVALPROCESSID<br>CATEGORIES_CURRENT | CATEGORYID<br>COMPANIES_CURRENT | COMPANYID   <br>DELIVERABLESCORECARDID <br>USERS_CURRENT | USERID<br>GROUPS_CURRENT | GROUPID<br>NOTAS_ATUAIS | NOTEID<br>USERS_CURRENT | USERID<br>MILESTONEPATH_CURRENT | MILESTONEPATHID <br>USERS_CURRENT | ID DE USUÁRIO <br>RATECARD_CURRENT | RATECARDID<br>PROGRAM_CURRENT | PROGRAMID<br>A tabela de Definição de Fila não tem suporte no momento<br>SCHEDULES_CURRENT | SCHEDULEID <br>Não é uma relação; usada para fins de aplicativo interno <br>TEAMS_CURRENT | TEAMID<br>Self</td>
    </tr>
    <tr>
        <td>Atribuição de Modelo</td>
        <td>Atribuição de Modelo</td>
        <td>TAREFAS | Atribuição de modelo</td>
        <td>TEMPLATEASSIGNMENTS_CURRENT<br>TEMPLATEASSIGNMENTS_DAILY_HISTORY<br>TEMPLATEASSIGNMENTS_EVENT</td>
        <td></td>
        <td>ASSIGNEDTOID<br>CATEGORYID<br>LASTUPDATEDBYID<br>OBJID<br>ROLEID<br>SYSID<br>TEAMID<br>TEAMTIMELINEABLEID<br>TEMPLATEASSIGNMENTID (self)<br>TEMPLATETASKID</td>
        <td>USERS_CURRENT | ID DE USUÁRIO<br>CATEGORIES_CURRENT | CATEGORYID<br>USERS_CURRENT | USERID<br>A ID do objeto identificado no campo OBJCODE<br>ROLES_CURRENT | ROLEID<br>Não é uma relação; usada para fins de aplicativo interno<br>TEAMS_CURRENT | Não há suporte atualmente para a tabela Cronometragem da Equipe <br>Self<br>TEMPLATETASKS_CURRENT |IDDATAREFA_MODELO<br></td>
    </tr>
    <tr>
        <td>Modelo de Tarefa</td>
        <td>Modelo de Tarefa</td>
        <td>TTSK | Modelo de Tarefa</td>
        <td>TEMPLATETASKS_CURRENT<br>TEMPLATETASKS_DAILY_HISTORY<br>TEMPLATETASKS_EVENT</td>
        <td></td>
        <td>APPROVALPROCESSID<br>ASSIGNEDTOID<br>CATEGORYID<br>ENTEREDBYID<br>EXCHANGERATEID<br>LASTNOTEID<br>LASTUPDATEDBYID<br>MILESTONEID<br>PARENTID<br>RECURRENCERULEID<br>ROLEID<br>SYSID<br>TEAMID<br>TEAMTIMELINEABLEID<br>TEMPLATEID <br>TEMPLATETASKID (self)</td>
        <td>APPROVALPROCESSES_CURRENT | APPROVALPROCESSID<br>USERS_CURRENT | ID DE USUÁRIO<br>CATEGORIES_CURRENT | CATEGORYID<br>USERS_CURRENT | USERID<br>EXCHANGERATES_CURRENT | EXCHANGERATEID<br>NOTES_CURRENT | NOTEID<br>USUÁRIOS_ATUAIS | ID DE USUÁRIO<br>MARCO_ATUAL | MILESTONEID<br>TEMPLATETASKS_CURRENT Atualmente, não há suporte para a tabela de Regras de Recorrência |TEMPLATETASKID<br>ROLES_CURRENT | ROLEID<br>Não é uma relação; usada para fins de aplicativo interno<br>TEAMS_CURRENT | A tabela TEMPLATES_CURRENT da <br>Team Timelineable não tem suporte no momento<br>TEMPLATES_CURRENT | TEMPLATEID<br>Self<br></td>
    </tr>
    <tr>
        <td>Predecessora da Tarefa de Modelo</td>
        <td>Predecessora do modelo</td>
        <td>TPRED | Predecessora</td>
        <td>TEMPLATEPREDECESSORS_CURRENT<br>TEMPLATEPREDECESSORS_DAILY_HISTORY<br>TEMPLATEPREDECESSORS_EVENT</td>
        <td></td>
        <td>PREDECESSORID<br>SUCCESSORID <br>TEMPLATEPREDECESSORID (self)<br>SYSID</td>
        <td>TEMPLATETASKS_CURRENT |TEMPLATETASKID<br>TEMPLATETASKS_CURRENT |TEMPLATETASKID <br>Self<br>Não é uma relação; usada para fins de aplicativo interno</td>
    </tr>
    <tr>
        <td>Planilha de horas</td>
        <td>Planilha de horas</td>
        <td>FOLHA | Planilha de horas</td>
        <td>FOLHAS_DE_HORAS_ATUAIS<br>FOLHAS_DE_HORAS_DIÁRIAS_HISTÓRICO<br>FOLHAS_DE_HORAS_EVENTO</td>
        <td></td>
        <td>APPROVERID<br>LASTNOTEID<br>LASTUPDATEDBYID<br>TIMESHEETID<br>TIMESHEETPROFILEID<br>USERID</td>
        <td>USER_CURRENT | ID DE USUÁRIO<br>NOTA_ATUAL | NOTEID<br>USER_CURRENT | USERID<br>Self<br>TIMESHEETPROFILES_CURRENT | TIMESHEETPROFILEID<br>USER_CURRENT | USERID</td>
    </tr>
    <tr>
        <td>Perfil da Planilha de Horas</td>
        <td>Perfil da Planilha de Horas</td>
        <td>TSPRO | Perfil da Planilha de Horas</td>
        <td>TIMESHEETPROFILES_CURRENT<br>TIMESHEETPROFILES_DAILY_HISTORY<br>TIMESHEETPROFILES_EVENT</td>
        <td></td>
        <td>APPROVERID<br>ENTEREDBYID <br>GROUPID<br>SYSID<br>TIMESHEETPROFILEID (self)</td>
        <td>USERS_CURRENT | USERID<br>USERS_CURRENT | USERID <br>GROUPS_CURRENT | GROUPID<br>Não é uma relação; usado para fins de aplicativo interno<br>Self</td>
    </tr>
    <tr>
        <td>Filtro da interface</td>
        <td>Filtro</td>
        <td>UIFT | Filtro</td>
        <td>UIFILTERS_CURRENT<br>UIFILTERS_DAILY_HISTORY<br>UIFILTERS_EVENT</td>
        <td></td>
        <td>APPGLOBALID<br>ENTEREDBYID <br>LASTUPDATEDBYID <br>OBJID<br>PREFERENCEID<br>SYSID <br>UIFILTERID (self)</td>
        <td>Não é uma relação; usada para fins de aplicativo interno<br>USERS_CURRENT | USERID <br>USERS_CURRENT | USERID <br>A ID do objeto identificado no campo OBJCODE<br>PREFERENCES_CURRENT | PREFERENCEID<br>Não é uma relação; usada para fins de aplicativo interno <br>Self</td>
    </tr>
    <tr>
        <td>IU Agrupada por</td>
        <td>Agrupamento</td>
        <td>UIGB | Agrupamento</td>
        <td>UIGROUPBYS_CURRENT<br>UIGROUPBYS_DAILY_HISTORY<br>UIGROUPBYS_EVENT</td>
        <td></td>
        <td>ENTEREDBYID<br>GROUPID <br>LASTUPDATEDBYID <br>SYSID <br>UITEMPLATEID (próprio)</td>
        <td>USERS_CURRENT | USERID<br>GROUPS_CURRENT | GROUPID <br>USUÁRIOS_ATUAIS | USERID <br>Não é uma relação; usada para fins de aplicativo interno <br>Self</td>
    </tr>
    <tr>
        <td>Modelo da UI</td>
        <td>Modelo de Layout</td>
        <td>UITMPL | Modelo de layout</td>
        <td>UITEMPLATES_CURRENT<br>UITEMPLATES_DAILY_HISTORY<br>UITEMPLATES_EVENT</td>
        <td></td>
        <td>APPGLOBALID<br>ENTEREDBYID <br>LASTUPDATEDBYID <br>OBJID<br>PREFERENCEID<br>SYSID <br>UIGROUPBYID (próprio)</td>
        <td>Não é uma relação; usada para fins de aplicativo interno<br>USERS_CURRENT | USERID <br>USERS_CURRENT | USERID <br>A ID do objeto identificado no campo OBJCODE<br>PREFERENCES_CURRENT | PREFERENCEID<br>Não é uma relação; usada para fins de aplicativo interno <br>Self</td>
    </tr>
    <tr>
        <td>Visualização da interface</td>
        <td>Exibir</td>
        <td>UIVIEW | Exibir</td>
        <td>UIVIEWS_CURRENT<br>UIVIEWS_DAILY_HISTORY<br>UIVIEWS_EVENT</td>
        <td></td>
        <td>APPGLOBALID<br>ENTEREDBYID <br>LASTUPDATEDBYID <br>OBJID<br>PREFERENCEID<br>SYSID <br>UIVIEWID (self)</td>
        <td>Não é uma relação; usada para fins de aplicativo interno<br>USERS_CURRENT | USERID <br>USERS_CURRENT | USERID <br>A ID do objeto identificado no campo OBJCODE<br>PREFERENCES_CURRENT | PREFERENCEID<br>Não é uma relação; usada para fins de aplicativo interno <br>Self</td>
    </tr>
    <tr>
        <td>Usuário</td>
        <td>Usuário</td>
        <td>USUÁRIO | Usuário</td>
        <td>USERS_CURRENT<br>USERS_DAILY_HISTORY<br>USERS_EVENT<br>USERS_CUSTOM_VALUE_CURRENT<br>USERS_CUSTOM_VALUE_DAILY_HISTORY<br>USERS_CUSTOM_VALUE_EVENT</td>
        <td></td>
        <td>ACCESSLEVELID<br>CATEGORYID<br>COMPANYID<br>DEFAULTHOURTYPEID<br>DELEGATIONTOID<br>EAUTHUSERID<br>ENTEREDBYID<br>HOMEGROUPID<br>HOMETEAMID<br>LASTENTEREDNOTEID<br>LASTUPDATEDBYID<br>LATESTUPDATENOTEID<br>LAYOUTTEMPLATEID<br>MANMANMANAGEMENT AGERID<br>PORTALPROFILEID<br>PREFUIID<br>PRIVATERATECARDID<br>RESOURCEPOOLID<br>ROLEID<br>SCHEDULEID<br>TIMESHEETPROFILEID<br>UITEMPLATEID<br>USERID<br>UUMUSERID</td>
        <td>ACCESSLEVELS_CURRENT |ACCESSLEVELID<br>CATEGORIES_CURRENT | CATEGORYID<br>COMPANIES_CURRENT | COMPANYID <br>HOURTYPE_CURRENT | HOURTYPEID<br>USER_CURRENT | USERID<br>Não é uma relação; usada para fins de aplicativo interno<br>USER_CURRENT | USERID<br>GROUP_CURRENT | GROUPID<br>EQUIPE_ATUAL | TEAMID<br>NOTA_ATUAL | NOTEID<br>USER_CURRENT | ID DE USUÁRIO<br>NOTA_ATUAL | NOTEID<br>A tabela de Modelo de Layout não será suportada<br>USER_CURRENT | A tabela USERID<br>Perfil de Portal não terá suporte<br>Não é uma relação; usada para fins de aplicativo interno<br>RATECARD_CURRENT | RATECARDID<br>RESOURCEPOOLS_CURRENT | RESOURCEPOOLID<br>FUNÇÃO_ATUAL | ROLEID<br>SCHEDULE_CURRENT | SCHEDULEID<br>TIMESHEETPROFILES_CURRENT | TIMESHEETPROFILEID<br>UITEMPLATES_CURRENT |UITEMPLATEID<br>Self<br>Não é uma relação; usada para fins de aplicativo interno</td>
    </tr>
    <tr>
        <td>Delegação de usuários</td>
        <td>Delegação de usuários</td>
        <td>USRDEL | Delegação de usuários</td>
        <td>USERDELEGATIONS_CURRENT<br>USERDELEGATIONS_DAILY_HISTORY<br>USERDELEGATIONS_EVENT</td>
        <td></td>
        <td>FROMUSERID<br>SYSID <br>TOUSERID <br>USERDELEGATIONID (próprio)</td>
        <td>USERS_CURRENT | USERID<br>Não é uma relação; usada para fins de aplicativo interno <br>USERS_CURRENT | ID DE USUÁRIO <br>Próprio</td>
    </tr>
    <tr>
        <td>Grupo do usuário</td>
        <td>Outros Grupos</td>
        <td>USRGPS | Grupo de usuários</td>
        <td>USERSGROUPS_CURRENT<br>USERSGROUPS_DAILY_HISTORY<br>USERSGROUPS_EVENT</td>
        <td></td>
        <td>GROUPID <br>SYSID<br>USERID <br>USERSGROUPID (próprio)</td>
        <td>GROUPS_CURRENT | GROUPID <br>Não é uma relação; usada para fins de aplicativo interno<br>USERS_CURRENT | ID DE USUÁRIO <br>Próprio</td>
    </tr>
    <tr>
        <td>Função do Usuário</td>
        <td>Outras funções</td>
        <td>USRROL | Função do usuário</td>
        <td>USERSROLES_CURRENT<br>USERSROLES_DAILY_HISTORY<br>USERSROLES_EVENT</td>
        <td></td>
        <td>ROLEID <br>SYSID<br>USERID    <br>USERROLESETID<br>USERSROLEID (próprio)</td>
        <td>FUNÇÕES_ATUAIS | ROLEID <br>Não é uma relação; usada para fins de aplicativo interno<br>USERS_CURRENT | USERID    <br>USERROLESET_CURRENT | USERROLESETID<br>Self</td>
    </tr>
    <tr>
        <td>UserPrefValue</td>
        <td>UserPrefValue</td>
        <td>USERPF | Preferência do usuário</td>
        <td>USERPREFVALUES_CURRENT<br>USERPREFVALUES_DAILY_HISTORY<br>USERPREFVALUES_EVENT</td>
        <td></td>
        <td>SYSID    <br>USERID <br>USERPREFVALUEID (próprio)</td>
        <td>Não é uma relação; usada para fins de aplicativo interno<br>USERS_CURRENT | USERID    <br>Próprio</td>
    </tr>
    <tr>
        <td>UserRoleSet</td>
        <td>UserRoleSet</td>
        <td>URSET | UserRoleSet</td>
        <td>USERROLESET_CURRENT<br>USERROLESET_DAILY_HISTORY<br>USERROLESET_EVENT</td>
        <td></td>
        <td>PRIMARYROLEID <br>SYSID<br>USERID    <br>USERROLESETID (próprio)</td>
        <td>FUNÇÕES_ATUAIS | ROLEID <br>Não é uma relação; usada para fins de aplicativo interno<br>USERS_CURRENT | ID DE USUÁRIO <br>Próprio</td>
    </tr>
    <tr>
        <td>DecisõesDoUsuário</td>
        <td>Decisões dos usuários</td>
        <td>USRDEC | Decisões de usuários</td>
        <td>USERSDECISIONS_CURRENT<br>USERSDECISIONS_DAILY_HISTORY<br>USERSDECISIONS_EVENT</td>
        <td></td>
        <td>USERDECISIONID (self)<br>SYSID <br>USERID  </td>
        <td>Self<br>Not uma relação; usado para fins internos do aplicativo <br>USERS_CURRENT | USERID </td>
    </tr>
    <tr>
        <td>Item de trabalho</td>
        <td>Item de trabalho</td>
        <td>WRKITM | Item de trabalho</td>
        <td>WORKITEMS_CURRENT<br>WORKITEMS_DAILY_HISTORY<br>WORKITEMS_EVENT</td>
        <td></td>
        <td>ASSIGNMENTID <br>OBJID<br>OPTASKID    <br>ID DO PROJETO <br>ID DO SISTEMA<br>ID DA TAREFA    <br>USERID <br>WORKITEMID (próprio)</td>
        <td>ATRIBUIÇÕES_ATUAIS | ASSIGNMENTID <br>A ID do objeto identificado no campo OBJOBJCODE<br>OPTASK_CURRENT | OPTASKID    <br>PROJETOS_ATUAIS | PROJECTID <br>Não é uma relação; usada para fins de aplicativo interno<br>TASKS_CURRENT | TASKID    <br>USUÁRIOS_ATUAIS | USERID    <br>Próprio </td>
    </tr>
  </tbody>
</table>
