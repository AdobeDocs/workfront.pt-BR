---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: Credenciais de usuário do Adobe Workfront versus Credenciais de usuário SAML
description: Após a criação do usuário, você pode editar o usuário e habilitar "Permitir apenas a autenticação SAML 2.0" para que o usuário e a senha sejam controlados pelo sistema SAML. Com essa opção ativada, o usuário só tem permissão para fazer logon via SAML.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: faa55b09-10c3-48e6-8b39-33f9feb0a335
TQID: https://experienceleague.adobe.com/8paS2GIumamOltxTC8Gw2mBZ4bKB6TOgbly7IBPKhDw
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2: id: c1579802-ddd4-4214-8a91-97b2066abe11id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 235
ht-degree: 0%

---

# Credenciais de usuário do Adobe Workfront versus credenciais de usuário SAML

Este artigo se concentra especificamente em [!DNL Adobe Workfront] e SAML e não aborda outros métodos de autenticação SSO.

Em um banco de dados, o [!DNL Workfront] armazena o endereço de email de cada usuário como seu nome de usuário [!DNL Workfront], juntamente com sua senha [!DNL Workfront]. Essas credenciais são replicadas nas sandboxes Pré-visualização e Atualização personalizada.

Durante a criação do usuário, se [!DNL Workfront] detectar que o SAML 2.0 está configurado, o padrão será &quot;Permitir apenas a autenticação SAML 2.0&quot; para o usuário. Se a caixa &quot;Enviar um email de convite para essa pessoa&quot; estiver habilitada, [!DNL Workfront] desabilitará &quot;Permitir apenas a Autenticação SAML 2.0&quot; e ocultará essa opção. Quando a opção &quot;Enviar um email de convite para essa pessoa&quot; estiver habilitada, o usuário se tornará um usuário [!DNL Workfront] não SAML.

Após a criação do usuário, você pode editar o usuário e habilitar **[!UICONTROL Permitir apenas a autenticação SAML 2.0]**, para que o usuário e a senha sejam controlados pelo sistema SAML.

Com isso feito, o usuário poderá fazer logon somente por meio do SAML. Quando eles vão para a URL [!DNL Workfront], são automaticamente redirecionados para o sistema SAML e solicitados a fornecer seu nome de usuário e senha SAML.

As credenciais SAML são armazenadas em um sistema SAML externo, como o ADFS da Microsoft, não no Workfront.
