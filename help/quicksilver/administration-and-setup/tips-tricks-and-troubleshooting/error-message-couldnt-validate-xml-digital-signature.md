---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: "Mensagem de erro: Não foi possível validar a assinatura digital XML"
description: Não é possível estabelecer uma conexão bem-sucedida com o ADFS.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: d30a67dd-4f91-41cf-b1ba-fefadc4e396a
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '304'
ht-degree: 0%

---

# Mensagem de erro: Não foi possível validar a assinatura digital XML

## Problema

Não é possível estabelecer uma conexão bem-sucedida com o ADFS.

![error_message.png](assets/error-message.png)

>[!NOTE]
>
>Se você estabelecer uma conexão de teste bem-sucedida e ainda tiver problemas, poderá ter mapeamentos de atributo incorretos ou problemas com as IDs de federação. Entre em contato com o suporte ao cliente com perguntas.

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plano</td> 
   <td>Qualquer Um</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licença</td> 
   <td>Plano</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Você deve ser um [!DNL Workfront] administrador. Para obter mais informações, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder ao usuário acesso administrativo total</a>.</p> <p><b>OBSERVAÇÃO</b>: Se ainda não tiver acesso, pergunte ao seu [!DNL Workfront] administrador se eles definirem restrições adicionais em seu nível de acesso. Para obter informações sobre como uma [!DNL Workfront] administrador pode modificar seu nível de acesso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Causa 1: O certificado está incorreto

### Solução

Recuperar manualmente o Certificado de Assinatura do Servidor ADFS:

1. Em [!DNL Windows], clique em **[!UICONTROL Iniciar]** > **[!UICONTROL Administração]** > **[!UICONTROL Gerenciamento ADFS 2.0]**.\
   A caixa de diálogo Gerenciamento do ADFS 2.0 é exibida.

1. Selecionar **[!UICONTROL Relação de Confiança]** > **[!UICONTROL Confianças de terceiros confiáveis]** no painel esquerdo.

1. Clique com o botão direito do mouse em **[!UICONTROL Confiança da Entidade Confiadora]** e selecione **[!UICONTROL Propriedades]**.

1. Clique no botão **[!UICONTROL Assinatura]** guia .
1. Clique no nome do Certificado de assinatura e clique em **[!UICONTROL Exibir]**.
1. Clique em Copiar para **[!UICONTROL Arquivo]**... e selecione **[!UICONTROL Próximo]**.

1. Selecionar **[!UICONTROL Codificado base 64 x.509 (CER)]** e clique em **[!UICONTROL Próximo]**.

1. Especifique o nome do arquivo e clique em **[!UICONTROL Próximo]**.
1. Clique em **[!UICONTROL Concluir]**.
1. Em [!DNL Adobe Workfront], navegue até **[!UICONTROL Configuração]** > **[!UICONTROL Sistema]** > **[!UICONTROL Logon único (SSO)]** e fazer upload manual do Certificado de assinatura.

## Causa 2: O certificado é assinado usando DSA quando [!DNL Workfront] está esperando uma assinatura RSA

### Solução

Recrie o certificado e use a assinatura RSA em vez do DSA.

## Causa 3: Dados XML incorretos

### Solução

Reexporte e importe os metadados XML do sistema de gerenciamento ADFS.

## Causa 4: Não foi possível executar a solicitação devido a um erro no lado do SAML

### Solução

Entre em contato com seu provedor SAML.
