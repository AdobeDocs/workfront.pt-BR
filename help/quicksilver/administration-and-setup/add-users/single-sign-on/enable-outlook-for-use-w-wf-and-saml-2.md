---
user-type: administrator
product-area: system-administration
navigation-topic: single-sign-on-in-workfront
title: Ativar o Outlook para uso com Workfront e SAML 2.0
description: Se você habilitar a autenticação SAML 2.0 e quiser que seus usuários possam fazer logon no Workfront a partir do Microsoft Outlook usando suas credenciais SAML 2.0, será necessário habilitar o SAML 2.0 para autenticar em suplementos do Office.
author: Caroline, Becky
feature: System Setup and Administration
role: Admin
exl-id: 8a55d364-962a-4eef-8968-b2233a71cf31
source-git-commit: 02191d80ea58f80de2e7be2ff55f43663e415e31
workflow-type: tm+mt
source-wordcount: '294'
ht-degree: 1%

---

# Ativar o Outlook para uso com Workfront e SAML 2.0

Se você habilitar a autenticação SAML 2.0 e quiser que seus usuários possam fazer logon no Workfront a partir do Microsoft Outlook usando suas credenciais SAML 2.0, será necessário habilitar o SAML 2.0 para autenticar em suplementos do Office.

>[!NOTE]
>
>Isso não está disponível se a instância do Workfront de sua organização usar um portal SSO personalizado.>
><!--
>or is enabled with Adobe IMS>
>-->
>Consulte seu administrador de rede ou de TI se precisar de mais informações.

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plano Adobe Workfront</td> 
   <td>Qualquer Um</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença Adobe Workfront</td> 
   <td>Plano</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Você deve ser um administrador do Workfront.</p> <p><b>OBSERVAÇÃO</b>: Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Ativar o Outlook para uso com Workfront e SAML 2.0

1. Clique em **Configuração** próximo ao canto superior direito do Adobe Workfront na Barra de navegação global.
1. Clique em **Sistema** > **Preferências**.

1. No **Segurança** seção , verifique se **Permitir autenticação SAML 2.0 em suplementos do Office 365** estiver ativado.

   Essa opção permite a incorporação do Workfront em um Iframe somente para suplementos do Office 365. Isso não abre uma falha de click-jacking, pois não há conteúdo clicável envolvido.

   Essa opção é ativada por padrão.

   >[!NOTE]
   >
   >Se você ativar a opção **Permitir incorporação de Workfront em um iframe**, a opção **Permitir autenticação SAML 2.0 em suplementos do Office 365** está esmaecida e ativada.
   >
   >![](assets/if-you-enable.png)

1. Clique em **Salvar**.

   As alterações salvas aqui afetam a experiência de todos os usuários no Workfront.
