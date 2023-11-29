---
title: Lista de modelos do espaço de trabalho
description: Um espaço de trabalho é uma coleção de tipos de registros operacionais e taxonomias usadas por uma equipe e representa o ciclo de vida do trabalho da equipe. O Maestri vem com um conjunto de modelos para você começar a usar tipos básicos de registros, taxonomias e campos ao criar seu espaço de trabalho.
hide: true
hidefromtoc: true
recommendations: noDisplay, noCatalog
exl-id: c4758b87-45dc-4ffd-b086-5e2e907bdf34
source-git-commit: 6d1d3d82e15f4232ff81294d9094c2683b01ca89
workflow-type: tm+mt
source-wordcount: '473'
ht-degree: 0%

---

<!--update the metadata with real information when making this available in TOC and in the left nav:
---
title: List of available workspace templates
description: You can use templates to create workspaces. This article provides a list of available workspace templates
hidefromtoc: yes
hide: yes
author: Alina
feature: Work Management
role: User
---

-->

# Lista de modelos do espaço de trabalho

>[!IMPORTANT]
>
>As informações neste artigo referem-se ao Adobe Maestro, que é uma nova oferta da Adobe Workfront.
>
>Atualmente, o Adobe Maestro faz parte de um programa beta aberto a um número limitado de clientes. Você deve ser um cliente do Workfront para usar os recursos do Maestro.
>
>Entre em contato com seu representante de conta para obter mais informações sobre como participar do programa beta para o Maestro.
>
>Para obter informações, consulte [Visão geral do Adobe Maestri](../maestro-overview.md).

Em Adobe Maestri, um espaço de trabalho é uma coleção de tipos de registros operacionais e taxonomias usadas por uma equipe e representa o ciclo de vida do trabalho da equipe.

O Maestri vem com um conjunto de modelos para você começar a usar tipos básicos de registros, taxonomias e campos ao criar seu espaço de trabalho. Para obter informações sobre como criar espaços de trabalho, consulte [Criar espaços de trabalho](../architecture/create-workspaces.md).

Este artigo descreve os modelos de espaço de trabalho disponíveis no Maestri.

## Considerações sobre modelos Maestri

* Cada modelo vem com um conjunto de tipos de registros operacionais e taxonomias. Para obter informações, consulte [Visão geral dos tipos de registro e taxonomias](../architecture/overview-of-record-types-and-taxonomies.md).
* Cada tipo de registro operacional e taxonomia vem com um conjunto de campos. Alguns desses campos são conexões com outros tipos de registros Maestro.
* É possível personalizar qualquer modelo.

<!-- I modeled this article by the "List of available Blueprints" and that articles does not have an Access area

## Access requirements

You must have the following: 

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
  <tr>
   <td role="rowheader"><p>Adobe Workfront plan*</p></td>
   <td>
<p>Any</p>
<!--the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>->
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront license*</p></td>
   <td>
   <p>Any</p> 
  <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p> </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Product</p></td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>
  <tr>
   <td role="rowheader">Access level*</td>
   <td> <p>Any</p>  
</td>
  </tr>
<tr>
   <td role="rowheader">Layout template</td>
   <td> <p>Your system administrator must add the Maestro area in your layout template. For information, see the "Enable Maestro for the users in your Workfront instance" section in the article <a href="../maestro/maestro-overview.md">Adobe Maestro overview</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

>[!NOTE]
>
>*If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

-->

## Modelos de espaço de trabalho do mestre

A seguir estão os modelos de espaço de trabalho no Maestro e o número de campos que eles incluem:

* **Gerenciamento de marketing**: é possível gerenciar todas as campanhas de marketing ao usar esse template. O template vem com o seguinte:

   * Tipos de registro operacional:

      * **Plano de marketing**: 7 campos e 5 campos vinculados
      * **Campaign**: 9 campos e 7 campos vinculados
      * **Programa**: 9 campos e 5 campos vinculados
      * **Atividade**: 6 campos e 5 campos vinculados
   * Taxonomias:
      * **Público**: 3 campos e 3 campos vinculados
      * **Segmento**: 5 campos e 1 campo vinculado
      * **Jornada do cliente**: 4 campos
      * **Oferta do produto**: 3 campos e 1 campo vinculado
      * **Região**: 1 campo
      * **Tático**: 1 campo
      * **Canais**: 1 campo e 1 campo vinculado
      * **Unidade de negócios**: 1 campo
      * **Função**: 1 campo

* **Gerenciamento de vendas**: você pode criar um sistema de vendas abrangente que simplifique seu processo de vendas e melhore a eficiência. O template vem com o seguinte:

   * Tipos de registro operacional:

      * **Oportunidade**: 7 campos e 4 campos vinculados
      * **Atividade**: 4 campos e 5 campos vinculados
      * **Campaign**: 5 campos e 3 campos vinculados
   * Taxonomias:
      * **Conta**: 4 campos e 3 campos vinculados
      * **Lead**: 12 campos e 2 campos vinculados
      * **Contato**: 10 campos e 2 campos vinculados
      * **Região**: 1 campo e 2 campos vinculados
      * **Setor**: 1 campo
      * **Centro de compras**: 1 campo
      * **Produto/Serviço**: 1 campo
      * **Concorrência**: 1 campo

* **Gerenciamento de produtos**: você pode criar um processo de gerenciamento de produtos eficiente e estruturado usando esse template. O template vem com o seguinte:

   * Tipos de registro operacional:

      * **Tema**: 8 campos e 2 campos vinculados
      * **Iniciativa**: 8 campos e 2 campos vinculados
      * **Épico**: 9 campos e 3 campos vinculados
      * **História de usuário**: 9 campos e 2 campos vinculados

   * Taxonomias:

      * **Cliente**: 6 campos e 1 campo vinculado
      * **Sprint**: 7 campos e 1 campo vinculado
      * **Equipe do produto**: 3 campos
      * **Solicitações de recursos**: 8 campos e 1 campo vinculado
      * **Setor**: 1 campo e 1 campo vinculado