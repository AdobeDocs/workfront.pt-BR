---
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
title: Armazenamento de campo Rich Text na API
description: Se um objeto como um projeto, problema ou tarefa contiver rich text, ele será armazenado e acessível como um valor de parâmetro por meio da API do Workfront.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 2e4b18be-14bb-4d47-8e63-e2f4a5dc376f
TQID: https://experienceleague.adobe.com/lLZZugNI5odziqyz7uBMnkiVoOdGcT-jKb90j9TUG1Q
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: d87de1f9-8e24-4c4d-aa4c-a403075091a1
role_v2: id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 174
ht-degree: 4%

---

# Armazenamento de campo de rich text na API

Se um objeto como um projeto, problema ou tarefa contiver rich text, ele será armazenado e acessível como um valor de parâmetro por meio da API do Workfront.

A solicitação de informações de texto de um objeto de projeto que contém rich text pode ser feita usando o campo **parameterValues**.

Por exemplo, uma simples solicitação HTTP pode se parecer com o seguinte:

`https://your-company.workfront.com/attask/api/v11.0/project?ID=your-project-ID&fields=parameterValues:*`

Se este projeto de exemplo continha um formulário personalizado com 3 campos personalizados: campo de cálculo, texto de parágrafo e rich 1. A solicitação acima retornará uma resposta que se parece com a seguinte, onde o campo &quot;rich 1&quot; é um campo de parâmetro rich text e o valor do texto é &quot;**Hello** *World!*&quot;:

```
{
    Data: {
        ID: "xxxxxxxxxxxxxxxxxxxxxxx",
        name: "new project with rich text",
        objCode: "PROJ",
        - parameterValues: {
            DE:rich 1: "{
                "blocks":[
                {
                    "key":"7eibh",
                    "text":"Hello Word!",
                    "type":"unstyled",
                    "depth":0,
                    "inlineStyleRanges":[
                    {
                        "offset":0,
                        "length":6,
                        "style":"BOLD"
                    },
                    {
                        "offset":6,
                        "length":5,
                        "style":"ITALIC"
                    }
                    ],
                    "entityRanges":[
                    ],
                "data":{
                }
                }
                ],
            "entityMap":{
            }
        }",
        DE: paragraph text: "here is some paragraph text",
        DE: calc field: "here is a calc field entry",
        }
    }
}
```

Para obter uma visão mais detalhada de como as informações de rich text são armazenadas e podem ser recuperadas por meio da API do Adobe Workfront, consulte [Campos de rich text na API do Adobe Workfront](../../../wf-api/general/rich-text-field-api.md).
