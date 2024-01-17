---
title: Gerenciar comentários de registro
description: É possível colaborar em registros Adobe Maestro, adicionando comentários ou respostas na área Comentários de um registro.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: 5f3d5c93c2fc721dda2dd04adac22190ef6a3f29
workflow-type: tm+mt
source-wordcount: '991'
ht-degree: 0%

---


# Gerenciar comentários de registro

<!--update the metadata with real information when making this available in TOC and in the left nav-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. </span>

<span class="preview">For information about the current release schedule, see [First Quarter 2024 release overview](/help/quicksilver/product-announcements/product-releases/24-q1-release-activity/24-q1-release-overview.md).</span> -->

É possível colaborar em registros Adobe Maestro, adicionando comentários ou respostas na área Comentários de um registro.

## Considerações sobre comentários em um registro

* Você pode adicionar comentários e respostas a registros operacionais e taxonomias no Maestro, na seção Comentários de um registro.

* Comentários adicionados aos registros vinculados não são exibidos nos registros a partir dos quais você está vinculando. Por exemplo, se você comentar em um registro de Produto Maestro que esteja vinculado a um registro de Campanha, o comentário será exibido somente no registro de Produto no Maestro e não no registro de Campanha do qual você está vinculando.

* Você pode adicionar comentários aos registros do Maestro criados como resultado de uma conexão entre um registro do Maestro e um objeto de outro aplicativo.

  Por exemplo, você pode comentar no registro Projeto Maestro depois de conectar projetos Workfront com registros Maestro. Para obter mais informações, consulte [Conectar registros](/help/quicksilver/maestro/records/connect-records.md).

* Comentários adicionados a objetos vinculados em outras aplicações não são exibidos no Maestro e comentários adicionados a objetos vinculados no Maestro não são exibidos em outras aplicações.

  Por exemplo, comentários adicionados a projetos no Workfront não são exibidos no mesmo projeto vinculado a uma campanha no Maestro, e comentários adicionados ao projeto no registro Maestro não são exibidos no Workfront.

* É possível marcar os usuários para chamar a atenção deles para uma atualização. Os usuários marcados não recebem uma notificação no aplicativo nem um email sobre a atualização. <!--this might change??-->

* Você pode adicionar uma atualização aos registros das seguintes áreas do Maestro:

   * Na página Detalhes.

  <!--* From the table view.-->

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Produto</p> </td>
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
   <td role="rowheader"><p>Configuração do nível de acesso</p></td>
   <td> <p>Não há controles de nível de acesso no Maestro. </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permissões</p></td>
   <td> <p>Exibir ou aumentar as permissões de um espaço de trabalho</a> </p>  
   <p>Os administradores do sistema têm permissões para todos os espaços de trabalho, incluindo aqueles que não criaram</p>
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Modelo de layout</p></td>
   <td> <p>O administrador do Workfront ou do grupo deve adicionar a área Maestri no modelo de layout. Para obter informações, consulte <a href="../access/access-overview.md">Visão geral do Access</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

### Gerenciar comentários nos registros

{{step1-to-maestro}}

O último espaço de trabalho acessado é aberto por padrão.
1. Escolha uma exibição de tabela na **Exibir** menu suspenso.
1. Clique no nome de um registro na exibição de tabela.

   O registro **Detalhes** é aberta. A área Comentários é aberta por padrão no painel direito.

1. Comece a inserir um comentário no **Novo comentário** caixa.

   ![](assets/empty-comment-box-on-record.png)

   >[!TIP]
   >
   >Sair da seção Comentários antes de terminar de digitar e enviar um comentário mantém o comentário na página no modo de rascunho mesmo depois de fazer logoff e logon novamente. As imagens adicionadas ao comentário também são salvas no rascunho. Os rascunhos são salvos por 7 dias após os quais são descartados e não podem ser recuperados. Comentários em rascunho só ficam visíveis para o usuário que os digita.

1. (Opcional) Para desfazer ou refazer uma alteração, use as seguintes teclas de atalho:
   * CTRL + Z (⌘+z para Mac) para desfazer uma alteração
   * CTRL + Y (⌘+y para Mac) para refazer uma alteração
1. (Opcional) Adicionar **@** seguido pelo nome de um usuário para marcar alguém na atualização.
1. (Opcional) Use as opções na barra de ferramentas de Rich Text para formatar o texto, adicionar emojis, links ou imagens à atualização e aprimorar o conteúdo. Para obter mais informações, consulte a seção &quot;Usar Rich Text em uma atualização do Workfront&quot; no artigo [Atualizar trabalho](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

   >[!TIP]
   >
   >Se outro usuário enviar um comentário para o mesmo item que você está atualizando, há uma linha vermelha com um indicador &quot;Novo&quot; para informá-lo sobre os comentários mais recentes.
   >
   >O indicador é exibido somente depois que o comentário foi enviado no item, e não quando o comentário ainda está composto.
   >
   >![](assets/new-line-indicator-comments.png)

1. Clique em **Enviar** para adicionar a atualização ao registro.
1. Para editar um comentário, clique no link **Mais** menu ![](assets/more-menu.png) no canto superior direito do comentário e clique em **Editar**.

   >[!IMPORTANT]
   >
   >Você pode editar seu comentário somente em 15 minutos a partir do envio.

1. Edite as informações no comentário, adicione ou remova imagens ou remova qualquer um dos usuários marcados. Um indicador &quot;editado&quot; é adicionado à esquerda do comentário.

   >[!TIP]
   >
   >Os comentários do ano atual não exibem o ano no carimbo de data. Passar o mouse sobre um carimbo de data e hora exibe a data completa, incluindo o ano.

1. (Opcional e condicional) Para pesquisar um comentário existente, comece digitando uma palavra-chave na caixa de pesquisa no canto superior direito do **Comentários** área.

   ![](assets/search-box-for-comments-area.png)

1. (Opcional) Clique em **Responder** ou comece a digitar um comentário no campo **Adicionar resposta...** para responder a um comentário existente, siga as etapas 4 a 8 acima. <!--(**************accurate??***********)-->

1. (Condicional e opcional) Se outros usuários tiverem adicionado comentários que são exibidos fora da área visível na seção Comentários enquanto você estava adicionando seus comentários, clique em **Exibir** dentro do **novo banner de comentários** na parte inferior da tela para exibir esses comentários.

   ![](assets/new-comments-banner-on-record.png)

   Comentários adicionais são exibidos na parte inferior da tela.

1. (Opcional) Clique no link **Curtir** para gostar de uma atualização ou confirmação de que você a leu. O ícone é atualizado com o número de curtidas.
1. (Condicional e opcional) Se você incluiu outras pessoas no seu comentário, clique nos avatares dos usuários incluídos na atualização para exibir uma lista de usuários com os quais o comentário é compartilhado.
1. (Opcional) Clique no link **Mais** ícone ![](assets/more-menu.png) no canto superior direito do comentário e clique em uma das seguintes opções, para copiar informações de um comentário:

   * **Copiar link**: isso copia um link para o comentário na área de transferência.
   * **Copiar texto do corpo** t: copia o texto do comentário para a área de transferência.
   * **Citar resposta**: copia o conteúdo do comentário para uma nova resposta. As imagens não são incluídas na resposta copiada.

   Para obter mais informações, consulte [Atualizar trabalho](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).
1. (Opcional) Clique no link **Mais** ícone ![](assets/more-menu.png) no canto superior direito do comentário e clique em **Excluir** para excluir o comentário.

