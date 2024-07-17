---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: "Mensagem de erro: não foi possível validar a assinatura digital XML"
description: Você não pode estabelecer uma conexão bem-sucedida com o ADFS.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: d30a67dd-4f91-41cf-b1ba-fefadc4e396a
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '310'
ht-degree: 1%

---

# Mensagem de erro: não foi possível validar a assinatura digital XML

## Problema

Você não pode estabelecer uma conexão bem-sucedida com o ADFS.

![mensagem_de_erro.png](assets/error-message.png)

>[!NOTE]
>
>Se você estabelecer uma conexão de teste bem-sucedida e ainda estiver com problemas, poderá ter mapeamentos de atributos incorretos ou problemas com as IDs da federação. Entre em contato com o suporte ao cliente se tiver dúvidas.

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plano</td> 
   <td>Qualquer</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licença</td> 
   <td>Plano</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Você deve ser um administrador [!DNL Workfront]. Para obter mais informações, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder a um usuário acesso administrativo total</a>.</p> <p><b>OBSERVAÇÃO</b>: se você ainda não tiver acesso, pergunte ao administrador do [!DNL Workfront] se ele definiu restrições adicionais no seu nível de acesso. Para obter informações sobre como um administrador do [!DNL Workfront] pode modificar seu nível de acesso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Causa 1: certificado incorreto

### Solução

Recuperar manualmente o Certificado de Autenticação do Servidor ADFS:

1. Em [!DNL Windows], clique em **[!UICONTROL Iniciar]** > **[!UICONTROL Administração]** > **[!UICONTROL Gerenciamento do ADFS 2.0]**.\
   A caixa de diálogo Gerenciamento do ADFS 2.0 é exibida.

1. Selecione **[!UICONTROL Relação de Confiança]** > **[!UICONTROL Relações de Confiança de Terceira Parte Confiável]** no painel esquerdo.

1. Clique com o botão direito do mouse em **[!UICONTROL Terceira Parte Confiável]** e selecione **[!UICONTROL Propriedades]**.

1. Clique na guia **[!UICONTROL Assinatura]**.
1. Clique no nome do Certificado de Autenticação e clique em **[!UICONTROL Exibir]**.
1. Clique em Copiar para **[!UICONTROL Arquivo]**... e selecione **[!UICONTROL Avançar]**.

1. Selecione **[!UICONTROL X.509 (CER) codificado na Base 64]** e clique em **[!UICONTROL Avançar]**.

1. Especifique o nome do arquivo e clique em **[!UICONTROL Avançar]**.
1. Clique em **[!UICONTROL Concluir]**.
1. Em [!DNL Adobe Workfront], navegue até **[!UICONTROL Configuração]** > **[!UICONTROL Sistema]** > **[!UICONTROL Logon Único (SSO)]** e carregue manualmente o Certificado de Autenticação.

## Causa 2: o certificado é assinado usando DSA quando [!DNL Workfront] está esperando uma assinatura RSA

### Solução

Recrie o certificado e use a assinatura RSA em vez do DSA.

## Causa 3: dados XML incorretos

### Solução

Reexportar e reimportar os metadados XML do sistema de gerenciamento ADFS.

## Causa 4: a solicitação não pôde ser executada devido a um erro no SAML

### Solução

Entre em contato com o provedor SAML.
