---
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
title: Armazenamento de campo de texto formatado na API
description: Se um objeto, como um projeto, problema ou tarefa, contiver rich text, ele será armazenado e acessível como valor de parâmetro por meio da API do Workfront.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 2e4b18be-14bb-4d47-8e63-e2f4a5dc376f
source-git-commit: e20934501c2117455ca7950834d868f78576dee7
workflow-type: tm+mt
source-wordcount: '171'
ht-degree: 0%

---

# Armazenamento de campo de texto formatado na API

Se um objeto, como um projeto, problema ou tarefa, contiver rich text, ele será armazenado e acessível como valor de parâmetro por meio da API do Workfront.

A solicitação de informações de texto a partir de um objeto de projeto que contenha rich text pode ser feita usando o campo **parameterValues**.

Por exemplo, uma simples solicitação HTTP pode parecer com o seguinte:

`https://your-company.workfront.com/attask/api/v11.0/project?ID=your-project-ID&fields=parameterValues:*`

Se este projeto de exemplo continha um formulário personalizado com 3 campos personalizados: campo de cálculo, texto de parágrafo e rich 1. Em seguida, a solicitação acima retornaria uma resposta que se assemelha ao seguinte, onde o campo &quot;rich 1&quot; é um campo de parâmetro de rich text e o valor do texto é &quot;**Hello** *Mundo!*&quot;:

```
{
	Data: {
		ID: “xxxxxxxxxxxxxxxxxxxxxxx”,
		name: “new project with rich text”,
		objCode: “PROJ”,
		- parameterValues: {
			DE:rich 1: “{
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
		}”,
		DE: paragraph text: “here is some paragraph text”,
		DE: calc field: “here is a calc field entry”,
		}
	}
}
```

Para obter uma análise mais detalhada de como as informações de rich text são armazenadas e podem ser recuperadas por meio da API do Adobe Workfront, consulte [Campos de rich text na API do Adobe Workfront](../../../wf-api/general/rich-text-field-api.md).
