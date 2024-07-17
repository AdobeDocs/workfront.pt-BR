---
content-type: tips-tricks-troubleshooting
product-previous: mobile
navigation-topic: tips-tricks-and-troubleshooting-mobile-apps
title: "Mensagem de Erro no  [!DNL Adobe Workfront] Aplicativo Móvel: 'Sua conta não está habilitada para API'."
description: "Mensagem de Erro no  [!DNL Adobe Workfront] Aplicativo Móvel: 'Sua conta não está habilitada para API'."
author: Lisa
feature: Get Started with Workfront
exl-id: 120e56f4-9fd5-4c41-890e-981937714db0
source-git-commit: fdef22d9685d349a6f9492dec98475493ee9c048
workflow-type: tm+mt
source-wordcount: '168'
ht-degree: 2%

---

# Mensagem de erro no aplicativo móvel [!DNL Adobe Workfront]: &quot;[!UICONTROL A API da sua conta não está habilitada.]&quot;

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] plano</strong></td> 
   <td> <p> Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>licença do Adobe [!DNL Workfront]</strong></td> 
   <td> <p>Plano</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurações de nível de acesso</strong></td> 
   <td> <p>[!UICONTROL Administrador do sistema] </p> </td> 
  </tr> 
 </tbody> 
</table>

## Problema

Ao tentar fazer logon no aplicativo móvel [!DNL Adobe Workfront], você recebe o seguinte erro: *[!UICONTROL Sua conta não tem a API habilitada. Informe o administrador do sistema e ele fará com que você seja configurado. Desculpe por isso.]*

## Causa

O administrador do [!DNL Workfront] não habilitou o ambiente [!DNL Workfront] para ser acessado de um dispositivo móvel.

## Solução

1. Faça logon no aplicativo Web [!DNL Workfront] como Administrador [!DNL Workfront].
1. Vá para a área **[!UICONTROL Configuração]**.
1. Expanda o menu **[!UICONTROL Sistema]** e clique em **[!UICONTROL Preferências]**.

1. Na seção **[!UICONTROL Segurança]**, selecione a opção **[!UICONTROL Permitir que as pessoas usem os aplicativos móveis de [!DNL Workfront] e o Suplemento [!DNL Workfront Outlook]]** para habilitá-lo.

1. Clique em **[!UICONTROL Salvar]**.\
   Todos os usuários no sistema agora podem acessar o [!DNL Workfront] por meio de seus aplicativos móveis e do [!DNL Outlook].
