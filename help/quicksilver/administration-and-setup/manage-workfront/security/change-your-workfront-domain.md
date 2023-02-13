---
user-type: administrator
product-area: system-administration
navigation-topic: security
title: Alterar o domínio do Adobe Workfront
description: Como administrador da Adobe Workfront e um contato autorizado do Suporte da Workfront, você pode solicitar ajuda da equipe de Suporte da Workfront para alterar o domínio Workfront de sua organização.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: d817bd2b-1aaa-4dde-8e75-392c1da2943a
source-git-commit: b413ffc2416439629e073b32b5e9828df2f5de90
workflow-type: tm+mt
source-wordcount: '459'
ht-degree: 0%

---

# Alterar o domínio do Adobe Workfront

>[!IMPORTANT]
>
>O procedimento descrito nesta página se aplica somente a organizações que ainda não foram integradas ao Admin Console. Se sua organização tiver sido integrada à Adobe Admin Console, você deverá executar essa ação por meio da Adobe Admin Console.
>
>Para alterar o domínio da Adobe Workfront se a organização tiver sido integrada à Adobe Admin Console, consulte [Configurar domínios](https://helpx.adobe.com/enterprise/using/set-up-identity.html#setup-domains).
>
>Para obter uma lista de procedimentos diferentes com base no fato de sua organização ter sido integrada à Adobe Admin Console, consulte [Diferenças de administração baseadas em plataforma (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

Como administrador da Adobe Workfront e um contato autorizado do Suporte da Workfront, você pode solicitar ajuda da equipe de Suporte da Workfront para alterar o domínio Workfront de sua organização.

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

## Solicitar uma alteração de domínio

1. Clique no botão **Suporte** na página Workfront One e comece a criar um caso de suporte.
1. No **Descrição** , inclua o novo domínio desejado, bem como o período em que deseja que o novo domínio seja ativado.
1. Termine de preencher as caixas do caso de suporte e clique em **Enviar**.

Você também pode chamar o Suporte da Workfront para obter ajuda para alterar seu domínio.

## Atualize o novo domínio se você for um cliente SSO

Se sua empresa utiliza SSO, as etapas a seguir são necessárias após alterar o domínio do Workfront.

>[!NOTE]
>
>Isso não estará disponível se a instância do Workfront de sua organização estiver habilitada com o Adobe IMS. Consulte seu administrador de rede ou de TI se precisar de mais informações.

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront, em seguida, clique em **Configuração** ![](assets/gear-icon-settings.png).

1. Na barra lateral esquerda, clique em **Sistema** > **Informações do cliente** e certifique-se de que seu domínio seja atualizado na página Informações do cliente .

1. Na barra lateral esquerda, clique em **Sistema** > **Logon único (SSO)**.

1. Clique em **Baixar metadados do SAML 2.0**.
1. Após o download do arquivo, abra-o e verifique o seguinte:

   1. **entityID** O está apontando para o novo domínio.
   1. Todos os locais dentro de **`<md:AssertionConsumerService>`** aponte para o novo domínio.

1. Forneça o arquivo de metadados baixado ao seu Provedor de identidade para que ele possa atualizá-lo da extremidade.
1. Certifique-se de que o domínio seja atualizado para todas as integrações do Workfront usadas por sua organização.
