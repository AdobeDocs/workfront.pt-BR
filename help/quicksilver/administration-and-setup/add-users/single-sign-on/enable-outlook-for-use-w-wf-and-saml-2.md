---
user-type: administrator
product-area: system-administration
navigation-topic: single-sign-on-in-workfront
title: Habilitar o Outlook para uso com Workfront e SAML 2.0
description: Se você habilitar a autenticação SAML 2.0 e quiser que os usuários façam logon no Workfront a partir do Microsoft Outlook usando suas credenciais do SAML 2.0, será necessário habilitar o SAML 2.0 para autenticar em suplementos do Office.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 8a55d364-962a-4eef-8968-b2233a71cf31
source-git-commit: af54faae1e78d7ffbe679fd82dfb5a3abd45f5cf
workflow-type: tm+mt
source-wordcount: '419'
ht-degree: 0%

---

# Habilitar o Outlook para uso com Workfront e SAML 2.0

>[!IMPORTANT]
>
>[O Microsoft está desabilitando o suporte para tokens herdados do Exchange online](https://learn.microsoft.com/en-us/office/dev/add-ins/outlook/faq-nested-app-auth-outlook-legacy-tokens), que são usados atualmente pelo suplemento do Workfront Outlook para autenticação. Essa alteração pela Microsoft já começou a afetar os clientes e continuará a ser implementada em fases até outubro de 2025.
>
>* **Depois que o Microsoft desabilitar totalmente esses tokens, a integração do Workfront para Microsoft Outlook não funcionará mais.**
>
>Como parte dessa alteração, a Microsoft tomou a decisão de alterar a maneira como os tokens são reativados. Após **30 de junho de 2025**, os administradores não poderão mais reabilitar tokens, somente o Suporte da Microsoft poderá conceder exceções. **Em 1º de outubro de 2025, os tokens herdados serão desativados para todos os locatários. Exceções não serão concedidas.**

Se você habilitar a autenticação SAML 2.0 e quiser que os usuários façam logon no Workfront a partir do Microsoft Outlook usando suas credenciais do SAML 2.0, será necessário habilitar o SAML 2.0 para autenticar em suplementos do Office.

>[!NOTE]
>
>Isso não estará disponível se a instância Workfront da sua organização usar um portal SSO personalizado.>
><!--
>or is enabled with Adobe IMS>
>-->
>Consulte o administrador de rede ou de TI se precisar de mais informações.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront</td> 
   <td>Qualquer</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td>Plano</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Você deve ser um administrador do Workfront.</p> <p><b>OBSERVAÇÃO</b>: se você ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais no seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## Habilitar o Outlook para uso com Workfront e SAML 2.0

{{step-1-to-setup}}

1. Clique em **Sistema** > **Preferências**.

1. Na seção **Segurança**, verifique se **Permitir autenticação SAML 2.0 nos suplementos do Office 365** está habilitado.

   Essa opção habilita a incorporação do Workfront em um Iframe somente para suplementos do Office 365. Isso não abre uma violação de clickjacking, pois não há nenhum conteúdo clicável envolvido.

   Essa opção está ativada por padrão.

   >[!NOTE]
   >
   >Se você habilitar a opção **Permitir incorporação do Workfront em um iframe**, a opção **Permitir autenticação SAML 2.0 nos suplementos do Office 365** ficará esmaecida e habilitada.
   >
   >![Permitir opção de incorporação](assets/if-you-enable.png)
   >

1. Clique em **Salvar**.

   As alterações salvas aqui afetam a experiência de todos os usuários no Workfront.
