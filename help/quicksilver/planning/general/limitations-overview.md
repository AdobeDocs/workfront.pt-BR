---
title: Visão Geral das Limitações de Objetos do Adobe Workfront Planning
description: O Adobe Workfront Planning tem limites para a quantidade de objetos que você pode criar em sua instância. Limites de objeto estão em vigor para melhorar o desempenho do produto e aprimorar sua experiência com o Workfront Planning.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
source-git-commit: f9abcd9ff4c80376bed229a1d65e0efcbfc332b0
workflow-type: tm+mt
source-wordcount: '316'
ht-degree: 1%

---


<!--check the workfront.com/plans article linked below to see if there is content in there about Planning - after August 28, 2024-->

# Visão geral das limitações de objetos do Adobe Workfront Planning

{{planning-important-intro}}


O Adobe Workfront Planning tem limites para a quantidade de objetos que você pode criar em sua instância. Limites de objeto estão em vigor para melhorar o desempenho do produto e aprimorar sua experiência com o Workfront Planning.

A tabela a seguir mostra os limites para quantos objetos você pode criar no Workfront Planning. As limitações estão sujeitas a mudanças conforme avançamos para as próximas fases do desenvolvimento.

| objeto do Adobe Workfront Planning | Limite |
|-------------------------------------------------------------------------------|:---------------------------------------------------------------------------------------------------------------:|
| Número de espaços de trabalho para uma instância do Workfront | ilimitado* |
| Número de seções para um espaço de trabalho | 50 |
| Número de Tipos de Registro para um espaço de trabalho | 1.000 (isso inclui tipos de registro de todas as seções e aqueles que são criados ao usar um modelo de espaço de trabalho) |
| Número de registros de um tipo de registro | 25.000 |
| Número de registros de um espaço de trabalho | 25.000 para clientes com o plano do Planning <br> 500.000 para clientes com o plano do Planning Plus |
| Número do total de registros para uma instância do tipo Workfront Planning | 500.000 para clientes com o plano do Planning <br>2 milhões para clientes com o plano do Planning Plus |
| Número de campos para um tipo de registro ou taxonomia | 500 |
| Número de caracteres de um campo de texto | 1.000 caracteres |
| Tamanho do arquivo que você pode colar em uma tabela do tipo record | 1 MB |
| Tamanho do arquivo que você pode importar por meio da API para uma tabela de tipo de registro | 1,5 MB |
| A velocidade com a qual as solicitações de API podem ser feitas | 200 solicitações por minuto |
| Número de visualizações que um usuário pode criar para um tipo de registro | 100 |

*Recomendamos não ter muitos espaços de trabalho, pois eles podem se tornar difíceis de gerenciar e seus fluxos de trabalho podem estar muito fragmentados.

Para obter informações sobre preços e pacotes do Workfront Planning, consulte [preços e pacotes do Adobe Workfront](https://business.adobe.com/products/workfront/pricing.html).

<!--
****************KEEP THIS COMMENTED OUT:
| Size of CSV of Excel file you can import** | 5MB |
**This functionality has been temporarily removed and it will be available at a later date.**********************
-->


<!--OLD limitations (before GA:)

|       Adobe Workfront Planning  object                                                          |                                                        Limit                                                    |
|-------------------------------------------------------------------------------|:---------------------------------------------------------------------------------------------------------------:|
|     Number of Workspaces for one Workfront instance                                      |   1,000                                                                                                         |
|     Number of sections for one workspace                                      |   50                                                                                                         |
|     Number of Record Types for one workspace                                            |   1,000 (this includes record types from all sections and those that are created when using a workspace template)  |
|     Number of records for one record type                                               |   50,000                                                                                                        |
|     Number of fields for one record type or taxonomy                            |   500                                                                                                           |
|     Number of characters for a text field                                                               |   1,000 characters                                                                                              |
|     Size of file that you can paste in a record type table                    |   1MB                                                                                                           |
|     Size of file that you can import through the API for a record type table  |   1.5MB                                                                                                         |
|     The rate at which API requests can be made                                    |   200 requests per minute                                                                                       |
| Number of views one user can create for one record type | 100 |

-->
<!--| Size of CSV of Excel file you can import* | 5MB |-->

<!--[!IMPORTANT]
>
>*This functionality has been temporarily removed and it will be available at a later date.-->

