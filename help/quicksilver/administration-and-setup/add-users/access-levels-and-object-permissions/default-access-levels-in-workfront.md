---
user-type: administrator
content-type: reference
product-area: system-administration
keywords: acesso,modelo,funil,diagrama,níveis,permissões
navigation-topic: access-levels
title: Níveis de acesso incorporados
description: Cada um dos seis atuais níveis de acesso incorporados foi projetado para um tipo específico de usuário, incluindo Administrador do sistema, Planejador, Trabalhador, Revisor, Solicitante e Usuário externo. Esses níveis de acesso permitem controlar o que os usuários podem editar e visualizar no sistema. Se você precisar de um nível de acesso personalizado, poderá copiar um nível de acesso incorporado e modificá-lo de acordo com a quantidade de acesso que você deseja que ele permita para os vários tipos de objeto do Workfront.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 5cb42dd8-1557-4fa4-ab3d-8278ce9afd96
source-git-commit: 85aa6cc865bfc28498cca17e1942c146eeb8e4fc
workflow-type: tm+mt
source-wordcount: '1715'
ht-degree: 6%

---

# Níveis de acesso incorporados

<!--Audited: 01/2024-->

>[!NOTE]
>
>Este artigo descreve os níveis de acesso incorporados atuais no Adobe Workfront. Para obter informações sobre os novos níveis de acesso incorporados, consulte [Visão geral sobre os novos níveis de acesso](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/access-level-overview.md).


Cada um dos seis atuais níveis de acesso incorporados foi projetado para um tipo específico de usuário. Esses níveis de acesso permitem controlar o que os usuários podem editar e visualizar no sistema.

Cada um dos seis níveis de acesso incorporados foi projetado para os seguintes tipos de usuários:

* Administrador de Sistema
* Planejador
* Trabalhador
* Revisor
* Solicitante
* Usuário externo

Dependendo do nível de acesso, até três configurações estão disponíveis para a maioria dos tipos de objeto do Workfront:

<table style="table-layout:auto">
    <tr>
        <td>Editar</td>
        <td>Os usuários podem criar, editar, excluir e compartilhar o objeto do Workfront</td>
    </tr>
    <tr>
        <td>Exibir</td>
        <td>Os usuários podem revisar e compartilhar o objeto do Workfront</td>
    </tr>
    <tr>
        <td>Sem acesso</td>
        <td>Os usuários não podem acessar o objeto do Workfront</td>
    </tr>
</table>

Se você precisar de um nível de acesso personalizado de Planejador, Trabalhador, Solicitante ou Revisor, poderá copiar o nível de acesso incorporado e determinar a quantidade de acesso que deseja que ele permita para os vários tipos de objetos do Workfront.

>[!TIP]
>
>Não é possível modificar os níveis de acesso de Administrador do Sistema ou Usuário Externo.

Para obter informações sobre como criar um nível de acesso personalizado ou modificar um dos níveis de acesso internos, consulte [Criar e modificar níveis de acesso personalizados](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

>[!IMPORTANT]
>
>É altamente recomendável que você deixe os níveis de acesso incorporados inalterados para que possa consultá-los após configurar os usuários.

Para obter informações gerais sobre esses níveis de acesso, consulte [Visão geral dos níveis de acesso](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

## Nível de acesso do administrador do sistema

Anexado à licença do Plano, o nível de acesso do Administrador do sistema integrado foi projetado para um usuário responsável pela administração do sistema Adobe Workfront. Não é possível modificar esse nível de acesso interno.

Usuários com nível de acesso de Administrador do sistema podem fazer tudo no Workfront. Eles podem exibir e editar todos os objetos e informações do Workfront inseridos no Workfront por todos os outros usuários.

Eles também têm acesso total à área Configuração, onde podem alterar qualquer configuração no nível do sistema. E eles podem acessar todas as áreas no ![Ícone do menu principal](assets/main-menu-icon.png) ou no ![Ícone do menu principal](assets/main-menu-icon.png) do menu principal, se disponível.

Para obter mais informações, consulte [Conceder a um usuário acesso administrativo total](../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md).

## Nível de acesso do planejador

Também anexado à licença do Plano, o nível de acesso do Planejador foi projetado para:

* Gerentes de grupos, equipes, projetos e recursos
* Qualquer pessoa responsável por planejar, criar e gerenciar tarefas, projetos, portfólios e programas
* Qualquer pessoa responsável pela atribuição de trabalho (tarefas e problemas) a outros usuários
* Usuários que criam relatórios e que aprovam folhas de horas, itens de trabalho e documentos
* Usuários que precisam de acesso a todas as áreas no ![Ícone do menu principal](assets/main-menu-icon.png) ou no ![Ícone do menu principal](assets/main-menu-icon.png) do menu principal, se disponível

Você pode criar uma versão personalizada do nível de acesso interno do Planejador e determinar a quantidade de acesso que ele permite para os vários tipos de objeto do Workfront. Para obter mais informações, consulte [Criar e modificar níveis de acesso personalizados](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

Estas são as configurações de acesso mais altas disponíveis para objetos no nível de acesso do Planejador:

| Tipo de objeto do Workfront | Sem acesso | Exibir acesso | Editar acesso |
|---|---|---|---|
| Projetos |   |   | ✓ µ |
| Tarefas |   |   | ✓ µ |
| Problemas |   |   | ✓ µ |
| Portfólios |   |   | ✓ µ |
| Programas |   |   | ✓ µ |
| Relatórios, painéis e calendários |   |   | ✓ µ |
| Filtros, visualizações e agrupamentos |   |   | ✓ µ |
| Documentos |   |   | ✓ µ |
| Usuários |   |   | ✓ µ |
| Equipes |   |   | ✓ µ |
| Modelos |   |   | ✓ µ |
| Dados financeiros |   |   | ✓ µ |
| Gerenciamento de recursos |   |   | ✓ µ |
| Planejador de cenários |   |   | ✓ (A configuração padrão é Sem acesso.) |
| Workfront Goals |   |   | ✓ (A configuração padrão é Sem acesso.) |

{style="table-layout:auto"}

## Nível de acesso do trabalhador

Anexado à licença de Trabalho, o nível de acesso Trabalhador foi projetado para usuários que executam o trabalho no Workfront. Eles não planejam o trabalho, eles o completam.

Usuários com este nível de acesso:

* São atribuídos a itens de trabalho para os quais eles podem contribuir e registrar horas
* Pode aprovar trabalho e documentos, mas não planilhas de horas
* Pode acessar e compartilhar relatórios
* Pode se comunicar com outros usuários no sistema
* Não é possível acessar todas as áreas no ![Ícone do menu principal](assets/main-menu-icon.png) ou no ![Ícone do menu principal](assets/main-menu-icon.png) do menu principal, se disponível, e a área &quot;Usuários&quot; se chama Equipes. Na área Equipes, os usuários com esse nível de acesso podem ver somente as equipes às quais pertencem, juntamente com o trabalho atribuído a essas equipes.
* Têm capacidade limitada para criar objetos; não podem criar projetos, portfólios, programas ou relatórios.

Você pode criar uma versão personalizada do nível de acesso interno do Worker e determinar a quantidade de acesso que ele permite para os vários tipos de objetos do Workfront. Para obter mais informações, consulte [Criar e modificar níveis de acesso personalizados](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

Estas são as configurações de acesso mais altas disponíveis para objetos no nível de acesso Trabalhador:

| Tipo de objeto do Workfront | Sem acesso | Exibir acesso | Editar acesso |
|---|---|---|---|
| Projetos |   |   | ✓ (Limitado: os usuários só podem compartilhar o projeto, criar tarefas e problemas nele e editar dados em formulários personalizados que já estão anexados a ele.) |
| Tarefas |   |   | ✓ µ |
| Problemas |   |   | ✓ µ |
| Portfólios |   | ✓ (A configuração padrão é Sem acesso.) |   |
| Programas |   | ✓ (A configuração padrão é Sem acesso.) |   |
| Relatórios, painéis e calendários |   | ✓ µ |   |
| Filtros, visualizações e agrupamentos |   |   | ✓ µ |
| Documentos |   |   | ✓ µ |
| Usuários |   |   | ✓ µ |
| Equipes |   |   | ✓ ➡ (Acesso limitado) |
| Modelos | ✓ µ |   |   |
| Dados financeiros |   | ✓ (A configuração padrão é Sem acesso. A configuração Exibir permite que o usuário visualize somente a área Finanças   em Detalhes do projeto.) |   |
| Gerenciamento de recursos |   | ✓ µ |   |
| Planejador de cenários |   |   | ✓ (A configuração padrão é Sem acesso.) |
| Workfront Goals |   |   | ✓ (A configuração padrão é Sem acesso.) |

{style="table-layout:auto"}

## Nível de acesso do revisor

Anexado à licença de Revisão, o nível de acesso de Revisor é projetado para executivos que solicitam trabalho de outros usuários e que revisam e aprovam o trabalho. Eles não são proprietários de projetos ou membros de equipes, mas precisam de acesso ao Workfront para ver os itens de trabalho que supervisionam.

Por exemplo, uma parte interessada com esse nível de acesso pode fazer logon no Workfront para participar de uma revisão contínua de materiais de marketing, ver atualizações de trabalho no trabalho e revisar documentos, aprovações, relatórios e calendários.

Usuários com o nível de acesso Revisor:

* Não é possível atribuir itens de trabalho nem aprovar folhas de horas
* Pode acessar as áreas Solicitações e Documentos no ![Ícone do menu principal](assets/main-menu-icon.png) ou no ![Ícone do menu principal](assets/main-menu-icon.png) do Menu principal, se disponível
* Têm capacidade limitada para criar objetos; não podem criar projetos, portfólios, programas ou relatórios.

Você pode criar uma versão personalizada do nível de acesso interno do Revisor e determinar a quantidade de acesso que ele permite para os vários tipos de objeto do Workfront. Para obter mais informações, consulte [Criar e modificar níveis de acesso personalizados](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

Mais limitadas para projetos e tarefas do que o nível de acesso Trabalhador, as configurações de acesso mais altas disponíveis para objetos no nível de acesso Revisor são as seguintes:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Tipo de objeto do Workfront</th> 
   <th>Sem acesso</th> 
   <th>Exibir acesso</th> 
   <th>Editar acesso</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Projetos</td> 
   <td> </td> 
   <td>✓ µ</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Tarefas</td> 
   <td> </td> 
   <td>✓ µ</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Problemas</td> 
   <td> </td> 
   <td> </td> 
   <td>✓ µ</td> 
  </tr> 
  <tr> 
   <td>Portfólios</td> 
   <td> </td> 
   <td>✓ (A configuração padrão é Sem acesso.)</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Programas</td> 
   <td> </td> 
   <td>✓ (A configuração padrão é Sem acesso.)</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Relatórios, painéis, calendários</td> 
   <td> </td> 
   <td>✓ µ</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Filtros, visualizações e agrupamentos</td> 
   <td> </td> 
   <td> </td> 
   <td>✓ µ</td> 
  </tr> 
  <tr> 
   <td>Documentos</td> 
   <td> </td> 
   <td> </td> 
   <td>✓ µ</td> 
  </tr> 
  <tr> 
   <td>Usuários</td> 
   <td> </td> 
   <td>✓ µ</td> 
   <td> </td> 
  </tr> 
<tr> 
   <td>Equipes</td> 
   <td> </td> 
   <td>✓ µ</td> 
   <td> </td> 
  </tr>

<tr> 
   <td>Modelos</td> 
   <td>✓ µ</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Dados financeiros</td> 
   <td> </td> 
   <td> <p>✓ (A configuração padrão é Sem acesso. A configuração Exibir permite que o usuário visualize somente a área Finanças   em Detalhes do projeto.)</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Gerenciamento de recursos</td> 
   <td> </td> 
   <td>✓ µ</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Planejador de cenários </td> 
   <td> </td> 
   <td> </td> 
   <td>✓ (A configuração padrão é Sem acesso.)</td> 
  </tr> 
  <tr> 
   <td>Workfront Goals </td> 
   <td> </td> 
   <td> </td> 
   <td>✓ (A configuração padrão é Sem acesso.)</td> 
  </tr> 
 </tbody> 
</table>

## Nível de acesso do solicitante

Anexado à licença de solicitação, o nível de acesso Solicitante foi projetado para usuários que fazem e recebem solicitações de trabalho simples no Workfront. Por padrão, eles são limitados à área Solicitações.

Por exemplo, um usuário pode registrar problemas na fila de solicitações de suporte técnico de sua organização.

Usuários com este nível de acesso:

* Pode fazer solicitações e atualizá-las
* Pode fazer upload e aprovar documentos
* Pode revisar o status de problemas que enviaram
* Não pode ser atribuído a itens de trabalho
* Só é possível acessar solicitações na área Solicitações do Menu Principal ![Ícone do Menu Principal](assets/main-menu-icon.png) ou do Menu Principal ![Ícone do Menu Principal](assets/main-menu-icon.png), se disponível. Para obter mais informações sobre filas de solicitações, consulte [Criar uma fila de solicitações](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

Você pode criar uma versão personalizada do nível de acesso integrado do Solicitante e determinar a quantidade de acesso que ele permite para os vários tipos de objeto do Workfront. Para obter mais informações, consulte [Criar e modificar níveis de acesso personalizados](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

Estas são as configurações de acesso mais altas disponíveis para objetos no nível de acesso Solicitante:

| Tipo de objeto do Workfront | Sem acesso | Exibir acesso | Editar acesso |
|---|---|---|---|
| Projeto |   | ✓ (Somente a página Detalhes do projeto) |   |
| Tarefa |   | ✓ (Somente a página Detalhes da tarefa) |   |
| Problema |   |   | ✓ µ |
| Portfólios | ✓ µ |   |   |
| Programas | ✓ µ |   |   |
| Relatórios, painéis e calendários |   | ✓ µ |   |
| Filtros, visualizações e agrupamentos |   |   | ✓ µ |
| Documentos |   |   | ✓ µ |
| Usuário |   | ✓ µ |   |
| Equipes |   | ✓ µ |   |
| Modelos | ✓ µ |   |   |
| Dados financeiros | ✓ µ |   |   |
| Gerenciamento de recursos | ✓ µ |   |   |
| Planejador de cenários | ✓ µ |   |   |
| Workfront Goals |   |   | ✓ (A configuração padrão é Sem acesso.) |

{style="table-layout:auto"}

## Nível de acesso de Usuário Externo

O nível de acesso de Usuário Externo não está anexado a uma licença paga do Workfront. É o nível de acesso mais restritivo, projetado principalmente para colaboradores, como consultores externos que não fazem logon no Workfront, mas precisam revisar, baixar ou exibir documentos ocasionalmente.

Os usuários do Workfront podem atribuir tarefas a usuários externos, mesmo que esses usuários não possam fazer logon no sistema. No entanto, não recomendamos atribuir tarefas e problemas a Usuários externos, pois esse trabalho permaneceria não resolvido no sistema.

Usuários com nível de acesso de Usuário Externo:

* Pode exibir somente documentos e relatórios de calendário compartilhados com eles
* Pode ver os usuários que compartilham documentos e relatórios de calendário com eles
* Podem aprovar os documentos compartilhados com eles

Não é possível modificar esse nível de acesso.

>[!IMPORTANT]
>
>O Usuário externo só estará disponível se a opção &quot;Colaborar com pessoas sem contas do Workfront usando seu endereço de email&quot; estiver ativada na área Preferências do sistema em Configuração. Para obter mais informações, consulte [Configurar preferências de segurança do sistema](/help/quicksilver/administration-and-setup/manage-workfront/security/configure-security-preferences.md).

Embora essas configurações não estejam visíveis na área Níveis de Acesso para o nível de acesso Usuário Externo, um usuário com esse acesso tem o seguinte acesso mais alto aos tipos de objeto do Workfront:

| Tipo de objeto do Workfront | Sem acesso | Exibir acesso | Editar acesso |
|---|---|---|---|
| Projeto | ✓ µ |   |   |
| Tarefa | ✓ µ | |   |
| Problema | ✓ µ |   |   |
| Portfólios | ✓ µ |   |   |
| Programas | ✓ µ |   |   |
| Relatórios, painéis e calendários |   | ✓ (Somente para relatórios de calendário; sem capacidade de compartilhar relatórios) |   |
| Filtros, visualizações e agrupamentos | ✓ µ |   |   |
| Documentos |   | ✓ (sem a capacidade de compartilhar documentos) |   |
| Usuários |   | ✓ µ |   |
| Equipes |   | ✓ µ |   |
| Modelos | ✓ µ |   |   |
| Dados financeiros | ✓ µ |   |   |
| Gerenciamento de recursos | ✓ µ |   |   |
| Planejador de cenários | ✓ µ |   |   |
| Workfront Goals | ✓ µ |   |   |
