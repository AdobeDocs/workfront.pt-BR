---
title: Nova visão geral dos níveis de acesso
user-type: administrator
content-type: reference
product-area: system-administration
keywords: acessar,nível,sistema,administrador,padrão,luz,contribuidor
navigation-topic: access-levels
description: Todos os usuários devem ter um nível de acesso para fazer logon e trabalhar no Workfront. Use o nível de acesso para controlar o que um usuário pode ver e fazer com determinados objetos e áreas do Workfront.
author: Courtney
feature: System Setup and Administration
role: Admin
exl-id: d297d8a4-5a4e-418f-983a-19545aeb0668
source-git-commit: 4af7a72a3633f1b669cbc681f230727cc4f54d1e
workflow-type: tm+mt
source-wordcount: '1626'
ht-degree: 4%

---

# Nova visão geral dos níveis de acesso

Como administrador do Adobe Workfront, você atribui um nível de acesso a um usuário para duas finalidades:

* Todos os usuários devem ter um nível de acesso para fazer logon e trabalhar no Workfront.
* Use o nível de acesso para controlar o que um usuário pode ver e fazer com determinados objetos e áreas do Workfront.

## Novos níveis de acesso integrados no Adobe Workfront {#built-in-access}

A Workfront tem 6 novos níveis de acesso integrados:

* Administrador de Sistema
* Padrão
* Leve
* Colaborador
* Externo

Dependendo do nível de acesso, até 3 permissões estão disponíveis para a maioria dos tipos de objetos Workfront:

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

Se precisar de um nível de acesso personalizado, copie o nível de acesso integrado e ajuste a quantidade de acesso que deseja que ele permita para os vários tipos de objetos Workfront. Para obter informações sobre como criar um nível de acesso personalizado, consulte [Criar ou modificar níveis de acesso personalizados](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

>[!IMPORTANT]
>
>É altamente recomendável deixar os níveis de acesso integrados inalterados para que você possa fazer referência a eles depois de configurar seus usuários.

### Nível de acesso do Administrador do sistema

Anexado à licença do Standard, esse nível de acesso integrado foi projetado para um usuário responsável pela administração do sistema Adobe Workfront. Não é possível modificar esse nível de acesso integrado.

Os usuários com o nível de acesso Administrador do sistema podem fazer tudo no Workfront. Eles podem exibir e editar todos os objetos e informações do Workfront inseridos no Workfront por todos os outros usuários.

Eles também têm acesso à área de configuração completa, onde podem alterar qualquer configuração no nível do sistema, e podem acessar todas as áreas no Menu principal.

Para obter mais informações, consulte [Conceder ao usuário acesso administrativo total](../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md).

### Nível de acesso padrão

Também anexado à licença Padrão, esse nível de acesso é projetado para usuários que:

* Planejar, criar e rastrear todos os projetos em um único local
* Automatizar processos de rotina
* Gerenciar recursos
* Rastrear e colaborar em solicitações
* Rastrear e relatar as finanças dos projetos
* Solicitações de trabalho de entrada
* Colaborar em projetos, tarefas e problemas

>[!NOTE]
>
>Você pode criar uma versão personalizada do nível de acesso integrado Padrão e ajustar a quantidade de acesso que ele permite para os vários tipos de objetos Workfront. Para obter informações sobre como criar um nível de acesso personalizado, consulte [Criar ou modificar níveis de acesso personalizados](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

#### **Detalhes de acesso**

Estas são as configurações de acesso mais altas disponíveis para objetos no nível de acesso Padrão:

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
| Quadros |   |   | ✓ |
| Página inicial |   |   | ✓ |
| Metas |   |   | ✓ |

{style="table-layout:auto"}

### Nível de acesso leve

Anexado à licença Light, esse nível de acesso é projetado para usuários que:

* Exibir todos os itens e atualizações vinculados ao trabalho
* Aprovar projetos, tarefas e problemas
* Exibir painéis e relatórios
* Rastrear tempo
* Criar e gerenciar problemas
* Fazer atualizações no trabalho

Usuários com o nível de acesso Light:

* Não é possível atribuir itens de trabalho ou aprovar folhas de horas
* Pode acessar solicitações e documentos no Menu principal.
* Ter capacidade limitada para criar objetos, eles não podem criar projetos, portfólios, programas ou relatórios.

>[!NOTE]
>
>Você pode criar uma versão personalizada do nível de acesso integrado Light e ajustar a quantidade de acesso que ele permite para os vários tipos de objetos Workfront. Para obter informações sobre como criar um nível de acesso personalizado, consulte [Criar ou modificar níveis de acesso personalizados](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

#### **Detalhes de acesso**

Estas são as configurações de acesso mais altas disponíveis para objetos no nível de acesso Light:

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
   <td>Equipes</td> 
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
   <td>✓</td> 
   <td> <p> </p> </td> 
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
   <td>Quadros </td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
     <tr> 
   <td>Página inicial </td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr>   
   <td>Metas </td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
 </tbody> 
</table>

### Nível de acesso do colaborador

Anexado à licença do Colaborador, esse nível de acesso é projetado para usuários que:

* Enviar solicitações
* Rastrear solicitações
* Atualizar e revisar solicitações.

Usuários com este nível de acesso integrado:

* Pode fazer solicitações e atualizar essas solicitações
* Pode carregar e aprovar documentos
* Pode revisar o status dos problemas que eles enviaram
* Não pode ser atribuído a itens de trabalho
* Pode acessar solicitações somente no Menu principal. Para obter mais informações sobre filas de solicitação, consulte [Criar uma fila de solicitações](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

>[!NOTE]
>
>Você pode criar uma versão personalizada do nível de acesso integrado do Contributor e ajustar a quantidade de acesso que ele permite para os vários tipos de objetos Workfront. Para obter informações sobre como criar um nível de acesso personalizado, consulte [Criar ou modificar níveis de acesso personalizados](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

#### **Detalhes de acesso**

Estas são as configurações de acesso mais altas disponíveis para objetos no nível de acesso do Contributor:

| Tipo de objeto Workfront | Sem acesso | Exibir acesso | Editar acesso |
|---|---|---|---|
| Projeto |   | ✓ (somente a página Detalhes do projeto) |   |
| Tarefa |   | ✓ (somente a página Detalhes) |   |
| Problema |   |   | ✓ |
| Portfólios | ✓ |   |   |
| Programas | ✓ |   |   |
| Relatórios (incluindo painéis e relatórios de calendário) |   | ✓ (somente a guia Detalhes) |   |
| Filtros, visualizações e agrupamentos |   |   | ✓ |
| Documento |   |   | ✓ |
| Usuário |   | ✓ |   |
| Equipes |   | ✓ |   |
| Modelo | ✓ |   |   |
| Dados financeiros | ✓ |   |   |
| Gerenciamento de recursos | ✓ |   |   |
| Planejador de cenários | ✓ |   |   |
| Quadros |   |   | ✓ (placas simples) |
| Página inicial |   | ✓ (Minhas atualizações) |   |
| Metas |   |   | ✓ |

{style="table-layout:auto"}

### Nível de acesso do usuário externo

Esse nível de acesso não está anexado a uma licença paga da Workfront. É o nível de acesso mais restritivo, projetado principalmente para colaboradores como consultores externos que não fazem logon no Workfront, mas precisam revisar, baixar ou exibir documentos ocasionalmente.

Usuários do Workfront podem atribuir tarefas a usuários externos, mesmo que usuários externos não possam fazer logon no sistema. Mas recomendamos que não seja, porque esse trabalho permaneceria por resolver no sistema.

Usuários com o nível de acesso Usuário externo:

* Pode exibir apenas documentos e relatórios de calendário compartilhados com eles
* Exibir os usuários que compartilham documentos e relatórios de calendário com eles
* Aprove os documentos compartilhados com eles

Não é possível modificar esse nível de acesso.

>[!IMPORTANT]
>
>Usuário externo está disponível somente se a opção &quot;Colaborar com pessoas sem contas do Workfront usando seu endereço de email&quot; estiver habilitada na área Preferências do sistema em Configurar. Para obter mais informações, consulte [Configurar preferências de segurança do sistema](/help/quicksilver/administration-and-setup/manage-workfront/security/configure-security-preferences.md).

#### **Detalhes de acesso**

Veja a seguir as configurações de acesso mais altas disponíveis para objetos no nível de acesso Usuário externo.

| Tipo de objeto Workfront | Sem acesso | Exibir acesso | Editar acesso |
|---|---|---|---|
| Projeto | ✓ |   |   |
| Tarefa | ✓ |   |   |
| Problema | ✓ |   |   |
| Portfólios | ✓ |   |   |
| Programas | ✓ |   |   |
| Relatórios (incluindo painéis e relatórios de calendário) |   | ✓ (apenas para relatórios de calendário; sem capacidade de compartilhar relatórios) |   |
| Filtros, visualizações e agrupamentos | ✓ |   |   |
| Documento |   | ✓ (Sem capacidade de compartilhar documentos) |   |
| Usuário |   | ✓ |   |
| Equipes | ✓ |   |   |
| Modelo | ✓ |   |   |
| Dados financeiros | ✓ |   |   |
| Gerenciamento de recursos | ✓ |   |   |
| Planejador de cenários | ✓ |   |   |
| Quadros | ✓ |   |   |
| Página inicial | ✓ |   |   |
| Metas | ✓ |   |   |


## Como os níveis de acesso e as permissões funcionam em conjunto

Os níveis de acesso definem o que os usuários podem ver e fazer com tipos de objetos gerais e áreas no sistema, como projetos, tarefas e problemas. As permissões definem o que você tem acesso em objetos específicos criados por outras pessoas no sistema, como um projeto criado para executar uma campanha de marketing.

A tabela a seguir compara o acesso geral de um usuário aos objetos (definido pelo nível de acesso do usuário) às permissões de um objeto compartilhado específico:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> </th> 
   <th>Nível de acesso </th> 
   <th>Permissões </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Concedido por um administrador do Workfront no nível de acesso de um usuário</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Concedido por um usuário que compartilha um objeto no nível do objeto</td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>Herdado de um objeto compartilhado de classificação superior 
   </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

As atividades que um usuário pode fazer com um objeto são definidas por uma combinação do nível de acesso e das permissões fornecidas a ele.

![](assets/security-model-hierachy-copy.png)

### Conceder permissões por meio do compartilhamento de objetos

Os usuários têm acesso a objetos individuais quando outros usuários compartilham e concedem certas permissões a esses objetos.

>[!NOTE]
>
>* Se um usuário compartilhar um objeto com determinadas permissões e esse objeto tiver qualquer objeto filho abaixo dele, o recipient herdará as mesmas permissões para esses objetos filho.
>* Se um nível de acesso impedir que os usuários excluam determinados objetos, isso não impede que eles excluam objetos filhos contidos nesses objetos.


Um usuário pode conceder ao recipient qualquer uma das seguintes permissões para o objeto individual:

* **Exibir**: Esse nível de permissão permite que o recipient compartilhe o objeto de uma das seguintes maneiras:

   * Em todo o sistema, para que todos os usuários possam visualizá-lo (não disponível para todos os objetos)
   * Com usuários externos que não têm uma licença Workfront (não disponível para todos os objetos)
   * Com um endereço de email (disponível somente para documentos e calendários)

* **Contribute**: (não disponível para todos os objetos)
* **Gerenciar**: Quando alguém compartilha um objeto, os direitos do recipient ao objeto são determinados por uma combinação do nível de acesso do recipient e das permissões para o objeto que foram concedidas pelo compartilhador. O menor grau de acesso disponível nessa combinação é o que determina o que o recipient pode fazer com o objeto.

### Cenários de exemplo

#### **Cenário 1**

Se o nível de acesso do destinatário não permitir a edição do projeto, essa pessoa não poderá editar ou excluir um projeto mesmo que o compartilhador tenha concedido permissões para gerenciá-lo.

Ou, se o nível de acesso do destinatário permitir a edição do projeto, mas o compartilhador tiver concedido permissões somente para visualização a um projeto, o usuário não poderá editar ou excluir o projeto.

#### **Cenário 2**

Quando Olivia compartilha um projeto do Workfront com Tony, o acesso de Tony a ele é determinado por uma combinação de duas coisas:

* Nível de acesso do Tony, atribuído pelo administrador do Workfront
* Permissões de Tony ao projeto, especificadas por Olivia

As ações de Tony no projeto podem ser ainda mais restritas no projeto, mas não podem ser irrestritas além do permitido no seu nível de acesso:

* Se o nível de acesso de Tony não lhe permite criar tarefas, ele não pode adicionar tarefas ao projeto, mesmo que Olivia lhe tenha dado permissões para adicionar tarefas a ele.
* Se o nível de acesso de Tony permitir que ele crie tarefas, mas Olivia não concedeu permissões para adicionar tarefas ao projeto, ele não poderá adicionar tarefas a esse projeto, mas poderá adicionar tarefas a outros projetos nos quais recebeu permissões para isso.
