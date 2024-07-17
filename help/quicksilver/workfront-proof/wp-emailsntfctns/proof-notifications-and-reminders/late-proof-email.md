---
content-type: reference
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: proof-notifications-and-reminders
title: Email de prova tardia
description: O email de Prova atrasada é enviado aos recipients quando uma prova está perto do prazo ou está atingindo o prazo. Esses tipos de emails não podem ser desativados no nível de prova, mas são configuráveis no nível de conta e de configurações pessoais do usuário.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 23eb75a7-d7b7-4043-afba-cf45c86ab1ae
source-git-commit: 0c40e2b4e691d63832842736eaf09eeb67127498
workflow-type: tm+mt
source-wordcount: '405'
ht-degree: 0%

---

# [!UICONTROL Email de prova atrasada]

>[!IMPORTANT]
>
>Este artigo se refere à funcionalidade no produto independente [!DNL Workfront Proof]. Para obter informações sobre provas dentro de [!DNL Adobe Workfront], consulte [Prova](../../../review-and-approve-work/proofing/proofing.md).

O email [!UICONTROL Prova atrasada] é enviado aos recipients quando uma prova estiver próxima do prazo ou estiver atingindo o prazo final. Esses tipos de emails não podem ser desativados no nível de prova, mas são configuráveis no nível de conta e de configurações pessoais do usuário.

* [!UICONTROL Emails de prova atrasada] são enviados automaticamente aos revisores quando uma prova atinge seu prazo final e nem todas as revisões ou decisões foram tomadas.

  Esses emails são ativados por padrão e não podem ser ajustados para todas as contas, mas os usuários podem desativá-los nos padrões de Revisão.

* Emails de risco são enviados aos revisores quando uma prova está próxima do prazo. Elas estão desabilitadas por padrão e podem ser habilitadas nas [!UICONTROL Configurações de Conta]. Após ativadas, elas também podem ser ajustadas nos [!UICONTROL padrões de revisão].

Essas notificações não podem ser personalizadas.

As pessoas que serão notificadas são:

* O Proprietário, somente quando o alerta de [!UICONTROL Email] quando as provas estão atrasadas é habilitado, é verificado nos [!UICONTROL padrões de Revisão do Proprietário].
* Os aprovadores que ainda não tomaram a decisão sobre a prova. Para obter informações sobre decisões, consulte [Tomar uma decisão sobre uma prova no visualizador de provas](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md)

>[!NOTE]
>
>Se as notificações por email estiverem desabilitadas como padrão nas [!UICONTROL Configurações da conta], nenhum email de [!UICONTROL Prova atrasada] será enviado, mesmo que os revisores e aprovadores ainda não tenham enviado seus comentários e decisões. Você também pode desabilitar emails de [!UICONTROL Prova atrasada] nos padrões de Prova.

Considere o seguinte sobre notificações de prova:

* O administrador [!DNL Workfront] ou o administrador [!DNL Workfront Proof] pode incluir o logotipo de sua organização em suas notificações por email, conforme explicado em [Marcar o [!DNL Workfront Proof] site](../../../workfront-proof/wp-acct-admin/branding/brand-wp-site.md).
* Se precisar compartilhar várias provas com os mesmos revisores e não quiser que eles recebam vários emails, você pode carregá-los ao mesmo tempo. Todos os revisores recebem um email detalhando todas as provas e incluindo um URL pessoal para cada prova.

  >[!NOTE]
  >
  >O Criador das provas recebe um email [!UICONTROL Proof made] separado para cada uma das provas criadas. Para obter mais informações, consulte [O email [!UICONTROL Prova feita]](../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/proof-made-email.md).

* Se você ou seus revisores não receberem uma notificação por email esperada, consulte [Configurar [!DNL Workfront Proof] emails para evitar filtros de spam](../../../workfront-proof/wp-emailsntfctns/avoiding-spam-filters/configure-wp-emails-avoid-spam-filters.md).
