---
title: Conceder a um usuário acesso administrativo total
description: Você pode conceder aos usuários acesso administrativo total ao Workfront.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 46bcb65a-1cb7-443b-88ba-6d0e516e3050
source-git-commit: c887569d59c7751210671cab97c492ee1752fffc
workflow-type: tm+mt
source-wordcount: '1579'
ht-degree: 1%

---

# Conceder acesso administrativo total a um usuário

>[!IMPORTANT]
>
>O procedimento descrito nesta página se aplica apenas a organizações que ainda não foram integradas ao Admin Console. Se sua organização tiver sido integrada à Adobe Admin Console, você deverá executar essa ação por meio da Adobe Admin Console.
>
>Para obter instruções sobre como conceder acesso completo de administrador na Adobe Admin Console, consulte [Gerenciar administradores do sistema na Adobe Admin Console](../../../administration-and-setup/add-users/create-and-manage-users/admin-console.md).
>
>Para obter uma lista de procedimentos que diferem com base no fato de sua organização ter sido integrada à Adobe Admin Console, consulte [Diferenças de administração baseadas em plataforma (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

Como administrador do Adobe Workfront, você pode criar outro administrador do Workfront atribuindo a ele o nível de acesso Administrador do sistema. Um usuário com esse nível de acesso tem acesso administrativo total a tudo no Workfront, incluindo itens que não foram criados por ele mesmo.

>[!NOTE]
>
>Isso é diferente de usar um nível de acesso para conceder aos usuários acesso administrativo a determinadas áreas do sistema. Para obter mais informações, consulte o seguinte:
>
>* [Conceder aos usuários acesso administrativo a determinadas áreas](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md)
>* [Acesso de um administrador do Workfront vs. acesso de um usuário do Plano com direitos administrativos](#access-of-a-workfront-administrator-vs-access-of-a-plan-user-with-administrative-rights) neste artigo
>

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront</td> 
   <td>Qualquer</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td>Plano</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Você deve ser um administrador do Workfront. Para obter mais informações, consulte <a href="#" class="MCXref xref selected">Conceder a um usuário acesso administrativo total</a>.</p> <p><b>OBSERVAÇÃO</b>: se você ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais no seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## Conceder acesso completo de Administrador do sistema a um único usuário

{{step-1-to-users}}

1. Clique no nome do usuário a quem deseja conceder direitos de administrador.
1. Clique no menu Mais ![](assets/more-icon.png) e em **Editar**.

1. Na caixa **Editar Pessoa** exibida, clique em **Acesso**.

1. Na lista suspensa **nível de acesso**, selecione o nível de acesso **Administrador do Sistema**.

   Dependendo das alterações feitas no sistema, o nome desse nível de acesso pode ter sido alterado.

1. Clique em **Salvar alterações.**

   O usuário agora tem direitos completos de Administrador do sistema no sistema.

## Acesso de um administrador do Workfront vs. acesso de um usuário do Plano com direitos administrativos  {#access-of-a-workfront-administrator-vs-access-of-a-plan-user-with-administrative-rights}

As duas tabelas abaixo mostram a diferença entre os direitos de acesso de um usuário com nível de acesso de administrador do Workfront e os de um usuário com uma licença de Plano com alguns direitos administrativos.

Os administradores do Workfront podem visualizar todos os objetos no sistema (independentemente de quem os criou), criar novos e modificar ou excluir os existentes. Eles têm acesso total a todos os objetos no sistema.

Os usuários com uma licença de Plano que podem editar a funcionalidade em uma área têm acesso total à funcionalidade nessa área.

>[!NOTE]
>
>Os usuários com uma licença de Plano designados como administradores de grupo podem executar algumas das ações permitidas para administradores do Workfront. Eles têm permissão para executar essas ações somente para os grupos que administram, seus subgrupos e os usuários nesses grupos e subgrupos. Para obter mais informações, consulte [Administradores de grupo](../../../administration-and-setup/manage-groups/group-roles/group-administrators.md).

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
   <th>administrador do Workfront </th> 
   <th>Usuário com uma licença de Plano e alguns direitos administrativos</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Preferências do projeto: Projetos</td> 
   <td>Acesso total</td> 
   <td>Sem acesso</td> 
  </tr> 
  <tr> 
   <td>Preferências do projeto: tarefas e problemas</td> 
   <td>Acesso total</td> 
   <td>Sem acesso</td> 
  </tr> 
  <tr> 
   <td>Preferências do Projeto: Status</td> 
   <td>Acesso total</td> 
   <td> <p>Sem acesso</p> </td> 
  </tr> 
  <tr> 
   <td>Preferências do projeto: Prioridades</td> 
   <td>Acesso total</td> 
   <td>Sem acesso</td> 
  </tr> 
  <tr> 
   <td>Preferências do projeto: severidades</td> 
   <td>Acesso total</td> 
   <td>Sem acesso</td> 
  </tr> 
  <tr> 
   <td>Preferências do Projeto: Taxas de Câmbio</td> 
   <td>Acesso total</td> 
   <td>Acesso total</td> 
  </tr> 
  <tr> 
   <td>Processos: Aprovações</td> 
   <td> <p>Acesso total</p> </td> 
   <td>Acesso total</td> 
  </tr> 
  <tr> 
   <td>Processos: Caminhos de Etapas</td> 
   <td>Acesso total</td> 
   <td>Acesso total</td> 
  </tr> 
  <tr> 
   <td>Formulários personalizados</td> 
   <td>Acesso total</td> 
   <td> <p>Gerenciar formulários personalizados que eles criaram ou formulários personalizados compartilhados com eles.</p> <p>Anexe formulários personalizados que eles criaram ou formulários personalizados compartilhados com eles a objetos que eles gerenciam ou para os quais eles contribuem com permissões.</p> </td> 
  </tr> 
  <tr> 
   <td>Lixeira: excluída recentemente</td> 
   <td>Acesso total</td> 
   <td> <p>Os usuários que são administradores de grupo podem restaurar projetos atribuídos a grupos que gerenciam e tarefas, problemas ou documentos associados a esses projetos.</p> </td> 
  </tr> 
  <tr> 
   <td>Lixeira: restaurada recentemente</td> 
   <td>Acesso total</td> 
   <td>Os usuários que são administradores de grupo podem ver os itens restaurados recentemente.</td> 
  </tr> 
  <tr> 
   <td>Função no trabalho</td> 
   <td>Acesso total</td> 
   <td> <p>Modificar mas não excluir funções de trabalho existentes.</p> <p>Adicionar novas funções de trabalho.</p> </td> 
  </tr> 
  <tr> 
   <td>Equipes</td> 
   <td>Acesso total</td> 
   <td> <p>Sem acesso para criar Equipes.</p> <p>Adicionar equipes existentes aos usuários ao criar ou editar usuários.</p> </td> 
  </tr> 
  <tr> 
   <td>Grupos</td> 
   <td>Acesso total</td> 
   <td> <p>Sem acesso para criar grupos.</p> <p>Somente administradores de grupo podem gerenciar a associação de grupo, os subgrupos e os status de nível de grupo dos grupos que gerenciam. </p> </td> 
  </tr> 
  <tr> 
   <td>Empresas</td> 
   <td>Acesso total</td> 
   <td>Acesso total</td> 
  </tr> 
  <tr> 
   <td>Fazer logon como</td> 
   <td>Acesso total </td> 
   <td> <p>Se o acesso administrativo ao grupo estiver ativado no nível de acesso e forem designados como administradores de grupo, eles poderão fazer logon como os usuários no grupo que administram e seus subgrupos. Eles não podem efetuar login como um Administrador do sistema.<br>Para obter mais informações sobre como habilitar o acesso administrativo de grupo para usuários, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Conceder acesso aos usuários</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Cronogramas</td> 
   <td>Acesso total</td> 
   <td> <p>Sem acesso para editar Cronogramas.</p> <p>Acesso para adicionar agendamentos existentes a outros usuários, no nível do usuário. </p> </td> 
  </tr> 
  <tr> 
   <td>Horas e planilhas de horas: Perfis de planilhas de horas</td> 
   <td>Acesso total</td> 
   <td> <p>Acesso para atribuir Perfis de Planilha de Horas aos usuários, no nível do usuário.</p> <p>Os usuários que são administradores de grupo podem criar Perfis de folha de horas para os grupos que administram e seus subgrupos. </p> </td> 
  </tr> 
  <tr> 
   <td>Horas e planilhas de horas: Tipos de horas</td> 
   <td>Acesso total</td> 
   <td> <p>Acesso para atribuir Tipos de horas aos usuários, no nível do usuário.</p> </td> 
  </tr> 
  <tr> 
   <td>Horas e Planilha de Horas: Preferências</td> 
   <td>Acesso total</td> 
   <td>Sem acesso</td> 
  </tr> 
  <tr> 
   <td>Email: Notificações: Notificações de Eventos</td> 
   <td>Ativar/ desativar tudo</td> 
   <td>Sem acesso</td> 
  </tr> 
  <tr> 
   <td>Email: Notificações: Notificações de lembrete</td> 
   <td>Acesso total</td> 
   <td>Acesso total</td> 
  </tr> 
  <tr> 
   <td>Email: Notificações: Modelos de email</td> 
   <td>Acesso total</td> 
   <td> <p>Sem acesso para editar Modelos de email.</p> <p>Acesso para adicionar Modelos de email existentes a Notificações de lembrete.</p> </td> 
  </tr> 
  <tr> 
   <td>Email: Lembretes automáticos</td> 
   <td>Acesso total</td> 
   <td>Sem acesso</td> 
  </tr> 
  <tr> 
   <td>Email: Convites</td> 
   <td>Acesso total</td> 
   <td> <p>Sem acesso para editar Convites por email.</p> <p>Acesso para reenviar convites por email a usuários não registrados somente na guia Pessoas.</p> </td> 
  </tr> 
  <tr> 
   <td>Email: Configuração</td> 
   <td>Acesso total</td> 
   <td> <p>Sem acesso</p> </td> 
  </tr> 
  <tr> 
   <td>Scorecards</td> 
   <td>Acesso total</td> 
   <td> <p>Acesso total</p> </td> 
  </tr> 
  <tr> 
   <td>Tipos de Despesas</td> 
   <td>Acesso total</td> 
   <td> <p>Sem acesso</p> </td> 
  </tr> 
  <tr> 
   <td>Tipos de Risco</td> 
   <td>Acesso total</td> 
   <td>Sem acesso</td> 
  </tr> 
  <tr> 
   <td>Níveis de Acesso</td> 
   <td> <p>Acesso total para modificar todos os níveis de acesso.</p> <p>Por padrão, os níveis de acesso Administrador do sistema e Usuário externo não podem ser modificados.</p> </td> 
   <td> <p>Sem acesso para editar Níveis de Acesso.</p> <p>Atribua um nível de acesso a outros usuários que seja inferior ou igual ao deles no nível do usuário.</p> </td> 
  </tr> 
  <tr> 
   <td>Interface: modelos de layout</td> 
   <td>Acesso total</td> 
   <td> <p>Acesso para atribuir modelos de layout existentes a outros usuários, no nível do usuário. </p> <p>Os usuários designados como administradores de grupo podem criar Modelos de layout para grupos e subgrupos que gerenciam.</p> </td> 
  </tr> 
  <tr> 
   <td>Interface: Feeds de atualização</td> 
   <td>Acesso total</td> 
   <td> <p>Sem acesso para modificar os Feeds de atualização.</p> <p>Acesso para adicionar campos a serem rastreados nos Feeds de atualização ao editar o Forms personalizado.</p> </td> 
  </tr> 
  <tr> 
   <td>Interface: filtros</td> 
   <td>Acesso total</td> 
   <td> <p>Não há acesso para criar Filtros na área Configuração.</p> <p>Acesso para criar novos filtros em uma lista de objetos.</p> </td> 
  </tr> 
  <tr> 
   <td>Interface: Exibições</td> 
   <td>Acesso total</td> 
   <td> <p>Sem acesso para criar Exibições na área Configuração.</p> <p>Acesso para criar novas visualizações em uma lista de objetos.</p> </td> 
  </tr> 
  <tr> 
   <td>Interface: agrupamentos</td> 
   <td>Acesso total</td> 
   <td> <p>Sem acesso para criar agrupamentos na área Configuração.</p> <p>Acesso para criar novos agrupamentos em uma lista de objetos.</p> </td> 
  </tr> 
  <tr> 
   <td>Interface: Controles de Lista</td> 
   <td>Acesso total</td> 
   <td> <p>Sem acesso</p> </td> 
  </tr> 
  <tr> 
   <td>Documentos: provedores de nuvem</td> 
   <td>Acesso total</td> 
   <td> <p>Sem acesso para configurar Provedores de nuvem.</p> <p>Acesso para vincular documentos de e para Provedores de nuvem na guia Documentos, depois que os Provedores de nuvem tiverem sido integrados ao Workfront.</p> </td> 
  </tr> 
  <tr> 
   <td>Documentos: mapeamento de metadados</td> 
   <td>Acesso total</td> 
   <td>Sem acesso</td> 
  </tr> 
  <tr> 
   <td>Documentos: integração do SharePoint</td> 
   <td>Acesso total</td> 
   <td> <p>Sem acesso para configurar uma integração com o SharePoint.</p> <p>Acesso para vincular documentos de e para o SharePoint na guia Documentos, após a configuração da integração do SharePoint com o Workfront.</p> </td> 
  </tr> 
  <tr> 
   <td>Documentos: Integração personalizada</td> 
   <td>Acesso total</td> 
   <td> <p>Sem acesso para configurar uma Integração personalizada.</p> <p>Acesso para vincular documentos de e para provedores de terceiros na guia Documentos, depois que os provedores de terceiros tiverem sido integrados ao Workfront.</p> </td> 
  </tr> 
  <tr> 
   <td>Sistema: marca</td> 
   <td>Acesso total</td> 
   <td>Sem acesso</td> 
  </tr> 
  <tr> 
   <td>Sistema: informações do cliente</td> 
   <td>Acesso total</td> 
   <td>Sem acesso</td> 
  </tr> 
  <tr> 
   <td>Sistema: Logon Único (SSO)</td> 
   <td>Acesso total</td> 
   <td>Sem acesso</td> 
  </tr> 
  <tr> 
   <td>Sistema: atualizar usuários para SSO</td> 
   <td>Acesso total</td> 
   <td>Sem acesso</td> 
  </tr> 
  <tr> 
   <td>Sistema: Início</td> 
   <td>Acesso total</td> 
   <td>Sem acesso</td> 
  </tr> 
  <tr> 
   <td>Sistema: Diagnóstico</td> 
   <td>Acesso total</td> 
   <td>Sem acesso</td> 
  </tr> 
  <tr> 
   <td>Sistema: Preferências</td> 
   <td>Acesso total</td> 
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
   <th>administrador do Workfront </th> 
   <th>Usuário com uma licença de Plano e alguns direitos administrativos</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Calendários</td> 
   <td>Acesso total</td> 
   <td>Gerenciar calendários que eles criam e calendários compartilhados com eles.</td> 
  </tr> 
  <tr> 
   <td>Painéis</td> 
   <td>Acesso total</td> 
   <td>Gerencie painéis que eles criam e painéis compartilhados com eles.</td> 
  </tr> 
  <tr> 
   <td>Documentos</td> 
   <td>Acesso total</td> 
   <td>Gerencie documentos dos quais fazem upload ou documentos compartilhados com eles.</td> 
  </tr> 
  <tr> 
   <td>Problemas</td> 
   <td>Acesso total</td> 
   <td>Gerencie problemas que eles criam ou problemas que são compartilhados com eles.</td> 
  </tr> 
  <tr> 
   <td>Portfólios</td> 
   <td>Acesso total</td> 
   <td>Gerencie portfólios que eles criam ou portfólios compartilhados com eles. </td> 
  </tr> 
  <tr> 
   <td>Programas</td> 
   <td>Acesso total</td> 
   <td>Gerencie programas que eles criam ou programas compartilhados com eles.</td> 
  </tr> 
  <tr> 
   <td>Projeto</td> 
   <td>Acesso total</td> 
   <td>Gerencie projetos que eles criam ou projetos compartilhados com eles.</td> 
  </tr> 
  <tr> 
   <td>Relatórios</td> 
   <td>Acesso total</td> 
   <td>Gerencie relatórios que eles criam ou relatórios compartilhados com eles. Exibir, copiar e editar relatórios do sistema.</td> 
  </tr> 
  <tr> 
   <td>Tarefas</td> 
   <td>Acesso total</td> 
   <td>Gerenciar tarefas que eles criam ou tarefas compartilhadas com a</td> 
  </tr> 
  <tr> 
   <td>Modelos</td> 
   <td>Acesso total</td> 
   <td>Gerenciar modelos que eles criam ou modelos compartilhados com eles</td> 
  </tr> 
  <tr> 
   <td>Planilhas de horas</td> 
   <td>Acesso total</td> 
   <td>Acesso total</td> 
  </tr> 
  <tr> 
   <td>Usuários</td> 
   <td>Acesso total</td> 
   <td> <p>Acesso limitado</p> <p>Eles não podem atribuir grupos a usuários para os quais não são administradores de grupo ou grupos que não são públicos.</p> <p>Eles não podem atribuir um nível de acesso aos usuários que seja superior ao seu próprio nível de acesso.</p> <p>Se o acesso administrativo ao grupo estiver ativado no nível de acesso e forem designados como administradores de grupo em um grupo, eles poderão redefinir a senha e fazer logon como os usuários no grupo que administram e seus subgrupos. Eles não podem redefinir a senha ou fazer logon como um Administrador do sistema.<br>Para obter mais informações sobre como habilitar o acesso administrativo de grupo para usuários, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Conceder acesso aos usuários</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
