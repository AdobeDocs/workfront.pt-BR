---
content-type: reference
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: proof-notifications-and-reminders
title: Novo email de prova
description: Faça com que este artigo funcione melhor para PiW.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: d879b1c6-e862-4653-aa93-90ad92170951
source-git-commit: 1030d4110fd5dabb3b5751387585cc66968c2326
workflow-type: tm+mt
source-wordcount: '800'
ht-degree: 0%

---

# Novo email de prova

>[!IMPORTANT]
>
>Este artigo se refere à funcionalidade no produto independente [!DNL Workfront Proof]. Para obter informações sobre prova dentro do [!DNL Adobe Workfront], consulte [Prova](../../../review-and-approve-work/proofing/proofing.md).

<!--
<p style="color: #000000;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Make this article work better for PiW.</p>
-->

Ao criar uma nova prova ou uma nova versão de prova, adicionar novas pessoas a uma prova ou adicionar um fluxo de trabalho a uma prova, é possível decidir se deseja enviar um email aos revisores, conforme explicado nestes artigos:

* [Criar uma prova avançada com um fluxo de trabalho automatizado](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md)
* [Gerar provas em [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md)

O email que seus recipients recebem é chamado de [!UICONTROL Nova prova] email. Somente o criador da prova e os usuários autorizados a adicionar revisores a uma prova podem controlar esse email. Os recipients não podem desativá-la.

O email de nova prova contém:

* Sua mensagem pessoal (se você optar por incluir uma)
* Se você sempre enviar a mesma mensagem personalizada para seus revisores, convém salvá-la em suas [!UICONTROL Configurações pessoais] no [!UICONTROL Padrões de provas] guia. Para obter mais informações, consulte.
* Link pessoal para a prova
* **[!UICONTROL Exibir detalhes]** link que direciona você ao associado [!DNL Workfront] objeto (como um projeto, tarefa ou problema)
* Miniatura da imagem de prova
* Os seguintes detalhes da prova:

   * Nome da prova
   * Número da versão
   * Lista dos revisores e seu progresso na prova
   * Um link para compartilhar a prova com outra pessoa

     Isso permite compartilhar o URL da prova e/ou o link de download do arquivo original. Isso não permite adicionar revisores explicitamente à prova, você só compartilhará o URL de prova pública e o recipient receberá acesso somente leitura à prova.

     Consulte [Compartilhar uma prova no [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/share-proof.md) para obter mais informações.

     Se não quiser que esse link apareça no email do destinatário, desative a opção [!UICONTROL Compartilhamento público] configurações na prova

     (Baixar arquivo original e URL público). Consulte [Gerenciar detalhes da prova no [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md) para obter mais informações.

## O registro de atividades

Envio de um [!UICONTROL Nova prova] email para um revisor está conectado no [!UICONTROL Atividade] seção de [!UICONTROL Detalhes da prova] página. Consulte  [Gerenciar[!UICONTROL  Detalhes da prova] in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md) para obter mais informações. Você pode verificar se a variável [!UICONTROL Nova prova] O email estava ativado no momento da criação de uma prova.

![New_Version_email_-_activity_log.png](assets/new-verison-email---acitivity-log-350x44.png)

>[!NOTE]
>
>* Se o criador ou proprietário da prova tiver [!UICONTROL Prova feita] emails desativados por padrão (em suas configurações pessoais), eles não receberão [!UICONTROL Prova feita] ou [!UICONTROL Nova prova] emails mesmo se a variável [!UICONTROL Notificar pessoas por e-mail] está marcada na página Nova prova. Para obter mais informações, consulte.
>* Se as notificações por email estiverem desativadas como padrão no [!UICONTROL Configurações da conta] o criador/proprietário da prova não receberá nenhuma [!UICONTROL Prova feita] ou [!UICONTROL Nova prova] emails mesmo se isso estiver ativado nas configurações pessoais e no [!UICONTROL Notificar] A caixa People by email está marcada na página New proof. Para obter mais informações, [A variável [!UICONTROL Prova feita] email](../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/proof-made-email.md) e consulte .
>



## Ativar o [!UICONTROL Nova prova] e incluir uma mensagem personalizada

Você pode especificar se deseja enviar um alerta por email para os revisores em uma prova ao criá-la ou quando adicionar alguém a ela.

* [Ao criar uma prova](#when-you-create-a-proof)
* [Ao adicionar um revisor a uma prova](#when-you-add-a-reviewer-to-a-proof)

### Ao criar uma prova {#when-you-create-a-proof}

Ao criar uma nova prova no [!UICONTROL Nova prova] página, sob o **[!UICONTROL Compartilhar]** você pode selecionar se deseja enviar alertas de email:

* Aqui você pode decidir se deseja [!UICONTROL Notificar pessoas por e-mail] (1). Se você desmarcar essa opção, nenhum dos revisores receberá um email para avisá-los de que a prova está pronta para a revisão.
* Você também pode incluir uma mensagem personalizada na notificação por email (2).
* Se decidir adicionar sua própria mensagem personalizada, você poderá inserir uma linha de assunto personalizada (3) e uma mensagem no corpo do email (4).
* Para descartar a mensagem personalizada, basta clicar no link (5).

  >[!NOTE]
  >
  >Se você sempre enviar a mesma mensagem personalizada para seus revisores, convém salvá-la nas configurações Pessoais no [!UICONTROL Padrões de provas] guia. Para obter mais informações, consulte.

![Nova_página_de_prova_1.png](assets/new-proof-page-1-350x186.png)

![Nova_página_de_prova_2.png](assets/new-proof-page-2-350x283.png)

### Ao adicionar um revisor a uma prova {#when-you-add-a-reviewer-to-a-proof}

É possível selecionar se um novo revisor adicionado a uma prova existente será notificado sobre a prova (semelhante ao acima).

* Primeiro, adicione novos revisores clicando no ícone **[!UICONTROL Compartilhar esta versão]** botão no **[!UICONTROL Detalhes da prova]** página 1.

![Proof_Details_page_1.png](assets/proof-details-page-1-350x118.png)

* Uma caixa é exibida na qual é possível adicionar novos revisores. Você pode decidir se deseja que eles sejam notificados por email (2) e escolher adicionar uma mensagem personalizada ao email (3).

![Proof_Details_page_2.png](assets/proof-details-page-2-350x174.png)

* Se optar por adicionar uma mensagem personalizada, a caixa é expandida e você poderá inserir uma linha de assunto personalizada (4) e um texto personalizado no corpo do email (5). Também é possível descartar a mensagem personalizada clicando no link (6).

![Proof_Details_page_3.png](assets/proof-details-page-3-350x258.png)
