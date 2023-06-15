---
user-type: administrator
product-area: system-administration
navigation-topic: security
title: Alterar o domínio do Adobe Workfront
description: Como administrador da Adobe Workfront e contato autorizado com o Suporte da Workfront, você pode solicitar ajuda da equipe de Suporte da Workfront para alterar o domínio do Workfront de sua organização.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: d817bd2b-1aaa-4dde-8e75-392c1da2943a
source-git-commit: b9e088a0cdb32f3e8c565ea17f4613dda104bd7b
workflow-type: tm+mt
source-wordcount: '431'
ht-degree: 0%

---

# Alterar o domínio do Adobe Workfront

>[!IMPORTANT]
>
>O procedimento descrito nesta página se aplica apenas a organizações que ainda não foram integradas ao Admin Console. Se sua organização tiver sido integrada à Adobe Admin Console, não será possível alterar o domínio do Workfront.
>
>Para obter uma lista de procedimentos que diferem dependendo de sua organização ter sido integrada à Adobe Admin Console, consulte [Diferenças de administração baseadas em plataforma (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

Como administrador da Adobe Workfront e contato autorizado com o Suporte da Workfront, você pode solicitar ajuda da equipe de Suporte da Workfront para alterar o domínio do Workfront de sua organização.

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront</td> 
   <td>Qualquer Um</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td>Plano</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Você deve ser um administrador do Workfront.</p> <p><b>NOTA</b>: se você ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Solicitar uma alteração de domínio

1. Clique em **Suporte** na página Workfront One e comece a criar um caso de suporte.
1. No **Descrição** inclua o novo domínio desejado, bem como o período em que deseja ativar o novo domínio.
1. Termine de preencher as caixas do caso de suporte e clique em **Enviar**.

Você também pode ligar para o Suporte da Workfront para obter ajuda sobre como alterar seu domínio.

## Atualize o novo domínio se você for um cliente de SSO

Se sua empresa utiliza SSO, as seguintes etapas serão necessárias depois que você alterar o domínio do Workfront.

>[!NOTE]
>
>Isso não estará disponível se a instância Workfront da sua organização estiver habilitada com o Adobe IMS. Consulte o administrador de rede ou de TI se precisar de mais informações.

1. Clique em **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront e clique em **Configuração** ![](assets/gear-icon-settings.png).

1. Na barra lateral esquerda, clique em **Sistema** > **Informações do cliente** e certifique-se de que seu domínio esteja atualizado na página Informações do cliente.

1. Na barra lateral esquerda, clique em **Sistema** > **Logon único (SSO)**.

1. Clique em **Baixar os Metadados do SAML 2.0**.
1. Depois que o arquivo for baixado, abra-o e verifique o seguinte:

   1. **entityID** O está apontando para o novo domínio.
   1. Todos os locais dentro de **`<md:AssertionConsumerService>`** aponte para o novo domínio.

1. Forneça o arquivo de metadados baixado ao seu provedor de identidade para que ele possa atualizá-lo.
1. Verifique se o domínio está atualizado para todas as integrações da Workfront usadas pela sua organização.
