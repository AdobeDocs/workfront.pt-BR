---
content-type: reference
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: proof-notifications-and-reminders
title: Email de prova tardia
description: O email de Prova de atraso é enviado aos recipients quando uma prova está próxima do prazo ou atinge o prazo. Esses tipos de emails não são possíveis de ser desativados em um nível de prova, mas podem ser configurados no nível de configurações pessoais de conta e usuário.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 23eb75a7-d7b7-4043-afba-cf45c86ab1ae
source-git-commit: 0c40e2b4e691d63832842736eaf09eeb67127498
workflow-type: tm+mt
source-wordcount: '405'
ht-degree: 0%

---

# [!UICONTROL Prova tardia] email

>[!IMPORTANT]
>
>Este artigo se refere à funcionalidade no produto independente [!DNL Workfront Proof]. Para obter informações sobre prova dentro de [!DNL Adobe Workfront], consulte [Tofing](../../../review-and-approve-work/proofing/proofing.md).

O [!UICONTROL Prova tardia] o email é enviado para os recipients quando uma prova estiver próxima do prazo ou atingir o prazo final. Esses tipos de emails não são possíveis de ser desativados em um nível de prova, mas podem ser configurados no nível de configurações pessoais de conta e usuário.

* [!UICONTROL Prova tardia] os emails são automaticamente enviados a revisores quando uma prova atinge seu prazo e nem todas as revisões ou decisões foram feitas.

   Esses emails são ativados por padrão e não podem ser ajustados para todas as contas, mas os usuários podem desativá-los em seus padrões de Verificação digital.

* Em risco, os emails são enviados aos revisores quando uma prova está perto do prazo. Eles são desativados por padrão e podem ser ativados na variável [!UICONTROL Configurações da conta]. Uma vez ativadas, elas também podem ser ajustadas na variável [!UICONTROL Padrões de prova].

Essas notificações não podem ser personalizadas.

As pessoas que serão notificadas são:

* O Proprietário, somente quando [!UICONTROL Email] alerta quando as provas estiverem atrasadas estiver marcado no [!UICONTROL Padrões de Verificação Linguística do Proprietário].
* Qualquer aprovador que ainda não tenha tomado a sua decisão sobre a prova. Para obter informações sobre decisões, consulte [Tome uma decisão em uma prova no visualizador de prova](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md)

>[!NOTE]
>
>Se as notificações por email estiverem desabilitadas como padrão no [!UICONTROL Configurações da conta], não [!UICONTROL Prova tardia] os emails serão enviados mesmo se os revisores e aprovadores ainda não tiverem enviado seus comentários e decisões. Você também pode desativar [!UICONTROL Prova tardia] emails nos padrões da Verificação de provas.

Considere o seguinte sobre as notificações de prova:

* Seu [!DNL Workfront] administrador ou [!DNL Workfront Proof] o administrador pode incluir o logotipo de sua organização nas notificações por email, como explicado em [Marca [!DNL Workfront Proof] site](../../../workfront-proof/wp-acct-admin/branding/brand-wp-site.md).
* Se você precisar compartilhar várias provas com os mesmos revisores e não quiser que eles recebam vários emails, é possível carregá-los ao mesmo tempo. Todos os revisores recebem um email detalhando todas as provas e incluindo um URL pessoal para cada prova.

   >[!NOTE]
   >
   >O criador das provas recebe uma [!UICONTROL Prova feita] email para cada prova criada. Para obter mais informações, consulte [O [!UICONTROL Prova Feita] email](../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/proof-made-email.md).

* Se você ou seus revisores não receberem uma notificação por email esperada, consulte  [Configurar [!DNL Workfront Proof] emails para evitar filtros de spam](../../../workfront-proof/wp-emailsntfctns/avoiding-spam-filters/configure-wp-emails-avoid-spam-filters.md).
