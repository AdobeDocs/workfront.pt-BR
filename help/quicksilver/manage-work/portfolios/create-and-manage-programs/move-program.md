---
product-area: programs
navigation-topic: create and manage programs
title: Adicionar um programa existente a uma Portfolio
description: Você pode adicionar programas existentes a um portfólio. Como os programas não podem existir em dois portfólios diferentes, a adição de um programa existente o move permanentemente de um portfólio para outro.
author: Alina
feature: Work Management, Strategic Planning
exl-id: 73dbe277-12d2-4041-8a02-91ccf5f8b465
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 9a35246858141a3b69ec85be3372c7a8d9497d6e
workflow-type: tm+mt
source-wordcount: '382'
ht-degree: 9%

---

# Adicionar um programa existente a um portfólio

<!--Audited: 05/2026-->

<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. The same features will also be available in the Production environment for all customers after a week from the Preview release. </span>   

<span class="preview">For more information, see [Interface modernization](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md). </span>
-->

Você pode adicionar programas existentes a um portfólio. Como os programas não podem existir em dois portfólios diferentes, a adição de um programa existente o move permanentemente de um portfólio para outro.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] pacote</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licença</td> 
   <td> <p>[!UICONTROL Padrão]</p><p>[!UICONTROL Plan]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>[!UICONTROL Editar] acesso a [!UICONTROL Portfólios] e [!UICONTROL Programas] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Permissões do [!UICONTROL Manage] para o portfólio e o programa</p> </td> 
  </tr> 
 </tbody> 
</table>

*Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--
Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td> <p>New: [!UICONTROL Standard] </p><p>Or </p><p>Current: [!UICONTROL Plan] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>[!UICONTROL Edit] access to Portfolios and Programs </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>[!UICONTROL Manage] permissions to the portfolio and the program</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

## Adicionar um programa existente a um portfólio

>[!NOTE]
>
>Quando sua organização usa o armazenamento em nuvem herdado do Workfront e do Adobe para documentos, os seguintes cenários existem:
>
>
>* Quando você adiciona um programa de armazenamento em nuvem do Adobe a um portfólio de armazenamento herdado do Workfront e o portfólio não tem documentos anexados a ele, o portfólio é convertido em armazenamento em nuvem do Adobe.
>* Quando você adiciona um programa de armazenamento em nuvem da Adobe a um portfólio de armazenamento Workfront herdado e o portfólio tem documentos anexados a ele, o armazenamento de documentos do portfólio permanece no armazenamento da Workfront. No entanto, o ícone de armazenamento herdado do Workfront ![ícone de armazenamento herdado do Workfront](assets/legacy-storage-project-icon.png) é removido do portfólio.
>* Não é possível adicionar um programa de armazenamento herdado do Workfront a um portfólio de armazenamento em nuvem da Adobe.
>
>Para obter mais informações, consulte [Visão geral do gerenciamento de documentos para projetos e objetos relacionados](/help/quicksilver/manage-work/projects/manage-projects/manage-documents-on-projects.md).
>
>Nem todas as instâncias do Workfront têm ambos os tipos de armazenamentos de documentos.

Para adicionar um programa existente a outro portfólio:

1. Vá para um portfólio e clique em **[!UICONTROL Programas]** no painel esquerdo.
1. Clique em **[!UICONTROL Novo Programa]**.
1. Clique em **[!UICONTROL Programa Existente]**.

   A caixa **Adicionar programas** é aberta. <!--check screen shot - I logged changes for this casing-->

   ![Adicionar caixa de programa](assets/add-programs-box.png)

   >[!IMPORTANT]
   >
   >A adição de um programa existente transporta todos os projetos associados a esse programa para o portfólio. Tenha cuidado para não mover projetos involuntariamente dessa maneira.

1. No campo **[!UICONTROL Adicionar programas a este portfólio]**, digite o nome de um programa e selecione-o quando ele for exibido na lista. <!--see the name of this field, I suggested changes here-->

   Você pode adicionar mais de um programa.

1. (Opcional) Clique no ícone **Excluir** ![Excluir ícone](assets/delete-icon.png) ao lado do nome de um programa se decidir não adicioná-lo ao portfólio.

1. Clique em **[!UICONTROL Adicionar programas]**.

   O programa é exibido na guia **[!UICONTROL Programas]** no portfólio selecionado.

