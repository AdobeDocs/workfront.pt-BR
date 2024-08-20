---
title: Visão Geral das Limitações de Objetos do Adobe Workfront Planning
description: O Adobe Workfront Planning tem limites para a quantidade de objetos que você pode criar em sua instância. Limites de objeto estão em vigor para melhorar o desempenho do produto e aprimorar sua experiência com o Workfront Planning.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: a2062658110792689c0a15dd1c616c58ebf7e07a
workflow-type: tm+mt
source-wordcount: '256'
ht-degree: 1%

---


<!--update the metadata with real information when making this available in TOC and in the left nav-->

# Visão geral das limitações de objetos do Adobe Workfront Planning

O Adobe Workfront Planning tem limites para a quantidade de objetos que você pode criar em sua instância. Limites de objeto estão em vigor para melhorar o desempenho do produto e aprimorar sua experiência com o Workfront Planning.

A tabela a seguir mostra os limites para quantos objetos você pode criar no Workfront Planning. As limitações estão sujeitas a mudanças conforme avançamos para as próximas fases do desenvolvimento.

| objeto do Adobe Workfront Planning | Limite |
|-------------------------------------------------------------------------------|:---------------------------------------------------------------------------------------------------------------:|
| Número de espaços de trabalho para uma instância do Workfront | 1.000 |
| Número de seções para um espaço de trabalho | 50 |
| Número de Tipos de Registro para um espaço de trabalho | 1.000 (isso inclui tipos de registro de todas as seções e aqueles que são criados ao usar um modelo de espaço de trabalho) |
| Número de registros de um tipo de registro | 50.000 |
| Número de campos para um tipo de registro ou taxonomia | 500 |
| Número de caracteres de um campo de texto | 1.000 caracteres |
| Tamanho do arquivo que você pode colar em uma tabela do tipo record | 1 MB |
| Tamanho do arquivo que você pode importar por meio da API para uma tabela de tipo de registro | 1,5 MB |
| A velocidade com a qual as solicitações de API podem ser feitas | 200 solicitações por minuto |
| Tamanho do CSV do arquivo do Excel que você pode importar* | 5 MB |
| Número de visualizações que um usuário pode criar para um tipo de registro | 100 |

<!--add to the table above: Maximum number of views created by one use 100 -->

>[!IMPORTANT]
>
>*Esta funcionalidade foi temporariamente desabilitada e estará disponível em uma data posterior.

<!--At GA, replace the table above with this:

|       Adobe Workfront Planning  object                                                          |                                                        Limit                                                    |
|-------------------------------------------------------------------------------|:---------------------------------------------------------------------------------------------------------------:|
|     Number of Workspaces for one Workfront instance                                      |   unlimited*                                                                                                        |
|     Number of sections for one workspace                                      |   50                                                                                                         |
|     Number of Record Types for one workspace                                            |   1,000 (this includes record types from all sections and those that are created when using a workspace template)  |
|     Number of records for one record type                                               |   25,000                                                                                                        |
|     Number of records for one workspace                                               |   25,000 for customers with the Planning plan <br> 500,000 for customers with the Planning Plus  plan                                                                                                         |
|     Number of total records for one instance of Workfront Planning type                                               |   500,000 for customers with the Planning plan <br>2 million for customers with the Planning Plus plan                                                                                                        |
|     Number of fields for one record type or taxonomy                            |   500                                                                                                           |
|     Number of characters for a text field                                                               |   1,000 characters                                                                                              |
|     Size of file that you can paste in a record type table                    |   1MB                                                                                                           |
|     Size of file that you can import through the API for a record type table  |   1.5MB                                                                                                         |
|     The rate at which API requests can be made                                    |   200 requests per minute                                                                                       |
| Size of CSV of Excel file you can import** | 5MB |
| Number of views one user can create for one record type | 100 |

*We recommend not to have too many workspaces, as they could become hard to manage and your workflows might be too fragmented.
**This functionality has been temporarily disabled and it will be available at a later date.
-->