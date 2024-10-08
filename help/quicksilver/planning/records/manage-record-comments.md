---
title: Gerenciar comentários de registro
description: É possível colaborar em registros do Adobe Workfront Planning, adicionando comentários ou respostas no painel direito de um registro. Você também pode exibir outras alterações feitas no registro e registradas pelo sistema nessa área.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 215883a4-e882-438e-9c21-954c0b1d741b
source-git-commit: bd202821687453288c96147933331c8a7a6b3acb
workflow-type: tm+mt
source-wordcount: '1267'
ht-degree: 0%

---

# Gerenciar comentários de registro

{{planning-important-intro}}

<!--update the system updates articles when we release to open beta - check the long commenting stream article list and see articles that document where in the system we have system updates; "Workfront Planning records" should be there-->

É possível colaborar em registros do Adobe Workfront Planning, adicionando comentários ou respostas no painel direito de um registro. Você também pode exibir outras alterações feitas no registro e registradas pelo sistema nessa área.

O painel direito de um registro exibe as seguintes seções:

* **Comentários**: exibe comentários e respostas que os usuários adicionam aos registros.
* **Histórico**: exibe as alterações registradas pelo sistema que os usuários fazem nos campos de registro. Para obter mais informações, consulte [Visão geral da seção de histórico](/help/quicksilver/planning/records/history-section-overview.md).

## Requisitos de acesso

+++ Expanda para exibir os requisitos de acesso do Workfront Planning.

Para acessar o Workfront Planning, é necessário ter o seguinte:

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Produtos</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Planejamento do Adobe Workfront<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>plano do Adobe Workfront*</p></td> 
   <td> 
<p>Qualquer um dos seguintes planos da Workfront:</p> 
<ul><li>Selecionar</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>O Workfront Planning não está disponível para planos herdados do Workfront</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Plano de planejamento do Adobe Workfront*</p></td> 
   <td> 
<p>Qualquer </p> 
<p>Para obter mais informações sobre o que está incluído em cada plano do Workfront Planning, entre em contato com seu gerente de conta da Workfront. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>plataforma Adobe Workfront</p></td> 
   <td> 
<p>A instância da Workfront de sua organização deve ser integrada à Adobe Unified Experience para acessar todos os recursos do Workfront Planning.</p> 
<p>Para obter mais informações, consulte <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Experiência unificada do Adobe para Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Licença da Adobe Workfront*</p></td> 
   <td><p> Colaborador, Leve ou Padrão</p>
   <p>O Workfront Planning não está disponível para licenças herdadas do Workfront</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Configuração do nível de acesso</p></td> 
   <td> <p>Não há controles de nível de acesso para o Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Permissões de objeto</p></td> 
   <td>   <p>Exibir ou aumentar permissões para um espaço de trabalho</a> </p>  
   <p>Os administradores do sistema têm permissões para todos os espaços de trabalho, incluindo aqueles que não criaram</p> </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Modelo de layout</p></td> 
   <td> <p>Todos os usuários, incluindo administradores do Workfront, devem receber um modelo de layout que inclua a área Planejamento no Menu principal. </p> </td> 
  </tr> 
</tbody> 
</table>

*Para obter mais informações sobre requisitos de acesso do Workfront, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--OLD: 

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Product</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront agreement</p></td>
   <td>
<p>Your organization must be enrolled in the early access stage for Workfront Planning </p>
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
   <td role="rowheader"><p>Access level configuration</p></td>
   <td> <p>There are no access level controls in Workfront Planning. </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>View or higher permissions to a workspace</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>Your Workfront or group administrator must add the Planning area in your layout template. For information, see <a href="/help/quicksilver/planning/access/access-overview.md">Access overview</a>. </p>  
</td>
  </tr>
 </tbody>
</table>
-->

## Considerações sobre comentários em um registro

* É possível adicionar comentários e respostas a registros no Workfront Planning, na seção Comentários de um registro.

* Comentários adicionados aos registros vinculados não são exibidos nos registros a partir dos quais você está vinculando. Por exemplo, se você comentar em um registro de Produto do Workfront Planning vinculado a um registro de Campanha, o comentário será exibido somente no registro de Produto no Workfront Planning e não no registro de Campanha do qual você está vinculando.

* É possível adicionar comentários a registros do Workfront Planning criados como resultado de uma conexão entre um registro e um objeto de outro aplicativo.

  Por exemplo, você pode comentar no registro do Project Workfront Planning depois de conectar os projetos Workfront aos registros do Workfront Planning. Para obter mais informações, consulte [Conectar registros](/help/quicksilver/planning/records/connect-records.md).

* Comentários adicionados a objetos vinculados em outros aplicativos não são exibidos no Workfront Planning e comentários adicionados a objetos vinculados no Workfront Planning não são exibidos em outros aplicativos.

  Por exemplo, comentários adicionados a projetos no Workfront não são exibidos no mesmo projeto vinculado a uma campanha no Workfront Planning, e comentários adicionados ao registro do projeto no Workfront Planning não são exibidos no Workfront.

* É possível marcar os usuários para chamar a atenção deles para uma atualização. Os usuários marcados não recebem uma notificação no aplicativo nem um email sobre a atualização. <!--this might change??-->

<!--replace the bullet above with this: * You can tag users to bring their attention to an update. Tagged users receive an in-app notification or an email notification about your update. 
   The following scenario exists:   

   * Adobe Unified Experience users receive both an in-app notification and an email notification. 
   * Users who are not in the Adobe Unified Experience receive only an email notification. 

      For information, see [Adobe Workfront Planning notifications: article index](/help/quicksilver/planning/notifications/notifications-information.md)
   
      To determine whether your company is using the Adobe Unified Experience, see [Adobe Unified Experience for Workfront](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md).
      -->

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

1. (Condicional) Se o painel direito não abrir por padrão, clique no ícone **Mostrar comentários** ![](assets/show-comments-icon.png) no canto superior direito para abrir a seção Comentários.

1. Comece a inserir um comentário na caixa **Novo comentário**.

   ![](assets/empty-comment-box-on-record.png)

   >[!TIP]
   >
   >Sair da seção Comentários antes de terminar de digitar e enviar um comentário mantém o comentário na página no modo de rascunho mesmo depois de fazer logoff e logon novamente. As imagens adicionadas ao comentário também são salvas no rascunho. Os rascunhos são salvos por 7 dias após os quais são descartados e não podem ser recuperados. Comentários em rascunho só ficam visíveis para o usuário que os digita.

1. (Opcional) Para desfazer ou refazer uma alteração, use as seguintes teclas de atalho:
   * CTRL + Z (⌘+z para Mac) para desfazer uma alteração
   * CTRL + Y (⌘+y para Mac) para refazer uma alteração
1. (Opcional) Adicione **@** seguido do nome de um usuário para marcar alguém na atualização.

   <!--Adobe Unified Experience users can receive an in-app and an email notification when they are tagged. All other users receive an email when they are tagged. For more information, see the section [Considerations about commenting on a record](#considerations-about-commenting-on-a-record) in this article. -->

1. (Opcional) Use as opções na barra de ferramentas de Rich Text para formatar o texto, adicionar emojis, links ou imagens à atualização e aprimorar o conteúdo. Para obter mais informações, consulte a seção &quot;Usar Rich Text em uma atualização do Workfront&quot; no artigo [Atualizar trabalho](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

   >[!TIP]
   >
   >Se outro usuário enviar um comentário para o mesmo item que você está atualizando, há uma linha vermelha com um indicador &quot;Novo&quot; para informá-lo sobre os comentários mais recentes.
   >
   >O indicador é exibido somente depois que o comentário foi enviado no item, e não quando o comentário ainda está composto.
   >
   >![](assets/new-line-indicator-comments.png)

1. Clique em **Enviar** para adicionar a atualização ao registro.
1. (Opcional) Para editar um comentário, clique no menu ![](assets/more-menu.png) de **Mais**, no canto superior direito do comentário, e clique em **Editar**.

   >[!IMPORTANT]
   >
   >Você pode editar seu comentário somente em 15 minutos a partir do envio.

1. Edite as informações no comentário, adicione ou remova imagens ou remova qualquer um dos usuários marcados. Um indicador &quot;editado&quot; é adicionado à esquerda do comentário.

   >[!TIP]
   >
   >Os comentários do ano atual não exibem o ano no carimbo de data. Passar o mouse sobre um carimbo de data e hora exibe a data completa, incluindo o ano.

1. (Opcional e condicional) Para pesquisar um comentário existente, comece digitando uma palavra-chave na caixa de pesquisa no canto superior direito da área **Comentários**.

   ![](assets/search-box-for-comments-area.png)

1. (Opcional) Clique em **Responder** ou comece a digitar um comentário na área **Adicionar resposta...** para responder a um comentário existente e, em seguida, siga as etapas 4 a 8 acima. <!--(**************accurate??***********)-->

1. (Condicional e opcional) Se outros usuários adicionaram comentários que são exibidos fora da área visível na seção Comentários enquanto você estava adicionando seus comentários, clique em **Exibir** dentro do **novo banner de comentários** na parte inferior da tela para exibir esses comentários.

   ![](assets/new-comments-banner-on-record.png)

   Comentários adicionais são exibidos na parte inferior da tela.

1. (Opcional) Clique no ícone **Curtir** para gostar de uma atualização ou confirmar que você a leu. O ícone é atualizado com o número de curtidas.
1. (Condicional e opcional) Se você incluiu outras pessoas no seu comentário, clique nos avatares dos usuários incluídos na atualização para exibir uma lista de usuários com os quais o comentário é compartilhado.
1. (Opcional) Clique no ícone ![](assets/more-menu.png) de **Mais** no canto superior direito do comentário e clique em uma das seguintes opções para copiar informações de um comentário:

   * **Copiar link**: copia um link para o comentário na área de transferência.
   * **Copiar texto do corpo**: copia o texto do comentário para a área de transferência.
   * **Resposta à cotação**: copia o conteúdo do seu comentário para uma nova resposta. As imagens não são incluídas na resposta copiada.

   Para obter mais informações, consulte [Atualizar trabalho](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/update-work.md).
1. (Opcional) Clique no ícone **Mais** ![](assets/more-menu.png) no canto superior direito do comentário e em **Excluir** para excluir o comentário.
1. (Opcional) Clique no ícone ![](assets/hide-comments-icon.png) de **Ocultar Comentários** para fechar o painel direito.

## Visão geral da seção Histórico

É possível revisar as alterações feitas no registro na seção History do painel direito de um registro.

Para obter mais informações, consulte [Visão geral da seção de histórico](/help/quicksilver/planning/records/history-section-overview.md).
