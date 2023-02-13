---
title: Conceder ao usuário acesso administrativo total
description: Você pode conceder aos usuários acesso administrativo total ao Workfront.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 46bcb65a-1cb7-443b-88ba-6d0e516e3050
source-git-commit: 253a116e04e0b3a729331f5d0a29405e82808390
workflow-type: tm+mt
source-wordcount: '1614'
ht-degree: 1%

---

# Conceder ao usuário acesso administrativo total

>[!IMPORTANT]
>
>O procedimento descrito nesta página se aplica somente a organizações que ainda não foram integradas ao Admin Console. Se sua organização tiver sido integrada à Adobe Admin Console, você deverá executar essa ação por meio da Adobe Admin Console.
>
>Para obter instruções sobre como conceder acesso total de administrador na Adobe Admin Console:
>
>* Consulte [Criar administradores de sistema no Workfront com a Adobe Admin Console](../../../administration-and-setup/add-users/create-and-manage-users/admin-console.md#create2)
>* Consulte a seção &quot;Editar detalhes do usuário&quot; no artigo [Gerenciar usuários individualmente](https://helpx.adobe.com/enterprise/using/manage-users-individually.html) na documentação do Adobe Admin Console.
>* Entre em contato com o administrador do Adobe Admin Console.
>
>Para obter uma lista de procedimentos diferentes com base no fato de sua organização ter sido integrada à Adobe Admin Console, consulte [Diferenças de administração baseadas em plataforma (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

Como administrador do Adobe Workfront, você pode criar outro administrador do Workfront atribuindo a ele o nível de acesso Administrador do sistema. Um usuário com esse nível de acesso tem acesso administrativo total a tudo no Workfront, incluindo itens que ele mesmo não criou.

>[!NOTE]
>
>Isso é diferente do uso de um nível de acesso para conceder aos usuários acesso administrativo a determinadas áreas do sistema. Para obter mais informações, consulte:
>
>* [Conceder aos usuários acesso administrativo a determinadas áreas](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md)
>* [Acesso de um administrador do Workfront vs. acesso de um usuário do Plano com direitos administrativos](#access-of-a-workfront-administrator-vs-access-of-a-plan-user-with-administrative-rights) neste artigo
>


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
   <td> <p>Você deve ser um administrador do Workfront. Para obter mais informações, consulte <a href="#" class="MCXref xref selected">Conceder ao usuário acesso administrativo total</a>.</p> <p><b>OBSERVAÇÃO</b>: Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Conceder acesso completo ao Administrador do sistema a um único usuário

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront, em seguida, clique em **Usuários** ![](assets/users-icon-in-main-menu.png).

1. Clique no nome do usuário ao qual você deseja conceder direitos de administrador.
1. Clique no menu Mais ![](assets/more-icon.png), depois clique em **Editar**.

1. No **Editar Pessoa** for exibida, clique em **Acesso**.

1. No **nível de acesso** selecione a lista suspensa **Administrador do sistema** nível de acesso.

   Dependendo das alterações feitas no sistema, o nome desse nível de acesso pode ter sido alterado.

1. Clique em **Salvar alterações.**

   O usuário agora tem direitos plenos de Administrador do sistema no sistema.

## Acesso de um administrador do Workfront vs. acesso de um usuário do Plano com direitos administrativos  {#access-of-a-workfront-administrator-vs-access-of-a-plan-user-with-administrative-rights}

As duas tabelas abaixo mostram a diferença entre os direitos de acesso de um usuário com um nível de acesso de administrador do Workfront e os de um usuário com uma licença do Plano com alguns direitos administrativos.

Os administradores do Workfront podem exibir todos os objetos no sistema (independentemente de quem os criou), criar novos objetos e modificar ou excluir os objetos existentes. Eles têm acesso total a todos os objetos no sistema.

Os usuários com uma licença do Plan que podem editar funcionalidade em uma área têm acesso total à funcionalidade nessa área.

>[!NOTE]
>
>Os usuários com uma licença do Plano designados como administradores de grupo podem executar algumas das ações permitidas para administradores do Workfront. Eles podem executar essas ações somente para os grupos que administram, seus subgrupos e os usuários nesses grupos e subgrupos. Para obter mais informações, consulte [Administradores do grupo](../../../administration-and-setup/manage-groups/group-roles/group-administrators.md).

* [Acesso à área Configuração](#access-to-the-setup-area)
* [Acesso a objetos](#access-to-objects)

### Acesso à área Configuração {#access-to-the-setup-area}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Área/objeto</th> 
   <th>Administrador do Workfront </th> 
   <th>Usuário com uma licença de Plano e alguns direitos administrativos</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Preferências do projeto: Projetos</td> 
   <td>Acesso completo</td> 
   <td>Sem acesso</td> 
  </tr> 
  <tr> 
   <td>Preferências do projeto: Tarefas e problemas</td> 
   <td>Acesso completo</td> 
   <td>Sem acesso</td> 
  </tr> 
  <tr> 
   <td>Preferências do projeto: Status</td> 
   <td>Acesso completo</td> 
   <td> <p>Sem acesso</p> </td> 
  </tr> 
  <tr> 
   <td>Preferências do projeto: Prioridades</td> 
   <td>Acesso completo</td> 
   <td>Sem acesso</td> 
  </tr> 
  <tr> 
   <td>Preferências do projeto: Severidades</td> 
   <td>Acesso completo</td> 
   <td>Sem acesso</td> 
  </tr> 
  <tr> 
   <td>Preferências do projeto: Taxas de Câmbio</td> 
   <td>Acesso completo</td> 
   <td>Acesso completo</td> 
  </tr> 
  <tr> 
   <td>Processos: Aprovações</td> 
   <td> <p>Acesso completo</p> </td> 
   <td>Acesso completo</td> 
  </tr> 
  <tr> 
   <td>Processos: Caminhos de marco</td> 
   <td>Acesso completo</td> 
   <td>Acesso completo</td> 
  </tr> 
  <tr> 
   <td>Formulários personalizados</td> 
   <td>Acesso completo</td> 
   <td> <p>Gerencie formulários personalizados que eles criaram ou compartilharam com eles.</p> <p>Anexe formulários personalizados que eles criaram ou formulários personalizados compartilhados com eles a objetos para os quais eles gerenciam ou contribuem com permissões.</p> </td> 
  </tr> 
  <tr> 
   <td>Lixeira: Recentemente Excluído</td> 
   <td>Acesso completo</td> 
   <td> <p>Os usuários que são administradores de grupo podem restaurar projetos atribuídos a Grupos que gerenciam, além de tarefas, problemas ou documentos associados a esses projetos.</p> </td> 
  </tr> 
  <tr> 
   <td>Lixeira: Restaurado recentemente</td> 
   <td>Acesso completo</td> 
   <td>Os usuários que são administradores de grupo podem ver os itens que restauraram recentemente.</td> 
  </tr> 
  <tr> 
   <td>Função no trabalho</td> 
   <td>Acesso completo</td> 
   <td> <p>Modifique, mas não exclua, as funções de job existentes.</p> <p>Adicionar novas funções de trabalho.</p> </td> 
  </tr> 
  <tr> 
   <td>Equipes</td> 
   <td>Acesso completo</td> 
   <td> <p>Sem acesso para criar equipes.</p> <p>Adicionar equipes existentes aos usuários ao criar ou editar usuários.</p> </td> 
  </tr> 
  <tr> 
   <td>Grupos</td> 
   <td>Acesso completo</td> 
   <td> <p>Sem acesso para criar Grupos.</p> <p>Somente administradores de grupo podem gerenciar associação de grupo, subgrupos e status de nível de grupo para os grupos que gerenciam. </p> </td> 
  </tr> 
  <tr> 
   <td>Empresas</td> 
   <td>Acesso completo</td> 
   <td>Acesso completo</td> 
  </tr> 
  <tr> 
   <td>Fazer logon como</td> 
   <td>Acesso completo </td> 
   <td> <p>Se o acesso administrativo do grupo estiver ativado em seu nível de acesso e for designado como administrador de grupo, eles poderão fazer logon como os usuários do grupo que administram e seus subgrupos. Eles não podem fazer logon como Administrador do sistema.<br>Para obter mais informações sobre como habilitar o acesso administrativo de grupo para usuários, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Conceder acesso aos usuários</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Cronogramas</td> 
   <td>Acesso completo</td> 
   <td> <p>Sem acesso para editar Agendamentos.</p> <p>Acesso para adicionar agendamentos existentes a outros usuários, no nível do usuário. </p> </td> 
  </tr> 
  <tr> 
   <td>Folha de Horas e Horas: Perfis de Folha de Horas</td> 
   <td>Acesso completo</td> 
   <td> <p>Acesso para atribuir Perfis de Folha de Horas existentes aos usuários, no nível do usuário.</p> <p>Os usuários que são administradores de grupo podem criar Perfis de folha de horas para os grupos que administram e seus subgrupos. </p> </td> 
  </tr> 
  <tr> 
   <td>Folha de Horas e Horas: Tipos de hora</td> 
   <td>Acesso completo</td> 
   <td> <p>Acesso para atribuir Tipos de hora a usuários, no nível do usuário.</p> </td> 
  </tr> 
  <tr> 
   <td>Folha de Horas e Horas: Preferências</td> 
   <td>Acesso completo</td> 
   <td>Sem acesso</td> 
  </tr> 
  <tr> 
   <td>Email: Notificações: Notificações de evento</td> 
   <td>Ativar/Desativar tudo</td> 
   <td>Sem acesso</td> 
  </tr> 
  <tr> 
   <td>Email: Notificações: Notificações de Lembrete</td> 
   <td>Acesso completo</td> 
   <td>Acesso completo</td> 
  </tr> 
  <tr> 
   <td>Email: Notificações: Modelos de email</td> 
   <td>Acesso completo</td> 
   <td> <p>Sem acesso para editar modelos de email.</p> <p>Acesso para adicionar modelos de email existentes às notificações de lembrete.</p> </td> 
  </tr> 
  <tr> 
   <td>Email: Lembretes Automáticos</td> 
   <td>Acesso completo</td> 
   <td>Sem acesso</td> 
  </tr> 
  <tr> 
   <td>Email: Convites</td> 
   <td>Acesso completo</td> 
   <td> <p>Sem acesso para editar os Convites por email.</p> <p>Acesso ao reenvio de convites por email para usuários não registrados somente na guia Pessoas.</p> </td> 
  </tr> 
  <tr> 
   <td>Email: Configuração</td> 
   <td>Acesso completo</td> 
   <td> <p>Sem acesso</p> </td> 
  </tr> 
  <tr> 
   <td>Scorecards</td> 
   <td>Acesso completo</td> 
   <td> <p>Acesso completo</p> </td> 
  </tr> 
  <tr> 
   <td>Tipos de Despesas</td> 
   <td>Acesso completo</td> 
   <td> <p>Sem acesso</p> </td> 
  </tr> 
  <tr> 
   <td>Tipos de Risco</td> 
   <td>Acesso completo</td> 
   <td>Sem acesso</td> 
  </tr> 
  <tr> 
   <td>Níveis de Acesso</td> 
   <td> <p>Acesso completo para modificar todos os níveis de acesso.</p> <p>Os níveis de acesso Administrador do sistema e Usuário externo não podem ser modificados por padrão.</p> </td> 
   <td> <p>Sem acesso para editar Níveis de Acesso.</p> <p>Atribua um nível de acesso a outros usuários que seja menor ou igual ao deles no nível do usuário.</p> </td> 
  </tr> 
  <tr> 
   <td>Interface: Modelos de layout</td> 
   <td>Acesso completo</td> 
   <td> <p>Acesso para atribuir Modelos de Layout existentes a outros usuários, no nível do usuário. </p> <p>Os usuários designados como administradores de grupo podem criar Modelos de layout para grupos e subgrupos que gerenciam.</p> </td> 
  </tr> 
  <tr> 
   <td>Interface: Atualizar feeds</td> 
   <td>Acesso completo</td> 
   <td> <p>Não há acesso para modificar os Feeds de atualização.</p> <p>Acesso para adicionar campos a serem rastreados nos Feeds de atualização ao editar o Forms personalizado.</p> </td> 
  </tr> 
  <tr> 
   <td>Interface: Filtros</td> 
   <td>Acesso completo</td> 
   <td> <p>Não há acesso para criar Filtros na área Configuração.</p> <p>Acesso para criar novos filtros em uma lista de objetos.</p> </td> 
  </tr> 
  <tr> 
   <td>Interface: Exibições</td> 
   <td>Acesso completo</td> 
   <td> <p>Sem acesso para criar Exibições na área Configuração.</p> <p>Acesso para criar novas exibições em uma lista de objetos.</p> </td> 
  </tr> 
  <tr> 
   <td>Interface: Agrupamentos</td> 
   <td>Acesso completo</td> 
   <td> <p>Sem acesso para criar Agrupamentos na área Configuração.</p> <p>Acesso para criar novos agrupamentos em uma lista de objetos.</p> </td> 
  </tr> 
  <tr> 
   <td>Interface: Controles de lista</td> 
   <td>Acesso completo</td> 
   <td> <p>Sem acesso</p> </td> 
  </tr> 
  <tr> 
   <td>Documentos: Provedores de nuvem</td> 
   <td>Acesso completo</td> 
   <td> <p>Sem acesso para configurar os provedores de nuvem.</p> <p>Acesso a vincular documentos de e para provedores de nuvem na guia Documentos, após os provedores de nuvem terem sido integrados ao Workfront.</p> </td> 
  </tr> 
  <tr> 
   <td>Documentos: Mapeamento de metadados</td> 
   <td>Acesso completo</td> 
   <td>Sem acesso</td> 
  </tr> 
  <tr> 
   <td>Documentos: Integração do SharePoint</td> 
   <td>Acesso completo</td> 
   <td> <p>Sem acesso para configurar uma integração do SharePoint.</p> <p>Acesso a vincular documentos de e para o SharePoint na guia Documents , após a configuração da integração do SharePoint com o Workfront.</p> </td> 
  </tr> 
  <tr> 
   <td>Documentos: Integração personalizada</td> 
   <td>Acesso completo</td> 
   <td> <p>Sem acesso para configurar uma Integração personalizada.</p> <p>Acesso a vincular documentos de e para provedores de terceiros na guia Documents , depois que os provedores de terceiros tiverem sido integrados ao Workfront.</p> </td> 
  </tr> 
  <tr> 
   <td>Sistema: Marca</td> 
   <td>Acesso completo</td> 
   <td>Sem acesso</td> 
  </tr> 
  <tr> 
   <td>Sistema: Informações do cliente</td> 
   <td>Acesso completo</td> 
   <td>Sem acesso</td> 
  </tr> 
  <tr> 
   <td>Sistema: Logon único (SSO)</td> 
   <td>Acesso completo</td> 
   <td>Sem acesso</td> 
  </tr> 
  <tr> 
   <td>Sistema: Atualizar usuários para SSO</td> 
   <td>Acesso completo</td> 
   <td>Sem acesso</td> 
  </tr> 
  <tr> 
   <td>Sistema: Primeiros Passos</td> 
   <td>Acesso completo</td> 
   <td>Sem acesso</td> 
  </tr> 
  <tr> 
   <td>Sistema: Diagnóstico</td> 
   <td>Acesso completo</td> 
   <td>Sem acesso</td> 
  </tr> 
  <tr> 
   <td>Sistema: Preferências</td> 
   <td>Acesso completo</td> 
   <td>Sem acesso</td> 
  </tr> 
 </tbody> 
</table>

### Acesso a objetos {#access-to-objects}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Área/objeto</th> 
   <th>Administrador do Workfront </th> 
   <th>Usuário com uma licença de Plano e alguns direitos administrativos</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Calendários</td> 
   <td>Acesso completo</td> 
   <td>Gerencie calendários que eles criam e calendários compartilhados com eles.</td> 
  </tr> 
  <tr> 
   <td>Painéis</td> 
   <td>Acesso completo</td> 
   <td>Gerencie painéis que eles criam e painéis compartilhados com eles.</td> 
  </tr> 
  <tr> 
   <td>Documentos</td> 
   <td>Acesso completo</td> 
   <td>Gerencie documentos carregados ou compartilhados com eles.</td> 
  </tr> 
  <tr> 
   <td>Problemas</td> 
   <td>Acesso completo</td> 
   <td>Gerencie problemas que eles criam ou problemas compartilhados com eles.</td> 
  </tr> 
  <tr> 
   <td>Portfólios</td> 
   <td>Acesso completo</td> 
   <td>Gerencie portfólios que eles criam ou portfólios compartilhados com eles. </td> 
  </tr> 
  <tr> 
   <td>Programas</td> 
   <td>Acesso completo</td> 
   <td>Gerencie programas que eles criam ou programas compartilhados com eles.</td> 
  </tr> 
  <tr> 
   <td>Projeto</td> 
   <td>Acesso completo</td> 
   <td>Gerencie projetos que eles criam ou projetos compartilhados com eles.</td> 
  </tr> 
  <tr> 
   <td>Relatórios</td> 
   <td>Acesso completo</td> 
   <td>Gerencie relatórios que eles criam ou relatórios compartilhados com eles. Exibir, copiar e editar relatórios do sistema.</td> 
  </tr> 
  <tr> 
   <td>Tarefas</td> 
   <td>Acesso completo</td> 
   <td>Gerenciar tarefas que eles criam ou tarefas compartilhadas com a</td> 
  </tr> 
  <tr> 
   <td>Modelos</td> 
   <td>Acesso completo</td> 
   <td>Gerenciar modelos que eles criam ou modelos compartilhados com eles</td> 
  </tr> 
  <tr> 
   <td>Folhas de horas</td> 
   <td>Acesso completo</td> 
   <td>Acesso completo</td> 
  </tr> 
  <tr> 
   <td>Usuários</td> 
   <td>Acesso completo</td> 
   <td> <p>Acesso limitado</p> <p>Eles não podem atribuir grupos a usuários para os quais não sejam administradores de grupo ou grupos que não sejam públicos.</p> <p>Eles não podem atribuir um nível de acesso a usuários que seja superior ao seu próprio nível de acesso.</p> <p>Se o acesso administrativo do grupo estiver ativado em seu nível de acesso e for designado como administrador de grupo em um grupo, eles poderão redefinir a senha e fazer logon como os usuários do grupo que administram e seus subgrupos. Eles não podem redefinir a senha ou fazer logon como Administrador do sistema.<br>Para obter mais informações sobre como habilitar o acesso administrativo de grupo para usuários, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Conceder acesso aos usuários</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
