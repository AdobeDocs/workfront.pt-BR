---
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: account-settings-workfront-proof
title: Configure a área suspensa em [!DNL Workfront Proof]
description: Como um [!DNL Workfront Proof] administrador, você pode definir, exibir e editar as configurações do Dropzone de seus usuários. Para obter informações sobre Dropzone, consulte O Dropzone.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: c5c0c7ac-f829-401d-a27c-9581856a7cec
source-git-commit: a6cd3fe793c197308105da27369191d84cb59377
workflow-type: tm+mt
source-wordcount: '498'
ht-degree: 0%

---

# Configure a área suspensa em [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Este artigo se refere à funcionalidade no produto independente [!DNL Workfront Proof]. Para obter informações sobre prova dentro de [!DNL Adobe Workfront], consulte [Tofing](../../../review-and-approve-work/proofing/proofing.md).

Como um [!DNL Workfront Proof] administrador, você pode definir, exibir e editar as configurações do Dropzone de seus usuários. Para obter informações sobre Dropzone, consulte [Dropzone](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/dropzone.md).

1. Clique em **[!UICONTROL Configurações]** > **[!UICONTROL Configurações da conta]**, em seguida, abra o **[!UICONTROL Dropzone]** guia .

1. Faça qualquer uma das seguintes alterações no **[!UICONTROL Detalhes da zona de transferência]** seção:

   * **[!UICONTROL Web Dropzone]**: Ative ou desative a área de transferência.
   * **[!UICONTROL URL do Web Dropzone]**: O URL que você deve inserir no navegador para enviar provas através do Dropzone.
   * **[!UICONTROL Dropzone de email]**: Ative ou desative a Área do email.

      >[!NOTE]
      >
      >Não há mais suporte para enviar emails para áreas de soltar.

   * **[!UICONTROL Proprietário da Zona Dropzone]**: Defina ou edite o proprietário do Dropzone. Essa é a pessoa que será notificada de novos envios ao Dropzone. Para ser definido como o proprietário do Dropzone, o usuário deve ser um Supervisor, Administrador, Administrador de Faturamento ou o Criador da conta. Para obter mais informações, consulte [Perfis de prova de permissões em [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md).

   * **[!UICONTROL Função padrão para criadores]**: Todos os envios são adicionados à prova com essa função como padrão.
   * **[!UICONTROL Notificação por email para todos os criadores]**: Defina a preferência de alerta por email para criadores de prova (enviadores) aqui. Consulte [Defina as configurações de notificação de email em [!DNL Workfront Proof]](../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md) para obter informações sobre as diferentes configurações de alerta disponíveis.

   * **[!UICONTROL Nova função de versão]**: Habilite e desabilite a função Nova versão no Dropzone. Isso fornece ou remove a capacidade das pessoas enviarem novas versões de provas via Dropzone.
   * **[!UICONTROL Excluir provas de rascunho após (dias)]**: Especifique o número de dias após o qual uma prova de rascunho será excluída. As provas permanecerão em um estado de rascunho se o envio do Dropzone não for concluído após o upload do arquivo para o Dropzone.
   * **[!UICONTROL Ocultar função de revisor]**: Ocultar o campo de função do revisor ao adicionar pessoas à Zona de controle.
   * **[!UICONTROL Enviar mensagem de prova na ativação]**: Configurar [!DNL Workfront Proof] para enviar emails de notificação de prova aos revisores automaticamente quando uma prova for ativada.
   * **[!UICONTROL Ativar prova ao enviar]**: Configurar [!DNL Workfront Proof] para ativar provas automaticamente ao enviar (removendo a necessidade de ativá-las manualmente).

   * Se uma prova for movida para fora do Dropzone (por exemplo, para outra pasta na sua conta), as configurações do Dropzone não serão mais aplicadas à prova. Isso é particularmente importante em relação às configurações de alertas de email.

1. Faça alterações no **[!UICONTROL Campos da zona livre]** seção para especificar quais campos são exibidos na variável [!UICONTROL Detalhes da prova] da página de envio do Dropzone quando provas são enviadas por meio do Dropzone.
1. No **[!UICONTROL Domínios permitidos]** , especifique domínios que você deseja que possam usar o Dropzone.

   * Você pode clicar em **[!UICONTROL Adicionar domínio]** para adicionar um domínio. Quando terminar de adicionar os detalhes do domínio, clique em **[!UICONTROL Salvar]**.

   * Você pode **[!UICONTROL Editar]** e **[!UICONTROL Excluir]** qualquer domínio existente que você tenha adicionado anteriormente.

1. Em **[!UICONTROL Pessoas para notificar]**, especifique as pessoas que você deseja que sejam notificadas junto com o proprietário do Dropzone quando novas provas forem enviadas para o Dropzone [Dropzone](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/dropzone.md)

   * Clique em **[!UICONTROL Adicionar pessoas]**, insira os detalhes do recipient e clique em **[!UICONTROL Salvar]**.

   * **[!UICONTROL Excluir]** pessoas que você adicionou anteriormente.
