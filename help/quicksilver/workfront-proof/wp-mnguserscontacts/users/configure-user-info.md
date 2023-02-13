---
product-previous: workfront-proof
product-area: documents;system-administration;user-management;setup
navigation-topic: users-workfront-proof
title: Configurar informações do usuário usando [!DNL Workfront Proof]
description: Configurar informações do usuário usando [!DNL Workfront Proof]
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: ae8d3a96-ebf1-48ee-a7b7-50d69bffbd36
source-git-commit: 1a85f2a214036b62d13cb01f0b7a77392648a5fd
workflow-type: tm+mt
source-wordcount: '558'
ht-degree: 0%

---

# Configurar informações do usuário usando [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Este artigo se refere à funcionalidade no produto independente [!DNL Workfront Proof]. Para obter informações sobre prova dentro de [!DNL Adobe Workfront], consulte [Tofing](../../../review-and-approve-work/proofing/proofing.md).

1. Comece a criar ou editar um usuário conforme descrito em [Criar usuários usando [!DNL Workfront Proof]](../../../workfront-proof/wp-mnguserscontacts/users/create-users.md).
1. Especifique as seguintes informações:

   * No **[!UICONTROL Detalhes pessoais]** seção:

      * **Endereço de email:** O endereço de email do usuário.
      * **Nome:** O nome do usuário.
      * **Sobrenome:** O sobrenome do usuário.
      * **Posição:** A posição do usuário na empresa.
      * **Perfil de permissão:** As permissões do usuário na conta de prova.
      * **Idioma:** O idioma principal do usuário.
      * **Fuso horário:** Selecione o fuso horário do usuário.
      * **Formato de data:** Selecione o formato de data preferencial do usuário.
      * **Aceitar - Emails de produto e marketing:** Selecione se deseja aceitar o usuário para emails de produto e marketing.
      * **Somente API:** Permite que o usuário faça logon somente por meio da API.
   * No **[!UICONTROL Detalhes do usuário]** digite as informações de contato do usuário, como endereço e número de telefone.
   * No **[!UICONTROL Configurações de prova padrão]** , defina as configurações que afetam a maneira como o usuário cria ou funciona em provas.

      * **Função de prova padrão:** Selecione uma função de prova padrão para o usuário. As opções de função são **[!UICONTROL Somente leitura]**, **[!UICONTROL Revisor]**, **[!UICONTROL Aprovador]**, **[!UICONTROL Revisor e Aprovador]**, **[!UICONTROL Autor]** ou **[!UICONTROL Moderador]**.

         Para obter mais informações sobre funções de prova, consulte [Gerenciar funções de prova em [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md).

      * **Bloquear a prova quando todas as decisões forem tomadas:** Bloqueia automaticamente a prova de novas alterações depois que todas as decisões na prova forem tomadas.
      * **Logon necessário. A prova só pode ser compartilhada com outros usuários:** Torna a prova disponível somente para usuários com [!DNL Workfront Proof] credenciais de logon.
      * **Só é necessária uma decisão:** Exige apenas uma decisão sobre uma prova.
      * **Download do arquivo original:** Permite que o usuário baixe o arquivo original para uma prova. Essa opção é ativada por padrão.

         Para obter mais informações sobre como baixar arquivos originais, consulte [Baixar arquivos armazenados em [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/download-files-stored.md).

         <!--      
        <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>Public sharing. The proof can be shared via a public URL or embedded code:</strong>Enables the user to share proofs via a public URL or embed code.<br>This option is enabled by default but is not available if the&nbsp;<strong>Login required</strong>option is selected.<br>For more information on sharing proofs, see "<a href="../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/share-public-url.md" class="MCXref xref" xrefformat="{para}">Share the Public URL in Workfront Proof</a>."</li>      
        -->

      * **Assinatura. As pessoas podem se inscrever para a prova por meio do URL público ou do código incorporado:** Permite que revisores externos à organização se inscrevam para a prova por meio do URL público ou do código incorporado.

         Quando esta opção é selecionada, **O assinante deve clicar em um link em um email para acessar uma prova** também está disponível. Selecione essa opção para exigir que o revisor externo clique em um link no email para acessar a prova.
Essa opção é ativada por padrão se a variável **Compartilhamento público** está selecionada.

      * **Função padrão para novos revisores convidados:** Selecione uma função de prova padrão para os revisores convidados. As opções são as mesmas do **Função de prova padrão.**
   * No **[!UICONTROL Configurações padrão de alerta de email]** seção:

      * **Alerta de email padrão:** Selecione a frequência com que o usuário recebe atualizações de email. Selecionar **Todas as atividades, Respostas aos meus comentários, Decisões, Decisão Final, Resumo por hora, Resumo diário,** ou **Desabilitado**.

         Para obter mais informações sobre as opções de alerta de email padrão, consulte [Defina as configurações de notificação de email em [!DNL Workfront Proof]](../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md)

      * **Alerta de email padrão para novos revisores de convidados:** Selecione a frequência com que os revisores convidados recebem atualizações por email. As opções são as mesmas para **Alerta de email padrão.**

      * **Envie uma confirmação por email quando as provas estiverem prontas:** Selecione para enviar automaticamente ao usuário um email de confirmação quando as provas estiverem prontas.
      * **Formato dos emails enviados para este usuário:** Selecionar **[!UICONTROL HTML]** ou **[!UICONTROL Texto sem formatação]** como o formato padrão para emails enviados ao usuário.
   * No **[!UICONTROL Configurações de mensagem personalizada]** seção: Criar configurações para modelos de prova.

      Para obter mais informações sobre modelos, consulte:

      * **Modelo de assunto da prova:** Crie um modelo para um assunto de prova.
      * **Modelo de mensagem de prova:** Crie um modelo para uma mensagem de prova e seu formato.
