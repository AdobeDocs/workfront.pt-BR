---
title: Visão Geral das Limitações de Objetos do Adobe Workfront Planning
description: O Adobe Workfront Planning tem limites para a quantidade de objetos que você pode criar em sua instância. Limites de objeto estão em vigor para melhorar o desempenho do produto e aprimorar sua experiência com o Workfront Planning.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 2a640cd5-f4a8-4ff3-81b6-32f85f6e4535
source-git-commit: 7f719c903ad4079470a6dbd046dce445ba227a5b
workflow-type: tm+mt
source-wordcount: '441'
ht-degree: 2%

---


# Visão geral das limitações de objetos do Adobe Workfront Planning

<span class="preview">As informações nesta página se referem a funcionalidades que ainda não estão disponíveis. Ela está disponível somente no ambiente de Pré-visualização para todos os clientes. Após os lançamentos mensais para produção, os mesmos recursos também ficam disponíveis no ambiente de produção para clientes que habilitaram lançamentos rápidos.</span>

<span class="preview">Para obter informações sobre versões rápidas, consulte [Habilitar ou desabilitar versões rápidas para sua organização](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}


O Adobe Workfront Planning tem limites para a quantidade de objetos que você pode criar em sua instância. Limites de objeto estão em vigor para melhorar o desempenho do produto e aprimorar sua experiência com o Workfront Planning.

A tabela a seguir mostra os limites para quantos objetos você pode criar no Workfront Planning. As limitações estão sujeitas a alterações.

| objeto do Adobe Workfront Planning | Limite |
|-------------------------------------------------------------------------------|:---------------------------------------------------------------------------------------------------------------:|
| Número de espaços de trabalho para uma instância do Workfront | ilimitado* |
| Número de seções para um espaço de trabalho | 50 |
| Número de tipos de registro para um espaço de trabalho | 100 (isso inclui tipos de registro de todas as seções e aqueles que são criados ao usar um modelo de espaço de trabalho) |
| Número de registros de um tipo de registro | 25.000 |
| Número de registros de um espaço de trabalho | 25.000 para clientes com o Planning <br> 500.000 para clientes com o Planning Plus |
| Número do total de registros para uma instância do Workfront Planning | 500.000 para clientes com o Planning <br>2 milhões para clientes com o Planning Plus |
| Número de campos para um tipo de registro ou taxonomia | 500 |
| Número de caracteres de um campo de texto de linha única | 1.000 caracteres |
| Número de caracteres para um campo de parágrafo | 10.000 caracteres |
| Número de campos de parágrafo para um tipo de registro | Campos de 20 parágrafos |
| Tamanho do arquivo que você pode colar em uma tabela do tipo record | 1 MB |
| Tamanho do arquivo que você pode importar por meio da API para uma tabela de tipo de registro | 1,5 MB |
| A velocidade com a qual as solicitações de API podem ser feitas | 200 solicitações por minuto |
| Número de visualizações que um usuário pode criar para um tipo de registro | 100 |
| Tamanho do CSV do arquivo do Excel que você pode importar para criar tipos de registro | 5 MB |
| Número de linhas que você pode importar em um arquivo CSV ou Excel para criar tipos de registro | 25.000 |
| Número de colunas que você pode importar em um arquivo CSV ou Excel para criar tipos de registro | 500 |
| <span class="preview">Número de campos de fórmula para um tipo de registro</span> | <span class="preview">20</span> |
| <span class="preview">Número de caracteres em uma expressão de campo de fórmula</span> | <span class="preview">50.000</span> |


*Recomendamos não ter muitos espaços de trabalho, pois eles podem se tornar difíceis de gerenciar e seus fluxos de trabalho podem estar muito fragmentados.

Para obter informações sobre preços e pacotes do Workfront Planning, entre em contato com seu gerente de conta.

<!--
****************KEEP THIS COMMENTED OUT:

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
