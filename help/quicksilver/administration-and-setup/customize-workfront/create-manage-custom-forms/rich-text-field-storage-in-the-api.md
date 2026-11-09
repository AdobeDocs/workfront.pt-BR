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
TQID: 'https://experienceleague.adobe.com/lLZZugNI5odziqyz7uBMnkiVoOdGcT-jKb90j9TUG1Q'
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
  - id: d5896d07-2812-5418-8b18-8957a0d7f0fb
    internal-label: System Setup and Administration
subfeature_v2:
  - id: d87de1f9-8e24-4c4d-aa4c-a403075091a1
    internal-label: Custom forms
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: d37b33ba0d7f3abaecd7982bed165d5a30aa9c5d
workflow-type: tm+mt
source-wordcount: '252'
ht-degree: 2%
---
# Armazenamento de campo de rich text na API

>[!NOTE]
>
>Os campos de rich text descritos neste artigo são os campos &quot;texto com formatação&quot;. Esse tipo de campo não está mais disponível para ser adicionado a novos campos, e os campos existentes devem ser convertidos para o tipo de campo &quot;rich text&quot;.
> 
>Observe que os novos campos de rich text armazenam o conteúdo como HTML, mas não armazenam os estilos aplicados no editor de campos. A remoção de informações de estilo do armazenamento pode ajudar a evitar problemas inesperados da interface do usuário e vulnerabilidades de segurança.

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
