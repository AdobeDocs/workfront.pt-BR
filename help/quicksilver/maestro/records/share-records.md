---
title: Compartilhar registros
description: Você pode compartilhar registros com outras pessoas para aumentar sua colaboração.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 83ff53ac-f18e-4b71-bdb2-57e05d69ed29
source-git-commit: 4e3449e7c31d29e1a289a7866ba98f873e62922c
workflow-type: tm+mt
source-wordcount: '381'
ht-degree: 0%

---

<!--update the metadata with real information when making this available in TOC and in the left nav-->
<!--should this move to the Access folder when we have sharing for ALL the objects???-->

# Compartilhar registros

>[!IMPORTANT]
>
>As informações neste artigo referem-se ao Adobe Maestro, que é uma nova oferta da Adobe Workfront.
>
>Atualmente, o Adobe Maestro faz parte de um programa beta aberto a um número limitado de clientes. Você deve ser um cliente do Workfront para usar os recursos do Maestro.
>
>Entre em contato com seu representante de conta para obter mais informações sobre como participar do programa beta para o Maestro.
>
>Para obter informações, consulte [Visão geral do Adobe Maestri](../maestro-overview.md).

Para colaborar com outros usuários, é possível compartilhar registros com outras pessoas.

Você pode compartilhar um registro Maestro das seguintes maneiras:

* Copie o link da página Detalhes de um registro do navegador quando a página estiver aberta.

* Copie um link para a página Detalhes do registro ao exibir registros na exibição de tabela do tipo de registro.

<!-- Update with this when we release permissions: 

* You can share all records in a workspace with other users by sharing the workspace. For more information, see [Grant access to Adobe Maestro](../access/grant-access.md).
-->

Este artigo descreve como você pode copiar um link para a página Detalhes de um registro da exibição de tabela de um tipo de registro.

<!-- add information about permissions, like:
- in the table below, you must have at least View permissions to the record
- the user you're sharing with must have at least View permissions to the record to view it
- etc - others???-->

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto">
 <col>
 <tbody>
<td>
   <p> produto Adobe</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>contrato do Adobe Workfront</p></td>
   <td>
<p>Sua organização deve estar inscrita no programa beta fechado do Adobe Maestro. Entre em contato com seu representante de conta para obter mais informações sobre esta nova oferta. </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>plano do Adobe Workfront</p></td>
   <td>
<p>Qualquer</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Licença do Adobe Workfront</p></td>
   <td>
   <p>Qualquer</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader">Nível de acesso</td>
   <td> <p>Qualquer</p>  
</td>
  </tr>
<tr>
   <td role="rowheader">Modelo de layout</td>
   <td> <p>O administrador do sistema deve adicionar a área Maestro no modelo de layout. Para obter informações, consulte <a href="../access/access-overview.md">Visão geral do Access</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

<!--
After permissions - replace the table with - below
****AND - see more above, another bullet point to update when permissions are released****

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Adobe product</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront agreement</p></td>
   <td>
<p>Your organization must be enrolled in the Adobe Maestro closed beta program. Contact your account representative to inquire about this new offering. </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront plan</p></td>
   <td>
<p>Any</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront license</p></td>
   <td>
   <p>Any</p> 
  </td>
  </tr>
  
  <tr>
   <td role="rowheader"><p>Access level</p></td>
   <td> <p>Any</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>Your Workfront or group administrator must add the Maestro area in your layout template. For information, see <a href="../access/access-overview.md">Access overview</a>. </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>View or higher permissions to a workspace</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>
</td>
  </tr>
 </tbody>
</table>

-->

<!--Maybe enable this at GA - but Maestro is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->

<!-- Notes for the table: for the "Workfront access" row: <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p>-->

## Compartilhar links de registro da exibição de tabela do tipo de registro

{#step1-to-maestro}

O espaço de trabalho que você acessou por último é aberto.
1. Clique em um cartão de tipo de registro.

   A página de tipo de registro é aberta.
1. (Condicional) No **Exibir** no canto superior direito da tabela, selecione uma exibição de tabela. Essa deve ser a exibição padrão, a menos que você tenha visualizado o tipo de registro na exibição de linha do tempo ao acessá-lo pela última vez.

   Os registros associados ao tipo de registro selecionado são exibidos na exibição de tabela.
1. Clicar com o botão direito do mouse em uma linha de registro

   Ou

   Passe o mouse sobre o nome de um registro, clique no **Mais** menu ![](assets/more-menu.png)e, em seguida, clique em **Copiar link**.

   ![](assets/contextual-menu-for-record-row.png)

   O link é copiado para a área de transferência.

1. Cole o link em um email ou janela de chat para compartilhar com outros usuários. Quando os usuários recebem o link, ele abre a página Detalhes do registro.

   >[!TIP]
   >
   >Os campos do registro na página Detalhes são os mesmos campos disponíveis na exibição Tabela do registro.


   <!--add there when it will be available: if they have access to this record-->
