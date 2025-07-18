---
title: Visão Geral dos Tipos de Registro
description: Os tipos de registro são os blocos de construção de um espaço de trabalho do Adobe Workfront Planning.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 1de095b3-78d9-44df-a678-51f4238deb91
source-git-commit: 298c542afea902d9fc14ef6a4470c0bc1d9bd33c
workflow-type: tm+mt
source-wordcount: '294'
ht-degree: 0%

---


# Visão geral dos tipos de registro

{{planning-important-intro}}

Diferentemente do Workfront, onde os tipos de objeto são predefinidos, no Adobe Workfront Planning você pode criar seus próprios tipos de objeto.

Por exemplo, no Workfront, os tipos de objeto de Programa, Portfolio, Projeto, Tarefa ou Problema já foram criados.

Os tipos de objeto do Workfront Planning são chamados de &quot;tipos de registro&quot; e existem apenas quando os usuários os criam.

Os tipos de registro são os blocos de construção de um espaço de trabalho do Workfront Planning e você deve criar todos eles para poder associá-los ao workflow e outras informações.

Os tipos de registro são organizados em espaços de trabalho.

Para obter informações sobre espaços de trabalho, consulte [Criar espaços de trabalho](/help/quicksilver/planning/architecture/create-workspaces.md).

## Visão geral do tipo de registro

No Workfront Planning, você pode criar tipos de registros personalizados que atendam às necessidades da sua organização.

Para obter informações sobre como criar tipos de registro, consulte [Criar tipos de registro](/help/quicksilver/planning/architecture/create-record-types.md).

* Quando você cria um espaço de trabalho a partir de um gabarito, os tipos de registro são criados nas seguintes seções do espaço de trabalho:

   * **Tipos de Registros Operacionais**: Tipos de registros que representam planos estratégicos, iniciativas ou trabalho planejado. Por exemplo, Campanha, Atividade, Tática e Oportunidade são tipos de registro operacional.
   * **Taxonomias**: tipos de registro que capturam atributos sobre um tipo de registro operacional. Por exemplo, Região, Endereço e Público são taxonomias.

  Você pode renomear ou excluir essas seções ou criar mais.

* Ao criar um tipo de registro em um espaço de trabalho criado do zero, você pode colocar o tipo de registro em qualquer seção criada no espaço de trabalho.
* Ao criar um tipo de registro, somente você e aqueles a quem você conceder permissões para acessar o espaço de trabalho poderão exibir o tipo de registro.
* Você deve criar um espaço de trabalho antes de criar tipos de registro para ele.
* Para limitações sobre quantos tipos de registros você pode ter em um espaço de trabalho ou instância do Workfront, consulte [Visão geral das limitações de objetos do Adobe Workfront Planning](/help/quicksilver/planning/general/limitations-overview.md).


<!--

### Operational Record Type{#operational-record-type}

An operational record type is a Wrorkfront Planning record type that represents work-related objects.  

(***********insert screen shot**************)
For more information about operational record types including how to create them, see [Create record types](/help/quicksilver/planning/architecture/create-record-types.md). 

### Taxonomy{#taxonomy}

A taxonomy is a record type that captures attributes about an operational record type. 

(**********add screen shot**********)

Although creating taxonomies is identical to creating operational record types, Workfront Planning distinguishes conceptually between an operational record type and a taxonomy record type. The purpose of taxonomies is to enhance operational record types. Taxonomies should not directly represent work objects.  (***********this is no longer true, but might be later?!: A taxonomy is a record without dates, like a static list of attributes.***********) 

(********mimic what you did above for operational record types to say that we can also import taxonomies from other applications too - this will be possible later; for example Team would be a taxonomy record type, etc*************)

For example, Audience, Region, or Address can be taxonomy-type record types.  

## Similarities and differences between operational record types and taxonomies

The following table illustrates some of the similarities and differences between operational record types and taxonomies: 

| Record type and characteristic                              | Operational Record Type | Taxonomy Record Type |
|-------------------------------------------------------------|:-----------------------:|:--------------------:|
| They are part of a workspace                                |            ✓            |           ✓          |
| You can create them automatically, from a workspace template                    |            ✓            |           ✓          |
| You can create them manually, from scratch                    |            ✓            |           ✓          |
| You can create them by copying and pasting information from an external file or list                   |            ✓            |           ✓          |
| You can create by importing an Excel or CSV file                    |            ✓            |                     |
| You can create read-only record types by connecting to object types from other applications                    |            ✓            |                     |
| They represent work-related objects                         |            ✓            |                      |
| They represent attributes about work-related objects        |                         |           ✓          |
| You can create from scratch                                 |            ✓            |           ✓          |
| You can create by importing an Excel or CSV file            |            ✓            |                      |
| You can connect the record type to an object from another application|            ✓            |                      |
| You can connect to other record types               |            ✓            |                    |
| You can view their associated records in a table view       |            ✓            |           ✓          |
| You can view their associated records in a timeline view    |            ✓            |           ✓          |

-->
