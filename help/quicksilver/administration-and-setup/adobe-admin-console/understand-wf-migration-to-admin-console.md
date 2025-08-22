---
user-type: Admin
content-type: reference
product-area: system-administration;workfront-integrations
navigation-topic: adobe-admin-console
title: Noções básicas sobre a migração do Workfront para o Adobe Admin Console
description: Este artigo descreve em termos gerais o processo de mover uma organização para a Adobe Admin Console, para que você, como administrador do Workfront, possa saber o que esperar.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 54d855e6-c387-458c-9cd3-f32318c8ae02
source-git-commit: c71c5c4a545f9256ecce123ae3513d01a7251ad7
workflow-type: tm+mt
source-wordcount: '1135'
ht-degree: 0%

---

# Noções básicas sobre a migração do Workfront para o Adobe Admin Console

<!--DELETE ME MARCH 2026-->

>[!IMPORTANT]
>
>Todas as organizações da Workfront foram integradas à Adobe Admin Console.
>
>Este artigo será removido em breve.

A Adobe está mudando a forma como você gerencia os usuários da Adobe Workfront, aumentando a produtividade para você e para a sua organização. Como parte dessa alteração, a Adobe está migrando sua instância do Workfront e seus usuários para a Adobe Admin Console. Essa é uma migração necessária e não afetará nenhum relatório, caminho de aprovação, conteúdo ou ativo. Isso afetará a maneira como você gerencia o acesso dos usuários e como eles fazem logon.

Este artigo descreve em termos gerais o processo de mover uma organização para a Adobe Admin Console, para que você, como administrador do Workfront, possa saber o que esperar.

Para saber como você pode usar o Adobe Admin Console para gerenciar seus direitos da Adobe em toda a organização, consulte [Gerenciar usuários na Adobe Admin Console](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/admin-console.md).

## O que está mudando?

Como parte da migração, seu gerenciamento de usuários passará do aplicativo do Workfront para o Adobe Admin Console com as seguintes funções administrativas:

* **Administradores do sistema** são superusuários com privilégios de todos os administradores. Eles atribuem todas as funções administrativas e gerenciam usuários para toda a organização para todos os produtos.

* **Os administradores de Perfil de Produto (administradores de sistema do Workfront)** gerenciam quais usuários da organização têm acesso ao Workfront.

* **Os usuários entrarão com a Adobe Identity.** Depois que o Adobe migrar os usuários existentes para o Adobe Admin Console, os usuários entrarão em suas instâncias do Workfront usando sua nova Identidade do Adobe - uma Adobe ID ou Adobe Federated ID (SSO).

* **Não há alteração na forma como você gerencia todas as outras funcionalidades** no próprio aplicativo do Workfront, incluindo o gerenciamento de recursos, funções de usuário, espaços de trabalho, funcionalidade e comportamento.

## Cronograma da Jornada de migração

Primeiro, o Adobe migrará sua instância do Workfront para o Adobe Admin Console e, em seguida, migrará todos os usuários existentes com endereços de email verificados. Se você for um administrador do sistema ou um administrador do Perfil de produto do Workfront (administrador do Workfront System), receberá emails orientando você durante a jornada de migração. Esta é uma linha do tempo do que você pode esperar:

### Migração do Workfront para o Adobe Admin Console concluída

Os administradores de sistema receberão um email quando a migração do Workfront para o Adobe Admin Console for concluída. No momento, talvez os administradores do sistema precisem concluir algumas etapas necessárias **antes de iniciar a migração do usuário**, para minimizar o impacto para os usuários do Workfront.

* **Se seus usuários do Workfront fizerem logon com SSO**, você deverá configurar o SSO no Adobe Admin Console para que seus usuários possam continuar a fazer logon com SSO. Se os usuários do Workfront não usarem o SSO no momento, mas você quiser configurá-lo no Adobe Admin Console, faça isso neste ponto da jornada de migração.
* **Se você já gerencia outros produtos da Adobe na sua Adobe Admin Console**, a Adobe poderá solicitar o seu consentimento para migrar automaticamente os usuários para o seu console existente. Clique no botão **Introdução** no email para navegar até a página de consentimento.
* **Se você tiver excluído o tipo de licença Solicitante** anteriormente, ele será adicionado ao sistema. Nenhum usuário será atribuído a esse tipo de licença, mas ele é necessário para a sincronização entre o Workfront e a Adobe Admin Console. Nenhuma ação é necessária em relação ao tipo de licença Solicitante.

Não há alterações no gerenciamento de usuários no momento. Os administradores do Workfront continuarão a gerenciar usuários no Workfront e os usuários continuarão a fazer logon com sua Workfront ID ou SSO até que a migração de usuários seja concluída.

### Agendar migração de usuário

Depois que o administrador do sistema concluir os pré-requisitos descritos na seção anterior, a Adobe agendará automaticamente a migração do usuário por 30 dias após a conclusão desses pré-requisitos e se comunicará com os administradores do Perfil de produto da Workfront (administradores do Workfront System) para gerenciar a migração do usuário.

Os administradores de Perfil de produto do Workfront (administradores do Workfront System) irão:

* Receba um e-mail com a data agendada de início da migração de usuários (cerca de 30 dias após a conclusão desses pré-requisitos)
* Obter acesso ao console do administrador designado do Workfront, onde eles têm a opção de alterar a data de migração

  >[!NOTE]
  >
  >Devido à complexidade da migração, as alterações de data são restritas a não mais de 30 dias além da data agendada. Entre em contato com o suporte se precisar de uma data posterior.

* Receba um email de lembrete 1 dia antes da data de início da migração do usuário

### Dia de Preparação de Usuários para Migração

Como administrador do Perfil de produto do Workfront (administrador do Workfront System), o é responsável por garantir que todos os usuários estejam preparados para o dia da migração.

* Prepare todos os usuários para a migração futura para o Adobe Identity, notificando-os do seguinte:

   * À medida que os usuários migram, eles recebem um email da Adobe notificando-os sobre a alteração na maneira como fazem logon no Workfront. Os usuários serão convidados a aceitar um convite para fazer logon usando a Adobe Identity pela primeira vez, fazendo logon com uma Adobe ID existente ou configurando uma nova com o mesmo endereço de email.

### O que esperar no dia da migração

* **A migração de usuário começará à meia-noite do Workfront Datacenter de hospedagem do cliente.**

* **O Adobe migrará automaticamente os administradores do Workfront primeiro.** Quando os administradores do Workfront migrarem para a Adobe Identity, eles receberão a função de administrador do Perfil de Produto do Adobe (administrador do Workfront System). As funções existentes que um usuário pode ter antes da migração não serão afetadas.

  >[!NOTE]
  >
  >Não haverá perda de acesso ao produto durante a migração do usuário. Se um usuário estiver conectado durante o tempo em que for migrado, não haverá impacto. No entanto, no próximo logon, será necessário que eles usem a Identidade da Adobe.



* **À medida que os usuários forem migrados, eles receberão um email da Adobe notificando-os sobre a alteração na maneira como entram no Workfront.** usuários serão convidados a aceitar um convite para entrar usando a Adobe Identity pela primeira vez, seja entrando com uma Adobe ID existente ou configurando uma nova Adobe ID usando o mesmo endereço de email.

  Para obter informações sobre como fazer logon no Workfront com uma Adobe ID, consulte [Fazer logon no Adobe Experience Cloud](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md#log-in-to-adobe-experience-cloud).

### Migração de usuário concluída

A Adobe notificará todos os administradores do sistema e administradores de perfil de produto (administradores do Workfront System) por email depois que todos os administradores e usuários forem migrados. No momento, todos os usuários da Workfront dessa instância farão logon na Workfront usando a Adobe Identity. Os administradores do sistema da Workfront e os administradores de perfil de produto (administradores do Workfront System) podem gerenciar o acesso do usuário na Adobe Admin Console. Se os clientes não estiverem usando uma forma de sincronização de diretórios no Console do administrador, eles poderão continuar a gerenciar o acesso ao Workfront no Aplicativo Workfront.

## Obter suporte

Para dúvidas ou dúvidas, siga as etapas descritas no artigo [Contate o Atendimento ao Cliente](/help/quicksilver/workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md).




