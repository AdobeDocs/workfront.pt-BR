---
title: Registros Duplicados
description: Você pode duplicar um registro existente na exibição de tabela. Uma cópia idêntica do registro existente é adicionada à página de tipo de registro.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 2fed8c96-0c9c-4662-a9c4-66dae507ff2a
source-git-commit: e26a3d0e283182e08902c263252c8d067838c23a
workflow-type: tm+mt
source-wordcount: '503'
ht-degree: 1%

---

# Registros duplicados

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

No Adobe Workfront Planning, um registro é uma instância de um tipo de registro.

Você pode duplicar um registro existente na exibição de tabela. Uma cópia idêntica do registro existente é adicionada à página de tipo de registro.

## Requisitos de acesso

+++ Expanda para exibir os requisitos de acesso para a funcionalidade neste artigo. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
</tr>   
<tr> 
   <td role="rowheader"><p>Pacote do Adobe Workfront</p></td> 
   <td> 
<p>Qualquer Workfront e qualquer pacote do Planning</p> <p>Qualquer fluxo de trabalho e qualquer pacote de planejamento</p>
<p>Para obter mais informações sobre o que está incluído em cada pacote do Workfront Planning, entre em contato com o representante de conta da Workfront. </p> 
   </td> 
  <tr> 
   <td role="rowheader"><p>Licença do Adobe Workfront</p></td> 
   <td><p>Standard</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Permissões de objeto</p></td> 
   <td>   <p>Contribuir com ou mais permissões para um espaço de trabalho e tipo de registro  </p>  
   <p>Os administradores do sistema têm permissões para todos os espaços de trabalho, incluindo aqueles que não criaram</p> </td> 
  </tr>   
</tbody> 
</table>

Para obter mais informações sobre requisitos de acesso do Workfront, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++   

<!--Old:

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Products</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront Planning<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront plan*</p></td> 
   <td> 
<p>Any of the following Workfront plans:</p> 
<ul><li>Select</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning is not available for legacy Workfront plans</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront Planning package*</p></td> 
   <td> 
<p>Any </p> 
<p>For more information about what is included in each Workfront Planning plan, contact your Workfront account manager. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront platform</p></td> 
   <td> 
<p>Your organization's instance of Workfront must be onboarded to the Adobe Unified Experience to be able to access Workfront Planning.</p> 
<p>For more information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront license*</p></td> 
   <td><p> Standard</p>
   <p>Workfront Planning is not available for legacy Workfront licenses</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Access level configuration</p></td> 
   <td> <p>There are no access level controls for Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td>   <p>Contribute or higher permissions to a workspace and record type</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p> </td> 
  </tr> 
</tbody> 
</table> -->


## Duplicar um registro <!--in a record type table (I don't think you can create them elsewhere right now)-->

Você pode criar registros na exibição de tabela de uma página de tipo de registro duplicando uma existente. Um registro idêntico ao existente é criado e adicionado ao registro original.


{{step1-to-planning}}

1. Clique no espaço de trabalho ao qual deseja adicionar registros.

   O espaço de trabalho é aberto e os tipos de registro são exibidos como cartões.

1. Clique em um cartão de tipo de registro. Para obter informações sobre como criar um tipo de registro, consulte [Criar tipos de registro](/help/quicksilver/planning/architecture/create-record-types.md).

   A página do tipo de registro é aberta na exibição acessada pela última vez. Por padrão, uma página do tipo de registro é aberta na exibição de tabela.
Todos os registros do tipo selecionado são exibidos na visualização.

1. (Condicional) Selecione uma exibição de tabela.

1. Siga um destes procedimentos:

   * Passe o mouse sobre o nome de um registro, em seguida, clique no menu **Mais** incorporado com o nome do registro e, em seguida, clique no ícone **Duplicar** ![Ícone duplicar cinza](assets/duplicate-icon-gray.png).

     ![Mais menus do registro na exibição de tabela](assets/more-menu-from-record-in-table-view.png)

   * Selecione um registro e clique no ícone **Duplicar** ![Ícone Duplicar branco e azul](assets/duplicate-icon-white-and-blue.png) na barra de ferramentas, na parte inferior da página.

     ![Duplicar ícone na barra de ferramentas na exibição de tabela](assets/duplicate-icon-in-toolbar-in-table-view.png)

   Um registro idêntico com um nome idêntico é criado abaixo do registro original. Todos os campos do novo registro são preenchidos com as mesmas informações do registro original.

1. (Opcional) Comece a atualizar as informações sobre o novo registro nos campos disponíveis na exibição de tabela ou clique no registro e atualize as informações na visualização ou página do registro.

   >[!NOTE]
   >
   >  * Não há campos obrigatórios para registros. No entanto, recomendamos adicionar informações para o campo principal de um registro, pois é útil identificar registros ao vincular registros uns aos outros. Para obter mais informações sobre campos primários, consulte [Gerenciar a exibição de tabela](/help/quicksilver/planning/views/manage-the-table-view.md) e [Visão geral do campo primário](/help/quicksilver/planning/fields/primary-field-overview.md).
   >
   >  * Os campos que se referem a outros tipos de registro ou campos calculados são campos somente leitura.

   Para obter mais informações sobre como editar registros, consulte [Editar registros](/help/quicksilver/planning/records/edit-records.md).

1. (Opcional) Use os seguintes atalhos de teclado para desfazer ou refazer a adição de novos registros ou suas informações ao adicioná-los na exibição de tabela:

   * CTRL + Z (⌘ + Z para Mac) para desfazer uma alteração
   * CTRL + Shift + Z (⌘ + Shift + Z para Mac) para refazer uma alteração.
