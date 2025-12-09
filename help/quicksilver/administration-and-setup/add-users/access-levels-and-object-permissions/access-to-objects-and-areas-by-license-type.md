---
user-type: administrator
content-type: reference
product-area: system-administration
navigation-topic: access-levels
title: Acesso a objetos e áreas por tipo de licença
description: A tabela abaixo informa o nível mais alto de acesso (Editar ou Exibir) que cada uma das licenças do Adobe Workfront permite para os objetos e áreas no Workfront.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: d8f2a295-c053-4763-bf6e-6e836087a839
source-git-commit: 1f1db1c9184a6a8a2abcd3139e4e4e61d2f08bc4
workflow-type: tm+mt
source-wordcount: '480'
ht-degree: 23%

---

# Acesso a objetos e áreas por tipo de licença

<!-- Audited: 11/2025 -->

>[!NOTE]
>
>As informações neste artigo se referem aos níveis de acesso herdados. Para obter informações sobre os novos níveis de acesso, consulte [Visão geral sobre os novos níveis de acesso](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/access-level-overview.md).

A tabela abaixo informa o nível mais alto de acesso (Editar ou Exibir) que cada uma das licenças do Adobe Workfront permite para os objetos e áreas no Workfront.

* Exibir: o usuário pode revisar e compartilhar itens.
* Editar: o usuário pode criar, editar, excluir e compartilhar itens.

  >[!NOTE]
  >
  >Quando outro usuário compartilha um objeto, o compartilhador pode especificar permissões que limitam sua capacidade de editá-lo. Para obter mais informações sobre os novos tipos de licença, consulte [Visão geral das permissões de compartilhamento em objetos](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

  >[!NOTE]
  >
  >Este artigo contém informações sobre o acesso a objetos para os tipos de licença herdados. Para obter informações sobre os novos tipos de licença, consulte [Visão geral sobre novos níveis de acesso](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/access-level-overview.md) e [Visão geral sobre novas licenças](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/licenses-overview.md).

|   | Plano | Trabalho | Revisar | Solicitação | Externo |
|---|---|---|---|---|---|
| Projetos | Editar | Editar (sem criar permissões) | Exibir | Visualização (somente a página Detalhes) | Sem acesso |
| Tarefas | Editar | Editar | Exibir | Exibir | Sem acesso |
| Problemas | Editar | Editar | Editar | Editar | Sem acesso |
| Portfólios | Editar | Exibir | Exibir | Sem acesso | Sem acesso |
| Programas | Editar | Exibir | Exibir | Sem acesso | Sem acesso |
| Relatórios, painéis e calendários | Editar | Exibir | Exibir | Visualização&#42; | Exibir (somente para calendários, sem permissões de compartilhamento) |
| Filtros, visualizações e agrupamentos | Editar | Editar | Editar | Editar | Sem acesso |
| Documentos | Editar | Editar | Editar | Editar | Exibir (sem permissões de compartilhamento) |
| Usuários | Editar | Exibir | Exibir | Exibir | Exibir |
| Equipes | Editar | Editar | Exibir | Exibir | Sem acesso |
| Modelos | Editar | Sem acesso | Sem acesso | Sem acesso | Sem acesso |
| Dados financeiros | Editar | Exibir (somente a área Finanças em Detalhes do Projeto) | Exibir | Sem acesso | Sem acesso |
| Gerenciamento de recursos | Editar | Exibir | Exibir | Sem acesso | Sem acesso |
| Planejador de cenários | Editar | Editar | Editar | Sem acesso | Sem acesso |
| Workfront Goals | Editar | Editar | Editar | Editar | Sem acesso |

&#42; usuários com uma licença de Solicitação podem exibir somente relatórios, painéis e calendários compartilhados com eles.

>[!NOTE]
>
>Os usuários com uma licença de Revisão ou uma licença de Solicitação têm recursos de compartilhamento limitados. Para obter mais informações, consulte [Visão geral das licenças](../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md).
>
>Usuários externos não podem pesquisar itens no Workfront. Eles podem exibir documentos e calendários compartilhados especificamente com eles. Eles também podem ver os usuários que compartilham itens com eles.

Você pode encontrar informações detalhadas sobre o que os níveis de acesso permitem para cada objeto e área nos seguintes artigos:

* [Conceder acesso aos projetos](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md)
* [Conceder acesso às tarefas](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md)
* [Conceder acesso aos problemas](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md)
* [Conceder acesso a documentos](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-documents.md)
* [Conceder acesso aos portfólios](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-portfolios.md)
* [Conceder acesso aos programas](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-programs.md)
* [Conceder acesso a relatórios, painéis e calendários](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md)
* [Conceder acesso a filtros, visualizações e agrupamentos](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-fvg.md)
* [Conceder acesso aos usuários](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md)
* [Conceder acesso às equipes](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-teams.md)
* [Conceder acesso aos modelos](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-templates.md)
* [Conceder acesso a dados financeiros](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md)
* [Conceder acesso ao Gerenciamento de Recursos](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md)
* [Conceder acesso ao Planejador de cenários](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md)
* [Conceder acesso ao Adobe Workfront Goals](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md)
