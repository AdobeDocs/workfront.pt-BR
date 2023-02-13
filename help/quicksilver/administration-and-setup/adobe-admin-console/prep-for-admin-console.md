---
filename: prep-for-admin-console
user-type: administrator
content-type: reference
product-area: system-administration;workfront-integrations
navigation-topic: adobe-admin-console
title: Preparar-se para integrar sua organização à Adobe Admin Console
description: Como o Adobe Workfront é um produto Adobe, você pode acessá-lo por meio da Adobe Admin Console. Isso permite gerenciar o Workfront junto com outras contas e produtos do Adobe para seus usuários em um local central.
author: Becky, Caroline
feature: System Setup and Administration
role: Admin
exl-id: d9b5e4a1-069e-48be-80d0-84f4bf8aea8b
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '671'
ht-degree: 0%

---

# Preparar-se para integrar sua organização à Adobe Admin Console

Como o Adobe Workfront é um produto Adobe, você pode acessá-lo por meio da Adobe Admin Console. Isso permite gerenciar o Workfront junto com outras contas e produtos do Adobe para seus usuários em um local central.

Todos os clientes do Workfront serão transferidos para a Adobe Admin Console. Depois que sua organização muda para a Adobe Admin Console, a autenticação da Workfront é gerenciada pela Adobe Admin Console. Preparar e fazer essa mudança mais cedo estabelece as bases para a eficiência no gerenciamento do trabalho e posiciona sua organização para uma inovação mais rápida no futuro

Para obter uma visão geral da Adobe Admin Console, consulte [Visão geral do Admin Console](https://helpx.adobe.com/br/enterprise/using/admin-console.html).

## Lista de verificação da migração

Para garantir que sua organização possa migrar para a Adobe Admin Console, você deve executar as seguintes ações

1. Identifique a Adobe Admin Console desejada onde deseja adicionar o Workfront.

   * Se sua organização não tiver uma Adobe Admin Console existente ou se você não quiser usar uma Adobe Admin Console existente, o Suporte da Workfront pode ajudá-lo a criar uma nova.

   * Se você tiver vários Adobe e não tiver certeza de qual é mais apropriado adicionar o Adobe Workfront, entre em contato com o Suporte da Workfront.

1. Confirme com o Suporte da Workfront se deseja usar uma Adobe Admin Console existente ou crie uma nova.

1. Configure o gerenciamento de identidade na Adobe Admin Console.

   >[!IMPORTANT]
   >
   >Esteja preparado para falar com o Suporte da Workfront e sua equipe de TI sobre as preferências de autenticação, como Logon único (SSO) ou não-SSO.

   Para obter instruções, consulte a seção Identity Management do Guia de implantação do Adobe Admin Console (https://helpx.adobe.com/enterprise/using/deployment-planning.html).

1. (Condicional) Se estiver usando o Logon único, conecte o novo Adobe Admin Console ao seu provedor SSO existente

   Para obter mais informações e instruções, consulte [Configurar identidade](https://helpx.adobe.com/enterprise/using/set-up-identity.html).

   >[!NOTE]
   >
   >Se sua organização não usar o Logon único, qualquer usuário migrado para a Adobe Admin Console receberá um email para criar sua conta e senha.

1. Certifique-se de que os endereços de email de usuário estejam prontos para migração:

   1. Remover emails duplicados do Workfront

      Para obter instruções, consulte Atualizar endereços de email de usuários existentes na instância do Workfront em Impedir usuários duplicados.

      Se houver um endereço de email duplicado em sua organização, o usuário representado pelo endereço de email com o `lastLoginDate` será movida para a organização da Adobe Admin Console. Quaisquer outros usuários com esse endereço de email serão desativados.

      >[!NOTE]
      >
      >Como apenas um usuário com um determinado endereço de email pode estar ativo em um determinado momento, se você precisar ativar outro usuário com o mesmo endereço de email de um usuário ativo no momento, primeiro deverá desativar o usuário ativo no momento antes de ativar o usuário desativado.

   2. (Condicional) Se estiver utilizando integrações de API personalizadas, confirme se os usuários têm um endereço de email válido que podem acessar.

   3. (Opcional) Recomendamos desativar os usuários que não precisam mais acessar o Workfront, para que não sejam adicionados à Adobe Admin Console.
   >[!IMPORTANT]
   >
   >Essas ações relacionadas aos emails do usuário devem ser concluídas antes que a organização comece a migrar para a Adobe Admin Console.

1. (Opcional) Atualize todas as integrações personalizadas para usar o OAuth2.

   Para obter instruções sobre como configurar integrações OAuth2, consulte [Criar aplicativos OAuth2 para integrações do Workfront](../../administration-and-setup/configure-integrations/create-oauth-application.md).

   A criação de integrações OAuth2 só está disponível na nova experiência do Workfront.

   >[!NOTE]
   >
   >Essa etapa é opcional, mas altamente recomendado, pois outras formas de autenticação e autorização da API serão substituídas no futuro.

Depois que a Adobe Admin Console for configurada com o Workfront, você poderá usá-la para gerenciar os usuários.

Para obter mais informações, consulte [Gerenciar usuários no Adobe Admin Console](../../administration-and-setup/add-users/create-and-manage-users/admin-console.md).

Para obter uma lista de outras ações diferentes com base no fato de sua organização ter sido integrada à Adobe Admin Console, consulte [Diferenças de administração baseadas em plataforma (Adobe Workfront/Adobe Business Platform)](../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).
