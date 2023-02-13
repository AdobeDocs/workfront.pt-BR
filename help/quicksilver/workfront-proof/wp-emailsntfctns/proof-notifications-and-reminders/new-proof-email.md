---
content-type: reference
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: proof-notifications-and-reminders
title: Novo email de prova
description: Melhore o funcionamento deste artigo para PiW.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: d879b1c6-e862-4653-aa93-90ad92170951
source-git-commit: 0c40e2b4e691d63832842736eaf09eeb67127498
workflow-type: tm+mt
source-wordcount: '812'
ht-degree: 0%

---

# Novo email de prova

>[!IMPORTANT]
>
>Este artigo se refere à funcionalidade no produto independente [!DNL Workfront Proof]. Para obter informações sobre prova dentro de [!DNL Adobe Workfront], consulte [Tofing](../../../review-and-approve-work/proofing/proofing.md).

<!--
<p style="color: #000000;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Make this article work better for PiW.</p>
-->

Ao criar uma nova prova ou uma nova versão de uma prova, adicionar novas pessoas a uma prova ou adicionar um workflow a uma prova, você pode decidir se deseja enviar um email para os revisores, conforme explicado nestes artigos:

* [Criar uma prova avançada com um fluxo de trabalho Automatizado](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md)
* [Gerar provas em [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md)

O email que seus recipients recebem é chamado de [!UICONTROL Nova prova] email. Somente o criador de prova e os usuários autorizados a adicionar revisores a uma prova podem controlar esse email. Os recipients não podem desabilitá-lo.

O novo email de prova contém:

* Sua mensagem pessoal (se você optar por incluir uma)
* Se você sempre enviar a mesma mensagem personalizada para seus revisores, pode ser uma boa ideia salvá-la em [!UICONTROL Configurações pessoais] nos termos do [!UICONTROL Padrões de prova] guia . Para obter mais informações, consulte .
* Link pessoal para a prova
* **[!UICONTROL Exibir detalhes]** link que leva você ao [!DNL Workfront] objeto (como um projeto, tarefa ou problema)
* Miniatura da imagem de prova
* Os seguintes detalhes da prova:

   * Nome da prova
   * Número da versão

      Para obter mais informações, consulte .

   * Lista dos revisores e seus progressos na prova
   * Um link para compartilhar a prova com outra pessoa

      Isso permite compartilhar o URL de prova e/ou o link de download do arquivo original. Isso não permite adicionar revisores explicitamente à prova, você só compartilhará o URL de prova pública e o recipient receberá acesso somente leitura à prova.

      Consulte [Compartilhar uma prova em [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/share-proof.md) para obter mais informações.

      Se você não quiser que esse link apareça no email do destinatário, desative o [!UICONTROL Compartilhamento público] na prova

      (Baixe o arquivo original e o URL público). Consulte [Gerenciar detalhes de prova em [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md) para obter mais informações.

## O registro de atividades

Envio de um [!UICONTROL Nova prova] o email para um revisor está conectado no [!UICONTROL Atividade] seção de [!UICONTROL Detalhes da prova] página. Consulte  [Gerenciar[!UICONTROL  Detalhes da prova] em [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md) para obter mais informações. Você pode verificar se a variável [!UICONTROL Nova prova] o email foi ativado no momento da criação de uma prova.

![New_Verison_email_-_acitivity_log.png](assets/new-verison-email---acitivity-log-350x44.png)

>[!NOTE]
>
>* Se o Criador ou o Proprietário da prova tiver [!UICONTROL Prova Feita] emails desativados por padrão (em suas configurações pessoais), eles não receberão nenhum [!UICONTROL Prova feita] ou [!UICONTROL Nova prova] emails mesmo se a variável [!UICONTROL Notificar pessoas por email] estiver marcada na página Nova prova . Para obter mais informações, consulte .
>* Se as notificações por email estiverem desabilitadas como padrão no [!UICONTROL Configurações da conta] o Criador/Proprietário da prova não receberá [!UICONTROL Prova feita] ou [!UICONTROL Nova prova] emails, mesmo se isso estiver ativado em suas configurações pessoais e a variável [!UICONTROL Notificar] pessoas por email está marcada na página Nova prova . Para obter mais informações, [O [!UICONTROL Prova Feita] email](../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/proof-made-email.md) e consulte .
>




## Ative o [!UICONTROL Nova prova] e-mail e incluir uma mensagem personalizada

Você pode especificar se deseja enviar um alerta por email para os revisores em uma prova ao criá-lo ou ao adicionar alguém a ele.

* [Ao criar uma prova](#when-you-create-a-proof)
* [Ao adicionar um revisor a uma prova](#when-you-add-a-reviewer-to-a-proof)

### Ao criar uma prova {#when-you-create-a-proof}

Ao criar uma nova prova no [!UICONTROL Nova prova] na página **[!UICONTROL Compartilhar]** selecione se deseja enviar alertas de email:

* Aqui você pode decidir se deseja [!UICONTROL Notificar pessoas por email] (1) Se você desmarcar essa opção, nenhum de seus revisores receberá um email informando que a prova está pronta para a revisão.
* Você também pode incluir uma mensagem Personalizada na notificação por email (2).
* Se decidir adicionar sua própria mensagem personalizada, você poderá colocar uma linha de assunto personalizada (3) e uma mensagem no corpo do email (4).
* Para descartar a mensagem personalizada, basta clicar no link (5).

   >[!NOTE]
   >
   >Se você sempre enviar a mesma mensagem personalizada para seus revisores, pode ser uma boa ideia salvá-la em suas configurações Pessoais na seção [!UICONTROL Padrões de prova] guia . Para obter mais informações, consulte .

![New_Proof_page_1.png](assets/new-proof-page-1-350x186.png)

![New_Proof_page_2.png](assets/new-proof-page-2-350x283.png)

### Ao adicionar um revisor a uma prova {#when-you-add-a-reviewer-to-a-proof}

Você pode selecionar se um novo revisor adicionado a uma prova existente será notificado da prova (semelhante ao acima).

* Primeiro, adicione novos revisores clicando no botão **[!UICONTROL Compartilhar esta versão]** no botão **[!UICONTROL Detalhes da prova]** página (1).

![Proof_Details_page_1.png](assets/proof-details-page-1-350x118.png)

* Uma caixa é exibida na qual é possível adicionar novos revisores. Em seguida, você pode decidir se deseja que eles sejam notificados por email (2) e optar por adicionar uma mensagem personalizada ao email (3).

![Proof_Details_page_2.png](assets/proof-details-page-2-350x174.png)

* Se você optar por adicionar uma mensagem personalizada, a caixa será expandida e será possível adicionar uma linha de assunto personalizada (4) e texto personalizado no corpo do email (5). Você também pode descartar a mensagem personalizada clicando no link (6).

![Proof_Details_page_3.png](assets/proof-details-page-3-350x258.png)
