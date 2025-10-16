---
title: Gerenciar comentários de registro
description: É possível colaborar em registros do Adobe Workfront Planning, adicionando comentários ou respostas no painel direito de um registro. Você também pode exibir outras alterações feitas no registro e registradas pelo sistema nessa área.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 215883a4-e882-438e-9c21-954c0b1d741b
source-git-commit: 8546311acf722c0f4d47d4663b02ff701416894a
workflow-type: tm+mt
source-wordcount: '875'
ht-degree: 0%

---

# Gerenciar comentários de registro

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

É possível colaborar em registros do Adobe Workfront Planning, adicionando comentários ou respostas no painel direito de um registro. Você também pode exibir outras alterações feitas no registro e registradas pelo sistema nessa área.

O painel direito de um registro exibe as seguintes seções:

* **Comentários**: exibe comentários e respostas que os usuários adicionam aos registros.
* **Histórico**: exibe as alterações registradas pelo sistema que os usuários fazem nos campos de registro. Para obter mais informações, consulte [Visão geral da seção de histórico](/help/quicksilver/planning/records/history-section-overview.md).

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
<ul> 
<li><p>Qualquer Workfront e qualquer pacote do Planning</p></li>
Ou
<li><p>Qualquer fluxo de trabalho e qualquer pacote de planejamento</p></li></ul>
<p>Para obter mais informações sobre o que está incluído em cada pacote do Workfront Planning, entre em contato com o representante de conta da Workfront. </p> 
   </td> 
  <tr> 
   <td role="rowheader"><p>Licença do Adobe Workfront</p></td> 
   <td><p>Colaborador ou superior</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Permissões de objeto</p></td> 
   <td>   <p>Exibir permissões ou mais altas para um espaço de trabalho e tipo de registro</p>  
   <p>Os administradores do sistema têm permissões para todos os espaços de trabalho, incluindo aqueles que não criaram</p> </td> 
  </tr> 
  </tr> 
  <tr>
   <td role="rowheader"><p>Modelo de layout</p></td>
   <td> Os usuários com uma licença Light ou Contributor devem receber um modelo de layout que inclua o Planning.
   <p>Usuários padrão e Administradores do sistema têm as áreas do Planning habilitadas por padrão.</p></div></li></ul>
</td>
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
   <td><p> Contributor or higher license</p>
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
   <td>   <p>View or higher permissions to a workspace and record type</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p> </td> 
  </tr> 
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> Users with a Light or Contributor license must be assigned a layout template that includes Planning.
   <p>Standard users and System Administrators have the Planning areas enabled by default.</p></div></li></ul>

</td>
  </tr>
</tbody> 
</table> -->



## Considerações sobre comentários em um registro

* É possível adicionar comentários e respostas a registros no Workfront Planning, na seção Comentários de um registro.

* Comentários adicionados aos registros vinculados não são exibidos nos registros a partir dos quais você está vinculando. Por exemplo, se você comentar em um registro de Produto do Workfront Planning vinculado a um registro de Campanha, o comentário será exibido somente no registro de Produto no Workfront Planning e não no registro de Campanha do qual você está vinculando.

* É possível adicionar comentários a registros do Workfront Planning criados como resultado de uma conexão entre um registro e um objeto de outro aplicativo.

  Por exemplo, você pode comentar no registro do Project Workfront Planning depois de conectar os projetos Workfront aos registros do Workfront Planning. Para obter mais informações, consulte [Conectar registros](/help/quicksilver/planning/records/connect-records.md).

* Comentários adicionados a objetos vinculados em outros aplicativos não são exibidos no Workfront Planning e comentários adicionados a objetos vinculados no Workfront Planning não são exibidos em outros aplicativos.

  Por exemplo, comentários adicionados a projetos no Workfront não são exibidos no mesmo projeto vinculado a uma campanha no Workfront Planning, e comentários adicionados ao registro do projeto no Workfront Planning não são exibidos no Workfront.

* É possível marcar usuários ou equipes para chamar a atenção deles para uma atualização. Tanto os usuários marcados individualmente quanto os usuários das equipes marcadas recebem uma notificação no aplicativo e um email sobre a sua atualização.

  >[!NOTE]
  >
  >   Somente usuários de clientes que integraram com a Experiência unificada da Adobe recebem uma notificação no aplicativo e uma notificação por email. Para determinar se sua empresa está usando a Experiência unificada da Adobe, consulte [Experiência unificada da Adobe para Workfront](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md).

* Você pode adicionar uma atualização aos registros e revisar o histórico de alterações das seguintes áreas do Workfront Planning:

   * Na página de detalhes do registro.
   * Em uma exibição, na caixa de detalhes do registro.

### Gerenciar comentários nos registros

{{step1-to-planning}}

1. Clique no cartão de um espaço de trabalho.

   O espaço de trabalho é aberto e os tipos de registro são exibidos em cartões.

1. Clique em um cartão de tipo de registro.
A página de tipo de registro é aberta e todos os registros desse tipo são exibidos.

1. Escolha uma exibição de tabela no menu suspenso **Exibir**.
1. Clique no nome de um registro na exibição de tabela.

   A página **Detalhes** do registro é aberta. A área Comentários é aberta por padrão no painel direito.

1. (Condicional) Se o painel direito não abrir por padrão, clique no ícone **Mostrar comentários** ![Mostrar comentários](assets/show-comments-icon.png) no canto superior direito para abrir a seção Comentários.

1. Comece a inserir um comentário na caixa **Novo comentário**.

   ![Caixa de comentário vazia no registro](assets/empty-comment-box-on-record.png)

   >[!TIP]
   >
   >Sair da seção Comentários antes de terminar de digitar e enviar um comentário mantém o comentário na página no modo de rascunho mesmo depois de fazer logoff e logon novamente. <!--this is no longer possible for records: Any images that are added to the comment are also saved in the draft. Drafts are saved for 7 days after which they are discarded and cannot be recovered. Drafted comments are only visible to the user entering them.-->

1. (Opcional) Para desfazer ou refazer uma alteração, use as seguintes teclas de atalho:
   * CTRL + Z (⌘+z para Mac) para desfazer uma alteração
   * CTRL + Y (⌘+y para Mac) para refazer uma alteração
1. (Opcional e condicional) Se a sua instância do Workfront fizer parte da Experiência unificada da Adobe, adicione **@** seguido do nome de um usuário ou de uma equipe para marcá-los na atualização. Para obter mais informações, consulte a seção [Considerações sobre comentários em um registro](#considerations-about-commenting-on-a-record) neste artigo.

1. (Opcional) Use as opções na barra de ferramentas de Rich Text para formatar o texto, adicionar emojis ou links para a atualização a fim de aprimorar o conteúdo.

   >[!TIP]
   >
   >Não é possível adicionar imagens a um comentário de registro.


1. Continue adicionando comentários ao registro.

   Para obter mais informações sobre a atualização de objetos, incluindo registros do Workfront Planning, consulte [Trabalho de atualização](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

1. (Opcional) Clique no ícone **Mais** ![Mais menu](assets/more-menu.png) no canto superior direito do comentário e em **Excluir** para excluir o comentário.
1. (Opcional) Clique no ícone **Ocultar Comentários** ![Ocultar comentários](assets/hide-comments-icon.png) para fechar o painel direito.

<!--
      >[!TIP]
      >
      >If another user submits a comment to the same item you are updating, there is a red line with a "New" indicator to inform you of the newer comments. 
      >
      >The indicator displays only after the comment was submitted on the item, and not when the comment is still composed. 
      >
      >![New line indicator in comments](assets/new-line-indicator-comments.png)
1. Click **Submit** to add the update to the record. 
1. (Optional) To edit a comment, click the **More** menu ![More menu](assets/more-menu.png) in the upper-right corner of the comment, then click **Edit**.
   >[!IMPORTANT]
   >
   >You can edit your comment only within 15 minutes from submitting it.  
1. Edit the information in the comment, add or remove images or remove any of the tagged users. An "edited" indicator is added to the left of the comment.
      >[!TIP]
      >
      >Comments from the current year do not display the year in the date stamp. Hovering over a timestamp displays the full date, including the year.
1. (Optional and conditional) To search for an existing comment, start typing a keyword in the search box in the upper-right corner of the **Comments** area.     
   ![Search box for comments](assets/search-box-for-comments-area.png)
1. (Optional) Click **Reply** or start typing a comment in the **Add reply ..** area, to reply to an existing comment, then follow steps 4-8 above. (**************accurate??***********)
1. (Conditional and optional) If other users have added comments that display outside of the visible area in the Comments section while you were adding your comments, click **View** inside the **new comments banner** at the bottom of the screen  to display these comments.
   ![New comments banner on record](assets/new-comments-banner-on-record.png)

    Additional comments display at the bottom of the screen.
1. (Optional) Click the **Like** icon to like an update or acknowledge that you read it. The icon updates with the number of likes.
1. (Conditional and optional) If you included additional people in your comment, click the avatars of the users included in the update to display a list of users that the comment is shared with. 
1. (Optional) Click the **More** icon ![More menu](assets/more-menu.png) in the upper-right corner of the comment and click one of the following options, to copy a information from a comment: 
    * **Copy link**: This copies a link to the comment to your clipboard.
    * **Copy body text**: This copies the text of the comment to your clipboard.
    * **Quote reply**: This copies the content of your comment into a new reply. Images are not included in the copied reply. 

    For more information, see [Update work](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/update-work.md). -->

## Visão geral da seção Histórico

É possível revisar as alterações feitas no registro na seção History do painel direito de um registro.

Para obter mais informações, consulte [Visão geral da seção de histórico](/help/quicksilver/planning/records/history-section-overview.md).
