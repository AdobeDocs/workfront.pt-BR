---
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: avoiding-spam-filters
title: Configurar  [!DNL Workfront Proof] emails para evitar filtros de spam
description: 'O filtro de spam do seu cliente de email tem um objetivo importante: proteger você contra emails de spam irritantes e possivelmente mal-intencionados. Porém, se você não tiver as configurações corretas no filtro de spam, ele poderá impedir que você veja os seguintes emails  [!DNL Workfront Proof]  importantes: notificações por email de prova, boletins informativos e comunicações especiais.'
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 1fce3d83-fdce-4ded-8e78-3468243a59e1
TQID: https://experienceleague.adobe.com/QMtIDexmxDDuKqTg-Z47-lMnQ27zDEdMtwg-8OUe3Uw
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 496
ht-degree: 0%

---

# Configurar emails do [!DNL Workfront Proof] para evitar filtros de spam

>[!IMPORTANT]
>
>Este artigo se refere à funcionalidade no produto independente [!DNL Workfront Proof]. Para obter informações sobre provas dentro de [!DNL Adobe Workfront], consulte [Prova](../../../review-and-approve-work/proofing/proofing.md).

O filtro de spam do seu cliente de email tem um objetivo importante: proteger você contra emails de spam irritantes e possivelmente mal-intencionados. Porém, se você não tiver as configurações corretas no filtro de spam, ele poderá impedir que você veja os seguintes emails importantes do [!DNL Workfront Proof]: notificações por email de prova, boletins informativos e comunicações especiais.

Para garantir que seus emails do [!DNL Workfront Proof] sejam sempre roteados para sua caixa de entrada em vez da pasta de spam, você deve adicionar o seguinte código ao incluo na lista de permissões:

* Servidor de email [!DNL Workfront Proof]: **[!DNL mx.proofhq.com]**
* [!DNL Workfront Proof] &quot;[!UICONTROL de]&quot; endereços de email (por exemplo, notification@proofhq.com)

Para obter mais informações sobre as URLs a serem adicionadas ao seu incluo na lista de permissões, consulte [Configurar incluo na lista de permissões do firewall](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md) no artigo [Configurar incluo na lista de permissões do firewall](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

## [!DNL Workfront Proof] &quot;[!UICONTROL de]&quot; endereços de email

Dependendo do seu tipo de cliente de email, talvez seja necessário adicionar [!DNL Workfront Proof] &quot;[!UICONTROL de]&quot; endereços de email a um dos itens a seguir para impedir que o filtro de spam encaminhe seus emails para a pasta de spam no futuro:

* Sua lista de contatos
* Sua lista [!UICONTROL Remetentes Confiáveis]
* Um filtro criado para enviar emails desses endereços para a sua caixa de entrada

Talvez também seja necessário remover todos os emails existentes do [!DNL Workfront Proof] da sua pasta de spam e verificar se algum dos endereços &quot;[!UICONTROL from]&quot; está na lista de endereços bloqueados. Esta página de ajuda lista os endereços [!DNL Workfront Proof] &quot;[!UICONTROL from]&quot; e mostra como adicioná-los ao filtro de spam nos seguintes clientes de email:

* [!DNL Gmail]
* [!DNL Microsoft Outlook 2003 - 2007]
* [!DNL Windows Live Hotmail]
* [!DNL Yahoo Mail]
* [!DNL Aol]

>[!NOTE]
>
>Se você tiver dúvidas sobre um procedimento descrito aqui, verifique a ajuda do seu cliente de e-mail.

Para obter mais informações, consulte [Definir configurações de spam para clientes de email comuns](../../../workfront-proof/wp-emailsntfctns/avoiding-spam-filters/configure-spam-settings-clients.md).

## O [!DNL Workfront Proof] &quot;[!UICONTROL de]&quot; endereços de email para copiar

Para garantir que os emails do [!DNL Workfront Proof] cheguem à sua caixa de entrada, será necessário adicionar dois endereços de email do [!DNL Workfront Proof] separadamente ao filtro de spam do seu cliente de email:

* O endereço de suporte geral, [!DNL support@proofhq.com], do qual [!DNL Workfront Proof] envia muitas comunicações por email
* Um endereço de notificação do qual [!DNL Workfront Proof] envia emails de notificação de prova para o criador da prova e os revisores com links para a prova. Pode ser um endereço geral, notification@support.proofhq.com, ou um endereço específico se você tiver um subdomínio personalizado ou um domínio de rótulo branco.

Para adicionar [!DNL Workfront Proof] &quot;[!UICONTROL de]&quot; endereços ao filtro do seu cliente de email:

1. Copie o endereço de email geral &quot;[!UICONTROL de]&quot; de suporte do [!DNL Workfront Proof] (support@proofhq.com) e cole-o no campo indicado para seu cliente de email.
1. Copie o endereço de email [!DNL Workfront Proof] &quot;[!UICONTROL from]&quot; apropriado e cole-o SEPARADAMENTE no campo indicado para seu cliente de email:

   * notification@support.proofhq.com se você NÃO tiver um subdomínio personalizado ou um domínio de rótulo branco
   * notification@yoursubdomain.proofhq.com se você tiver um subdomínio personalizado; substitua o nome do subdomínio neste endereço
   * notification@yoursubdomain.yourdomain.com se você tiver um domínio de rótulo branco; substitua o nome do subdomínio e o nome do domínio neste endereço

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">See the relevant section below for your email client to find out where to paste in these two Workfront Proof "[!UICONTROL from]" addresses.</p>
-->
