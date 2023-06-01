---
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: Atualizar trabalho
description: Você pode adicionar uma atualização em um objeto do Adobe Workfront (projeto, tarefa ou problema) para comunicar o progresso no objeto. Os usuários atribuídos ou inscritos no objeto podem exibir sua atualização. Também é possível marcar os usuários para chamar a atenção deles para a atualização.
author: Alina
feature: Get Started with Workfront
exl-id: 0f4d6895-6326-4a83-9bbc-bb58c876e7fc
source-git-commit: 7c458a41cd5376b746c93e9ed8e4f379a0ed1f4b
workflow-type: tm+mt
source-wordcount: '3181'
ht-degree: 1%

---

# Atualizar trabalho

<!--take "Beta" references out when we remove the beta-->

<span class="preview">As informações destacadas nesta página se referem a funcionalidades ainda não disponíveis no geral. Ela está disponível somente no ambiente de Pré-visualização.</span>

>[!NOTE]
>
>No momento, estamos reprojetando a experiência de comentários no Adobe Workfront.
>
>Para obter mais informações sobre a nova experiência de comentários, consulte [Nova experiência de comentários](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md).
>
>Você pode acessar a nova experiência para os seguintes objetos:
> * Problemas, <span class="preview">projetos, tarefas e documentos</span>.
   >
   >     Isso está disponível quando você ativa a experiência de comentários Beta.
   >
   >     Essa funcionalidade está disponível somente para a seção Atualizações e não está disponível para as seguintes áreas:
   >
   >     * Página inicial
   >     * Painel Resumo em listas
   >     * Painel Resumo em Planilhas de Horas
>
> * Metas

   >
   >   A nova experiência de comentários é o padrão para metas. Você deve ter uma licença adicional para acessar o Workfront Goals. Para obter mais informações, consulte [Requisitos para usar as metas do Workfront](../../workfront-goals/goal-management/access-needed-for-wf-goals.md).
   >
   >    Para obter informações sobre comentários sobre metas, consulte [Gerenciar comentários de meta em Metas do Adobe Workfront](../../workfront-goals/goal-management/manage-goal-comments.md).


Você pode adicionar comentários à maioria dos objetos no Adobe Workfront na seção Atualizações. Para obter mais informações sobre quais objetos exibem a seção Atualizações, consulte [Visão geral da seção Atualizações](../updating-work-items-and-viewing-updates/updates-tab-overview.md).

Você pode adicionar uma atualização em um objeto do Workfront (projeto, tarefa ou problema) para comunicar o progresso no objeto enquanto comenta no objeto. Os usuários atribuídos ou inscritos no objeto podem exibir sua atualização. Também é possível marcar os usuários para chamar a atenção deles para a atualização. Os usuários marcados receberão uma notificação no aplicativo e um email sobre a atualização.

As informações nesta página descrevem como você pode comentar em objetos do Workfront e como atualizar projetos, tarefas e problemas. Para obter informações sobre comentários sobre metas, consulte [Gerenciar comentários de meta em Metas do Adobe Workfront](../../workfront-goals/goal-management/manage-goal-comments.md). Você deve ter uma licença adicional para acessar o Workfront Goals.


Você pode adicionar uma atualização a projetos, tarefas e problemas nas seguintes áreas do Workfront:

* De um objeto do Workfront, na seção Atualizações
* Na área Início (para tarefas e problemas)
* No painel Resumo, em uma lista de objetos (para tarefas e problemas)
* Na folha de horas (para tarefas e problemas)

## Requisitos de acesso

<!--
drafted for P&P release:
<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront plan*</strong></td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront license*</strong></td> 
   <td> <p>Current license: Contributor or higher for issues and documents: Light or higher for all other objects</p> 
   Or
   <p>Legacy  license: Request or higher for issues and documents; Review or higher for all other objects</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Access level configurations*</strong></td> 
   <td> <p>View or Edit access for the object the update is on</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Object permissions</strong></td> 
   <td> <p>View access to the object</p> <p>For information on requesting additional access, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->
Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>plano do Adobe Workfront*</strong></td> 
   <td> <p>Qualquer Um</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Licença da Adobe Workfront*</strong></td> 
   <td> <p>Solicitação ou superior para problemas e documentos; revisão ou superior para todos os outros objetos</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurações de nível de acesso*</strong></td> 
   <td> <p>Acesso de Visualização ou Edição para o objeto no qual a atualização está</p> <p><b>Nota</b>

Se você ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader"><strong>Permissões de objeto</strong></td> 
   <td> <p>Visualizar acesso ao objeto</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir seu plano, tipo de licença ou acesso, entre em contato com o administrador do Workfront.

## Adicionar uma atualização a um item de trabalho

<!--drafted for the commenting experience - change the NOTE at the top of the following section with every new release to other objects -->

Adicionar uma atualização a um item de trabalho difere dependendo de qual versão da seção Atualizações e qual objeto você escolhe.

### Adicionar uma atualização a um item de trabalho na seção Atualizações atual

>[!NOTE]
>
>A seguinte funcionalidade está disponível para todos os objetos, exceto metas. Você deve ter uma licença adicional para acessar o Workfront Goals. Para obter informações sobre comentários sobre metas, consulte [Gerenciar comentários de meta em Metas do Adobe Workfront](../../workfront-goals/goal-management/manage-goal-comments.md)

1. Vá para o item de trabalho para o qual deseja fornecer uma atualização (como um projeto, tarefa ou problema).
1. Clique em **Atualizações** seção.
1. Clique em **Iniciar uma nova atualização,** em seguida, digite a atualização.
1. (Opcional) Use Rich Text ou adicione emojis, links ou imagens à atualização para aprimorar o conteúdo. Para obter mais informações, consulte [Usar Rich Text em uma atualização do Workfront](#use-rich-text-in-a-workfront-update) neste artigo
1. (Opcional) Atualize qualquer uma das seguintes informações sobre o item de trabalho:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Notificar</strong></td> 
      <td>Identifique os usuários que devem ser notificados sobre a atualização. Os usuários atribuídos ou inscritos no objeto recebem automaticamente uma notificação quando uma atualização é feita.<br><p>Para obter informações sobre como incluir outras pessoas em uma atualização, consulte <a href="../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md" class="MCXref xref">Marcar outros usuários em atualizações</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Data de confirmação</strong></td> 
      <td>No seletor de datas, selecione a data em que você confirma a conclusão do item de trabalho. Para obter informações sobre a Data de confirmação, consulte <a href="../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md" class="MCXref xref">Visão geral da data de compromisso</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Condição</strong></td> 
      <td>Selecione uma nova condição para a tarefa ou problema. Para obter informações sobre como selecionar uma condição, consulte <a href="../../manage-work/projects/updating-work-in-a-project/update-condition-for-tasks-and-issues.md" class="MCXref xref">Atualizar condição para tarefas e problemas</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Status</strong></td> 
      <td>Clique na seta ao lado do status atual e selecione o status desejado no menu suspenso. Para obter informações sobre como configurar um Status, consulte <a href="../../manage-work/projects/updating-work-in-a-project/update-task-status.md" class="MCXref xref">Atualizar status da tarefa</a>.<p>A atualização do status de um item de trabalho não altera automaticamente o status de um projeto. Dependendo de como seu projeto está configurado, você pode fazer atualizações no status do projeto separadamente. Para obter mais informações sobre os vários tipos de atualização de projeto, consulte <a href="../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">Selecione o tipo de atualização do projeto </a>.</p><p><b>Nota</b>

   Você não pode alterar o status de um item de trabalho enquanto ele estiver no status Aprovação pendente.</p></td>
   </tr> 
     <tr> 
      <td role="rowheader"><strong>Barra de conclusão</strong></td> 
      <td>(Disponível somente em tarefas) Indique a porcentagem de trabalho concluído deslizando a barra de progresso para a porcentagem desejada. Você também pode clicar duas vezes na barra de conclusão e inserir o percentual concluído.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Privativo(s) de minha empresa</strong></td> 
      <td> <p>Desabilite esta opção para impedir que usuários fora da sua empresa tenham acesso a esta atualização.</p> 
      <p><b>Nota</b></p>
      <p>Essa opção é exibida somente quando o usuário está associado a uma Empresa.</p>
      </td> 
     </tr> 
    </tbody> 
   </table>

1. Clique em **Atualizar** para adicionar a atualização ao objeto do Workfront.

   >[!NOTE]
   >
   >Uma pequena janela pop-up será exibida por sete segundos após clicar em **Atualizar**, permitindo que você desfaça a atualização e retorne ao painel de edição antes que a atualização seja publicada. A atualização será publicada se você ignorar a janela pop-up desfazer, esperar que ela desapareça ou sair da página.
   >
   >Se o administrador do Workfront selecionar a configuração &quot;Nunca permitir que os usuários excluam comentários&quot; no seu nível de acesso, não será possível desfazer um comentário. Para obter mais informações, consulte [Criar e modificar níveis de acesso personalizados](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

1. Para responder a uma atualização, consulte [Responder a atualizações](../../workfront-basics/updating-work-items-and-viewing-updates/reply-to-updates.md).

### Adicionar uma atualização a um item de trabalho usando a experiência de comentário Beta

1. Localize o objeto que você deseja atualizar e clique no nome dele para abrir a página do objeto.
1. Clique em  **Atualizações** no painel esquerdo.
1. Ativar o **Comentando Beta** no canto superior direito da área Atualizações, clique em **Concordo** no acordo Beta. Isso alterna a área Atualizações para a experiência de comentários Beta.
A variável **Comentários** é selecionada por padrão.
1. Comece a inserir um comentário no **Novo comentário** caixa.

   <span class="preview">![](assets/comment-box-empty-unshimmed.png)</span>

   >[!TIP]
   >
   >Sair da seção Atualizações antes de terminar de digitar e enviar um comentário mantém o comentário na página no modo de rascunho mesmo depois de fazer logoff e logon novamente. As imagens adicionadas ao comentário também são salvas no rascunho. Os rascunhos são salvos por 7 dias após os quais são descartados e não podem ser recuperados. Comentários em rascunho só ficam visíveis para o usuário que os digita.

1. (Opcional) Na **Marcar pessoas ou equipes** digite o nome ou o email de um usuário ou de uma equipe que deseja incluir neste comentário e, em seguida, selecione-o quando ele for exibido na lista.
1. (Opcional) Para adicionar formatação de rich text à atualização, use uma das seguintes opções no **Rich Text** barra de ferramentas para aprimorar o texto:

   * Negrito
   * Itálico
   * Sublinhar
   * Link
   * Lista com marcadores
   * Lista numerada
   * Adicionar anexo <!--(mark this parenthesis as draft: ************ this might be renamed to "Add image")-->

   Para obter mais informações, consulte [Usar Rich Text em uma atualização do Workfront](#use-rich-text-in-a-workfront-update) neste artigo. <!--remove this list, above, when we get to parity for Rich Text-->

   >[!TIP]
   >
   >Se outro usuário enviar um comentário para o mesmo item que você está atualizando, haverá uma linha vermelha com um indicador &quot;Novo&quot; para informá-lo dos comentários mais recentes.
   >
   >O indicador só é exibido depois que o comentário foi enviado sobre o item, e não quando o comentário ainda está composto.
   >
   >O indicador &quot;Novo&quot; é exibido somente quando o usuário que inseriu uma nova atualização, bem como o usuário que está inserindo uma atualização no momento, estão usando a nova experiência de comentário.
   >![](assets/real-time-new-red-indicator-unified-commenting.png)


1. Clique em **Enviar** para adicionar a atualização ao objeto do Workfront.
1. (Opcional) Para editar um comentário, **Mais** menu ![](assets/more-menu.png) à direita do ícone Curtir e, em seguida, clique em **Editar**.
1. Edite as informações no comentário, adicione ou remova imagens ou remova qualquer um dos usuários marcados.
Você pode editar seu comentário em até 15 dias a partir do envio. Um indicador &quot;Editado&quot; é adicionado à esquerda do carimbo de data que é exibido quando o comentário é atualizado.

   ![](assets/edited-tag-on-comment-unified-commenting.png)

   >[!TIP]
   >
   >* Um email é gerado para notificar os usuários sobre sua atualização somente quando você envia a atualização original. Nenhum email é gerado após a edição da atualização.
   >* O carimbo de data ao lado do comentário é a data do comentário original, não a data da última edição.


1. (Opcional) Clique em **Responder** para responder a um comentário existente, siga as etapas 4 a 7 acima. <!--(**************insure this stays accurate***********)-->. Para obter informações sobre como responder a uma atualização, consulte [Responder a atualizações](../../workfront-basics/updating-work-items-and-viewing-updates/reply-to-updates.md).
1. (Condicional e opcional) Se outros usuários tiverem adicionado comentários que são exibidos fora da área visível na seção Atualizações, clique em **Exibir** dentro do azul **novo banner de comentários** na parte inferior da tela para exibir esses comentários.

   ![](assets/blue-new-comments-banner-with-view-button.png)

   Comentários adicionais são exibidos na parte inferior da tela.

   >[!NOTE]
   >
   >   O indicador &quot;novos comentários&quot; e o botão &quot;Exibir&quot; são exibidos somente quando os usuários que inseriram as novas atualizações, bem como o usuário que está atualmente visualizando a seção Atualizações, estão usando a nova experiência de comentário.


1. (Opcional) Clique no link **Curtir** ícone![](assets/like-icon.png). O ícone é atualizado com o número de curtidas.
1. (Condicional e Opcional) Se você incluiu outras pessoas no seu comentário, clique no número de membros incluídos na atualização para exibir uma lista de entidades com as quais o comentário inserido é compartilhado.

   ![](assets/members-icons-expanded-unshimmed.png)
1. (Opcional) Clique no link **Atividade do sistema** para ver as atualizações registradas pelo sistema. Quando o objeto ou qualquer um de seus filhos é atualizado, o Workfront gera uma observação sobre essa atualização e a exibe na guia Atividade do sistema.

   Para obter mais informações, consulte [Visão geral da seção Atualizações](../updating-work-items-and-viewing-updates/updates-tab-overview.md)

   >[!TIP]
   >
   >Não é possível adicionar um comentário a uma atualização do sistema.


## Usar Rich Text em uma atualização do Workfront{#use-rich-text-in-a-workfront-update}

<!--remove this top note when we get to parity with the current version, OR change the note to mention that some options are ONLY available in the Beta version and not the current one.-->

>[!NOTE]
>
>Algumas das opções na barra de ferramentas de Rich Text podem não estar disponíveis para a experiência de comentários Beta.

Você pode aprimorar suas atualizações usando Rich Text ou adicionando vários itens a ele, como emojis, links ou imagens.

1. Vá para a área Atualizações e comece a digitar um comentário.
1. (Opcional) Para adicionar formatação de rich text à atualização, use os atributos na variável **Rich Text** à medida que você digita.

   | **Atributo** | **Botão da barra de ferramentas** | **Teclas de atalho do Mac** | **Teclas de atalho do Windows** |
   |---|---|---|---|
   | Negrito | ![mceclip10.png](assets/mceclip10.png) | ⌘+b | Ctrl+O |
   | Itálico | ![mceclip9.png](assets/mceclip9.png) | ⌘+i | Ctrl+I |
   | Sublinhar | ![mceclip8.png](assets/mceclip8.png) | ⌘+u | Ctrl+S |
   | Hiperlink | ![mceclip7.png](assets/mceclip7.png) | <br>Para abrir a caixa Criar links ou Adicionar links: ⌘+K</br> <br>Na experiência de comentário beta, para colar um link sobre o texto selecionado: ⌘+V</br> | <br>Para abrir a caixa Criar links ou Adicionar links: Ctrl+K</br> <br>Na experiência de comentário beta, para colar um link sobre o texto selecionado: Ctrl+V</br> |
   | Lista com marcadores | ![mceclip6.png](assets/mceclip6.png) | ⌘+Shift+8 | Ctrl+Shift+8 |
   | Lista numerada | ![mceclip5.png](assets/mceclip5.png) | ⌘+Shift+7 | Ctrl+Shift+7 |
   | Cotação de bloco | ![](assets/block-quote-icon-large.png) | ⌘+Shift+9 | Ctrl+Shift+9 |

   Para interromper a formatação do texto, desmarque o atributo no **Rich Text** barra de ferramentas.

   <!-- in the table above: take "Create Links" verbiage from the hyperlink when the old commenting is removed and the commenting beta is the only way to comment-->

   >[!NOTE]
   >
   >* A formatação também é exibida em qualquer notificação por email que os usuários recebem contendo sua atualização.
   >* A formatação de Rich Text aplicada a uma atualização em um email não é exibida na atualização quando visualizada na guia Atualizações.
   >* Se sua organização usar o Workfront com o Internet Explorer, qualquer texto formatado colado em uma atualização perderá sua formatação Rich Text e será exibido como texto sem formatação. É possível reformatar o texto usando os atributos na barra de ferramentas Rich Text.
   >* A formatação Rich Text não está disponível para atualizações feitas na área Folhas de horas ou para objetos de Nota e Última condição exibidos em um relatório.


1. (Opcional) Se quiser incluir texto de atualizações anteriores ou de outras fontes e diferenciá-lo da sua própria atualização, você poderá marcá-lo como uma Cotação de Bloqueio. Clique em **Cotação de bloco** ícone ![](assets/block-quote-small.png) e digite o texto que deseja citar. O texto citado é exibido marcado com uma linha cinza vertical. Clique em **Cotação de bloco** para retornar à formatação normal.

   ![](assets/block-quote-marked-350x144.png)

1. (Opcional) Adicione emojis à atualização.

   >[!NOTE]
   >
   >* O Workfront não substitui emoticons de pontuação, como :) por emojis.
   >* Os emojis não estão disponíveis para atualizações feitas na área Folhas de horas ou para objetos de Nota e Última condição exibidos em um relatório.
   >* O recurso emoji no Workfront utiliza caracteres Unicode e, como tal, é exibido apenas em navegadores e sistemas operacionais que oferecem suporte a pontos de código Unicode. Usuários em uma plataforma, navegador ou versão de sistema operacional diferente da sua podem não ter acesso aos mesmos emojis.
   >* Um emoji não suportado é representado por uma caixa preta ou branca.
   >* O Windows 7 suporta apenas emojis em preto-e-branco.
   >* Os emojis aplicados a uma atualização feita por email não são exibidos na atualização quando visualizados na área Atualizações.


1. (Opcional) Para adicionar um link de URL a fontes de informações adicionais:

   1. Clique em na atualização em que deseja inserir um link.
   1. No **Rich Text** barra de ferramentas, clique no link **Hiperlink** ícone ![](assets/link-icon.png).

   1. No **Criar link** que aparece, em **URL**, digite ou cole o URL da origem à qual deseja vincular.

   1. Em **Texto a ser exibido**, digite ou cole o texto do link.
   1. Clique em **Salvar**.

1. (Opcional) Para anexar uma imagem à atualização, siga um destes procedimentos, dependendo do ambiente usado:

   * Clique em **Imagem** ícone ![](assets/addimageicon-35x32.png) e navegue até a imagem no computador ou arraste a imagem até a área de atualização, ao usar a experiência de atualização atual

   Ou

   Clique em **Adicionar anexo** ícone ![](assets/add-image-paperclip-icon.png) e navegue até a imagem em seu computador ao usar a experiência de comentários Beta. <!--the name of the icon and the icon for it might change-->

   >[!NOTE]
   >
   >* O administrador do Workfront deve ativar a adição de imagens na seção Preferências de atualização de feeds da área Interface do Workfront antes que você possa ver os ícones de Imagem ou Adicionar anexo. Para obter informações, consulte [Configurar preferências para atualizações de usuário](../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-preferences-user-updates.md).
   >* O tamanho máximo do arquivo de imagem é 7 MB. Os tipos de arquivo de imagem compatíveis são .jpg, .gif e .png.
   >* As imagens podem ser acessadas na seção Atualizações em um objeto e também estão disponíveis na área Documentos.
   >* É possível enviar uma atualização com uma imagem e nenhum texto.
   >* Quando você exclui um comentário que contém uma imagem, os seguintes cenários existem, dependendo da experiência escolhida:
      >
      >     * Na experiência de comentários atual, a imagem permanece na área Documentos, mas não é mais visível na seção Atualizações.
      >     * Na nova experiência de comentários, a imagem é removida da seção Atualizações, bem como da área Documentos. A imagem também é excluída da área Documentos ao editar um comentário e excluir a imagem.
   >* Quando alguém exclui uma imagem anexada a um comentário da área Documentos, ela também é removida do comentário.


1. Clique em **Atualizar**  ou **Enviar**, ao usar a experiência de comentários Beta.


## Copiar informações de atualização

<!--drafted for beta release toggle - remove when copying an update will be available:

>[!NOTE]
>
>Copying an update is not possible when using the Beta commenting experience.
-->

Há várias maneiras de copiar uma atualização. Depois de copiar um link, você pode compartilhá-lo com outras pessoas para direcioná-las para a atualização.

* [Copiar a atualização](#copy-the-update)
* [Copiar o link da thread](#copy-the-thread-link)
* [Copiar o link de atualização](#copy-the-update-link)

### Copiar a atualização {#copy-the-update}

Esta opção copia o texto de uma atualização específica para a área de transferência.

1. Vá para a atualização ou resposta que deseja copiar.
1. Clique em **Mais** e clique em **Copiar texto do corpo**.

   ![Selecionar Copiar texto do corpo](assets/update-stream-copy-body-text-350x152.png)

### Copiar o link da thread {#copy-the-thread-link}

Essa opção copia o link completo da thread para a área de transferência, para que você possa compartilhar a thread com outros usuários.

1. Vá para o thread de atualização que deseja copiar.

1. Clique em **Mais** e clique em **Copiar link da discussão** ou **Copiar link**, ao usar a experiência Beta.

   ![](assets/update-stream-comment-menu-marked-350x152.png)

### Copiar o link de atualização {#copy-the-update-link}

Esta opção copia um link de atualização específico para a área de transferência. Quando você compartilha o link de atualização, o usuário que o segue vê uma borda ao redor da atualização.

1. Vá para a atualização ou resposta que deseja copiar.
1. Clique em **Mais** ao lado da atualização individual e clique em **Copiar link de atualização** ou **Copiar link**, ao usar a experiência Beta.

   ![](assets/update-stream-reply-menu-marked-350x182.png)

## Excluir uma atualização ou resposta

Dependendo do acesso que seu administrador do Workfront fornecer, talvez você possa excluir as atualizações adicionadas na guia Atualizações de um objeto. Para obter mais informações, consulte [Criar ou modificar níveis de acesso personalizados](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md#creating-a-new-access-from-scratch) no artigo [Criar ou modificar níveis de acesso personalizados](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

Nenhum usuário do Workfront (incluindo o administrador do Workfront) pode excluir atualizações feitas por outro usuário. No entanto, se o nível de acesso de um usuário permitir que ele exclua suas próprias atualizações, o administrador do Workfront poderá fazer logon como esse usuário e excluir as atualizações feitas. Para obter mais informações, consulte [Criar ou modificar níveis de acesso personalizados](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md#creating-a-new-access-from-scratch) e [Fazer logon como outro usuário](../../administration-and-setup/add-users/create-and-manage-users/log-in-as-another-user.md).

1. Vá para a atualização ou resposta que deseja excluir.
1. Clique em **Mais** menu ao lado da atualização ou resposta que deseja excluir e clique em **Excluir**.

   ![](assets/update-stream-comment-menu-marked-350x152.png)

1. Na mensagem exibida, clique em **Confirmar o** ou clique em **Excluir**, ao usar a experiência de comentários Beta.

   >[!NOTE]
   >
   >Excluir uma atualização com uma imagem anexada exclui o comentário e a imagem. Para obter mais informações, consulte [Usar rich text em uma atualização do Workfront](#use-rich-text-in-a-workfront-update) neste artigo.

   Quando o comentário excluído tiver respostas associadas, há uma indicação de que o comentário foi removido com o nome do usuário que o removeu.

   ![](assets/removed-comment-indicator-new-experience.png)

   Ao usar a experiência de comentários Beta, os comentários excluídos são removidos imediatamente do Workfront. Um usuário que usa a seção Atualizações vê um comentário sendo excluído por outro usuário em tempo real.

   <!--when we remove the beta, take out the first part of the sentence above about only when commenting in beta experience. Leave the rest though-->

## Adicionar uma atualização em uma Planilha de Horas

1. Vá para uma Planilha de Horas na qual você deseja fazer uma atualização.
1. Clique na Planilha de horas para abri-la.
1. Na parte inferior da Planilha de horas, clique em **Incluir um comentário**.
1. Na caixa exibida na parte inferior da Planilha de horas, digite uma atualização.

   ![timesheet_update_stream.png](assets/timesheet-update-stream-350x50.png)

1. (Condicional)Para salvar sua atualização sem enviar a Planilha de horas para aprovação, clique em **Salvar para mais tarde**.

   Ou

   Para salvar sua atualização e enviar a Planilha de horas para aprovação, clique em **Enviar para aprovação**.

   Ou

   Se sua Planilha de Horas não estiver configurada com um aprovador, clique em **Salvar e fechar planilha de horas** para salvar a atualização.

## Ativar ou desativar atualizações do sistema

<!--remove the preview tag with 23.2 production, but keep the note till we remove Beta and it becomed the only exprience: -->

>[!NOTE]
>
>Não é possível desativar as atualizações do sistema ao usar a experiência de comentários Beta.
>As informações nesta seção se referem apenas à funcionalidade disponível na seção Atualizações atual.
>Para obter mais informações sobre atualizações do sistema na versão Beta, consulte [Visão geral da seção Atualizações](../updating-work-items-and-viewing-updates/updates-tab-overview.md).


A seção Atualizações de um objeto do Workfront exibe dois tipos de informações:

* **Atualizações de usuário:** Atualizações de usuário são comentários que você e outros usuários do sistema inseriram.

   ![](assets/user-update-cl-350x277.png)

* **Atualizações do sistema:** As atualizações de sistema registram a remoção de ativos, a adição ou exclusão de versões, a anexação ou remoção de uma solicitação de aprovação, bem como quaisquer edições ou alterações feitas nos documentos no objeto.

   ![](assets/system-updates-cl-350x277.png)

Dependendo da sua licença do Workfront, as atualizações do sistema podem ser ativadas por padrão. Os administradores do Workfront podem determinar o que é rastreado nas atualizações do sistema, conforme explicado em [Atualizações rastreadas pelo sistema](../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/system-tracked-update-feeds.md). Você também pode filtrar as atualizações ou atividades do sistema para ver apenas as atualizações do usuário para todos os objetos.

Para obter mais informações sobre a diferença entre atualizações do usuário e do sistema, consulte [Atualizações rastreadas pelo sistema](../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/system-tracked-update-feeds.md).

Para ativar ou desativar as atualizações do sistema:

1. Clique em **Atualizações** em um objeto.
1. Clique em **Mostrar atualizações do sistema** para deslizar o switch para a esquerda (desativado) ou para a direita (ativado).

   ![](assets/show-system-updates-qs-350x55.png)

   Essa opção é mantida em todos os objetos no Workfront e permanece na posição selecionada, mesmo que você faça logout do Workfront.

