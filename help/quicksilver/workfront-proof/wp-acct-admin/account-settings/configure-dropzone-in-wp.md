---
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: account-settings-workfront-proof
title: Configurar a zona de destino em  [!DNL Workfront Proof]
description: Como administrador do  [!DNL Workfront Proof] , você pode definir, exibir e editar as configurações da Zona de destino de seus usuários. Para obter informações sobre Dropzone, consulte A área de lançamento.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: c5c0c7ac-f829-401d-a27c-9581856a7cec
source-git-commit: a6cd3fe793c197308105da27369191d84cb59377
workflow-type: tm+mt
source-wordcount: '498'
ht-degree: 0%

---

# Configurar a zona de destino em [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Este artigo se refere à funcionalidade no produto independente [!DNL Workfront Proof]. Para obter informações sobre provas dentro de [!DNL Adobe Workfront], consulte [Prova](../../../review-and-approve-work/proofing/proofing.md).

Como administrador do [!DNL Workfront Proof], você pode definir, exibir e editar as configurações da Zona de destino de seus usuários. Para obter informações sobre Dropzone, consulte [A Dropzone](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/dropzone.md).

1. Clique em **[!UICONTROL Configurações]** > **[!UICONTROL Configurações de Conta]** e abra a guia **[!UICONTROL Dropzone]**.

1. Faça qualquer uma das seguintes alterações na seção **[!UICONTROL Detalhes da área de lançamento]**:

   * **[!UICONTROL Dropzone da Web]**: Habilite ou desabilite a Dropzone.
   * **[!UICONTROL URL do Dropzone da Web]**: o URL que você deve inserir no navegador para enviar provas por meio do Dropzone.
   * **[!UICONTROL Área de Descarte de Email]**: habilitar ou desabilitar a Área de Descarte de Email.

     >[!NOTE]
     >
     >Não há mais suporte para enviar e-mails para áreas de lançamento.

   * **[!UICONTROL Proprietário da Dropzone]**: Defina ou edite o proprietário da Dropzone. Essa é a pessoa que será notificada sobre novos envios para o Dropzone. Para ser definido como o proprietário da zona de destino, o usuário deve ser um supervisor, administrador, administrador de cobrança ou o criador da conta. Para obter mais informações, consulte [Perfis de permissões de prova em [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md).

   * **[!UICONTROL Função padrão para criadores]**: todos os remetentes são adicionados à prova com esta função como padrão.
   * **[!UICONTROL Notificação por email para todos os criadores]**: Defina a preferência de alerta por email para criadores de provas (remetentes) aqui. Consulte [Definir configurações de notificação por email em [!DNL Workfront Proof]](../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md) para obter informações sobre as diferentes configurações de alerta disponíveis.

   * **[!UICONTROL Nova função de versão]**: habilite e desabilite a função Nova Versão na Dropzone. Isso dá ou remove a capacidade de as pessoas enviarem novas versões de provas por meio do Dropzone.
   * **[!UICONTROL Excluir provas de rascunho após (dias)]**: especifique o número de dias após o qual uma prova de rascunho será excluída. As provas permanecerão em um estado de rascunho se o envio do Dropzone não for concluído depois de fazer upload do arquivo para o Dropzone.
   * **[!UICONTROL Ocultar função de revisor]**: oculta o campo de função de revisor ao adicionar pessoas à Dropzone.
   * **[!UICONTROL Enviar mensagem de prova na ativação]**: configure o [!DNL Workfront Proof] para enviar emails de notificação de prova automaticamente para os revisores quando uma prova for ativada.
   * **[!UICONTROL Ativar prova no envio]**: configure o [!DNL Workfront Proof] para ativar provas automaticamente no envio (removendo a necessidade de ativá-las manualmente).

   * Se uma prova for movida para fora da área de lançamento (por exemplo, para outra pasta na sua conta), as configurações da área de lançamento não serão mais aplicadas à prova. Isso é particularmente importante em relação às configurações de alerta por email.

1. Faça alterações na seção **[!UICONTROL Dropzone fields]** para especificar quais campos são exibidos na seção [!UICONTROL Detalhes da prova] da página de envio do Dropzone quando as provas são enviadas por meio do Dropzone.
1. Na seção **[!UICONTROL Domínios permitidos]**, especifique os domínios aos quais você deseja permitir o uso de Dropzone.

   * Você pode clicar em **[!UICONTROL Adicionar domínio]** para adicionar um domínio. Quando terminar de adicionar os detalhes do domínio, clique em **[!UICONTROL Salvar]**.

   * Você pode **[!UICONTROL Editar]** e **[!UICONTROL Excluir]** todos os domínios existentes adicionados anteriormente.

1. Em **[!UICONTROL Pessoas a serem notificadas]**, especifique as pessoas que você deseja notificar junto com o proprietário da Dropzone quando novas provas forem enviadas para a Dropzone [The Dropzone](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/dropzone.md)

   * Clique em **[!UICONTROL Adicionar pessoas]**, insira os detalhes do destinatário e clique em **[!UICONTROL Salvar]**.

   * **[!UICONTROL Excluir]** pessoas adicionadas anteriormente.
