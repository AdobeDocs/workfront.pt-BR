---
title: Gerenciar o GenStudio Workspace no Adobe Workfront Planning
description: O espaço de trabalho do GenStudio for Performance Marketing está disponível no Adobe Workfront Planning quando sua empresa comprou ambos os produtos e sua instância do Workfront está integrada à instância do GenStudio da empresa. Você pode exibir o espaço de trabalho do GenStudio no Planning e atualizar informações em ambos os sistemas.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: d6140b05-26c3-4298-a2f9-53695aa021cb
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '1474'
ht-degree: 1%

---


<!--Better metadata, at publishing:
---
title: Manage the GenStudio Workspace in Adobe Workfront Planning
description: The GenStudio for Performance Marketing workspace is available in Adobe Workfront Planning when your company has purchased both products and your instance of Workfront is integrated with your company's instance of GenStudio. You can view the GenStudio workspace from Planning and update information in both systems.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
---
-->

<!--MUST update the access requirements below - not complete!!!!!!!!!-->

# Gerenciar o espaço de trabalho do GenStudio no Adobe Workfront Planning

<!--<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

O espaço de trabalho do Adobe GenStudio for Performance Marketing está disponível no Adobe Workfront Planning quando sua empresa comprou ambos os produtos e sua instância do Workfront está integrada à instância do GenStudio da empresa.

Você pode exibir o espaço de trabalho do GenStudio no Planning e atualizar informações em ambos os sistemas.

Para obter informações sobre como usar e gerenciar o espaço de trabalho do GenStudio no GenStudio Performance Marketing, consulte [Guia do Usuário do Adobe GenStudio for Performance Marketing](https://experienceleague.adobe.com/pt-br/docs/genstudio-for-performance-marketing/user-guide/home).

Para obter informações gerais sobre a integração do GenStudio com o Workfront Planning, consulte [Introdução ao Adobe Workfront Planning e à integração com o Adobe GenStudio for Performance Marketing](/help/quicksilver/planning/planning-and-genstudio-integration/get-started-with-workfront-planning-and-genstudio-integration.md).

>[!IMPORTANT]
>
>As etapas descritas neste artigo ilustram como você pode atualizar o espaço de trabalho do GenStudio no Workfront Planning quando tem permissões de gerenciamento para ele.
> Nem todos os recursos estão disponíveis quando você tem permissões do Contribute para o espaço de trabalho do GenStudio.
>
>Se sua empresa tiver várias instâncias do Workfront, todos os usuários receberão permissões do Contribute no espaço de trabalho do GenStudio no Workfront Planning.

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
<p>Qualquer Workfront e qualquer pacote do Planning</p>
<p>Qualquer fluxo de trabalho e qualquer pacote de planejamento</p>
<p>Para obter mais informações sobre o que está incluído em cada pacote do Workfront Planning, entre em contato com o representante de conta da Workfront. </p> 
   </td> 
   <tr> 
<td> 
   <p> Produtos adicionais</p> </td> 
   <td> 
   <p> Adobe GenStudio for Performance Marketing</p></td> 
  </tr>
  <tr> 
   <td role="rowheader"><p>Licença do Adobe Workfront</p></td> 
   <td><p>Padrão</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Funções de usuário do Adobe GenStudio for Performance Marketing</p></td> 
   <td><p><ul><li>Qualquer função de usuário do GenStudio para acessar Campanhas, Produtos e Personalidades</li>
   <li>GenStudio System Manager para acessar Ativações <!--and Events--></li></ul>
   Para obter informações, consulte <a href="https://experienceleague.adobe.com/pt-br/docs/genstudio-for-performance-marketing/user-guide/intro/user-roles">Funções e permissões de usuário</a>. 
   </p>
  </td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Permissões de objeto</p></td> 
   <td>  
   <p>No Workfront Planning: </p>
   <ul>
   <li><p>Gerenciar permissões no espaço de trabalho do GenStudio para adicionar novos campos ou tipos de registro ao espaço de trabalho do GenStudio</p></li>
   <li><p>Contribuir com permissões para o espaço de trabalho do GenStudio para adicionar, atualizar ou excluir registros no espaço de trabalho do GenStudio</p> </li>  
   </ul>
   <p>Nenhum usuário pode remover tipos de registro ou campos do GenStudio for Performance Marketing do espaço de trabalho do GenStudio no Workfront Planning</p>
   <p>No Adobe GenStudio for Performance Marketing: <p>
   <ul>
   <li><p> Quaisquer permissões no Adobe GenStudio for Performance Marketing</p></li>
   <li><p> Criar permissões no Adobe GenStudio for Performance Marketing para criar itens</p></li></ul>
   </td>  
</tbody> 
</table>

Para obter informações sobre o acesso ao Adobe Workfront Planning, consulte [Visão geral do acesso ao Adobe Workfront Planning](/help/quicksilver/planning/access/access-overview.md).

Para obter mais informações sobre o Adobe GenStudio for Performance Marketing, consulte [Guia do Usuário do Adobe GenStudio for Performance Marketing](https://experienceleague.adobe.com/pt-br/docs/genstudio-for-performance-marketing/user-guide/home).

+++   

<!--Old:

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
    <td role="rowheader"><p>Adobe Workfront package</p></td> 
   <td> 
<p>Any Workfront package</p>
<p>Any Planning package</p>  

   </td> </tr>
   <tr> 
<td> 
   <p> Additional products</p> </td> 
   <td> 
   <p> Adobe GenStudio for Performance Marketing</p></td> 
  </tr>
  <tr> 
   <td role="rowheader"><p>Adobe Workfront license</p></td> 
   <td><p> Standard</p>
  </td> 
  </tr> 
   
  <tr> 
   <td role="rowheader"><p>Adobe GenStudio for Performance Marketing user roles</p></td> 
   <td><p><ul><li>Any GenStudio user role to access Campaigns, Products, and Personas</li>
   <li>GenSudio System Manager to access Activations ****** and Events*********</li></ul>
   For information, see <a href="https://experienceleague.adobe.com/pt-br/docs/genstudio-for-performance-marketing/user-guide/intro/user-roles">User roles and permissions</a>. 
   </p>
  </td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td>  
   <p>In Workfront Planning: </p>
   <ul>
   <li><p>Manage permissions to the GenStudio workspace to add new fields or record types to the GenStudio workspace</p></li>
   <li><p>Contribute permissions to the GenStudio workspace to add, update, or delete records in the GenStudio workspace</p> </li>  
   </ul>
   <p>No users can remove GenStudio for Performance Marketing record types or fields from the GenStudio workspace in Workfront Planning</p>
   <p>In Adobe GenStudio for Performance Marketing: <p>
   <ul>
   <li><p> Any permissions in Adobe GenStudio for Performance Marketing</p></li>
   <li><p> Create permissions in Adobe GenStudio for Performance Marketing to create items</p></li></ul>
   </td> 
  </tr> 
</tbody> 
</table> -->

## Considerações para o gerenciamento de um espaço de trabalho do GenStudio no Workfront Planning

* Sua organização deve comprar o Adobe GenStudio for Performance Marketing antes de exibir um espaço de trabalho do GenStudio no Workfront Planning.

* Dependendo de quantas instâncias do Workfront sua organização tiver, você terá automaticamente as seguintes permissões para o espaço de trabalho do GenStudio no Planning:

  <!--this table is also in the Get started article-->

  <table style="table-layout:auto"> 
   <col> 
   </col> 
   <col> 
   </col> 
   <tbody> 
      <tr> 
      <td role="rowheader"><p>Uma instância do Workfront</p></td> 
      <td> 
   <p>O espaço de trabalho do GenStudio está visível na sua instância do Workfront Planning</p>
   <p>Os administradores do Workfront têm permissões para Gerenciar o espaço de trabalho do GenStudio no Planning</p>
   <p>Todos os outros usuários têm acesso ao espaço de trabalho do GenStudio no Planning</p>
   </td> </tr>
      <tr> 
   <td> 
      <p> Várias instâncias do Workfront</p> </td> 
      <td> 
      <p>O espaço de trabalho do GenStudio está visível em todas as instâncias do Workfront</p>
   <p>Todos os usuários com acesso ao GenStudio for Performance Marketing e ao Workfront Planning têm permissões do Contribute no GenStudio no Planning</p> </td> 
   </tr>
      </tbody> 
   </table>

* A atualização da configuração do espaço de trabalho, dos tipos de registro, das views e dos campos de um espaço de trabalho do GenStudio é idêntica à atualização de um espaço de trabalho do Workfront Planning com seus elementos.
<!--Is this just preview?? * You can build hierarchies for the record types in the GenStudio workspace. For more information, see [Create workspace hierarchies](/help/quicksilver/planning/architecture/create-workspace-hierarchies.md).
* You cannot include GenStudio Brands in a hierarchy. -->

<!--
## Manage GenStudio workspace from Workfront Planning

CAN YOU DO THIS?? 
- OPTIONS FROM THE WORKSPACE CARD ??
- OPTIONS FROM THE MORE MENU ON A WORKSPACE ??
-->

## Gerenciar o espaço de trabalho do GenStudio no Workfront Planning

>[!NOTE]
>
>Antes de gerenciar o espaço de trabalho do GenStudio, consulte o artigo [Introdução à integração do Adobe Workfront Planning e do Adobe GenStudio for Performance Marketing](/help/quicksilver/planning/planning-and-genstudio-integration/get-started-with-workfront-planning-and-genstudio-integration.md) para obter mais informações.
>

1. Faça logon no Workfront como um usuário que também tem acesso ao GenStudio.

{{step1-to-planning}}

A página principal do Workfront Planning é aberta.

1. Clique em **Outros espaços de trabalho** e localize um espaço de trabalho que tenha uma indicação criada pelo **Sistema** e tenha a marca **GenStudio** em seu cartão.

   ![Cartão de espaço de trabalho do GenStudio com marca](assets/genstudio-card-with-tag-highlighted.png)

1. Clique no **cartão do espaço de trabalho do GenStudio** para abrir o espaço de trabalho do GenStudio no Workfront Planning.
1. Por padrão, os seguintes tipos de registro do GenStudio são criados e ficam visíveis no Workfront Planning:

   * Campanhas
   * Produtos
   * Personas
   * Ativações
   * Canais
   * Regiões

   Há uma indicação no cartão de tipo de registro do GenStudio de que eles foram originalmente criados no GenStudio.

   <!--check screen shot-->

   ![Cartão do tipo de registro GenStudio com marca](assets/genstudio-record-type-with-tag-and-tooltip-highlighted.png)

1. Clique no menu **Mais** ![Mais menu](assets/more-menu.png) à direita do nome do espaço de trabalho e clique em uma das seguintes opções:

   * **Editar**

     Para obter informações, consulte [Editar espaços de trabalho](/help/quicksilver/planning/architecture/edit-workspaces.md).
     <!--* **Delete** - this will generate an error message, per Iskuhi, so don't document as an option/ possibility-->

     <!--For information, see [Delete workspaces](/help/quicksilver/planning/architecture/delete-workspaces.md). -->

1. Clique em **Compartilhar** no canto superior direito para compartilhar o espaço de trabalho com outras pessoas.

   Para obter informações, consulte [Compartilhar espaços de trabalho](/help/quicksilver/planning/access/share-workspaces.md)

   >[!NOTE]
   >
   >Existem as seguintes limitações de compartilhamento:
   >
   >* Não é possível remover usuários do GenStudio do espaço de trabalho do GenStudio depois de compartilhar esse espaço de trabalho com eles.
   >* Se um usuário tiver permissões no GenStudio, o acesso não poderá ser alterado para Exibir no Workfront Planning. Eles devem receber pelo menos permissões do Contribute no espaço de trabalho do GenStudio no Planning.
   >* Não é possível desabilitar permissões herdadas para tipos de registros do GenStudio no espaço de trabalho do GenStudio.

1. Clique em qualquer um dos cartões de tipo de registro para exibir os registros desse tipo.

   Para gerenciar o tipo de registro, as exibições e os campos, consulte a seção [Gerenciar tipos de registro do GenStudio no Workfront Planning](#manage-genstudio-record-types-from-workfront-planning) neste artigo.


## Gerenciar tipos de registros, views e registros do espaço de trabalho do GenStudio no Workfront Planning

>[!NOTE]
>
>Antes de gerenciar o espaço de trabalho do GenStudio, consulte o artigo [Introdução à integração do Adobe Workfront Planning e do Adobe GenStudio for Performance Marketing](/help/quicksilver/planning/planning-and-genstudio-integration/get-started-with-workfront-planning-and-genstudio-integration.md) para obter mais informações.
>

1. Vá para o espaço de trabalho do GenStudio no Workfront Planning e abra uma página de tipo de registro, conforme descrito na seção [Gerenciar o espaço de trabalho do GenStudio no Workfront Planning](#manage-the-genstudio-workspace-from-workfront-planning) neste artigo.

1. Clique no menu **Mais** ![Mais menu](assets/more-menu.png) à direita de um nome de tipo de registro e clique em uma das seguintes opções:

   * **Editar**

     Para obter informações, consulte [Editar tipos de registros](/help/quicksilver/planning/architecture/edit-record-types.md).
   * **Gerenciar automações**

     Para obter informações, consulte [Configurar automações do Adobe Workfront Planning](/help/quicksilver/planning/records/configure-automations-to-create-records.md).
   * **Gerenciar formulários de solicitação**

     Você pode criar vários formulários de solicitação. Os formulários de solicitação estarão disponíveis na área Solicitações do Workfront e você também pode compartilhá-los publicamente ou com um link.

     Para obter informações, consulte [Criar e gerenciar um formulário de solicitação no Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).

1. Para compartilhar uma exibição ou o tipo de registro, faça o seguinte:

   * Clique em **Compartilhar** no canto superior direito da página de tipo de registro e em uma das seguintes opções:
      * **Compartilhar o tipo de registro**
Para obter informações, consulte [Compartilhar tipos de registros](/help/quicksilver/planning/access/share-record-types.md).
      * **Compartilhar a exibição atual**
Para obter informações, consulte [Compartilhar exibições](/help/quicksilver/planning/access/share-views.md).
      * **Copiar o link de exibição**
Um link para a exibição é copiado para a área de transferência.
      * **Exportar a exibição atual**
Para obter informações, consulte [Exportar registros da exibição de tabela](/help/quicksilver/planning/records/export-records-from-the-table-view.md).

        >[!NOTE]
        >
        >Não é possível remover usuários do GenStudio de tipos de registro no espaço de trabalho do GenStudio depois de compartilhar esse espaço de trabalho ou os tipos de registro com eles.

1. Para gerenciar as exibições de tipo de registro, faça o seguinte:

   * Clique em **+ Exibição** para criar uma exibição para o tipo de registro do GenStudio.

     Para obter informações, consulte [Gerenciar exibições de registros](/help/quicksilver/planning/views/manage-record-views.md).

   * Clique no ícone **Tela cheia** ![Abrir exibição completa no ícone de tela cheia](assets/open-full-screen-icon.png) para abrir qualquer exibição no modo de tela cheia.

   * Gerencie os elementos de uma visualização a partir de qualquer visualização.

     Por exemplo, é possível alterar o filtro, os agrupamentos, a classificação e as configurações de uma exibição, quando disponíveis.

     Para obter informações, consulte [Gerenciar exibições de registros](/help/quicksilver/planning/views/manage-record-views.md).

1. Para adicionar registros, siga um destes procedimentos:

   * Clique em **Novo registro** de qualquer modo de exibição para criar registros do zero

   * Importar registros usando um arquivo Excel ou CSV na exibição de tabela

   * Clique em qualquer lugar nas exibições de linha do tempo ou calendário para adicionar registros.

     Para obter informações, consulte [Criar registros](/help/quicksilver/planning/records/create-records.md).

     Os registros são visíveis no Workfront e no GenStudio.

     >[!NOTE]
     >
     >Não é possível adicionar registros para o tipo de registro Ativações.

1. Para editar registros, siga um destes procedimentos:

   * Editar registros embutidos na exibição de tabela

   * Clique em um registro de qualquer exibição para abrir a página de detalhes.

     Para obter informações, consulte [Editar registros](/help/quicksilver/planning/records/edit-records.md).

     As alterações feitas no espaço de trabalho do GenStudio no Planning ficam imediatamente visíveis no GenStudio.

1. Selecione um registro na exibição de tabela e clique em **Excluir**.

   Para obter informações, consulte [Excluir registros](/help/quicksilver/planning/records/delete-records.md).

   Os registros excluídos são removidos imediatamente do GenStudio.

   >[!TIP]
   >
   >Os registros excluídos podem ser recuperados da exibição de tabela Compartimento excluído recentemente no Workfront Planning. Os registros excluídos do GenStudio também podem ser recuperados do compartimento Excluído recentemente no Workfront Planning.

   Para obter informações, consulte [Restaurar registros excluídos](/help/quicksilver/planning/records/restore-deleted-records.md)

1. Clique no ícone + no canto superior direito da exibição em tabela para criar o seguinte:

   * Campos

     Para obter informações, consulte [Criar campos](/help/quicksilver/planning/fields/create-fields.md)

   * Conexões

     Para obter informações, consulte [Conectar tipos de registros](/help/quicksilver/planning/architecture/connect-record-types.md)

     Os campos criados no espaço de trabalho do GenStudio estão visíveis nas seguintes áreas:

      * Exibições do Workfront Planning
      * Detalhes do registro do Workfront Planning
      * Detalhes do registro do GenStudio

     >[!NOTE]
     >
     >* Você pode adicionar mais campos somente quando tem Gerenciar permissões no GenStudio.
     >* Os campos criados no Workfront Planning não estão visíveis na exibição de lista no GenStudio.
     >
     >* É possível conectar qualquer tipo de registro do GenStudio ao tipo de registro do Brands GenStudio.
     >  Os produtos e personalidades estão conectados às marcas por padrão.

1. Passe o mouse sobre um campo na exibição de tabela, em seguida, clique no menu suspenso para executar um dos seguintes procedimentos:

   * Classificar por ele
   * Ocultar
   * Editar suas configurações

   <!--* Delete it - not possible now, per Iskuhi; the link is there but it will generate an error-->

   <!--GenStudio-native fields are note removed from GenStudio. -->

   >[!NOTE]
   >
   >* Você pode editar a configuração de um campo do GenStudio somente quando tem permissões de gerenciamento no GenStudio.
   >* Não é possível excluir um campo do GenStudio.

<!--Is this just Preview?? Or direct to Prod?? 

## Create workspace hierarchies in the GenStudio workspace

Creating hierarchies in the GenStudio workspace is similar to creating hierarchies in any workspace. 

>[!NOTE]
>
>You cannot add GenStudio Brands to a hierarchy in the GenStudio workspace.

For information, see [Create workspace hierarchies](/help/quicksilver/planning/architecture/create-workspace-hierarchies.md)
-->
