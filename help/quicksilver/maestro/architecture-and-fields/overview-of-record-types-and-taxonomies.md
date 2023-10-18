---
title: Visão geral dos tipos de registro e taxonomias
description: Os tipos de registros são os blocos de construção de um espaço de trabalho Maestro.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 1de095b3-78d9-44df-a678-51f4238deb91
source-git-commit: b02c81873d84946f8db54bcf9a1a464de38781de
workflow-type: tm+mt
source-wordcount: '542'
ht-degree: 0%

---

<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

# Visão geral dos tipos de registro e taxonomias

>[!IMPORTANT]
>
>As informações neste artigo referem-se ao Adobe Maestro, que é uma nova oferta do Adobe.
>
>Atualmente, o Adobe Maestro faz parte de um programa beta aberto a um número limitado de clientes.
>
>Entre em contato com seu representante de conta para obter mais informações sobre como participar do programa beta para o Maestro.
>
>Para obter informações, consulte [Visão geral do Adobe Maestri](../maestro-overview.md).

Ao contrário do Workfront, onde os tipos de objetos são predefinidos, no Adobe Maestro, você pode criar seus próprios tipos de objetos. Por exemplo, no Workfront, os tipos de objeto de Programa, Portfolio, Projeto, Tarefa ou Problema já foram criados.

Os tipos de objetos maestro são chamados de &quot;tipos de registros&quot;. Os tipos de registros são os blocos de construção de um espaço de trabalho Maestro. Para obter informações sobre espaços de trabalho, consulte [Criar espaços de trabalho](../architecture-and-fields/create-workspaces.md).

## Visão geral do tipo de registro

No Maestro, você pode criar tipos de registros personalizados que atendam às necessidades da sua organização.

* A seguir estão os tipos de registros Maestri:

   * [Tipo de Registro Operacional](#operational-record-type): um tipo de registro que representa planos estratégicos, iniciativas ou trabalho planejado. Por exemplo, Campanha, Atividade, Tática e Oportunidade podem ser tipos de registro operacional.
   * [Taxonomia](#taxonomy): Tipos de registro que capturam atributos sobre um tipo de registro operacional. Por exemplo, Região, Endereço, Público-alvo podem ser taxonomias.

* Ao criar um tipo de registro, todos na organização podem exibi-lo, editá-lo ou excluí-lo. <!--this will change with access levels and permissions-->
* Você deve criar um espaço de trabalho antes de criar tipos de registro para ele.
* Você pode ter um total combinado de 1.000 tipos de registros operacionais e taxonomias em um espaço de trabalho. Isso inclui tipos de registro ou taxonomias criadas do zero ou importadas de outros sistemas.

### Tipo de Registro Operacional{#operational-record-type}

Um tipo de registro operacional é um tipo de registro Maestro que representa objetos relacionados ao trabalho.

![](assets/operational-record-type-blank.png)

Para obter mais informações sobre tipos de registros operacionais, incluindo como criá-los, consulte [Criar tipos de registro](../architecture-and-fields/create-record-types.md).

### Taxonomia{#taxonomy}

Uma taxonomia é um tipo de registro que captura atributos sobre um tipo de registro operacional.

![](assets/taxonomy-record-type-blank.png)

Para obter mais informações sobre tipos de registros de taxonomia, consulte [Criar uma taxonomia](../architecture-and-fields/create-a-taxonomy.md).

Embora a criação de taxonomias seja idêntica à criação de tipos de registros operacionais, Maestri distingue conceitualmente entre um tipo de registro operacional e um tipo de registro de taxonomia. O objetivo das taxonomias é aprimorar os tipos de registros operacionais. As taxonomias não devem representar diretamente objetos de trabalho.  <!--this is no longer true, but might be later?!: A taxonomy is a record without dates, like a static list of attributes.-->

<!--mimic what you did above for operational record types to say that we can also import taxonomies from other applications too - this will be possible later; for example Team would be a taxonomy record type, etc -->

Por exemplo, Público, Região ou Endereço podem ser tipos de registro do tipo taxonomia.

Para obter mais informações, consulte [Criar uma taxonomia](../architecture-and-fields/create-a-taxonomy.md).

## Semelhanças e diferenças entre tipos de registros operacionais e taxonomias

A tabela a seguir ilustra algumas das semelhanças e diferenças entre os tipos de registros operacionais e taxonomias:

| Tipo e característica do registro | Tipo de Registro Operacional | Tipo de registro de taxonomia |
|-------------------------------------------------------------|:-----------------------:|:--------------------:|
| Eles fazem parte de um espaço de trabalho | ✓ µ | ✓ |
| É possível criá-los automaticamente a partir de um modelo de espaço de trabalho | ✓ | ✓ |
| É possível criá-los manualmente, do zero | ✓ | ✓ |
| É possível criá-los copiando e colando informações de um arquivo ou lista externa | ✓ | ✓ |
| Você pode criar importando um arquivo Excel ou CSV | ✓ |                     |
| Você pode criar tipos de registro somente leitura conectando a tipos de objeto de outros aplicativos | ✓ |                     |
| Eles representam objetos relacionados ao trabalho | ✓ |                      |
| Eles representam atributos sobre objetos relacionados ao trabalho |                         | ✓ |
| É possível criar do zero | ✓ | ✓ |
| Você pode criar importando um arquivo Excel ou CSV | ✓ |                      |
| Você pode conectar o tipo de registro a um objeto de um aplicativo de terceiros | ✓ |                      |
| Você pode se conectar a outros tipos de registros do Maestro | ✓ |                    |
| É possível exibir seus registros associados em uma exibição de tabela | ✓ | ✓ |
| É possível exibir seus registros associados em uma exibição de linha do tempo | ✓ | ✓ |
