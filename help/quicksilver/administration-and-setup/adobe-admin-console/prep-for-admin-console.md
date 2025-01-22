---
filename: prep-for-admin-console
user-type: administrator
content-type: reference
product-area: system-administration;workfront-integrations
navigation-topic: adobe-admin-console
title: Prepare-se para integrar sua organização à Adobe Admin Console
description: Como o Adobe Workfront é um produto Adobe, você pode acessá-lo pelo Adobe Admin Console. Isso permite gerenciar o Workfront juntamente com outras contas e produtos Adobe para seus usuários em um local central.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: d9b5e4a1-069e-48be-80d0-84f4bf8aea8b
source-git-commit: eb68357ed4fd8f323707aa4a54a0f946253bf4e0
workflow-type: tm+mt
source-wordcount: '647'
ht-degree: 0%

---

# Prepare-se para integrar sua organização à Adobe Admin Console

<!-- Audited: 12/2023 -->

Como o Adobe Workfront é um produto Adobe, você pode acessá-lo pelo Adobe Admin Console. Isso permite gerenciar o Workfront juntamente com outras contas e produtos Adobe para seus usuários em um local central.

Todos os clientes do Workfront serão transferidos para o Adobe Admin Console. Depois que sua organização muda para a Adobe Admin Console, a autenticação da Workfront é gerenciada pelo Console. Preparar e fazer essa mudança mais rápido estabelece a base para a eficiência no gerenciamento de trabalho e posiciona sua organização para uma inovação mais rápida no futuro

Para obter uma visão geral do Adobe Admin Console, consulte [Visão geral do Admin Console](https://helpx.adobe.com/br/enterprise/using/admin-console.html).

## Lista de verificação de migração

Para garantir que sua organização possa migrar para a Adobe Admin Console, você deve executar as seguintes ações.

1. Identifique a Adobe Admin Console desejada à qual você deseja adicionar o Workfront.

   * Se sua organização não tiver uma Adobe Admin Console existente ou se você não quiser usar uma Adobe Admin Console existente, o Suporte da Workfront poderá ajudá-lo a criar uma nova.

   * Se você tiver vários Admin Console Adobe e não tiver certeza de qual deles é o mais apropriado para adicionar o Workfront, entre em contato com o Suporte da Workfront.

1. Confirme com o Suporte da Workfront se deseja usar um Adobe Admin Console existente ou criar um novo.

1. Configure o gerenciamento de identidades no Adobe Admin Console.

   >[!IMPORTANT]
   >
   >Esteja preparado para falar com o Suporte da Workfront e sua equipe de TI sobre preferências de autenticação, como logon único (SSO) ou não-SSO.

   Para obter instruções, consulte a seção Identity Management do [Guia de Implantação do Adobe Admin Console](https://helpx.adobe.com/enterprise/using/deployment-planning.html).

1. (Condicional) Se estiver usando o Logon único, conecte a nova Adobe Admin Console ao seu provedor SSO existente.

   Para obter mais informações e instruções, consulte [Configurar identidade](https://helpx.adobe.com/enterprise/using/set-up-identity.html).

   >[!NOTE]
   >
   >Se sua organização não usar Logon único, os usuários migrados para a Adobe Admin Console receberão um email para criar sua conta e senha.

1. Verifique se os endereços de email do usuário estão prontos para migração:

   1. Remova emails duplicados do Workfront.

      Para obter instruções, consulte [Atualizar endereços de email de usuários existentes na instância do Workfront](/help/quicksilver/administration-and-setup/manage-workfront/security/prevent-duplicate-users.md#update-email-addresses-of-existing-users-in-your-workfront-instance) em [Impedir usuários duplicados](/help/quicksilver/administration-and-setup/manage-workfront/security/prevent-duplicate-users.md).

      Se houver endereços de email duplicados em sua organização, o usuário representado pelo endereço de email com o `lastLoginDate` mais recente será movido para a organização da Adobe Admin Console. Qualquer outro usuário com esse endereço de email será desativado.

      >[!NOTE]
      >
      >Como apenas um usuário com determinado endereço de email pode estar ativo em um determinado momento, se você precisar ativar outro usuário com o mesmo endereço de email que um usuário ativo no momento, será necessário desativar o usuário ativo no momento antes de ativar o usuário desativado.

   1. (Condicional) Se estiver utilizando integrações de API personalizadas, confirme se esses usuários têm um endereço de email válido que podem acessar.

   1. (Opcional) Recomendamos desativar todos os usuários que não precisam mais acessar o Workfront para que não sejam adicionados ao Adobe Admin Console.

   >[!IMPORTANT]
   >
   >Essas ações relacionadas aos emails do usuário devem ser concluídas antes que sua organização comece a migrar para o Adobe Admin Console.

1. (Opcional) Atualize todas as integrações personalizadas para usar o OAuth2.

   Para obter instruções sobre como configurar integrações OAuth2, consulte [Criar aplicativos OAuth2 para integrações do Workfront](../../administration-and-setup/configure-integrations/create-oauth-application.md).

   >[!NOTE]
   >
   >Essa etapa é opcional, mas altamente recomendada, pois outras formas de autenticação e autorização de API serão descontinuadas no futuro.

Depois que o Adobe Admin Console for configurado com o Workfront, você poderá usá-lo para criar administradores de sistema do Workfront.

Para obter mais informações, consulte [Gerenciar usuários na Adobe Admin Console](../../administration-and-setup/add-users/create-and-manage-users/admin-console.md).

Para obter uma lista de outras ações diferentes com base no fato de sua organização ter sido integrada à Adobe Admin Console, consulte [Diferenças de administração baseadas em plataforma (Adobe Workfront/Adobe Business Platform)](../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).
