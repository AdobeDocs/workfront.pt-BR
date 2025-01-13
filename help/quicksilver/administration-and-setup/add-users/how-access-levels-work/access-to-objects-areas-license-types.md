---
user-type: administrator
content-type: reference
product-area: system-administration
navigation-topic: access-levels
title: Acesso a Objetos e Áreas por Novas Licenças
description: A tabela abaixo informa o nível mais alto de acesso (Editar ou Exibir) que cada uma das licenças do Adobe Workfront permite para os objetos e áreas no Workfront.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 87fb5673-6e36-4182-958a-d69a56fe7b68
source-git-commit: b333ea67bb909ca55306f6474832c275ebad590c
workflow-type: tm+mt
source-wordcount: '410'
ht-degree: 23%

---

# Acesso a objetos e áreas por novas licenças

<!-- Audited: 2/2024 -->

A tabela abaixo informa o nível mais alto de acesso (Editar ou Exibir) que cada uma das licenças do Adobe Workfront permite para os objetos e áreas no Workfront.

* **Exibir**: o usuário pode revisar e compartilhar itens.
* **Editar**: o usuário pode criar, editar, excluir e compartilhar itens.

  >[!NOTE]
  >
  >Quando outro usuário compartilha um objeto, o compartilhador pode especificar permissões que limitam sua capacidade de editá-lo. Para obter mais informações, consulte [Visão geral das permissões de compartilhamento em objetos](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

<table style="table-layout:auto">
    <tr>
        <td></td>
        <td>Padrão</td>
        <td>Leve</td>
        <td>Colaborador</td>
        <td>Externo</td>
    </tr>
    <tr>
        <td>Projetos</td>
        <td>Editar</td>
        <td>Exibir</td>
        <td>Exibir</td>
        <td>Sem acesso</td>
    </tr>
    <tr>
        <td>Tarefas</td>
        <td>Editar</td>
        <td>Exibir</td>
        <td>Exibir</td>
        <td>Exibir</td>
    </tr>
    <tr>
        <td>Problemas</td>
        <td>Editar</td>
        <td>Editar</td>
        <td>Editar</td>
        <td>Sem acesso</td>
    </tr>
    <tr>
        <td>Portfólios</td>
        <td>Editar</td>
        <td>Exibir</td>
        <td>Exibir</td>
        <td>Sem acesso</td>
    </tr>
    <tr>
        <td>Programas</td>
        <td>Editar</td>
        <td>Exibir</td>
        <td>Exibir</td>
        <td>Sem acesso</td>
    </tr>
    <tr>
        <td>Relatórios, painéis e calendários</td>
        <td>Editar</td>
        <td>Exibir</td>
        <td>Visualização*</td>
        <td>Exibir (somente para calendários, sem permissões de compartilhamento)</td>
    </tr>
    <tr>
        <td>Filtros, visualizações e agrupamentos</td>
        <td>Editar</td>
        <td>Editar</td>
        <td>Editar</td>
        <td>Sem acesso</td>
    </tr>
    <tr>
        <td>Documentos</td>
        <td>Editar</td>
        <td>Editar</td>
        <td>Editar</td>
        <td>Exibir (sem permissões de compartilhamento)</td>
    </tr>
    <tr>
        <td>Usuários</td>
        <td>Editar</td>
        <td>Exibir</td>
        <td>Exibir</td>
        <td>Exibir</td>
    </tr>
    <tr>
        <td>Equipes</td>
        <td>Editar</td>
        <td>Exibir</td>
        <td>Exibir</td>
        <td>Sem acesso</td>
    </tr>
    <tr>
        <td>Modelos</td>
        <td>Editar</td>
        <td>Sem acesso</td>
        <td>Sem acesso</td>
        <td>Sem acesso</td>
    </tr>
    <tr>
        <td>Dados financeiros</td>
        <td>Editar</td>
        <td>Sem acesso</td>
        <td>Sem acesso</td>
        <td>Sem acesso</td>
    </tr>
    <tr>
        <td>Gerenciamento de recursos</td>
        <td>Editar</td>
        <td>Exibir</td>
        <td>Sem acesso</td>
        <td>Sem acesso</td>
    </tr>
    <tr>
        <td>Planejador de cenários</td>
        <td>Editar</td>
        <td>Exibir</td>
        <td>Sem acesso</td>
        <td>Sem acesso</td>
    </tr>
    <tr>
        <td>Workfront Goals</td>
        <td>Editar</td>
        <td>Editar</td>
        <td>Editar</td>
        <td>Sem acesso</td>
    </tr>
</table>

&#42; usuários com uma licença de Colaborador podem exibir somente relatórios, painéis e calendários compartilhados com eles.

>[!NOTE]
>
>* Os usuários com uma licença Light ou de Colaborador têm recursos de compartilhamento limitados. Para obter mais informações, consulte [Visão geral das licenças](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/licenses-overview.md).
>
>* Usuários externos não podem pesquisar itens no Workfront. Eles podem exibir documentos e calendários compartilhados especificamente com eles. Eles também podem ver os usuários que compartilham itens com eles.
>
>* Usuários colaboradores e usuários externos não podem ver o conteúdo compartilhado em todo o sistema.  Ela deve ser compartilhada explicitamente com eles.

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
