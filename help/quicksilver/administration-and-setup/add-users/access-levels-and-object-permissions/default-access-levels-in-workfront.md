---
user-type: administrator
content-type: reference
product-area: system-administration
keywords: acessar,modelo,funil,diagrama,níveis,permissões
navigation-topic: access-levels
title: Níveis de acesso integrados no Adobe Workfront
description: Cada um dos seis níveis de acesso incorporados foi projetado para um tipo específico de usuário, incluindo Administrador do sistema, Planejador, Trabalhador, Revisor, Solicitante e Usuário externo. Esses níveis de acesso permitem controlar o que os usuários podem editar e visualizar no sistema. Se você precisar de um nível de acesso personalizado, é possível copiar e-in access level e determinar a quantidade de acesso que deseja que ele permita para os vários tipos de objetos Workfront.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 5cb42dd8-1557-4fa4-ab3d-8278ce9afd96
source-git-commit: 02191d80ea58f80de2e7be2ff55f43663e415e31
workflow-type: tm+mt
source-wordcount: '1499'
ht-degree: 5%

---

# Níveis de acesso integrados no Adobe Workfront

Cada um dos seis níveis de acesso integrados é projetado para um tipo específico de usuário:

* Administrador de Sistema
* Planejador
* Trabalhador
* Oliveira
* Solicitante
* Usuário externo

Dependendo do nível de acesso, até 3 configurações estão disponíveis para a maioria dos tipos de objetos Workfront:

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
        <td>Os usuários não podem acessar o objeto Workfront</td>
    </tr>
</table>

Se você precisar de um nível de acesso personalizado de Planejador, Trabalhador, Solicitante ou Revisor, poderá copiar o nível de acesso integrado e determinar a quantidade de acesso que deseja que ele permita para os vários tipos de objetos Workfront. Para obter informações sobre como criar um nível de acesso personalizado ou modificar um dos níveis de acesso incorporados, consulte [Criar ou modificar níveis de acesso personalizados](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

>[!IMPORTANT]
>
>É altamente recomendável deixar os níveis de acesso integrados inalterados para que você possa fazer referência a eles depois de configurar seus usuários.

Para obter informações gerais sobre esses níveis de acesso, consulte [Visão geral dos níveis de acesso](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

## Nível de acesso do Administrador do sistema

Anexado à licença do Plano, esse nível de acesso integrado foi projetado para um usuário responsável pela administração do sistema Adobe Workfront. Não é possível modificar esse nível de acesso integrado.

Os usuários com o nível de acesso Administrador do sistema podem fazer tudo no Workfront. Eles podem exibir e editar todos os objetos e informações do Workfront inseridos no Workfront por todos os outros usuários.

Eles também têm acesso à área de configuração completa, onde podem alterar qualquer configuração no nível do sistema. E podem acessar todas as áreas no Menu principal ![](assets/main-menu-icon.png).

Para obter mais informações, consulte [Conceder ao usuário acesso administrativo total](../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md).

## Nível de acesso do planejador

Também anexado à licença do Plano, esse nível de acesso foi projetado para:

* Gerentes de grupos, equipes, projetos e recursos
* Qualquer pessoa responsável pelo planejamento, criação e gerenciamento de tarefas, projetos, portfólios e programas
* Qualquer pessoa responsável por atribuir trabalho (tarefas e problemas) a outros usuários
* Usuários que criam relatórios e aprovam folhas de horas, itens de trabalho e documentos
* Usuários que precisam de acesso a todas as áreas no Menu principal ![](assets/main-menu-icon.png)

Você pode criar uma versão personalizada do nível de acesso integrado do Planejador e determinar a quantidade de acesso que ele permite para os vários tipos de objetos Workfront. Para obter mais informações, consulte [Níveis de acesso integrados no Adobe Workfront](#Customiz) neste artigo.

Estas são as configurações de acesso mais altas disponíveis para objetos no nível de acesso do Planejador:

| Tipo de objeto Workfront | Sem acesso | Exibir acesso | Editar acesso |
|---|---|---|---|
| Projetos |   |   | ✓ |
| Tarefas |   |   | ✓ |
| Problemas |   |   | ✓ |
| Portfólios |   |   | ✓ |
| Programas |   |   | ✓ |
| Relatórios (incluindo painéis e relatórios de calendário) |   |   | ✓ |
| Filtros, visualizações e agrupamentos |   |   | ✓ |
| Documentos |   |   | ✓ |
| Usuários |   |   | ✓ |
| Modelos |   |   | ✓ |
| Dados financeiros |   |   | ✓ |
| Gerenciamento de recursos |   |   | ✓ |
| Planejador de cenários |   |   | ✓ (A configuração padrão é Sem acesso.) |
| Workfront Goals |   |   | ✓ (A configuração padrão é Sem acesso.) |

{style="table-layout:auto"}

## Nível de acesso do trabalhador

Anexado à licença de Trabalho, esse nível de acesso integrado é projetado para usuários que realizam o trabalho no Workfront. Não planeiam o trabalho; eles concluem.

Usuários com este nível de acesso:

* São atribuídos a itens de trabalho onde podem contribuir e registrar o tempo
* Pode aprovar trabalhos e documentos, mas não folhas de horas
* Pode acessar e compartilhar relatórios
* Pode se comunicar com outros usuários no sistema
* Pode acessar todas as áreas no Menu principal ![](assets/main-menu-icon.png), mas a área &quot;Usuários&quot; é chamada de Equipes. Na área Equipes, os usuários com esse nível de acesso podem exibir somente as equipes às quais pertencem, juntamente com o trabalho atribuído a essas equipes.
* Ter capacidade limitada para criar objetos, eles não podem criar projetos, portfólios, programas ou relatórios.

Você pode criar uma versão personalizada do nível de acesso integrado do Worker e determinar a quantidade de acesso que ele permite para os vários tipos de objetos Workfront. Para obter mais informações, consulte [Níveis de acesso integrados no Adobe Workfront](#Customiz) neste artigo.

Estas são as configurações de acesso mais altas disponíveis para objetos no nível de acesso do Trabalhador:

| Tipo de objeto Workfront | Sem acesso | Exibir acesso | Editar acesso |
|---|---|---|---|
| Projetos |   |   | ✓ (Limitado: os usuários só podem compartilhar o projeto, criar tarefas e problemas nele e editar dados em formulários personalizados que já estejam anexados a ele.) |
| Tarefas |   |   | ✓ |
| Problemas |   |   | ✓ |
| Portfólios |   | ✓ (A configuração padrão é Sem acesso.) |   |
| Programas |   | ✓ (A configuração padrão é Sem acesso.) |   |
| Relatórios (incluindo painéis e relatórios de calendário) |   | ✓ |   |
| Filtros, visualizações e agrupamentos |   |   | ✓ |
| Documentos |   |   | ✓ |
| Usuários |   |   | ✓ |
| Modelos | ✓ |   |   |
| Dados financeiros |   | ✓ (A configuração padrão é Sem acesso. A configuração Exibir permite que o usuário exiba somente a área Financeira em Detalhes do projeto.) |   |
| Gerenciamento de recursos |   | ✓ |   |
| Planejador de cenários |   |   | ✓ (A configuração padrão é Sem acesso.) |
| Workfront Goals |   |   | ✓ (A configuração padrão é Sem acesso.) |

{style="table-layout:auto"}

## Nível de acesso do revisor

Anexado à licença de Revisão, esse nível de acesso é projetado para executivos que solicitam trabalho de outros usuários e que revisam e aprovam o trabalho. Esses não são proprietários de projetos ou membros da equipe, mas precisam acessar o Workfront para ver os itens de trabalho que eles supervisionam.

Por exemplo, uma parte interessada com esse nível de acesso pode fazer logon no Workfront para participar de uma revisão contínua dos materiais de marketing, consultar atualizações de trabalho no trabalho e revisar documentos, aprovações, relatórios e calendários.

Usuários com o nível de acesso do Revisor:

* Não é possível atribuir itens de trabalho ou aprovar folhas de tempo
* Pode acessar solicitações e documentos no Menu principal ![](assets/main-menu-icon.png).
* Ter capacidade limitada para criar objetos, eles não podem criar projetos, portfólios, programas ou relatórios.

Você pode criar uma versão personalizada do nível de acesso integrado do Revisor e determinar a quantidade de acesso que ele permite para os vários tipos de objetos Workfront. Para obter mais informações, consulte [Níveis de acesso integrados no Adobe Workfront](#Customiz) neste artigo.

Mais limitadas para projetos e tarefas do que o nível de acesso do Trabalhador, as configurações de acesso mais alto disponíveis para objetos no nível de acesso do Revisor são as seguintes:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Tipo de objeto Workfront</th> 
   <th>Sem acesso</th> 
   <th>Exibir acesso</th> 
   <th>Editar acesso</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Projetos</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Tarefas</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Problemas</td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Portfólios</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Programas</td> 
   <td> </td> 
   <td>✓ (A configuração padrão é Sem acesso.)</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Relatórios (incluindo painéis e relatórios de calendário)</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Filtros, visualizações e agrupamentos</td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Documentos</td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Usuários</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Modelos</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Dados financeiros</td> 
   <td> </td> 
   <td> <p>✓ (A configuração padrão é Sem acesso. A configuração Exibir permite que o usuário exiba somente a área Financeira em Detalhes do projeto.)</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Gerenciamento de recursos</td> 
   <td> </td> 
   <td>✓</td> 
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

Anexado à licença da Solicitação, esse nível de acesso integrado foi projetado para usuários que fazem e recebem solicitações de trabalho simples no Workfront. Por padrão, eles estão limitados à área Solicitações .

Por exemplo, um usuário pode registrar problemas na fila de solicitações de suporte técnico de sua organização.

Usuários com este nível de acesso integrado:

* Pode fazer solicitações e atualizar essas solicitações
* Pode carregar e aprovar documentos
* Pode revisar o status dos problemas que eles enviaram
* Não pode ser atribuído a itens de trabalho
* Pode acessar solicitações somente no Menu principal ![](assets/main-menu-icon.png). Para obter mais informações sobre filas de solicitação, consulte [Criar uma fila de solicitações](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

Você pode criar uma versão personalizada do nível de acesso integrado do Requester e determinar a quantidade de acesso que ele permite para os vários tipos de objetos Workfront. Para obter mais informações, consulte [Níveis de acesso integrados no Adobe Workfront](#Customiz) neste artigo.

Estas são as configurações de acesso mais altas disponíveis para objetos no nível de acesso do Solicitante:

| Tipo de objeto Workfront | Sem acesso | Exibir acesso | Editar acesso |
|---|---|---|---|
| Projeto |   | ✓ (somente a página Detalhes do projeto) |   |
| Tarefa |   | ✓ (somente a página Detalhes) |   |
| Problema |   |   | ✓ |
| Portfólios | ✓ |   |   |
| Programas | ✓ |   |   |
| Relatórios (incluindo painéis e relatórios de calendário) |   | ✓ (somente a página Detalhes) |   |
| Filtros, visualizações e agrupamentos |   |   | ✓ |
| Documento |   |   | ✓ |
| Usuário |   | ✓ |   |
| Modelo | ✓ |   |   |
| Dados financeiros | ✓ |   |   |
| Gerenciamento de recursos | ✓ |   |   |
| Planejador de cenários | ✓ |   |   |
| Workfront Goals |   |   | ✓ (A configuração padrão é Sem acesso.) |

{style="table-layout:auto"}

## Nível de acesso do usuário externo

Esse nível de acesso não está anexado a uma licença paga da Workfront. É o nível de acesso mais restritivo, projetado principalmente para colaboradores, como consultores externos que não fazem logon no Workfront, mas precisam revisar, baixar ou exibir documentos ocasionalmente.

Usuários do Workfront podem atribuir tarefas a usuários externos, mesmo que usuários externos não possam fazer logon no sistema. Mas recomendamos que não seja, porque esse trabalho permaneceria por resolver no sistema.

Usuários com o nível de acesso Usuário externo:

* Pode exibir apenas documentos e relatórios de calendário compartilhados com eles
* Veja os usuários que compartilham documentos e relatórios de calendário com eles
* Aprove os documentos compartilhados com eles

Não é possível modificar esse nível de acesso.

>[!IMPORTANT]
>
>Usuário externo está disponível somente se a opção &quot;Colaborar com pessoas sem contas do Workfront usando seu endereço de email&quot; estiver habilitada na área Preferências do sistema em Configurar. Para obter mais informações, consulte [Configurar preferências de segurança do sistema](/help/quicksilver/administration-and-setup/manage-workfront/security/configure-security-preferences.md).

Veja a seguir as configurações de acesso mais altas disponíveis para objetos no nível de acesso Usuário externo.

| Tipo de objeto Workfront | Sem acesso | Exibir acesso | Editar acesso |
|---|---|---|---|
| Projeto | ✓ |   |   |
| Tarefa | ✓ | ✓ |   |
| Problema | ✓ |   |   |
| Portfólios | ✓ |   |   |
| Programas | ✓ |   |   |
| Relatórios (incluindo painéis e relatórios de calendário) |   | ✓ (apenas para relatórios de calendário; sem capacidade de compartilhar relatórios) |   |
| Filtros, visualizações e agrupamentos | ✓ |   |   |
| Documento |   | ✓ (sem a capacidade de compartilhar documentos) |   |
| Usuário |   | ✓ |   |
| Modelo | ✓ |   |   |
| Dados financeiros | ✓ |   |   |
| Gerenciamento de recursos | ✓ |   |   |
| Planejador de cenários | ✓ |   |   |
| Workfront Goals | ✓ |   |   |
