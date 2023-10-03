---
product-previous: workfront-proof
product-area: documents;system-administration;user-management;setup
navigation-topic: users-workfront-proof
title: Configurar informações do usuário usando o [!DNL Workfront Proof]
description: Configurar informações do usuário usando o [!DNL Workfront Proof]
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: ae8d3a96-ebf1-48ee-a7b7-50d69bffbd36
source-git-commit: f776fb88000ea6044b88cba88d0cb7198c205d05
workflow-type: tm+mt
source-wordcount: '565'
ht-degree: 0%

---

# Configurar informações do usuário usando o [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Este artigo se refere à funcionalidade no produto independente [!DNL Workfront Proof]. Para obter informações sobre prova dentro do [!DNL Adobe Workfront], consulte [Prova](../../../review-and-approve-work/proofing/proofing.md).

1. Comece a criar ou editar um usuário conforme descrito em [Criar usuários usando [!DNL Workfront Proof]](../../../workfront-proof/wp-mnguserscontacts/users/create-users.md).
1. Especifique as seguintes informações:

   * No **[!UICONTROL Detalhes pessoais]** seção:

      * **Endereço de email:** O endereço de email do usuário.
      * **Nome:** O nome do usuário.
      * **Sobrenome** O sobrenome do usuário.
      * **Posição:** A posição do usuário na empresa.
      * **Perfil de permissão:** As permissões do usuário na conta de prova.
      * **Idioma:** O idioma principal do usuário.
      * **Fuso horário:** Selecione o fuso horário do usuário.
      * **Formato de data:** Selecione o formato de data preferido do usuário.
      * **Aceitar - emails de produto e marketing:** Escolha se o usuário deve aceitar para emails de produto e marketing.
      * **Somente API:** Permite que o usuário faça logon somente por meio da API.

   * No **[!UICONTROL Detalhes do usuário]** digite as informações de contato do usuário, como endereço e número de telefone.
   * No **[!UICONTROL Configurações de prova padrão]** defina as configurações que afetam a maneira como o usuário cria ou trabalha em provas.

      * **Função de prova padrão:** Selecione uma função de prova padrão para o usuário. As opções de função são **[!UICONTROL Somente leitura]**, **[!UICONTROL Revisor]**, **[!UICONTROL Aprovador]**, **[!UICONTROL Revisor e Aprovador]**, **[!UICONTROL Autor]** ou **[!UICONTROL Moderador]**.

        Para obter mais informações sobre funções de prova, consulte [Gerenciar funções de prova no [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md).

      * **Bloquear a prova quando todas as decisões forem tomadas:** Bloqueia automaticamente a prova contra outras alterações depois que todas as decisões sobre a prova são tomadas.
      * **Logon necessário. A prova só pode ser compartilhada com outros usuários:** Disponibiliza a prova somente para usuários com [!DNL Workfront Proof] credenciais de logon.
      * **É necessária somente uma decisão:** Requer apenas uma decisão sobre uma prova.
      * **Download do arquivo original:** Permite que o usuário baixe o arquivo original para uma prova. Essa opção está ativada por padrão.

        Para obter mais informações sobre como baixar arquivos originais, consulte [Baixar Arquivos Armazenados em [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/download-files-stored.md).

        <!--      
        <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>Public sharing. The proof can be shared via a public URL or embedded code:</strong>Enables the user to share proofs via a public URL or embed code.<br>This option is enabled by default but is not available if the&nbsp;<strong>Login required</strong>option is selected.<br>For more information on sharing proofs, see "<a href="../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/share-public-url.md" class="MCXref xref" xrefformat="{para}">Share the Public URL in Workfront Proof</a>."</li>      
        -->

      * **Assinatura. As pessoas podem se inscrever para a prova por meio do URL público ou do código de inserção:** Permite que revisores externos à organização se inscrevam para a prova por meio da URL pública ou do código de inserção.

        Quando essa opção é selecionada, **O assinante deve clicar em um link em um email para acessar uma prova** O também está disponível. Selecione essa opção para exigir que o revisor externo clique em um link no email para acessar a prova.
Essa opção estará ativada por padrão se a variável **Compartilhamento público** for selecionada.

      * **Função padrão para novos revisores convidados:** Selecione uma função de prova padrão para revisores convidados. As opções são as mesmas do **Função de prova padrão**, com exceção de Moderador e Autor.

   * No **[!UICONTROL Configurações padrão de alerta por email]** seção:

      * **Alerta de email padrão:** Selecione a frequência com que o usuário recebe atualizações por email. Selecionar **Todas as atividades, Respostas aos meus comentários, Decisões, Decisão final, Resumo por hora, Resumo diário,** ou **Desabilitado**.

        Para obter mais informações sobre as opções padrão de alerta por email, consulte [Definir configurações de notificação por email no [!DNL Workfront Proof]](../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md)

      * **Alerta de email padrão para novos revisores convidados:** Selecione a frequência com que os revisores convidados recebem atualizações por email. As opções são as mesmas para **Alerta de email padrão.**

      * **Envie um email de confirmação quando as provas estiverem prontas:** Selecione para enviar automaticamente ao usuário um email de confirmação quando as provas estiverem prontas.
      * **Formato dos emails enviados a este usuário:** Selecionar **[!UICONTROL HTML]** ou **[!UICONTROL Texto sem formatação]** como o formato padrão para emails enviados ao usuário.

   * No **[!UICONTROL Configurações de mensagem personalizadas]** seção: criar configurações para modelos de prova.

     Para obter mais informações sobre modelos, consulte:

      * **Modelo de assunto da prova:** Crie um modelo para um assunto de prova.
      * **Modelo da mensagem de prova:** Crie um modelo para uma mensagem de prova e seu formato.
