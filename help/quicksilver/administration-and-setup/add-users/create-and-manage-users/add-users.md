---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
title: Adicionar usuários
description: Como administrador do Workfront ou usuário com acesso administrativo total, você pode adicionar usuários no Workfront.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: e95dbc32-915b-4ea7-a5ad-e1da99edfbe3
source-git-commit: 9bcd792139f8f2f0198da943e5c63a2add32e856
workflow-type: tm+mt
source-wordcount: '1176'
ht-degree: 1%

---

# Adicionar usuários

>[!IMPORTANT]
>
>O procedimento descrito nesta página se aplica somente a organizações que ainda não foram integradas ao Admin Console. Se sua organização tiver sido integrada à Adobe Admin Console, você deverá executar essa ação por meio da Adobe Admin Console.
>
>Para obter instruções sobre como adicionar um usuário no Adobe Admin Console:
>
>* Consulte [Criar usuários no Workfront com a Adobe Admin Console](../../../administration-and-setup/add-users/create-and-manage-users/admin-console.md#create)
>* Consulte a seção &quot;Adicionar usuários&quot; no artigo [Gerenciar usuários individualmente](https://helpx.adobe.com/enterprise/using/manage-users-individually.html)
>* Entre em contato com o administrador do Adobe Admin Console.
>
>Para obter uma lista de procedimentos diferentes com base no fato de sua organização ter sido integrada à Adobe Admin Console, consulte [Diferenças de administração baseadas em plataforma (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

Você pode adicionar usuários no Adobe Workfront criando usuários individuais do zero ou copiando usuários existentes.

Para obter informações sobre como importar vários usuários simultaneamente, consulte [Importar usuários](../../../administration-and-setup/add-users/create-and-manage-users/import-users.md).

<!--
Replace this intro with something like the following when we switch to Admin Console:
As an Adobe administrator, you can add users in Adobe Workfront by adding them to your Workfront product profile in the Adobe Admin Console. For instructions, see <a href="../../../administration-and-setup/add-users/create-and-manage-users/admin-console.md" class="MCXref xref">Manage users in the Adobe Admin Console</a>.
-->

## Requisitos de acesso

Você deve ter o seguinte para executar as etapas neste artigo:

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
   <td> <p>Você deve ter uma das seguintes opções:</p> 
    <ul> 
     <li> <p>O nível de acesso do Administrador do sistema. Para obter mais informações, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder ao usuário acesso administrativo total</a>. </p> </li> 
     <li> <p><b>Usuários</b> na configuração do seu nível de acesso configurado como <b>Editar</b> acesso, com <b>Criar</b> e pelo menos um dos dois <b>Administrador do usuário</b> opções ativadas em <b>Ajustar as configurações</b> <img src="assets/gear-icon-in-access-levels.png">. </p> <p>Dessas duas opções, se Usuário <b>Administrador (usuários do grupo)</b> estiver habilitado, você deve ser um administrador de grupo de um grupo no qual o usuário é membro.</p> <p>Para obter mais informações sobre o <b>Usuários</b> configurar em um nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Conceder acesso aos usuários</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Pré-requisitos

Antes de adicionar um usuário, reúna as informações sobre ele listadas abaixo e determine quais informações você deseja associar a ele:

* Quais são as informações pessoais do usuário? No mínimo, você precisa do seguinte:

   * Nome completo
   * Um nome de usuário
   * Senha padrão
   * Endereço de email

   >[!NOTE]
   >
   >Você pode determinar se os usuários podem exibir as informações de contato de outros usuários ajustando a configuração da Exibição de usuários ao especificar níveis de acesso para objetos Workfront. Para obter mais informações, consulte [Criar ou modificar níveis de acesso personalizados](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

* Qual é a posição do novo usuário na empresa? Essa pessoa tem alguma informação direta? A quem essa pessoa se reporta?
* Qual função a pessoa preenche? Essa função de trabalho existe no Workfront? Existe um limite para o número de pessoas que podem preencher essa função? Para obter informações sobre como criar funções de cargo, consulte [Criar e gerenciar funções de trabalho](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).
* Qual nível de acesso o usuário deve ter? Ele já existe ou você precisa criar um novo? Para obter mais informações, consulte [Criar ou modificar níveis de acesso personalizados](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
* Em qual grupo doméstico este usuário deve estar? A pessoa deve estar em mais de um grupo? Para obter informações sobre grupos, consulte [Visão geral dos grupos](../../../administration-and-setup/manage-groups/groups-overview/groups.md).
* Em qual equipe principal este usuário deve estar? A pessoa deve estar em mais de uma equipe? Para obter informações sobre as equipes, consulte [Visão geral das equipes](../../../people-teams-and-groups/create-and-manage-teams/teams-overview.md).
* Quais informações personalizadas você precisa associar a este usuário?

   Se as informações sobre os usuários forem capturadas em campos personalizados criados, será necessário ter um formulário personalizado pronto ao criar um usuário. Para obter informações sobre formulários personalizados, consulte [Criar ou editar um formulário personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

## Criar um usuário do zero

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront, em seguida, clique em **Usuários** ![](assets/users-icon-in-main-menu.png).

1. Clique em **Novo usuário > Novo usuário** para adicionar um usuário que ainda não foi adicionado ao Workfront.

   Ou

   Clique em **Novo usuário > Importar usuários** para adicionar usuários carregando um arquivo de importação de planilha.

   Se você estiver importando usuários, não será necessário continuar com essas etapas. Para obter mais informações, consulte [Importar usuários](../../../administration-and-setup/add-users/create-and-manage-users/import-users.md).

1. No **Novo usuário** for exibida, clique em **Mostrar opções avançadas**, configure as opções disponíveis para inserir as informações da pessoa.

   Para obter informações sobre essas opções, consulte [Editar o perfil de um usuário](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

1. Siga um destes procedimentos:

   * Sair **Enviar um email de convite para esta pessoa** habilitado. Se você fizer isso, o usuário receberá um email onde poderá seguir um link para criar sua própria senha para o Workfront. Os usuários que não aceitam o convite por email e criam uma senha do Workfront são listados como Não registrados no Workfront.
   * Desativar **Enviar um email de convite para esta pessoa** e digite a **Senha** para a pessoa e confirme-a no **Confirmar senha** caixa. Você precisará compartilhar essa senha com o usuário fora do Workfront.

   >[!NOTE]
   >
   >Se o administrador do Workfront ativou uma integração SSO com o Workfront, a função Somente permitir &lt;sso configuration=&quot;&quot;> O campo Autenticação fica oculto se você desativar o convite por email. A ID de Federação ou &lt;sso configuration=&quot;&quot;> O campo Nome de usuário permanece visível.

   >[!NOTE]
   Se sua organização tiver sido integrada ao Admin Console e você adicionar um usuário por meio do Workfront, você não terá a opção de enviar um convite por email.
   Novos usuários do Adobe são adicionados ao Admin Console e o Admin Console fornece um email convidando-os a concluir o processo de registro. Todos os usuários devem concluir o processo de registro para acessar qualquer sistema de Adobe.
   Para usuários existentes do Adobe, o usuário pode ou não receber um email sobre a disponibilidade do Workfront. Esta é uma preferência controlada pelo administrador do Adobe para o produto.

1. Clique em **Adicionar este usuário**.

   Ou

   Clique em **Adicionar usuário da pessoa e iniciar outra** para salvar o novo usuário e adicionar outro.

## Copiar um usuário para criar um novo

Você pode criar um usuário copiando um usuário existente.

>[!NOTE]
Ao criar um usuário dessa forma, todas as informações são copiadas do usuário original para o usuário recém-criado, exceto para o seguinte:
* As informações na seção Informações pessoais .
* Quando eu fizer logon, mostre: A guia de aterrissagem padrão para o nível de acesso é selecionada nesta caixa.
* Superior imediato de
>


Para criar um novo usuário copiando um existente:

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront, em seguida, clique em **Usuários** ![](assets/users-icon-in-main-menu.png).
1. Selecione o usuário que deseja copiar e clique no ícone Copiar ![](assets/copy-icon.png).
1. No **Novo usuário** for exibida, edite os campos disponíveis para o novo usuário.

   Para obter informações sobre todos os campos associados a um usuário, consulte [Editar o perfil de um usuário](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

1. Clique em **Adicionar este usuário**.

   Ou

   Clique em **Adicionar usuário da pessoa e iniciar outra** para salvar o novo usuário e adicionar outro.

Isso cria uma nova conta no Workfront para o usuário.

Se você selecionou a opção de enviar um convite para o usuário, ele deverá receber um email onde poderá seguir um link para criar a senha do Workfront.

>[!NOTE]
Se sua organização tiver sido integrada ao Admin Console e você adicionar um usuário por meio do Workfront, você não terá a opção de enviar um convite por email.
Novos usuários do Adobe são adicionados ao Admin Console e o Admin Console fornece um email convidando-os a concluir o processo de registro. Todos os usuários devem concluir o processo de registro para acessar qualquer sistema de Adobe.
Para usuários existentes do Adobe, o usuário pode ou não receber um email sobre a disponibilidade do Workfront. Esta é uma preferência controlada pelo administrador do Adobe para o produto.
