---
user-type: administrator
product-area: system-administration
navigation-topic: security
title: Alterar o domínio do Adobe Workfront
description: Como administrador da Adobe Workfront e contato autorizado com o Suporte da Workfront, você pode solicitar ajuda da equipe de Suporte da Workfront para alterar o domínio do Workfront de sua organização.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: d817bd2b-1aaa-4dde-8e75-392c1da2943a
source-git-commit: be11c7417023ce2f310fce3e0cf77724d101b89e
workflow-type: tm+mt
source-wordcount: '242'
ht-degree: 17%

---

# Alterar o domínio do Adobe Workfront

<!--Remove me October 2026-->

>[!IMPORTANT]
>
>O procedimento descrito nesta página foi aplicado apenas a organizações que ainda não foram integradas ao Admin Console. Como todas as organizações foram integradas à Adobe Admin Console, **não é possível alterar seu domínio do Workfront**.
>
>Para obter uma lista de procedimentos que diferem com base no fato de sua organização ter sido integrada à Adobe Admin Console, consulte [Diferenças de administração entre a Adobe Workfront e a Adobe Business Platform](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).
>
>Este artigo será removido em breve.

Como administrador da Adobe Workfront e contato autorizado com o Suporte da Workfront, você pode solicitar ajuda da equipe de Suporte da Workfront para alterar o domínio do Workfront de sua organização.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacote do Adobe Workfront</td> 
   <td><p>Qualquer</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td><p>Padrão</p><p>Plano</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Você deve ser um administrador do Workfront.</p> </p> </td> 
  </tr> 
 </tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Solicitar uma alteração de domínio

1. Comece a criar um tíquete de suporte no Experience League.
1. Na caixa **Descrição**, inclua o novo domínio desejado, bem como o período em que deseja ativar o novo domínio.
1. Termine de preencher as caixas do caso de suporte e clique em **Enviar**.

Você também pode ligar para o Suporte da Workfront para obter ajuda sobre como alterar seu domínio.

<!--

## Update the new domain if you are an SSO customer

If your company utilizes SSO, the following steps are required after you have your Workfront domain changed.

>[!NOTE]
>
>This is not available if your organization's Workfront instance is enabled with Adobe IMS. See your network or IT administrator if you need more information.

{{step-1-to-setup}}

1. In the left sidebar, click **System** > **Customer Info** and make sure that your domain is updated on the Customer Info page.

1. In the left sidebar, click **System** > **Single Sign-On (SSO)**.

1. Click **Download SAML 2.0 Metadata**.
1. After the file is downloaded, open it and make sure of the following:

   1. **entityID** is pointing to the new domain.
   1. All locations within **`<md:AssertionConsumerService>`** point to the new domain.

1. Provide the downloaded metadata file to your Identity Provider so that they can update it on their end.
1. Make sure the domain is updated for all Workfront integrations used by your organization.


-->
