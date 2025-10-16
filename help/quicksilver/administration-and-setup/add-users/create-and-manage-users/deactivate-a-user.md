---
title: Desativar ou reativar um usuário
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: Os administradores do Workfront podem desativar ou reativar um usuário.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: aba243ba-46c2-4eb7-b704-4368bf0ae3cc
source-git-commit: 72d0b8e0e190f774c7e3f14a78904fb1dd3f2b14
workflow-type: tm+mt
source-wordcount: '1081'
ht-degree: 2%

---

# Desativar ou reativar um usuário {#deactivate-or-reactivate-a-user}

>[!CONTEXTUALHELP]
>id="wf_users_deactivate_user"
>title="Desativar um usuário"
>abstract="A desativação de usuários os remove do Workfront e do Frame.io. Usuários desativados podem ser reativados posteriormente."

<!--Audited 5/2025-->

<!--

>[!IMPORTANT]
>
>The procedure described on this page applies only to organizations that have not yet been onboarded to the Admin Console. If your organization has been onboarded to the Adobe Admin Console, you must perform this action through the Adobe Admin Console.
>
>For instructions on deactivating a user in the Adobe Admin Console, see the section "Remove users" in the article [Manage users individually](https://helpx.adobe.com/br/enterprise/using/manage-users-individually.html) or contact your Adobe Admin Console Administrator.
>
>For a list of procedures that differ based on whether your organization has been onboarded to the Adobe Admin Console, see [Platform-based administration differences (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

-->

Se um usuário sair da organização, é recomendável desativá-lo no sistema para evitar que outros usuários fiquem confusos ao adicioná-lo a atualizações ou atribuí-lo a um trabalho. Quando você desativa um usuário, outros usuários não veem mais seus nomes quando procuram pessoas no sistema.

Os administradores podem ver usuários inativos na área Configuração.

É possível reativar um usuário a qualquer momento.

>[!IMPORTANT]
>
>* Recomendamos que você desative os usuários que saíram da organização em vez de excluí-los. Se um usuário for excluído, todo o histórico no Workfront associado a esse usuário será perdido. Isso inclui suas atribuições de trabalho, sua associação com notas, horas, documentos e todos os outros objetos que eles já criaram.
>
>* A desativação de um usuário no Workfront remove as licenças do usuário para o Workfront e para a prova digital. Além disso, o usuário não pode mais receber trabalho. Quando um usuário é desativado, a licença e a licença de prova do Workfront desse usuário ficam disponíveis para serem usadas por outro usuário. Todas as outras informações no perfil do usuário desativado permanecem inalteradas.
>
>* A desativação de um usuário no Workfront não o remove do Perfil de produto do Workfront no Adobe Admin Console. Para obter mais informações, consulte [Excluir usuários](../../../administration-and-setup/add-users/create-and-manage-users/delete-a-user.md).


## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Pacote do Adobe Workfront</td> 
   <td><p>Qualquer</p></td> 
  </tr> 
  <tr> 
   <td>Licença do Adobe Workfront</td> 
   <td><p>Standard</p><p>Plano</p></td> 
  </tr> 
  <tr> 
   <td>Configurações de nível de acesso</td> 
   <td> <p>Você deve ter um dos seguintes:</p> 
    <ul> 
     <li> <p>O nível de acesso Administrador do sistema. </li> 
     <li> <p>A configuração <b>Usuários</b> no seu nível de acesso foi configurada para <b>Editar</b> acesso, com as opções <b>Criar</b> e pelo menos uma das duas opções <b>Administrador de Usuários</b> habilitadas em <b>Ajustar suas configurações</b> <img src="assets/gear-icon-in-access-levels.png">. </p> <p>Dessas duas opções, se <b>Administrador de Usuários (Usuários de Grupo)</b> estiver habilitado, você deverá ser um administrador de grupo de um grupo do qual o usuário seja membro.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Pré-requisitos

Antes de desativar um administrador do Workfront ou usuário de licença Standard ou Plan, você deve associar seus objetos e atividades a outro usuário.

Para obter mais informações, consulte [Sobre a desativação de administradores do Workfront e usuários de licenças Padrão ou Plano](#about-deactivating-workfront-administrators-and-plan-license-users) neste artigo.

## Desativar um usuário

Esteja ciente do seguinte ao desativar um usuário:

* O usuário não poderá acessar o sistema.
<!--* The user will be removed from Frame.io review links, assets, projects, and accounts.
   * Reactivating the user does not automatically add them back to the Frame.io items. You must reassign the user manually to Workfront projects, tasks, and assets that require Frame.io collaboration.-->
* Todos os dados associados ao usuário serão retidos.
* Você pode atribuir uma licença de usuário desativada a outro usuário.

Para desativar um usuário:

{{step-1-to-users}}

1. Selecione um usuário na lista de usuários.
1. Clique no ícone **Mais** ![Mais ícone](assets/more-icon.png) e em **Desativar**.

1. Na caixa de diálogo **Desativar usuário**, clique em **Desativar**.

## Programar usuários para desativação

Como gerente, talvez você queira marcar os usuários para desativação antes que eles realmente saiam da organização. Por exemplo, se você estiver trabalhando com um usuário vinculado por contrato, ele estará no sistema por um período de tempo limitado e você saberá a data de encerramento. Você pode agendá-los para serem desativados nessa data.

Os administradores do Workfront e os usuários da licença de plano podem ver a data de desativação em seus perfis de usuário.

Para programar um usuário para desativação:

{{step-1-to-users}}

1. Selecione o usuário na lista de usuários.

   Ou

   (Opcional) Selecione vários usuários para agendá-los para desativação em massa.

1. Clique no ícone **Editar** ![Ícone Editar](assets/edit-icon.png).
1. No painel esquerdo da caixa **Editar Usuário**, clique em **Planejamento de Recursos**.
1. Clique em **Definir data de desativação**.

1. Selecione a data e a hora para a **Data de Desativação**.

   >[!NOTE]
   >
   >* Na caixa de hora, você pode selecionar apenas incrementos de hora inteira, não minutos.
   >* Se você selecionar uma hora para o dia atual que já passou, o Workfront agendará a desativação para o dia seguinte às 12:00 AM.
   >* A hora selecionada corresponde ao fuso horário do computador do usuário que está agendando a desativação.

1. Clique em **Salvar**.

O usuário é desativado no dia selecionado algum tempo depois do horário selecionado. Se você selecionou vários usuários para desativar em massa, todos os usuários selecionados serão desativados no dia selecionado algum tempo depois do horário selecionado.

Recomendamos criar um relatório para os usuários que você agendou para desativação para manter-se informado sobre quais usuários estão prestes a serem desativados. Não há confirmação de que a desativação ocorreu após a desativação dos usuários.

## Reativar um usuário

{{step-1-to-users}}

1. Selecione um usuário, clique no ícone **Mais** ícone ![Mais](assets/more-icon.png) e clique em **Ativar**.

1. Na caixa de diálogo **Reativar usuário**, selecione um novo **Nível de acesso** no menu suspenso e clique em **Reativar**.
<!--
### Asset review and approval impact when you reactivate a user

Deactivated users lose access to their assigned Frame.io accounts as well as assigned projects, assets, and review links. If you choose to reactivate the user, you must manually reassign them to projects, tasks, and assets that require Frame.io collaboration. -->

### Impacto da revisão quando você reativa um usuário

Os usuários desativados perdem a função de prova padrão atribuída e a licença de prova (se você estiver em um Plano herdado do Workfront Premium). Se você optar por reativar o usuário, será necessário:

* Reatribua a licença (se você estiver em um Plano Workfront Premium Legacy). Para obter mais informações sobre planos de revisão de texto do Workfront, consulte [Acesso à funcionalidade de revisão de texto no Workfront](../../../administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md).
* Verifique se eles têm a função de prova correta. Os usuários de prova reativados recebem o que for especificado como a função de prova padrão para novos usuários. Consulte [Configurar funções de prova padrão](../../../administration-and-setup/manage-workfront/configure-proofing/configure-default-proofing-roles.md) para obter mais informações.

## Sobre a desativação de administradores do Workfront e usuários de licenças Padrão ou Plano

Antes de desativar um administrador do Workfront ou um usuário com uma licença do Plano, é importante verificar se há objetos e atividades do Workfront envolvendo essa pessoa e associá-los a outro administrador do Workfront ou usuário de licença do Plano, conforme necessário.

Esses objetos e atividades podem incluir o seguinte:

* Tarefas ou problemas atribuídos ao usuário.
* Projetos pertencentes ao usuário.
* Relatórios configurados para serem executados com os direitos de acesso do usuário.
* Modelos de propriedade do usuário.
* Projetos e modelos nos quais o usuário foi definido como um gerenciador de recursos.
* Solicitar regras de roteamento de fila. O administrador do Workfront ou o usuário da licença de Plano é o Atribuído padrão.
* Processos de aprovação que têm um estágio incluindo o usuário (especialmente se eles foram o único aprovador no estágio).
* Planilha de horas que lista o usuário como um aprovador.
* Perfis de folha de horas que listam o usuário como um aprovador.
* Fluxos de trabalho automatizados de provas que incluem o usuário.

## Impacto do planejamento de recursos ao agendar a desativação de um usuário

Quando você agenda a desativação de um usuário, ele não aparece mais no Planejador de recursos como disponível para as horas de orçamento. Se permanecerem como parte dos Conjuntos de recursos, aparecerão no Planejador de recursos, mas sua disponibilidade será definida como zero horas a partir da data de desativação programada.

O Planejador de recursos considera todas as funções de trabalho dos usuários e as Datas de conclusão planejadas das tarefas e calcula os recursos de acordo.

Para obter mais informações sobre o Planejador de recursos, consulte [Visão geral do Planejador de recursos](../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

