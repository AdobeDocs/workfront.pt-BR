---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
title: Adicionar usuários
description: Como administrador do Workfront ou usuário com acesso administrativo total, você pode adicionar usuários no Workfront.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: e95dbc32-915b-4ea7-a5ad-e1da99edfbe3
source-git-commit: 7697327455a7ffdc1a15bfa1676c3a0b091abd04
workflow-type: tm+mt
source-wordcount: '1129'
ht-degree: 1%

---

# Adicionar usuários

<!--Audited 2/2024-->

>[!IMPORTANT]
>
>Se sua organização tiver sido integrada à Adobe Admin Console, você deverá criar administradores de sistema por meio da Adobe Admin Console.
>
>Para obter instruções sobre como criar administradores de sistema no Adobe Admin Console, consulte [Gerenciar administradores de sistema no Adobe Admin Console](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/admin-console.md).
>
>Os administradores de grupo em organizações que foram integradas à Adobe Admin Console podem usar esse procedimento para criar usuários e enviá-los para aprovação do administrador.
>
>Para obter uma lista de procedimentos que diferem com base no fato de sua organização ter sido integrada à Adobe Admin Console, consulte [Diferenças de administração baseadas em plataforma (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

Você pode adicionar usuários no Adobe Workfront criando usuários individuais do zero ou copiando usuários existentes.

Para obter informações sobre como importar vários usuários simultaneamente, consulte [Importar usuários](../../../administration-and-setup/add-users/create-and-manage-users/import-users.md).

<!--
Replace this intro with something like the following when we switch to Admin Console:
As an Adobe administrator, you can add users in Adobe Workfront by adding them to your Workfront product profile in the Adobe Admin Console. For instructions, see <a href="../../../administration-and-setup/add-users/create-and-manage-users/admin-console.md" class="MCXref xref">Manage users in the Adobe Admin Console</a>.
-->

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte para executar as etapas deste artigo:

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
   <td><p>Novo: Padrão</p><p>Ou</p><p>Atual: Plano</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Você deve ter um dos seguintes:</p> 
    <ul> 
     <li> <p>O nível de acesso Administrador do sistema. </li> 
     <li> <p>A configuração <b>Usuários</b> no seu nível de acesso foi configurada para <b>Editar</b> acesso, com as opções <b>Criar</b> e pelo menos uma das duas opções <b>Administrador de Usuários</b> habilitadas em <b>Ajustar suas configurações</b> <img src="assets/gear-icon-in-access-levels.png">. </p> <p>Dessas duas opções, se <b>Administrador de Usuários (Usuários de Grupo)</b> estiver habilitado, você deverá ser um administrador de grupo de um grupo do qual o usuário seja membro.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Pré-requisitos

Antes de adicionar um usuário, colete as informações sobre o usuário listado abaixo e determine quais informações você deseja associar a esse usuário:

* Quais são as informações pessoais do usuário? No mínimo, você precisa do seguinte:

   * Nome completo
   * Um nome de usuário
   * Senha padrão
   * Endereço de email

  >[!NOTE]
  >
  >Você pode determinar se os usuários podem exibir as informações de contato de outros usuários ajustando a definição Exibição de Usuários ao especificar níveis de acesso para objetos do Workfront. Para obter mais informações, consulte [Criar ou modificar níveis de acesso personalizados](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

* Qual é a posição do novo usuário na empresa? Essa pessoa tem algum subordinado direto? A quem esta pessoa está subordinada?
* Qual função a pessoa desempenha? Essa função de trabalho existe no Workfront? Há um limite para o número de pessoas que podem preencher essa função de trabalho? Para obter informações sobre como criar funções de trabalho, consulte [Criar e gerenciar funções de trabalho](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).
* Que nível de acesso o usuário deve ter? Ele já existe ou você precisa criar um novo? Para obter mais informações, consulte [Criar ou modificar níveis de acesso personalizados](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
* Em qual grupo padrão esse usuário deve estar? A pessoa deve estar em mais de um grupo? Para obter informações sobre grupos, consulte [Visão geral sobre grupos](../../../administration-and-setup/manage-groups/groups-overview/groups.md).
* Em qual equipe inicial este usuário deve estar? A pessoa deve pertencer a mais de uma equipe? Para obter informações sobre equipes, consulte [Visão geral das equipes](../../../people-teams-and-groups/create-and-manage-teams/teams-overview.md).
* Quais informações personalizadas você precisa associar a este usuário?

  Se informações sobre usuários forem capturadas em campos personalizados criados, você deve ter um formulário personalizado pronto ao criar um usuário. Para obter informações sobre formulários personalizados, consulte [Criar um formulário personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

## Criar um usuário do zero

{{step-1-to-users}}

1. Clique em **Novo usuário > Novo usuário** para adicionar um usuário que ainda não foi adicionado ao Workfront.

   Ou

   Clique em **Novo usuário > Importar usuários** para adicionar usuários carregando um arquivo de importação de planilha.

   Se você estiver importando usuários, não será necessário continuar com essas etapas. Para obter mais informações, consulte [Importar usuários](../../../administration-and-setup/add-users/create-and-manage-users/import-users.md).

1. Na caixa **Novo Usuário** exibida, clique em **Mostrar Opções Avançadas** e configure as opções disponíveis para inserir as informações da pessoa.

   Para obter informações sobre essas opções, consulte [Editar perfil de usuário](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

1. Siga um destes procedimentos:

   * Deixe **Enviar um email de convite para esta pessoa** habilitado. Se você fizer isso, o usuário receberá um email onde poderá seguir um link para criar sua própria senha do Workfront. Os usuários que não aceitam o convite por email e criam uma senha do Workfront são listados como Não registrado no Workfront.
   * Desabilite **Enviar um email de convite a essa pessoa**, digite uma **Senha** para a pessoa e confirme-a na caixa **Confirmar Senha**. Você precisará compartilhar essa senha com o usuário fora do Workfront.

   >[!NOTE]
   >
   >* Se o administrador do Workfront ativou uma integração de SSO com o Workfront, o campo Permitir apenas &lt;Configuração de SSO> autenticação ficará oculto se você desativar o convite por email. O campo ID da Federação ou &lt;Configuração do SSO> Nome de Usuário permanece visível.
   >
   * Se sua organização tiver sido integrada ao Admin Console e você adicionar um usuário por meio do Workfront, você não terá a opção de enviar um convite por email.
   >
   Para os usuários existentes do Adobe, o usuário pode ou não receber um email sobre a disponibilidade do Workfront. Esta é uma preferência controlada pelo administrador de Adobe do produto.

1. Clique Em **Adicionar Esta Pessoa**.

   Ou

   Clique em **Adicionar pessoa e iniciar outra** para salvar o novo usuário e adicionar outro.

   >[!NOTE]
   >
   Se você for um administrador de grupo que adiciona um usuário a uma organização que foi integrada à Adobe Admin Console, as opções para esta etapa serão **Enviar usuário para Aprovação do Administrador** e **Enviar para Aprovação e Iniciar outro**. O usuário é criado com um status Desativado e Pendente de Aprovação. Um administrador do Workfront deve aprovar o usuário, que o ativa no Workfront e o adiciona à Adobe Admin Console.

## Copiar um usuário para criar um novo

Você pode criar um usuário copiando um usuário existente.

>[!NOTE]
>
Quando você cria um usuário dessa maneira, todas as informações são copiadas do usuário original para o usuário recém-criado, exceto para o seguinte:
>
* As informações na seção Informações pessoais.
* Quando eu fizer logon, mostrar: a guia de aterrissagem padrão do nível de acesso é selecionada nesta caixa.
* Superior imediato de
>

Para criar um novo usuário copiando um usuário existente:

{{step-1-to-users}}

1. Selecione o usuário que deseja copiar e clique no ícone Copiar ![](assets/copy-icon.png).
1. Na caixa **Copiar Usuário** que é exibida, edite os campos disponíveis para o novo usuário.

   Para obter informações sobre todos os campos associados a um usuário, consulte [Editar perfil de usuário](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

1. Clique Em **Adicionar Esta Pessoa**.

   Ou

   Clique em **Adicionar pessoa e iniciar outra** para salvar o novo usuário e adicionar outro.

Isso cria uma nova conta no Workfront para o usuário.

Se você selecionou a opção para enviar um convite para o usuário, ele deve receber um email onde possa seguir um link para criar sua senha do Workfront.

>[!NOTE]
>
Se sua organização tiver sido integrada ao Admin Console e você adicionar um usuário por meio do Workfront, você não terá a opção de enviar um convite por email.
>
Para os usuários existentes do Adobe, o usuário pode ou não receber um email sobre a disponibilidade do Workfront. Esta é uma preferência controlada pelo administrador de Adobe do produto.
