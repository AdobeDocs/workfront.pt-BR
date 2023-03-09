---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: Adicionar opções de prova avançada com a API do Adobe Workfront
description: Adicionar opções de prova avançada com a API do Adobe Workfront
author: Becky
feature: Workfront API, Workfront Proof
exl-id: 5fcdf07e-d077-4d6a-bc3f-973983877c7c
source-git-commit: e2a334ad16fc16b49d8e8b8186fa89fc0e09d998
workflow-type: tm+mt
source-wordcount: '613'
ht-degree: 0%

---


# Adicionar opções de prova avançada ao criar uma prova por meio da API do Adobe Workfront

Ao criar uma prova na API do Workfront, você pode adicionar opções de prova avançada.

Use um dos seguintes workflows para adicionar opções de prova a uma prova usando a API:

* (Recomendado) Crie uma prova simples usando a API do Workfront e adicione opções de prova avançada à prova usando a API ProofHQ

* Criar uma prova com opções de prova avançada usando JSON na API do Workfront

## Criar uma prova usando as APIs do Workfront e ProofHQ (recomendado) {#create-a-proof-using-the-workfront-and-proofhq-apis-recommended}

Esta seção descreve como criar uma prova com opções de prova avançada por meio da API do Workfront, usando uma combinação de APIs Workfront e ProofHQ.

A API ProofHQ inclui várias ações não disponíveis para provas na API do Workfront. Usando essas ações, você pode modificar ou configurar a prova com mais precisão do que a disponível na API do Workfront.

Para obter uma visão geral da API ProofHQ, consulte [Visão geral do PoofHQ](../../proofhq-api/general/overview.md). Você também pode consultar a [Documentação do ProofHQ](https://api.proofhq.com/home.html).

>[!NOTE]
>
>* A API do Workfront é uma API REST-ful. A API ProofHQ é uma API SOAP.
>* Provas criadas na API ProofHQ não são vinculadas automaticamente ao Workfront. Portanto, recomendamos criar provas na API do Workfront antes de atualizá-las com a API ProofHQ.
>


### Criar uma prova com opções de prova avançada

1. Crie uma prova usando o `Document createProof` na API do Workfront.

   >[!NOTE]
   Ao criar a prova, defina `{}` como o valor de `advancedProofingOptions` parâmetro.

1. Depois que a prova for criada, use a API ProofHQ para adicionar opções avançadas.

### Exemplos

Esta seção mostra algumas atualizações de exemplo que você pode fazer com a API ProofHQ.

**Exemplos:**

* [Uma prova pode ser baixada, tem uma mensagem e é compartilhada publicamente](#proof-can-be-downloaded-has-a-message-and-is-shared-publicly)
* [Atualizar um estágio para que ele não seja privado, obrigatório e exija apenas uma aprovação](#update-a-stage-so-that-it-is-not-private-not-mandatory-and-requires-only-one-approval)
* [Adicionar dois recipients a uma prova sem um tomador de decisão principal](#add-two-recipients-to-a-proof-with-no-primary-decision-maker)

**Uma prova pode ser baixada, tem uma mensagem e é compartilhada publicamente**

A documentação desse endpoint pode ser encontrada no [Atualização da API ProofHQ updateProof](https://api.proofhq.com/home/proofs/updateproof.html) página.

<!-- [Copy](javascript:void(0);) -->

```
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:soap="https://{{soap_host}}/">
    <soapenv:Header/>
    <soapenv:Body>
        <soap:updateProof>
            <SessionID>{{session_id}}</SessionID>
            <FileID>{{file_id}}</FileID>
            <OwnerID>0</OwnerID>
            <Name>{{proof_name}}}</Name>
            <Subject>Email subject here</Subject>
            <Message>Email message here</Message>
            <EnableDownload>true</EnableDownload>
            <EnableTeamURL>true</EnableTeamURL>
        </soap:updateProof>
    </soapenv:Body>
</soapenv:Envelope>
```

**Atualizar um estágio para que ele não seja privado, obrigatório e exija apenas uma aprovação**

A documentação desse endpoint pode ser encontrada no [API ProofHQ updateWorkflowProofStage](https://api.proofhq.com/updateworkflowproofstage.html) página.

<!-- [Copy](javascript:void(0);) -->

```
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:soap="https://{{soap_host}}/">
    <soapenv:Header/>
    <soapenv:Body>
        <soap:updateWorkflowProofStage>
        <SessionID>{{session_id}}</SessionID>
        <FileID>{{proof_id}}</FileID>
        <Stage>
            <stage_id>{{stage_id}}</stage_id>
            <name>{{stage_name}}</name>
                <stage_one_decision_only>true</stage_one_decision_only>
                <stage_private>false</stage_private>
                <mandatory>false</mandatory>
            </Stage>
        </soap:updateWorkflowProofStage>
    </soapenv:Body>
</soapenv:Envelope>
```

**Adicionar dois recipients a uma prova sem um tomador de decisão principal**

A documentação desse endpoint pode ser encontrada no [API de ProofHQ addWorkflowProofReviewed](https://api.proofhq.com/addworkflowproofreviewers.html) página.

<!-- [Copy](javascript:void(0);) -->

```
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:soap="https://{{soap_host}}/">
    <soapenv:Header/>
    <soapenv:Body>
        <soap:addWorkflowProofReviewers>
            <SessionID>{{session_id}}</SessionID>
            <FileID>{{proof_id}}</FileID>
            <Recipients>
                <item>
                <email>{{recipient_email_1}}</email>
                <role>5</role>
                <name>{{recipient_name_1}}</name>
                <primary_decision_maker>false</primary_decision_maker>
                <stage_id>{{stage_id}}</stage_id>
                </item>
                <item>
                <email> {{recipient_email_2}} </email>
                <role>5</role>
                <name> {{recipient_name_2}} </name>
                <primary_decision_maker>false</primary_decision_maker>
                <stage_id>{{stage_id}}</stage_id>
                </item>
            </Recipients>
            <SuppressNewProofNotification></SuppressNewProofNotification>
        </soap:addWorkflowProofReviewers>
    </soapenv:Body>
</soapenv:Envelope>
```

## Criar uma prova usando JSON na API do Workfront

Esta seção descreve como criar uma prova com opções de prova avançada por meio da API do Workfront, usando JSON como um valor de parâmetro na API do Workfront

### Criar uma prova com opções de prova avançada

É possível criar provas por meio da API do Workfront usando o `Document createProof` ação. Esta ação aceita o `advancedProofingOptions` que tem o tipo de valor de `string`. Para incluir opções de prova avançada no `createProof` ação, você deve inserir as opções no campo `advancedProofingOptions` no formato JSON.

>[!NOTE]
Pode ser difícil prever os campos a serem incluídos no JSON advancedProofingOptions. Você pode examinar os dados de rede de sua organização ao usar a prova avançada no Workfront e basear seu JSON nos campos e valores normalmente usados por sua organização.
Como esses campos podem ser difíceis de prever, recomendamos criar uma prova usando a API do Workfront e, em seguida, atualizá-la usando a API ProofHQ. Para obter mais informações, consulte [Criar uma prova usando as APIs do Workfront e ProofHQ (recomendado)](#create-a-proof-using-the-workfront-and-proofhq-apis-recommended) neste artigo

### Exemplo

Este exemplo mostra campos e formatação que você pode usar ao criar seu JSON para o `advancedProofingOptions` parâmetro. Seu `advancedProofingOptions` O arquivo JSON pode ter mais ou menos campos do que mostrados aqui.

**Exemplo:**

<!-- [Copy](javascript:void(0);) -->

```
{
    "stages": [
        {
            "name": "stage1",
            "lockOn": 1,
            "position": 1,
            "isPrivate": false,
            "activateOn": 1,
            "recipients": [
                {
                    "name": "",
                    "role": 5,
                    "email": "user1_email@example.com",
                    "recipient_id": "",
                    "notifications": 0,
                    "isPrimaryDecisionMaker": null
                },
                {
                    "name": "",
                    "role": 5,
                    "email": "user2_email@example.com",
                    "recipient_id": "",
                    "notifications": 0,
                    "isPrimaryDecisionMaker": false
                }
            ],
            "isMandatory": false,
            "deadlineDate": null,
            "deadlineTime": null,
            "isOneApproval": true,
            "activateOnDate": null,
            "parentPosition": null,
            "activateOnDecision": null,
            "deadlineCalculateOn": null,
            "deadlineBusinessDays": null
        }
    ],
    "message": "",
    "subject": "",
    "templates": [],
    "hasMessage": true,
    "canDownload": true,
    "customfields": [],
    "hasPublicSharing": true,
    "isAutomatedWorkflow": true,
    "stageBasedVisibility": 0
}
```
