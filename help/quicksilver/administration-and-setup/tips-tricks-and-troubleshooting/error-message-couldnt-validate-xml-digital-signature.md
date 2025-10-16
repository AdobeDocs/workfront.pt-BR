---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 'Mensagem de erro: Não foi possível validar a assinatura digital XML'
description: Você não pode estabelecer uma conexão bem-sucedida com o ADFS.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: d30a67dd-4f91-41cf-b1ba-fefadc4e396a
source-git-commit: 929502c256011b464d938ad1095c127407e4a795
workflow-type: tm+mt
source-wordcount: '268'
ht-degree: 2%

---

# Mensagem de erro: não foi possível validar a assinatura digital XML

## Problema

Você não pode estabelecer uma conexão bem-sucedida com o ADFS.

![mensagem_de_erro.png](assets/error-message.png)

>[!NOTE]
>
>Se você estabelecer uma conexão de teste bem-sucedida e ainda estiver com problemas, poderá ter mapeamentos de atributos incorretos ou problemas com as IDs da federação. Entre em contato com o suporte ao cliente se tiver dúvidas.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] pacote</td> 
   <td><p>Qualquer</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] licença</td> 
   <td><p>Standard</p>
       <p>Plano</p></td>
  </tr> 
  <tr> 
   <td>Configurações de nível de acesso</td> 
   <td>[!UICONTROL Administrador do Sistema]</td> 
  </tr> 
 </tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

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
