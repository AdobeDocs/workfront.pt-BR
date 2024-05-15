---
title: Desativar ou reativar um usuário
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: Como administrador do Workfront, você pode desativar ou reativar um usuário.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: aba243ba-46c2-4eb7-b704-4368bf0ae3cc
source-git-commit: ece0275518169fd67708dce903b8bf46a9ee7b1b
workflow-type: tm+mt
source-wordcount: '1170'
ht-degree: 0%

---

# Desativar ou reativar um usuário

<!--Audited 2/2024-->

<!--

>[!IMPORTANT]
>
>The procedure described on this page applies only to organizations that have not yet been onboarded to the Admin Console. If your organization has been onboarded to the Adobe Admin Console, you must perform this action through the Adobe Admin Console.
>
>For instructions on deactivating a user in the Adobe Admin Console, see the section "Remove users" in the article [Manage users individually](https://helpx.adobe.com/enterprise/using/manage-users-individually.html) or contact your Adobe Admin Console Administrator.
>
>For a list of procedures that differ based on whether your organization has been onboarded to the Adobe Admin Console, see [Platform-based administration differences (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

-->

Se um usuário sair da organização, talvez seja necessário removê-lo do Adobe Workfront. Eles não devem permanecer ativos no sistema, pois isso criaria confusão para outros usuários ao adicioná-los a atualizações ou atribuí-los ao trabalho. Quando você desativa um usuário, outros usuários não veem mais seus nomes quando procuram pessoas no sistema.

Os administradores podem ver usuários inativos na área Configuração.

É possível reativar um usuário a qualquer momento.

>[!IMPORTANT]
>
>Recomendamos que você desative os usuários que saíram da organização em vez de excluí-los. Se um usuário for excluído, todo o histórico no Workfront associado a esse usuário será perdido. Isso inclui suas atribuições de trabalho, sua associação com notas, horas, documentos e todos os outros objetos que eles já criaram.
>
>A desativação de um usuário no Workfront remove as licenças do usuário para o Workfront e para a prova digital. Além disso, o usuário não pode mais receber trabalho. Quando um usuário é desativado, a licença e a licença de prova do Workfront desse usuário ficam disponíveis para serem usadas por outro usuário. Todas as outras informações no perfil do usuário desativado permanecem inalteradas.
>
>Para obter mais informações sobre o impacto da exclusão e da desativação de usuários, consulte [Excluir usuários](../../../administration-and-setup/add-users/create-and-manage-users/delete-a-user.md).

## Requisitos de acesso

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
   <td>  <p>Novo: Padrão </p> <p>Ou </p><p>Atual: Plano </p>   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Você deve ter um dos seguintes:</p> 
    <ul> 
     <li> <p>O nível de acesso Administrador do sistema. Para obter informações, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder acesso administrativo total a um usuário</a>. </p> </li> 
     <li> <p><b>Usuários</b> no seu nível de acesso configurado para <b>Editar</b> acesso, com <b>Criar</b> e pelo menos um dos dois <b>Administrador de Usuários</b> opções ativadas em <b>Ajuste as configurações</b> <img src="assets/gear-icon-in-access-levels.png">. </p> <p>Dessas duas opções, se o usuário <b>Administrador (Usuários de grupo)</b> estiver ativado, você deve ser um administrador de grupo de um grupo do qual o usuário seja membro.</p> <p>Para obter mais informações sobre o <b>Usuários</b> em um nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Conceder acesso aos usuários</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Pré-requisitos

Antes de desativar um administrador do Workfront ou usuário de licença Standard ou Plan, você deve associar seus objetos e atividades a outro usuário.

Para obter mais informações, consulte [Sobre a desativação de administradores do Workfront e usuários da licença de plano](#about-deactivating-workfront-administrators-and-plan-license-users) neste artigo.

## Desativar um usuário

Esteja ciente do seguinte ao desativar um usuário:

* O usuário não poderá acessar o sistema.
<!--* The user will be removed from Frame.io review links, assets, projects, and accounts.
   * Reactivating the user does not automatically add them back to the Frame.io items. You must reassign the user manually to Workfront projects, tasks, and assets that require Frame.io collaboration.-->
* Todos os dados associados ao usuário serão retidos.
* Você pode atribuir uma licença de usuário desativada a outro usuário.

Para desativar um usuário:

1. Clique em **[!UICONTROL Menu principal]** ícone ![Menu principal](/help/_includes/assets/main-menu-icon.png) no canto superior direito do Adobe Workfront ou (se disponível), clique no link **[!UICONTROL Menu principal]** ícone ![Menu principal](/help/_includes/assets/main-menu-icon-left-nav.png) no canto superior esquerdo e clique em **Usuários** ![](assets/users-icon-in-main-menu.png).

1. Selecione um usuário, clique no botão **Mais** ícone ![](assets/more-icon.png)e, em seguida, clique em **Desativar**.

1. Clique em **Desativar** na caixa exibida.

## Programar usuários para desativação

Como gerente, talvez você queira marcar os usuários para desativação antes que eles realmente saiam da organização. Por exemplo, se você estiver trabalhando com um usuário vinculado por contrato, ele estará no sistema por um período de tempo limitado e você saberá a data de encerramento. Você pode agendá-los para serem desativados nessa data.

Os administradores do Workfront e os usuários da licença de plano podem ver a data de desativação em seus perfis de usuário.

Para programar um usuário para desativação:

1. Clique em **[!UICONTROL Menu principal]** ícone ![Menu principal](/help/_includes/assets/main-menu-icon.png) no canto superior direito do Adobe Workfront ou (se disponível), clique no link **[!UICONTROL Menu principal]** ícone ![Menu principal](/help/_includes/assets/main-menu-icon-left-nav.png) no canto superior esquerdo e clique em **Usuários** ![](assets/users-icon-in-main-menu.png).

1. Selecione o nome do usuário.

   Ou

   (Opcional) Selecione vários usuários para agendá-los para desativação em massa.

1. Clique no ícone Editar ![](assets/edit-icon.png).
1. Na caixa Editar Usuário exibida, clique em **Planejamento de recursos** para ir para aquela área.
1. Ativar o **Desativação programada** opção.

1. No calendário exibido, especifique a data e a hora da **Data de desativação programada**.

   >[!NOTE]
   >
   >* Na caixa de hora, você pode selecionar apenas incrementos de hora inteira, não minutos.
   >* Se você selecionar uma hora para o dia atual que já passou, o Workfront agendará a desativação para o dia seguinte às 12h. A hora selecionada corresponde ao fuso horário do computador do usuário que está agendando a desativação.

1. Clique em **Salvar alterações**.

   O usuário é desativado no dia selecionado algum tempo depois do horário selecionado. Se você selecionou vários usuários para desativar em massa, todos os usuários selecionados serão desativados no dia selecionado algum tempo depois do horário selecionado.

Recomendamos criar um relatório para os usuários que você agendou para desativação, a fim de manter-se informado sobre quais usuários estão prestes a serem desativados. Não há confirmação de que a desativação ocorreu depois que os usuários foram desativados.

## Reativar um usuário

1. Clique em **[!UICONTROL Menu principal]** ícone ![Menu principal](/help/_includes/assets/main-menu-icon.png) no canto superior direito do Adobe Workfront ou (se disponível), clique no link **[!UICONTROL Menu principal]** ícone ![Menu principal](/help/_includes/assets/main-menu-icon-left-nav.png) no canto superior esquerdo e clique em **Usuários** ![](assets/users-icon-in-main-menu.png).

1. Selecione um usuário, clique no ícone Mais ![](assets/more-icon.png)e, em seguida, clique em **Ativar**.

1. Atribuir um novo **Nível de acesso** no menu suspenso, depois clique em **Reativar**.
<!--
### Asset review and approval impact when you reactivate a user

Deactivated users lose access to their assigned Frame.io accounts as well as assigned projects, assets, and review links. If you choose to reactivate the user, you must manually reassign them to projects, tasks, and assets that require Frame.io collaboration. -->

### Impacto da revisão quando você reativa um usuário

Os usuários desativados perdem a função de prova padrão atribuída e a licença de prova (se você estiver em um Plano herdado do Workfront Premium). Se você optar por reativar o usuário, será necessário:

* Reatribua a licença (se você estiver em um Plano Workfront Premium Legacy). Para obter mais informações sobre planos de prova do Workfront, consulte [Acesso à funcionalidade de prova no Workfront](../../../administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md).
* Verifique se eles têm a função de prova correta. Os usuários de prova reativados recebem o que for especificado como a função de prova padrão para novos usuários. Consulte [Configurar funções de prova padrão](../../../administration-and-setup/manage-workfront/configure-proofing/configure-default-proofing-roles.md) para obter mais informações.

## Sobre a desativação de administradores do Workfront e usuários de licenças Padrão ou Plano

Antes de desativar um administrador do Workfront ou um usuário com uma licença do Plano, é importante verificar se há objetos e atividades do Workfront envolvendo essa pessoa e associá-los a outro administrador do Workfront ou usuário de licença do Plano, conforme necessário.

Esses objetos e atividades podem incluir o seguinte:

* Tarefas ou problemas atribuídos ao usuário
* Projetos de propriedade do usuário
* Relatórios configurados para serem executados com os direitos de acesso do usuário
* Modelos de propriedade do usuário
* Projetos e modelos nos quais o usuário foi definido como um gerenciador de recursos
* Regras de roteamento de fila de solicitações nas quais o administrador do Workfront ou o usuário de licença de Plano é o Atribuído padrão
* Processos de aprovação que têm um estágio incluindo o usuário (especialmente se foram o único aprovador no estágio)
* Folhas de horas que listam o usuário como um aprovador
* Perfis de folha de horas que listam o usuário como um aprovador
* Fluxos de trabalho automatizados de provas que incluem o usuário

## Impacto do planejamento de recursos ao agendar a desativação de um usuário

Quando você agenda a desativação de um usuário, ele não aparece mais no Planejador de recursos como disponível para as horas de orçamento. Se permanecerem como parte dos Conjuntos de recursos, aparecerão no Planejador de recursos, mas sua disponibilidade será definida como zero horas a partir da data de desativação programada.

O Planejador de recursos considera todas as funções de trabalho dos usuários e as Datas de conclusão planejadas das tarefas e calcula os recursos de acordo.

Para obter mais informações sobre o Planejador de recursos, consulte [Visão geral do Planejador de recursos](../../../resource-mgmt/resource-planning/get-started-resource-planner.md).
