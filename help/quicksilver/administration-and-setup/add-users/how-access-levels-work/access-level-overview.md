---
title: Visão Geral dos Novos Níveis de Acesso
user-type: administrator
content-type: reference
product-area: system-administration
keywords: acesso,nível,sistema,administrador,padrão,claro,colaborador
navigation-topic: access-levels
description: Todos os usuários devem ter um nível de acesso para fazer logon e trabalhar no Workfront. Você usa o nível de acesso para controlar o que um usuário pode ver e fazer com determinados objetos e áreas do Workfront.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: d297d8a4-5a4e-418f-983a-19545aeb0668
source-git-commit: 822c4e13ab62d129d0a7c603105251e52578576d
workflow-type: tm+mt
source-wordcount: '1745'
ht-degree: 5%

---

# Visão geral dos novos níveis de acesso

Como administrador do Adobe Workfront, você atribui um nível de acesso a um usuário para duas finalidades:

* Todos os usuários devem ter um nível de acesso para fazer logon e trabalhar no Workfront.
* Você usa o nível de acesso para controlar o que um usuário pode ver e fazer com determinados objetos e áreas do Workfront.

## Novos níveis de acesso incorporados no Adobe Workfront {#built-in-access}

O Workfront tem cinco novos níveis de acesso incorporados:

* Administrador de Sistema
* Padrão
* Leve
* Colaborador
* Externo

Dependendo do nível de acesso, até três permissões estão disponíveis para a maioria dos tipos de objeto do Workfront:

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

Se você precisar de um nível de acesso personalizado, poderá copiar o nível de acesso incorporado e ajustar a quantidade de acesso que deseja que ele permita para os vários tipos de objeto do Workfront. Para obter informações sobre como criar um nível de acesso personalizado, consulte [Criar ou modificar níveis de acesso personalizados](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

>[!IMPORTANT]
>
>É altamente recomendável que você deixe os níveis de acesso incorporados inalterados para que possa consultá-los após configurar os usuários.

### Nível de acesso do administrador do sistema

Anexado à licença Standard, esse nível de acesso integrado foi projetado para um usuário responsável pela administração do sistema Adobe Workfront. Não é possível modificar esse nível de acesso interno.

Os usuários com nível de acesso de Administrador do sistema podem fazer tudo dentro do Workfront. Eles podem exibir e editar todos os objetos e informações do Workfront inseridos no Workfront por todos os outros usuários.

Eles também têm acesso à área Configuração completa, onde podem alterar qualquer configuração no nível do sistema e acessar todas as áreas no Menu principal.

Para obter mais informações, consulte [Conceder a um usuário acesso administrativo total](../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md).

### Nível de acesso padrão

Também anexado à licença Standard, esse nível de acesso foi projetado para usuários que:

* Planejar, criar e acompanhar todos os projetos em um único local
* Automatizar processos de rotina
* Gerenciar recursos
* Rastrear e colaborar em solicitações
* Rastrear e gerar relatórios sobre as finanças do projeto
* Solicitações de trabalho de entrada de início
* Colaborar em projetos, tarefas e problemas

>[!NOTE]
>
>Você pode criar uma versão personalizada do nível de acesso interno Padrão e ajustar a quantidade de acesso permitida para os vários tipos de objeto do Workfront. Para obter informações sobre como criar um nível de acesso personalizado, consulte [Criar ou modificar níveis de acesso personalizados](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

#### **Detalhes de acesso**

Estas são as configurações de acesso mais altas disponíveis para objetos no nível de acesso Padrão:

| Tipo de objeto do Workfront | Sem acesso | Exibir acesso | Editar acesso |
|---|---|---|---|
| Projetos |   |   | ✓ µ |
| Tarefas |   |   | ✓ µ |
| Problemas |   |   | ✓ µ |
| Portfólios |   |   | ✓ µ |
| Programas |   |   | ✓ µ |
| Relatórios (incluindo painéis e relatórios de calendário) |   |   | ✓ µ |
| Filtros, visualizações e agrupamentos |   |   | ✓ µ |
| Documentos |   |   | ✓ µ |
| Usuários |   |   | ✓ µ |
| Modelos |   |   | ✓ µ |
| Dados financeiros |   |   | ✓ µ |
| Gerenciamento de recursos |   |   | ✓ µ |
| Planejador de cenários |   |   | ✓ (A configuração padrão é Sem acesso.) |
| Quadros |   |   | ✓ µ |
| Início |   |   | ✓ µ |
| Metas |   |   | ✓ µ |

{style="table-layout:auto"}

### Nível de acesso leve

Anexado à licença Light, esse nível de acesso foi projetado para usuários que:

* Exibir todos os itens e atualizações vinculados ao trabalho
* Aprovar projetos, tarefas e problemas
* Exibir painéis e relatórios
* Rastrear horário e aprovar planilhas de horas
* Criar e gerenciar problemas
* Fazer atualizações no trabalho

Usuários com nível de acesso Light:

* Itens de trabalho podem ser atribuídos, mas não podem ser concluídos.
* É possível acessar solicitações e documentos no menu principal.
* Têm capacidade limitada para criar objetos; não podem criar projetos, portfólios, programas ou relatórios.

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
   <td>Relatórios (incluindo painéis e relatórios de calendário)</td> 
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
   <td></td> 
   <td> <p>✓ µ</p> </td> 
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
   <td>Quadros </td> 
   <td> </td> 
   <td> </td> 
   <td>✓ µ</td> 
     <tr> 
   <td>Início </td> 
   <td> </td> 
   <td> </td> 
   <td>✓ µ</td> 
  </tr> 
  <tr>   
   <td>Metas </td> 
   <td> </td> 
   <td> </td> 
   <td>✓ µ</td> 
 </tbody> 
</table>

### Nível de acesso do colaborador

Anexado à licença do Colaborador, esse nível de acesso foi projetado para usuários que:

* Enviar solicitações
* Rastrear solicitações
* Atualizar e revisar solicitações
* Aprovar solicitações

Usuários com este nível de acesso incorporado:

* Pode fazer solicitações e atualizá-las
* Pode fazer upload e aprovar documentos
* Pode aprovar projetos, tarefas e problemas
* Pode revisar o status de problemas que enviaram
* Podem ser atribuídos a itens de trabalho, mas não podem concluí-los
* Pode acessar solicitações somente no menu principal. Para obter mais informações sobre filas de solicitações, consulte [Criar uma fila de solicitações](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

>[!NOTE]
>
>Você pode criar uma versão personalizada do nível de acesso interno do Colaborador e ajustar a quantidade de acesso que ele permite para os vários tipos de objeto do Workfront. Para obter informações sobre como criar um nível de acesso personalizado, consulte [Criar ou modificar níveis de acesso personalizados](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

#### **Detalhes de acesso**

Estas são as configurações de acesso mais altas disponíveis para objetos no nível de acesso Colaborador:

| Tipo de objeto do Workfront | Sem acesso | Exibir acesso | Editar acesso |
|---|---|---|---|
| Projeto |   | ✓ µ |   |
| Tarefa |   | ✓ µ |   |
| Problema |   |   | ✓ µ |
| Portfólios |   | ✓ µ |   |
| Programas |   | ✓ µ |   |
| Relatórios (incluindo painéis e relatórios de calendário) |   | ✓ (Somente a guia Detalhes ) |   |
| Filtros, visualizações e agrupamentos |   |   | ✓ µ |
| Documento |   |   | ✓ µ |
| Usuário |   | ✓ µ |   |
| Equipes |   | ✓ µ |   |
| Modelo | ✓ µ |   |   |
| Dados financeiros | ✓ µ |   |   |
| Gerenciamento de recursos | ✓ µ |   |   |
| Planejador de cenários | ✓ µ |   |   |
| Quadros |   |   | ✓ (Cartões simples) |
| Início |   | ✓ (Minhas atualizações) |   |
| Metas |   |   | ✓ µ |

{style="table-layout:auto"}

>[!IMPORTANT]
>
>A partir da versão 24.7, os Colaboradores terão acesso de Visualização a Programas e Portfolio por padrão.
>
> 
>Os colaboradores integrados antes da versão 24.7 continuarão a ter acesso a Programas e Portfolio por padrão. Se necessário, é possível atualizar o acesso para visualizá-los manualmente.

### Nível de acesso de Usuário Externo

Este nível de acesso não está anexado a uma licença paga do Workfront. É o nível de acesso mais restritivo, projetado principalmente para colaboradores como consultores externos que não fazem logon no Workfront, mas precisam revisar, baixar ou exibir documentos ocasionalmente.

Os usuários do Workfront podem atribuir tarefas a usuários externos, mesmo que esses usuários não possam fazer logon no sistema. Mas nós desaconselhamos isso porque esse trabalho ficaria por resolver no sistema.

Usuários com nível de acesso de Usuário Externo:

* Pode exibir somente documentos e relatórios de calendário compartilhados com eles
* Exibir os usuários que compartilham documentos e relatórios de calendário com eles
* Aprovar os documentos compartilhados com eles

Não é possível modificar esse nível de acesso.

>[!IMPORTANT]
>
>O Usuário externo só estará disponível se a opção &quot;Colaborar com pessoas sem contas do Workfront usando seu endereço de email&quot; estiver ativada na área Preferências do sistema em Configuração. Para obter mais informações, consulte [Configurar preferências de segurança do sistema](/help/quicksilver/administration-and-setup/manage-workfront/security/configure-security-preferences.md).

#### **Detalhes de acesso**

Estas são as configurações de acesso mais altas disponíveis para objetos no nível de acesso Usuário externo.

| Tipo de objeto do Workfront | Sem acesso | Exibir acesso | Editar acesso |
|---|---|---|---|
| Projeto | ✓ µ |   |   |
| Tarefa | ✓ µ |   |   |
| Problema | ✓ µ |   |   |
| Portfólios | ✓ µ |   |   |
| Programas | ✓ µ |   |   |
| Relatórios (incluindo painéis e relatórios de calendário) |   | ✓ (Somente para relatórios de calendário; sem capacidade de compartilhar relatórios) |   |
| Filtros, visualizações e agrupamentos | ✓ µ |   |   |
| Documento |   | ✓ (Sem capacidade de compartilhar documentos) |   |
| Usuário |   | ✓ µ |   |
| Equipes | ✓ µ |   |   |
| Modelo | ✓ µ |   |   |
| Dados financeiros | ✓ µ |   |   |
| Gerenciamento de recursos | ✓ µ |   |   |
| Planejador de cenários | ✓ µ |   |   |
| Quadros | ✓ µ |   |   |
| Início | ✓ µ |   |   |
| Metas | ✓ µ |   |   |


## Como os níveis de acesso e as permissões funcionam juntos

Os níveis de acesso definem o que os usuários podem ver e fazer com tipos de objetos gerais e áreas no sistema, como projetos, tarefas e problemas. As permissões definem o que você tem acesso em objetos específicos criados por outras pessoas no sistema, como um projeto criado para executar uma campanha de marketing.

A tabela a seguir compara o acesso geral de um usuário a objetos (definido pelo nível de acesso do usuário) com permissões para um objeto compartilhado específico:

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
   <td>✓ µ</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Concedido por um usuário que compartilha um objeto no nível do objeto</td> 
   <td> </td> 
   <td>✓ µ</td> 
  </tr> 
  <tr> 
   <td> <p>Herdado de um objeto compartilhado de classificação mais alta 
   </td> 
   <td> </td> 
   <td>✓ µ</td> 
  </tr> 
 </tbody> 
</table>

As atividades que um usuário pode fazer com um objeto são definidas por uma combinação de seu nível de acesso e as permissões concedidas a ele.

![](assets/security-model-hierachy-copy.png)

### Conceder permissões por meio do compartilhamento de objetos

Os usuários obtêm acesso a objetos individuais quando outros usuários compartilham e concedem determinadas permissões nesses objetos.

>[!NOTE]
>
>* Se um usuário compartilhar um objeto com determinadas permissões e esse objeto tiver quaisquer objetos filho abaixo dele, o recipient herdará as mesmas permissões para esses objetos filho.
>* Se um nível de acesso impedir que os usuários excluam determinados objetos, isso não os impedirá de excluir objetos filho contidos nesses objetos.

Um usuário pode conceder ao recipient qualquer uma das seguintes permissões para o objeto individual:

* **Exibir**: este nível de permissão permite que o destinatário compartilhe o objeto de uma das seguintes maneiras:

   * Em todo o sistema, para que todos os usuários possam visualizá-lo (não disponível para todos os objetos)
   * Com usuários externos que não têm uma licença do Workfront (não disponível para todos os objetos)
   * Com um endereço de email (disponível somente para documentos e calendários)

* **Contribute**: (não disponível para todos os objetos)
* **Gerenciar**: quando alguém compartilha um objeto, os direitos do destinatário ao objeto são determinados por uma combinação do nível de acesso do destinatário e das permissões do objeto que foram concedidas pelo compartilhador. O grau mais baixo de acesso disponível nessa combinação é o que determina o que o recipient pode fazer com o objeto.

### Exemplos de cenários

#### **Cenário 1**

Se o nível de acesso do recipient não permitir a edição do projeto, essa pessoa não poderá editar ou excluir um projeto, mesmo que o compartilhador tenha concedido permissões para gerenciá-lo.

Ou, se o nível de acesso do recipient permitir a edição do projeto, mas o compartilhador conceder permissões somente de visualização para um projeto, o usuário não poderá editar nem excluir o projeto.

#### **Cenário 2**

Quando Olivia compartilha um projeto do Workfront com Tony, o acesso de Tony a ele é determinado por uma combinação de duas coisas:

* Nível de acesso de Tony, atribuído pelo administrador do Workfront
* As permissões de Tony para o projeto, especificado por Olivia

As ações de Tony no projeto podem ser restritas ainda mais no projeto, mas elas não podem ser irrestritas além do que é permitido em seu nível de acesso:

* Se o nível de acesso de Tony não permite que ele crie tarefas, ele não pode adicionar tarefas ao projeto, mesmo se Olivia lhe deu permissões para adicionar tarefas a ele.
* Se o nível de acesso de Tony permite que ele crie tarefas, mas Olivia não concedeu permissões para adicionar tarefas ao projeto, ele não pode adicionar tarefas a esse projeto, mas ele pode adicionar tarefas a outros projetos onde ele tem permissões para fazê-lo.
