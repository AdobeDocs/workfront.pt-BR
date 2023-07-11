---
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: Marcar outros usuários em atualizações
description: Ao fornecer comentários de atualização em um objeto do Adobe Workfront, todos os usuários do projeto podem ver as informações enviadas. No entanto, pode haver momentos em que os usuários que não estão no projeto se beneficiem de visualizar essas informações. Em vez de incluir esses usuários no projeto, você pode marcá-los na atualização para compartilhá-los com eles. Os usuários marcados receberão uma notificação de evento.
author: Alina
feature: Get Started with Workfront
exl-id: c4c0d74f-ac50-4fc5-89d6-28f004c25b29
source-git-commit: 4116cd1610cc5b8de0407a96a4bc67532d78a25e
workflow-type: tm+mt
source-wordcount: '1485'
ht-degree: 0%

---

# Marcar outros usuários em atualizações

<!--take "Beta" references out when we remove the beta-->


<span class="preview">As informações destacadas nesta página se referem a funcionalidades ainda não disponíveis no geral. Ela está disponível somente no ambiente de Pré-visualização.

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
> * Metas, cartões na área Quadros
>
>   A nova experiência de comentários é a única experiência para metas e cartões. Você deve ter uma licença adicional para acessar o Workfront Goals. Para obter mais informações, consulte [Requisitos para usar as metas do Workfront](../../workfront-goals/goal-management/access-needed-for-wf-goals.md).
>
>     É possível adicionar e exibir atualizações em cartões na área Quadros ao ativar as seções Comentários e Atividade do sistema em um cartão. Para obter mais informações, consulte [Adicionar um cartão ad hoc a um quadro](../../agile/get-started-with-boards/add-card-to-board.md).


Você pode adicionar tags aos usuários ao fazer uma atualização em um objeto se quiser chamar a atenção deles para um objeto que, de outra forma, eles poderiam não seguir.
Em vez de incluir esses usuários no objeto atribuindo-os a ele ou fazendo com que eles se subscrevam a ele, você pode marcá-los na atualização para compartilhá-lo com eles. Os usuários marcados receberão uma notificação sobre a atualização inserida.

>[!NOTE]
>
>O usuário deve ativar uma notificação pessoal em seu perfil para receber a notificação por email. Para obter mais informações, consulte [Ativar ou desativar suas próprias notificações de eventos](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).
>

Para obter informações sobre como adicionar atualizações a objetos do Workfront, consulte [Atualizar trabalho](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

>[!NOTE]
>
>Quando um problema é convertido em um projeto ou tarefa, as atualizações são copiadas para o novo projeto ou tarefa, mas os usuários marcados não. Para continuar a conversa, você deve marcar os participantes novamente.

## Requisitos de acesso

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
   <td> <p>Solicitante ou superior para problemas e documentos; Revisor ou superior para todos os outros objetos</p> 
   <p><b>Nota</b>

Se você ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader"><strong>Permissões de objeto</strong></td> 
   <td> <p>Visualizar acesso ao objeto</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Para descobrir que plano, tipo de licença ou acesso você tem, entre em contato com o administrador do Workfront.

## Marcar outros usuários em atualizações

Marcar outras pessoas em uma atualização difere de acordo com a experiência e o objeto selecionado.

### Marcar outras pessoas sobre atualizações na seção Atualizações atual

Você pode marcar os usuários manualmente na seção Atualizações atual.

1. Comece a atualizar um item de trabalho, conforme descrito em [Atualizar trabalho](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).
1. No **Notificar** comece digitando o nome do usuário ou da equipe que deseja incluir e clique no nome quando ele aparecer na lista suspensa.

   Ou

   Digite o símbolo @ na caixa **Iniciar uma nova atualização** comece digitando o nome do usuário ou da equipe que deseja incluir na atualização e clique no nome quando ele aparecer na lista suspensa.

   >[!TIP]
   >
   >Para identificar o usuário correto quando há usuários com nomes semelhantes ou idênticos, observe o avatar, a função principal do usuário ou seu endereço de email. Os usuários devem estar associados a pelo menos uma função de trabalho para exibi-la quando você marcá-los em uma atualização.

   ![](assets/tag-users-in-update.png)

1. (Opcional) Para tornar a atualização privada, ative **Privativo(s) de minha empresa** no canto inferior direito da caixa de atualização. Isso torna a atualização visível apenas para os usuários em sua empresa. A variável **Privativo(s) de minha empresa** A opção está disponível somente quando uma Empresa é especificada no perfil do Workfront.

   >[!NOTE]
   >
   >Os usuários marcados fora da empresa ainda podem receber uma notificação no aplicativo ou um email, mesmo que não vejam os comentários privados na guia Atualizações. Recomendamos não marcar usuários externos em uma atualização se você não quiser compartilhar as informações com eles.

1. (Opcional) Para adicionar vários usuários e equipes, repita a etapa 2.

   >[!NOTE]
   >
   >Todos os usuários e membros da equipe listados no campo Notificar recebem uma notificação no aplicativo para a atualização e podem receber um email, dependendo da configuração de suas configurações de notificação por email. Os usuários que marcam a si mesmos em um comentário ou resposta recebem uma notificação para esse comentário ou resposta e podem ver seu nome no campo Notificar para o restante da thread, mas não recebem outra notificação, a menos que marquem a si mesmos novamente. Para obter mais informações, consulte [Ativar ou desativar suas próprias notificações de eventos](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md) e [Configurar notificações de eventos para todos no sistema](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

1. Clique em **Atualizar**.\
   Os usuários incluídos na atualização recebem automaticamente a permissão Exibir ao objeto e podem exibir e responder às atualizações feitas no objeto.

   Você pode ver quem foi marcado em cada resposta na parte superior da thread de atualização. Esses usuários, juntamente com quaisquer usuários que se inscreveram no objeto, recebem uma notificação sempre que uma atualização ou resposta é feita no objeto.

   ![](assets/tagging-transparency-350x192.png)

   Para obter informações sobre a funcionalidade adicional disponível ao atualizar um item de trabalho, consulte [Atualizar trabalho](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

### Marque outras pessoas sobre atualizações na experiência de comentários Beta

<!--replace the first paragraph in this section with the commented out piece when this releases to preview - July 13, 2023??

You can tag others on updates in the new commenting experience in the following ways:

* <span class="preview"> **Automatically**: When a user adds a comment or a reply, they are automatically tagged and added to the Tag people or teams area of the commenting box. </span>
* **Manually**: When you manually add a user to the Tag people area of the commenting box.

You can also remove users who are tagged by mistake when you edit or reply to a comment.-->


Você pode adicionar tags manualmente a outras pessoas em atualizações na experiência de comentários Beta. Também é possível remover usuários que foram marcados por engano ao editar ou responder a um comentário.

1. Comece a atualizar um item de trabalho, conforme descrito em [Atualizar trabalho](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md). <!--<span class="preview">As the comment owner, you are automatically tagged and added to the Tag people or teams area of the commenting box. </span> -->
1. No **Marcar pessoas ou equipes** comece digitando o nome do usuário ou da equipe que deseja incluir e clique no nome quando ele aparecer na lista suspensa.

   Ou

   Digite o símbolo @ na caixa **Escreva um comentário** comece digitando o nome do usuário ou da equipe que deseja incluir na atualização e clique no nome quando ele aparecer na lista suspensa.

   >[!TIP]
   >
   >Para identificar o usuário correto quando há usuários com nomes semelhantes ou idênticos, observe o avatar, a função principal do usuário ou seu endereço de email. Os usuários devem estar associados a pelo menos uma função de trabalho para exibi-la quando você marcá-los em uma atualização.

   ![](assets/tag-others-unified-commenting.png)

1. (Opcional) Para tornar a atualização privada, ative **Privativo(s) de minha empresa** no canto inferior direito da caixa de atualização. Isso torna a atualização visível apenas para os usuários em sua empresa. A variável **Privativo(s) de minha empresa** A opção está disponível somente quando uma Empresa é especificada no perfil do Workfront.

   >[!NOTE]
   >
   >* Essa opção é exibida somente quando o usuário está associado a uma Empresa.
   >* Os usuários marcados fora da empresa ainda podem receber uma notificação no aplicativo ou um email, mesmo que não vejam os comentários privados na guia Atualizações. Recomendamos não marcar usuários externos em uma atualização se você não quiser compartilhar as informações com eles.

1. (Opcional) Para adicionar vários usuários e equipes, repita a etapa 2. <!--insure this stays accurate-->

   >[!NOTE]
   >
   >Todos os usuários e membros da equipe listados no campo &quot;Marcar pessoas ou equipes&quot; recebem uma notificação no aplicativo para a atualização e podem receber um email, dependendo da configuração de suas configurações de notificação por email. Os usuários que marcam a si mesmos em um comentário ou resposta recebem uma notificação para esse comentário ou resposta e podem ver seu nome na lista como um membro do thread para o restante do thread, mas não recebem outra notificação, a menos que marquem a si mesmos novamente. Para obter mais informações, consulte [Ativar ou desativar suas próprias notificações de eventos](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md) e [Configurar notificações de eventos para todos no sistema](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

1. Clique em **Enviar**.\
   Os usuários incluídos na atualização recebem automaticamente a permissão Exibir ao objeto e podem exibir e responder às atualizações feitas no objeto.

   Veja quem foi marcado em cada resposta no texto da atualização, na área Membros. Esses usuários, juntamente com quaisquer usuários que se inscreveram no objeto, recebem uma notificação sempre que uma atualização ou resposta é feita no objeto.
1. (Opcional) Clique no número de **Membros** incluído na atualização para exibir uma lista de entidades com as quais a atualização inserida é compartilhada.

   ![](assets/members-icons-expanded-unshimmed.png)

   Para obter informações sobre a funcionalidade adicional disponível ao atualizar um item de trabalho, consulte [Atualizar trabalho](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

1. (Opcional) Clique no link **Mais** menu ![](assets/more-menu.png) à direita do ícone Curtir e, em seguida, clique em **Editar**. Remova os usuários marcados e clique em **Enviar**. Você pode editar um comentário somente em 15 minutos após inseri-lo. Só é possível editar os comentários adicionados.