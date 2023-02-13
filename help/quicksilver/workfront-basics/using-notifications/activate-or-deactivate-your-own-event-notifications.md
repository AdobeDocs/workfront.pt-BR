---
product-area: setup
navigation-topic: notifications
title: Ativar ou desativar suas próprias notificações de evento
description: O administrador do Adobe Workfront configura quais notificações de evento os usuários recebem quando os eventos ocorrem no Workfront.
author: Lisa
feature: Get Started with Workfront
exl-id: 3d1f877e-6bb4-494e-b08e-c18ec87dd001
source-git-commit: ea16b13b6ecb6ecea365c6c4d31ee23b7bb712c6
workflow-type: tm+mt
source-wordcount: '623'
ht-degree: 0%

---

# Ativar ou desativar suas próprias notificações de evento

Seu Adobe [!DNL Workfront] O administrador configura quais notificações de evento os usuários recebem quando os eventos ocorrem no Workfront (como descrito em [[!UICONTROL Configurar evento] notificações para todos no sistema](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md)).

O administrador de grupo também pode configurar quais notificações de evento são ativadas para você e para os usuários do Grupo doméstico. Se o seu [!UICONTROL Grupo Doméstico] for um subgrupo, você receberá as notificações de evento ativadas para o grupo de nível superior acima do seu grupo.

Você pode personalizar isso ainda mais, configurando quais notificações recebe. Você também pode escolher se deseja receber notificações como eventos ou em um email de resumo diário.

Para obter informações sobre notificações por email, consulte [[!DNL Adobe Workfront] notificações](../../workfront-basics/using-notifications/wf-notifications.md).

>[!NOTE]
>
>* Se você ativar um tipo de notificação e depois descobrir que não está recebendo notificações desse tipo, pode ser porque esse tipo não se aplica à sua função.
>* O [!DNL Workfront] administrador ou um administrador de grupo não pode configurar notificações para [!DNL Workfront Goals]. Para obter mais informações sobre quais notificações a variável [!DNL Workfront] administrador pode configurar, consulte [Configurar notificações de evento para todos no sistema](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md). Para obter informações sobre como configurar notificações individuais para [!DNL Workfront Goals] continue lendo este artigo.
>


## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront plan*]</strong></td> 
   <td> <p>Qualquer Um</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licença*</strong></td> 
   <td> <p>[!UICONTROL Trabalho] ou superior</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano ou tipo de licença você possui, entre em contato com seu [!DNL Workfront] administrador.

## Exibir e modificar as configurações de notificação por email

1. Clique no botão **[!UICONTROL Menu principal]** ícone ![](assets/main-menu-icon.png) no canto superior direito de [!DNL Adobe Workfront]e, em seguida, clique no nome de usuário ao lado da imagem do perfil.

1. Clique no botão **[!UICONTROL Mais]** ícone ![](assets/more-icon.png) , depois clique em **[!UICONTROL Editar]**.

1. No **[!UICONTROL Editar Pessoa]** for exibida, vá para a caixa **[!UICONTROL Notificações]** seção.

1. Clique em uma categoria para exibir as configurações de notificação relacionadas a essa categoria.

   ![](assets/my-profile-notifications.png)

1. Marque ou desmarque as caixas de seleção à direita para especificar se deseja receber ou não notificações diariamente, instantaneamente ou em ambos.

   Você também pode usar as caixas de seleção de uma categoria para ativar ou desativar todas as notificações nessa categoria.

   >[!NOTE]
   >
   >Se você for membro da equipe de um projeto, continuará recebendo notificações por email até que seja removido da equipe, mesmo que não tenha mais acesso ao projeto. Para obter instruções sobre como remover usuários de uma equipe, consulte [Remover usuários de projetos](../../manage-work/projects/manage-projects/remove-users-from-projects.md).

   Para o **[!UICONTROL Comunicação]** , você pode selecionar notificações individuais somente para delivery instantâneo. Para que as notificações sejam entregues em um resumo diário, selecione todas.

   Se todas as notificações por email de uma determinada categoria forem ativadas, a caixa no título da categoria aparecerá como selecionada. Se todas as notificações por email em uma determinada categoria estiverem desativadas, a caixa não estará selecionada. Se algumas notificações forem ativadas e outras forem desativadas, a caixa de seleção categoria aparecerá como uma linha reta.\
   Quando você modifica uma configuração de notificação, o rótulo **[!UICONTROL Editado]** for exibido para essa configuração de notificação, para que você saiba que essa configuração de notificação foi modificada.

1. Se você selecionou notificações para serem enviadas como resumo diário, selecione a hora do dia em que deseja recebê-las na parte superior do **[!UICONTROL Notificações]** na seção **[!UICONTROL Receita diária por email após]** menu.

   ![](assets/digest-time-stamp-my-settings-350x78.png)

   O resumo diário inclui eventos que atendem aos critérios das notificações 24 horas antes do horário selecionado. Você recebe um email de resumo diário para cada tipo de notificação.\
   O resumo diário pode chegar após o tempo selecionado, dependendo de quantos emails estão na fila para entrega no sistema. A hora listada é a hora local, conforme especificado nas configurações do navegador.

1. (Condicional e opcional) Ao modificar as configurações de notificações por email no ambiente de Visualização, ative a **[!UICONTROL Receber emails deste ambiente de teste]** configuração para receber emails. Os emails não são gerados automaticamente do ambiente de Visualização.

   ![](assets/receive-emails-from-sandbox-setting-edit-350x223.png)

1. Clique em **[!UICONTROL Salvar alterações]**.
