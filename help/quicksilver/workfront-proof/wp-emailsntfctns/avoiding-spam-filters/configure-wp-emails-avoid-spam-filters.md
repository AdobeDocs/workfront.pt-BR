---
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: avoiding-spam-filters
title: Configurar [!DNL Workfront Proof] emails para evitar filtros de spam
description: "O filtro de spam do seu cliente de email tem um objetivo importante: protegendo você de emails de spam incômodos e possivelmente mal-intencionados. Mas, se você não tiver as configurações corretas no filtro de spam, ele poderá impedir que você veja o seguinte [!DNL Workfront Proof] emails: prova de notificações por email, boletins informativos e comunicações especiais."
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 1fce3d83-fdce-4ded-8e78-3468243a59e1
source-git-commit: c989687e9adaf12a31a920921bf8fb69425ca1c5
workflow-type: tm+mt
source-wordcount: '493'
ht-degree: 0%

---

# Configurar [!DNL Workfront Proof] emails para evitar filtros de spam

>[!IMPORTANT]
>
>Este artigo se refere à funcionalidade no produto independente [!DNL Workfront Proof]. Para obter informações sobre prova dentro de [!DNL Adobe Workfront], consulte [Tofing](../../../review-and-approve-work/proofing/proofing.md).

O filtro de spam do seu cliente de email tem um objetivo importante: protegendo você de emails de spam incômodos e possivelmente mal-intencionados. Mas, se você não tiver as configurações corretas no filtro de spam, ele poderá impedir que você veja o seguinte [!DNL Workfront Proof] emails: prova de notificações por email, boletins informativos e comunicações especiais.

Para certificar-se de que [!DNL Workfront Proof] os emails são sempre roteados para a caixa de entrada em vez da pasta de spam, você deve adicionar o seguinte à  de lista de permissões:

* [!DNL Workfront Proof] servidor de correio: **[!DNL mx.proofhq.com]**
* [!DNL Workfront Proof] &quot;[!UICONTROL from]&quot; endereços de email (por exemplo, notification@proofhq.com)

Para obter mais informações sobre URLs a serem adicionados à sua lista de permissões, consulte [Configurar a  lista de permissões do firewall](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md) no artigo [Configurar a  lista de permissões do firewall](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

## [!DNL Workfront Proof] &quot;[!UICONTROL from]&quot; endereços de email

Dependendo do tipo de cliente de email, talvez seja necessário adicionar [!DNL Workfront Proof] &quot;[!UICONTROL from]&quot; endereços de email para um dos seguintes itens para impedir que o filtro de spam roteie seus emails para sua pasta de spam no futuro:

* Sua lista de contatos
* Seu [!UICONTROL Remetentes Seguros] lista
* Um filtro que você cria para enviar emails desses endereços para sua caixa de entrada

Talvez também seja necessário remover qualquer [!DNL Workfront Proof] emails da sua pasta de spam e verifique se algum dos &quot;[!UICONTROL from]Os endereços &quot; estão na lista de endereços bloqueados. Esta página de ajuda lista os [!DNL Workfront Proof] &quot;[!UICONTROL from]&quot; aborda e mostra como adicioná-los ao filtro de spam nos seguintes clientes de email:

* [!DNL Gmail]
* [!DNL Microsoft Outlook 2003 - 2007]
* [!DNL Windows Live Hotmail]
* [!DNL Yahoo Mail]
* [!DNL Aol]

>[!NOTE]
>
>Se tiver alguma dúvida sobre um procedimento descrito aqui, verifique a ajuda do seu cliente de email.

Para obter mais informações, consulte [Definir configurações de spam para clientes de email comuns](../../../workfront-proof/wp-emailsntfctns/avoiding-spam-filters/configure-spam-settings-clients.md).

## O [!DNL Workfront Proof] &quot;[!UICONTROL from]&quot; endereços de email para copiar

Para certificar-se de que [!DNL Workfront Proof] os emails chegam à sua caixa de entrada, será necessário adicionar dois [!DNL Workfront Proof] endereços de email separadamente para o filtro de spam do cliente de email:

* O endereço geral de suporte, [!DNL support@proofhq.com]dos quais [!DNL Workfront Proof] envia muitas comunicações por email
* Um endereço de notificação do qual [!DNL Workfront Proof] envia emails de notificação de prova para o criador de prova e os revisores com links para a prova. Pode ser um endereço geral, notification@support.proofhq.com, ou um endereço específico se você tiver um subdomínio personalizado ou um domínio de rótulo branco.

Para adicionar [!DNL Workfront Proof] &quot;[!UICONTROL from]&quot; endereça-se ao filtro do cliente de email:

1. Copie o geral [!DNL Workfront Proof] suporte &quot;[!UICONTROL from]&quot; endereço de email (support@proofhq.com) e cole-o no campo indicado para seu cliente de email.
1. Copie um dos itens a seguir [!DNL Workfront Proof] &quot;[!UICONTROL from]&quot; endereços de email e cole-os SEPARADAMENTE no campo indicado para seu cliente de email:

   * notification@support.proofhq.com se você NÃO tiver um subdomínio personalizado ou um domínio de rótulo branco
   * notification@yoursubdomain.proofhq.com se você tiver um subdomínio personalizado; substitua o nome do seu subdomínio neste endereço
   * notification@yoursubdomain.yourdomain.com se você tiver um domínio de rótulo branco; substitua o nome do seu subdomínio e o nome do domínio neste endereço

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">See the relevant section below for your email client to find out where to paste in these two Workfront Proof "[!UICONTROL from]" addresses.</p>
-->
