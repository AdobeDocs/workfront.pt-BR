---
product-area: projects
navigation-topic: approvals
title: Delegar solicitação de aprovação
description: A delegação de solicitações de aprovação permite que você atribua outro usuário para aprovar suas solicitações por um período de tempo, por exemplo, se você estiver fora do escritório em férias.
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: 01b76dd5-98cb-4f0d-97ff-7e665f843a9c
source-git-commit: e0f6078cfab1b325302dbda8a656d2a65ee0b95c
workflow-type: tm+mt
source-wordcount: '1209'
ht-degree: 0%

---

# Delegar solicitação de aprovação

Você pode delegar temporariamente o trabalho ao qual está atribuído enquanto estiver fora do escritório. Você pode delegar atribuições de tarefas e problemas ou pode delegar solicitações de aprovação. Este artigo descreve como delegar solicitações de aprovação. Para obter informações sobre delegação de atribuições de tarefas e problemas, consulte [Delegar tarefas e problemas](../../manage-work/delegate-work/how-to-delegate-work.md).

Você pode delegar os seguintes tipos de aprovações, independentemente de como a aprovação foi atribuída a você (seja atribuída diretamente a você, a uma equipe da qual você é membro ou à sua função de trabalho):

* Aprovações de projetos
* Aprovações de tarefas
* Aprovações de problemas

Não é possível delegar aprovações de planilhas de horas, documentos ou provas.

>[!NOTE]
>
>Para garantir que não ocorram inconsistências com as datas que você agenda para que suas aprovações sejam delegadas, recomendamos que o fuso horário do seu perfil de usuário corresponda ao da sua agenda. Para obter mais informações, consulte os seguintes artigos:
>
>* [Criar um agendamento](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)
>* [Editar o perfil de um usuário](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)
>

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><p>plano do Adobe Workfront*</p></td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Licença da Adobe Workfront*</p></td> 
   <td> <p>Revisar ou superior</p> </td> 
  </tr> 
 </tbody> 
</table>

Para descobrir o tipo de plano ou licença que você tem, entre em contato com o administrador do Workfront.

+++

## Entender o acesso do usuário a aprovações delegadas

Durante o período de aprovação designado, o usuário ao qual você delega uma solicitação de aprovação tem as seguintes habilidades:

* Pode aprovar ou rejeitar solicitações de aprovação existentes onde nenhuma decisão foi tomada
* Pode aprovar e rejeitar novas solicitações de aprovação recebidas durante um período especificado
* Recebe acesso de visualização a objetos que estão aguardando aprovação

  >[!NOTE]
  >
  > O administrador do Adobe Workfront pode impedir que os usuários acessem determinados tipos de objetos. Quando um usuário não tem acesso a um tipo de objeto e uma aprovação desse tipo é delegada ao usuário, ele não tem acesso de Visualização ao objeto. No entanto, o usuário ainda pode aprovar ou rejeitar solicitações de aprovação da página **Página inicial**, conforme descrito em [Aprovando trabalho](../../review-and-approve-work/manage-approvals/approving-work.md).\
  >Por exemplo, o usuário A pertence ao grupo A. O administrador do Workfront restringiu os direitos de acesso do Grupo A para que os usuários desse grupo não possam exibir tarefas no Workfront. Se uma solicitação de aprovação de tarefa for delegada ao Usuário A, o Usuário A não poderá exibir a tarefa à qual a aprovação está associada. No entanto, o usuário A pode aprovar ou rejeitar a solicitação de aprovação da página inicial.

  Para obter informações sobre como o administrador do Workfront pode restringir o acesso a tipos de objetos na Configuração, consulte  [Criar ou modificar níveis de acesso personalizados](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). 

Depois que a delegação de aprovação é interrompida ou cancelada, o usuário designado como aprovador:

* Não tem mais acesso para aprovar trabalho para itens que exigem aprovação
* Continua a ter acesso de Visualização aos itens de trabalho\
  Os usuários que receberam acesso de visualização a objetos por meio de uma delegação de aprovação retêm esse acesso mesmo após a delegação de aprovação parar ou ser cancelada. Para remover o acesso de Visualização a quaisquer objetos aos quais o usuário tinha acesso durante o tempo em que as aprovações estavam sendo delegadas, você deve ir para o objeto e remover os direitos de acesso diretamente do objeto.

## Delegar suas aprovações a outro usuário {#delegate-your-approvals-to-another-user}

Você pode delegar os seguintes tipos de aprovações, independentemente de como a aprovação foi atribuída a você (seja atribuída diretamente a você, a uma equipe da qual você é membro ou à sua função de trabalho):

* Aprovações de projetos
* Aprovações de tarefas
* Aprovações de problemas

Não é possível delegar aprovações de planilhas de horas, documentos ou provas.

Considere o seguinte ao delegar aprovações:

* Quando você delega aprovações, todas as suas aprovações são delegadas. Você não pode delegar solicitações de aprovação individuais.
* Você pode delegar aprovações a apenas um usuário; não pode delegar aprovações a vários usuários ao mesmo tempo.\
  Todas as aprovações de todos os projetos, tarefas e problemas são delegadas ao usuário que você designar.
* No máximo 5 usuários podem delegar aprovações para o mesmo usuário ao mesmo tempo. Em outras palavras, um único usuário não pode ser designado como aprovador temporário para mais de 5 usuários ao mesmo tempo.
* A atividade relacionada às aprovações é exibida na guia Atualizações. Você deve ter a opção Mostrar atualizações do sistema habilitada. O usuário que delega a aprovação e o usuário ao qual as aprovações estão sendo delegadas recebem uma notificação por email sobre a atividade de aprovação.

### Delegar aprovações da área Página inicial


Para delegar aprovações a outro usuário:

1. Clique no **[!UICONTROL Menu Principal]** ![Ícone do Menu Principal](assets/main-menu-icon.png) no canto superior direito e clique em **[!UICONTROL Página Inicial]**.
1. (Condicional) Clique em **Personalizar** para adicionar o widget **Minhas aprovações**.
1. Vá para o widget Minhas aprovações e clique em **Delegar minhas aprovações**.

   >[!NOTE]
   >
   >Os administradores do Workfront podem desativar delegações de aprovação na área de configuração. Se as delegações de aprovação estiverem desativadas, você não verá o botão Delegar aprovações.

   ![Delegar aprovações na página inicial](assets/delegate-approvals-home.png)

1. Especifique as seguintes informações na seção Delegar minhas aprovações:

   * **Nome**: comece a digitar o nome do usuário ao qual deseja delegar aprovações e clique no nome quando ele aparecer no menu suspenso.
   * **Data de início**: selecione a data para que as aprovações comecem a ser encaminhadas. O encaminhamento começa às 12h00 da data que você selecionar.:00\
     A Data inicial deve ser a data atual ou uma data futura.
   * **Data final**: siga um destes procedimentos:
      * Selecione a data para que as aprovações parem de ser encaminhadas. O encaminhamento termina às 23h:59 na data selecionada.
      * Selecione **Nenhuma data de término** para configurar o Workfront para delegar aprovações indefinidamente.

1. Clique em **Salvar**.

### Delegar aprovações do seu perfil de usuário

1. Clique no ícone **Menu principal** > **seu nome** > **Folga** no painel esquerdo.
1. Clique em **Delegar aprovações**.

   >[!NOTE]
   >
   >Os administradores do Workfront podem desativar delegações de aprovação na área de configuração. Se as delegações de aprovação estiverem desativadas, você não verá o botão Delegar aprovações.

1. Especifique as seguintes informações na seção Delegar minhas aprovações:

   * **Nome**: comece a digitar o nome do usuário ao qual deseja delegar aprovações e clique no nome quando ele aparecer no menu suspenso.
   * **Data de início**: selecione a data para que as aprovações comecem a ser encaminhadas. O encaminhamento começa às 12h00 da data que você selecionar.:00\
     A Data inicial deve ser a data atual ou uma data futura.
   * **Data final**: siga um destes procedimentos:
      * Selecione a data para que as aprovações parem de ser encaminhadas. O encaminhamento termina às 23h:59 na data selecionada.
      * Selecione **Nenhuma data de término** para configurar o Workfront para delegar aprovações indefinidamente.

## Atualizar ou interromper uma delegação de aprovações {#update-or-stop-an-approval-delegation}

1. Clique no **[!UICONTROL Menu Principal]** ![Ícone do Menu Principal](assets/main-menu-icon.png) no canto superior direito e clique em **[!UICONTROL Página Inicial]**.
1. (Condicional) Clique em **Personalizar** para adicionar o widget **Minhas aprovações**.

1. Vá para o widget Minhas aprovações e clique em **Editar delegação**.
   ![Editar delegações](assets/edit-delegations.png)
<!--
   Or

   If your system or group administrator enabled task and issue delegation, click **Edit delegation**, then click **Delegate approvals**.   -->

1. (Condicional) Siga um destes procedimentos:

   * Para atualizar a delegação de aprovação existente: Altere as informações exibidas e clique em **Salvar**.

   * Para interromper a delegação existente: clique em **Parar delegação** e em **Parar delegação** para confirmar.

## Exibir aprovações delegadas {#view-delegated-approvals}

Você pode exibir somente os seguintes tipos de delegações de aprovação no widget Minhas aprovações:

* Aprovações de projetos
* Aprovações de tarefas
* Aprovações de problemas

Para exibir aprovações delegadas:

1. Clique no **[!UICONTROL Menu Principal]** ![Ícone do Menu Principal](assets/main-menu-icon.png) no canto superior direito e clique em **[!UICONTROL Página Inicial]**.
1. (Condicional) Clique em **Personalizar** para adicionar o widget **Minhas aprovações**.
1. No widget **Minhas aprovações**, clique no menu suspenso **Filtro** e clique em **Aprovações delegadas**.\
   Todas as aprovações delegadas a você são exibidas na lista.
