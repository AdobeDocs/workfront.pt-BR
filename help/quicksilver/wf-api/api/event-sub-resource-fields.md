---
content-type: api
navigation-topic: api-navigation-topic
title: Campos de recurso de assinatura do evento
description: Campos de recurso de assinatura do evento
author: Becky
feature: Workfront API
role: Developer
exl-id: 54859930-7619-4b93-8dff-29b10e43d6d5
source-git-commit: 1e8b25a0e6ff5c402bb662ef4b1831056e08c58b
workflow-type: tm+mt
source-wordcount: '850'
ht-degree: 10%

---

# Campos de recurso de assinatura do evento

Os campos de recurso de assinatura de evento representam acionadores para eventos que fazem com que uma assinatura de evento envie uma mensagem de saída para um ponto de extremidade configurado. Quando um campo de recurso é editado, um evento UPDATE é acionado.

Observe que os dados podem ser filtrados usando a filtragem aninhada. Para obter mais informações, consulte [Uso de filtros aninhados](/help/quicksilver/wf-api/general/event-subs-api.md#using-nested-filters) no artigo API de Assinatura de Evento.

A tabela a seguir lista os campos disponíveis para recursos de assinatura de eventos:

>[!NOTE]
>
>Alguns objetos estão disponíveis somente nas Assinaturas de Eventos versão 2. Esses objetos são anotados na tabela.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Recurso</th> 
   <th>objCode</th> 
   <th>Campo</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Aprovação<p>(Subs de Evento v2)</p></td> 
   <td>aprovação</td> 
   <td>createdAt</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>creatorID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>customerID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> ID </td> 
  </tr> 
  <tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> isLocked </td> 
  </tr> 
  <tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> objCode </td> 
  </tr> 
  <tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>objID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>status</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>updatedAt</td> 
  </tr> 
  <tr> 
   <td>Estágio de aprovação<p>(Subs de Evento v2)</p></td> 
   <td>approval_stage</td> 
   <td>approvalID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>createdAt</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>creatorID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>customerID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> deadlineDate </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> ID </td> 
  </tr> 
  <tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> isLocked </td> 
  </tr> 
  <tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> name </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> objCode </td> 
  </tr> 
  <tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>objID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>status</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>updatedAt</td> 
  </tr> 
  <tr> 
   <td>Participante do estágio de aprovação<p>(Subs de Evento v2)</p></td> 
   <td>approval_stage_component</td> 
   <td>createdAt</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>customerID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> deadlineDate </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> decisão </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> decisionDate </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> decisionUserID </td> 
  </tr> 
  <tr> 
  <tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> objCode </td> 
  </tr> 
  <tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>objID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> ID do participante </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> componentMetadata </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> FunçãoParticipante </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> componentType </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> realUserID </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> requesterID </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> stageID </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>status</td> 
  </tr> 
  <tr> 
   <td>Atribuição</td> 
   <td>ATRIBUIR</td> 
   <td>actualWorkCompleted</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>accessIDs</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>actualWorkPerDayStartDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>assignedByID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>assignedToID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> assignmentPercent </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> avgWorkPerDay </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> categoryID </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> classifierID </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> customerID </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> financeLastUpdateDate </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> ID </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>isPrimary</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> isTeamAssignment </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> lastUpdateDate </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> lastUpdatedByID </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> objCode </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> objectCategories </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> opTaskID </td> 
  </tr>
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> parameterValues </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> projectedAvgWorkPerDay </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> projectedUserAllocationPercentage </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> projectID </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>roleID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> securityRootID </td> 
  </tr> 
  <tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>status</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>taskID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>teamID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>trabalho</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>workPerDate <p>[!BADGE Removed]{type=denied tooltip="Este campo foi removido em 26 de outubro de 2023."}</span></td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>workPerDayList</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>workRequired</td> 
  </tr> 
  <tr> 
   <td>Empresa</td> 
   <td>COMPY</td> 
   <td>categoryID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>customerID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>enteredByID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> ID </td> 
  </tr> 
  <tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> extRefID </td> 
  </tr> 
  <tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> groupID </td> 
  </tr> 
  <tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdateDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdatedByID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>name</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> objCode </td> 
  </tr> 
  <tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> parameterValues </td> 
  </tr> 
  <tr> 
  <tr> 
   <td>Painel</td> 
   <td>PTLTAB</td> 
   <td>accessIDs</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>customerID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>descrição</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>docID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>extRefID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> <p>lastUpdateDate</p> <p>Observação: LastUpdateDate só acionará um evento na primeira vez que for atualizado durante cada dia. </p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdatedByID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>name</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>objCode</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>portalProfileID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>userID</td> 
  </tr> 
  <tr> 
   <td>Documento</td> 
   <td>DOCU</td> 
   <td>accessIDs</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>categoryID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>currentVersionID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>customer:isAdvancedDocMgmtEnabled</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>customerID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>descrição</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>documentRequestID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>extRefID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>grupos<p><b>OBSERVAÇÃO</b>: este campo não é filtrável.</p></td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>iterationID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastNoteID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdateDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> lastUpdatedByID </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>name</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>noteID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>objCode</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>objID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>opTaskID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>ownerID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>parameterValues</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>portfolioID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>programID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>projectID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> <p>referenceNumber</p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>referenceObjID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>releaseVersionID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>securityRootID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>taskID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>templateID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>templateTaskID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>topObjID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>userID</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>VersãoDocumento</span> </td> 
   <td><span>DOCV</span> </td> 
   <td><span>IDsAcessadores</span> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>ativeProofStages</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>customerID</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>IDdoDocumento</span> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>documentProviderID</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>docSize</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>entryDate</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>enteredByID</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>ext</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>externalIntegrationType</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>externalStorageID</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>nomeDoArquivo</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>tipoArquivo</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>ID</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>local</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>objCode</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>IDdoStatusdeAprovaçãodeProva</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>proofedByUserID</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>proofDeadlineDate</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>proofDecision</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>proofID</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>proofName</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>proofOwnerID</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>proofPages</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>proofProgress</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>proofStageID</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>versão</span> </td> 
  </tr> 
  <tr> 
   <td>Despesa</td> 
   <td>EXPNS</td> 
   <td> atualAmount </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> atualUnitAmount </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> billingRecordID </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> categoryID </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>customerID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>customFormsIDs</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>descrição</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>effectivenessDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>enteredByID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>entryDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>expObjCode</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>costTypeID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>extRefID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>ID </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>isBillable</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> isReembolsable </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> isReimbursed </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdateDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdatedByID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>objCode</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>objectCategories</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>objID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>parameterValues*</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>plannedAmount</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>plannedDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>plannedUnitAmount</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>projectID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>referenceObjCode</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>referenceObjID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>referenceObjectName</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>securityRootID </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>taskID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>templateID </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>templateTaskID </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>topObjCode</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>topObjID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>topReferenceObjCode</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>topReferenceObjID</td> 
  </tr> 
  <tr> 
   <td>Campo<p>(Subs de Evento v2)</p></td> 
   <td>CAMPO</td> 
   <td>createdAt</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> createdBy </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> customerId </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> dateOptions </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> descrição </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> displayName </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> formulaOptions </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> hasError </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> linkedField </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> lookupOptions </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> numberOptions </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> objCode </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> opções </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> referenceOptions </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> tipo </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> updatedAt </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> updatedBy </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> userOptions </td> 
  </tr> 
  <tr> 
   <td>Hora</td> 
   <td>HORA</td> 
   <td>accessIDs</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> atualCost </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>approvedByID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>approvedOnDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>billingRecordID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>customerID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>descrição</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>dupID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>entryDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>externalTimesheetID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>extRefID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>horas</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>hourTypeID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdateDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdatedByID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>objCode</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>opTaskID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>ownerID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>projectID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>projectOverheadID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>referenceObjCode</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>referenceObjID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>roleID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>securityRootID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>status</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>taskID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>timesheetID</td> 
  </tr> 
  <tr> 
   <td>Problema</td> 
   <td>OPTASK</td> 
   <td>accessIDs</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>approvalProcessID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>assignedToID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>categoryID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>currentApprovalStepID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>customerID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>descrição</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>enteredByID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>entryDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>extRefID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>groupID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>iterationID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>kanbanBoardID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastConditionNoteID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastNoteID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdateDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdatedByID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>name</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>objCode</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>ownerID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>parameterValues*</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>plannedCompletionDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>prioridade</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>projectID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>queueDefID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>queueTopicID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>referenceNumber</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>referenceObjID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>rejectionIssueID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>resolveOpTaskID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>resolveProjectID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>resolveTaskID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>resolvingObjID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>roleID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>rootGroupID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>securityRootID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>sourceObjID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>sourceTaskID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>status</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>submitByID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>teamID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>workflowAutomationID</td> 
  </tr> 
  <tr> 
   <td>Nota</td> 
   <td>Nota</td> 
   <td>accessIDs</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>attachDocumentID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>attachObjID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>attachOpTaskID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>attachWorkID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>attachWorkUserID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>auditRecordID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>customerID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>documentID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>entryDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>externalServiceID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>extRefID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>iterationID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>noteText</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>objCode</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>objID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>opTaskID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>ownerID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>parentEndorsementID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>parentJournalEntryID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>parentNoteID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>portfolioID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>programID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>projectID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>proofActionID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>richTextNoteID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>securityRootID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>assunto</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>taskID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>templateID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>templateTaskID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>threadID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>timesheetID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>topObjID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>userID</td> 
  </tr> 
  <tr> 
   <td>Portfólio</td> 
   <td>PORTA</td> 
   <td>accessIDs</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>alignmentScoreCardID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>categoryID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>customerID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>descrição</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>enteredByID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>entryDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>extRefID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>groupID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdateDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdatedByID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>name</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>objCode</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>ownerID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>parameterValues*</td> 
  </tr> 
  <tr> 
   <td>Programa</td> 
   <td>PRGM</td> 
   <td>accessIDs</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>categoryID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>customerID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>descrição</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>enteredByID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>extRefID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>groupID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdateDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdatedByID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>name</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>objCode</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>ownerID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>parameterValues*</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>portfolioID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>securityRootID</td> 
  </tr> 
  <tr> 
   <td>Projeto</td> 
   <td>PROJ</td> 
   <td>accessIDs</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>alignmentScoreCardID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>approvalProcessID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>attachedRateCardID </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>categoryID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>companyID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>convertedOpTaskID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>convertedOpTaskOriginatorID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>moeda</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>currentApprovalStepID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>customerID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>deliverableScoreCardID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>descrição</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>enteredByID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>entryDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>extRefID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>financeLastUpdateDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>groupID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>ID</td> 
  </tr> 
    <tr> 
   <td> </td> 
   <td> </td> 
   <td>issueWorkflowAutomationID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastCalcDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastConditionNoteID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastNoteID</td> 
  </tr> 
<tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdateDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpatedByID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>milestonePathID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>name</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>objCode</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>ownerID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>parameterValues*</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>plannedCompletionDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>popAccountID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>preserveBilling</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>prioridade</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>programID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>queueDefID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>referenceNumber</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>rejectionIssueID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>resourcePoolID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>rootGroupID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>scheduleID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>sponsorID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>status</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>submitByID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>taskWorkflowAutomationID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>teamID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>templateID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>workflowAutomationID</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>AprovaçãoDeProva</span> </td> 
   <td><span>PRFAPL</span> </td> 
   <td><span>IDsAcessadores</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>decisãodeAprovador</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>IDdoAprovador</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>customerID</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>IDdoDocumento</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>documentVersionID</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>ID</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>isAwaitingDecision</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>objCode</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>proofCreationDate</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>requesterID</span> </td> 
  </tr> 
  <tr> 
   <td>Registro<p><p>(Subs de Evento v2)</p></td> 
   <td>GRAVAR</td> 
   <td>createdAt</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>createdBy</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>customerId</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>dados<p><b>OBSERVAÇÃO</b>: este campo não é filtrável.</p></td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>id</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>objCode</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>recordExternalOptions</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>recordTypeId</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>updatedAt</td> 
  </tr> 
  <tr> 
   <td>Tipo de registro<p><p>(Subs de Evento v2)</p> </td> 
   <td>RECORD_TYPE </td> 
   <td>cor</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>createdAt</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>createdBy</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>customerId</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>dados<p><b>OBSERVAÇÃO</b>: este campo não é filtrável.</p></td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>descrição</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>displayName</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>externalOptions</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>campos<p><b>OBSERVAÇÃO</b>: este campo não é filtrável.</p></td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>ícone</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>id</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>isExternal</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>isTaxonomy</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>objCode</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>permissão</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>primaryFieldId</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>recordsCount</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>updatedAt</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>updatedBy</td> 
  </tr> 
  <tr> 
   <td>Relatório</td> 
   <td>PTLSEC</td> 
   <td>accessIDs</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>appGlobalID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>customerID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>descrição</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>enteredByID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>extRefID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>filterID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>groupByID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdateDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdatedByID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastViewedByID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>name</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>objCode</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>objID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>referenceID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>publicRunAsUserID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>reportFolderID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>runAsUserID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>scheduledReportID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>securityRootID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>uiObjCode</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>viewID</td> 
  </tr> 
  <tr> 
   <td>Tarefa</td> 
   <td>TAREFA</td> 
   <td>accessIDs</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>approvalProcessID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>assignedToID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>billingRecordID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>categoryID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>convertedOpTaskID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>convertedOpTaskOriginatorID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>currentApprovalStepID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>customerID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>descrição</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>enteredByID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>entryDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdateDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>extRefID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>groupID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>iterationID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>kanbanBoardID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastConditionNoteID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastNoteID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdateDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdatedByID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>milestoneID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>name</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>objCode</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>parameterValues*</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>parentID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>plannedCompletionDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>prioridade</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>projectID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>recurrenceRuleID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>referenceNumber</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>rejectionIssueID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>roleID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>rootGroupID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>securityRootID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>status</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>submitByID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>teamID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>templateTaskID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>workflowAutomationID</td> 
  </tr> 
  <tr> 
   <td>Modelo</td> 
   <td>TMPL</td> 
   <td>accessIDs</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>approvalProcessID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>categoryID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>companyID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>deliverableScoreCardID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>customerID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>descrição</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>enteredByID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>entryDate</td> 
  </tr> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>extRefID</td> 
  </tr> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>groupID</td> 
  </tr> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>ID</td> 
  </tr> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>issueWorkflowAutomationID</td> 
  </tr> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastNoteID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdateDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdatedByID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>milestonePathID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>name</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>objCode</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>ownerID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>parameterValues*</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>prioridade</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>programID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>queueDefID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>portfolioID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>referenceNumber</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>scheduleID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>sponsorID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>taskWorkflowAutomationID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>teamID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>workflowAutomationID</td> 
  </tr> 
  <tr> 
   <td>Planilha de horas</td> 
   <td>FOLHA</td> 
   <td>approverID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>approversListString</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>customerID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>displayName</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>endDate </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>extRefID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>hasNotes</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>hoursDuration</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>isEditable</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastNoteID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdateDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdatedByID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>objCode</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>overtimeHours</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>regularHours</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>startDate </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>status</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>timesheetProfileID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>totalHours</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>userID</td> 
  </tr> 
  <tr> 
   <td>Usuário</td> 
   <td>USUÁRIO</td> 
   <td>accessLevelID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>categoryID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>companyID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>customerID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>defaultHourTypeID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>delegationToID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>eauthUserID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>emailAddr</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>enteredByID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>extRefID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>homeGroupID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>homeTeamID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>isActive</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastEnteredNoteID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastLoginDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastNoteID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdateDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdatedByID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>latestUpdateNoteID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>layoutTemplateID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>logTimeInDays</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>managerID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>name</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>objCode</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>parameterValues*</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>portalProfileID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>resourcePoolID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>roleID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>scheduleID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>timesheetProfileID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>título</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>uiTemplateID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>uumUserID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>workHoursPerDay </td> 
  </tr> 
  <tr> 
   <td>Espaço de trabalho<p><p>(Subs de Evento v2)</p></td> 
   <td>WORKSPACE</td> 
   <td>cor</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>createdAt</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>createdBy</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>customerId</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>ícone </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>id</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>name</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>objCode</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>permissão</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>recordTypes</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>updatedAt</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>updatedBy</td> 
  </tr> 
 </tbody> 
</table>

&#42;Um parameterValue é um valor de campo personalizado associado a vários recursos (ou objetos) do Workfront. Uma mensagem de saída de assinatura de evento inclui uma lista completa de parameterValues preenchidos (campos personalizados).
