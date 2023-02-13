---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: Credenciais do usuário do Adobe Workfront versus [!DNL SAML] credenciais do usuário
description: Após a criação do usuário, você pode editar o usuário e ativar a opção "Permitir somente autenticação SAML 2.0" para que o usuário e a senha sejam controlados pelo sistema SAML. Com essa opção ativada, o usuário só tem permissão para fazer logon via SAML. Quando eles vão para o [!DNL Workfront] URL, eles são automaticamente redirecionados para o sistema SAML e solicitados a fornecer seu nome de usuário e senha SAML.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: faa55b09-10c3-48e6-8b39-33f9feb0a335
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '250'
ht-degree: 0%

---

# Credenciais do usuário do Adobe Workfront versus credenciais do usuário SAML

Este artigo se concentra especificamente em [!DNL Adobe Workfront] e SAML e não abrange outros métodos de autenticação SSO.

Em um banco de dados, [!DNL Workfront] armazena o endereço de email do usuário eawch como seu [!DNL Workfront] nome de usuário, juntamente com seus [!DNL Workfront] senha. Essas credenciais são replicadas nas sandboxes de Pré-visualização e Atualização Personalizada.

Durante a criação do usuário, se [!DNL Workfront] O detecta que o SAML 2.0 está configurado, o padrão é &quot;Permitir somente autenticação SAML 2.0&quot; para o usuário. Se a caixa &quot;Enviar um email de convite para essa pessoa&quot; estiver ativada, [!DNL Workfront] desativa &quot;Permitir somente autenticação SAML 2.0&quot; e oculta essa opção. Quando &quot;Enviar um email de convite para essa pessoa&quot; estiver ativado, o usuário se tornará um não SAML [!DNL Workfront] usuário.

Após a criação do usuário, você pode editar o usuário e ativar **[!UICONTROL Permitir apenas a autenticação SAML 2.0]** para que seu usuário e senha sejam controlados pelo sistema SAML.

Com isso concluído, o usuário poderá fazer logon somente via SAML. Quando eles vão para o [!DNL Workfront] URL, eles são automaticamente redirecionados para o sistema SAML e solicitados a fornecer seu nome de usuário e senha SAML.

As credenciais SAML são armazenadas em um sistema SAML externo, como o Microsoft ADFS, e não no Workfront.
