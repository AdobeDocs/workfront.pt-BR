---
product-area: projects
navigation-topic: approvals
title: Delegar solicitação de aprovação
description: Delegar solicitações de aprovação permite atribuir outro usuário para aprovar suas solicitações por um período de tempo, por exemplo, se você estiver fora do escritório durante as férias.
author: Courtney
feature: Work Management
exl-id: 01b76dd5-98cb-4f0d-97ff-7e665f843a9c
source-git-commit: d04afc0cc55a71e48c357af2ed4446c22dab1ba4
workflow-type: tm+mt
source-wordcount: '1203'
ht-degree: 0%

---

# Delegar solicitação de aprovação

Você pode delegar temporariamente o trabalho ao qual está atribuído enquanto está fora do escritório. Você pode delegar tarefas e emitir atribuições ou pode delegar solicitações de aprovação. Este artigo descreve como delegar solicitações de aprovação. Para obter informações sobre delegação de tarefas e atribuições de emissão, consulte [Gerenciar delegação de tarefa e emissão](../../manage-work/delegate-work/how-to-delegate-work.md).

>[!NOTE]
>
>Para garantir que nenhuma inconsistência ocorra com as datas agendadas para que suas aprovações sejam delegadas, recomendamos que o fuso horário do seu perfil de usuário corresponda ao de seu agendamento. Para obter mais informações, consulte os seguintes artigos:
>
>* [Criar um agendamento](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)
>* [Editar o perfil de um usuário](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)
>


## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><p>Plano Adobe Workfront*</p></td> 
   <td> <p>Qualquer Um</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Licença da Adobe Workfront*</p></td> 
   <td> <p>Revisar ou superior</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano ou tipo de licença você possui, entre em contato com o administrador da Workfront.

## Entender o acesso do usuário para aprovações delegadas

Durante o período de aprovação designado, o usuário para o qual você delega uma solicitação de aprovação tem as seguintes habilidades:

* Pode aprovar ou rejeitar solicitações de aprovação existentes, onde nenhuma decisão foi tomada
* Pode aprovar e rejeitar novas solicitações de aprovação recebidas durante um período de tempo especificado
* É concedido à View acesso a objetos que estão aguardando aprovação

   >[!NOTE]
   >
   > O administrador do Adobe Workfront pode impedir que os usuários acessem determinados tipos de objetos. Quando um usuário não tem acesso a um tipo de objeto e uma aprovação desse tipo é delegada ao usuário, ele não tem acesso de Exibição ao objeto. No entanto, o usuário ainda pode aprovar ou rejeitar solicitações de aprovação do **Início** conforme descrito em [Aprovar trabalho](../../review-and-approve-work/manage-approvals/approving-work.md).\
   Por exemplo, o Usuário A pertence ao Grupo A. O administrador do Workfront restringiu os direitos de acesso do Grupo A para que os usuários desse grupo não possam visualizar as tarefas no Workfront. Se uma solicitação de aprovação de tarefa for delegada ao Usuário A, o Usuário A não poderá visualizar a tarefa à qual a aprovação está associada. No entanto, o Usuário A pode aprovar ou rejeitar a solicitação de aprovação na Página inicial.

   Para obter informações sobre como o administrador do Workfront pode restringir o acesso aos tipos de objetos dentro da Configuração, consulte  [Criar ou modificar níveis de acesso personalizados](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). 

Depois que a delegação de aprovação para ou é cancelada, o usuário designado como aprovador:

* Não tem mais acesso para aprovar o trabalho de itens que exigem aprovação
* Continua a ter acesso de Exibição aos itens de trabalho\
   Os usuários que receberam acesso de Exibição a objetos por meio de uma delegação de aprovação mantêm esse acesso de Exibição mesmo após a delegação de aprovação ser interrompida ou ser recuperada. Para remover o Acesso de visualização a quaisquer objetos aos quais o usuário teve acesso durante o tempo em que as aprovações foram delegadas, você deve ir para o objeto e remover os direitos de acesso diretamente do objeto.

## Delegar solicitações de aprovação na área inicial

* [Delegar suas aprovações a outro usuário](#delegate-your-approvals-to-another-user)
* [Atualizar ou parar uma delegação de aprovação](#update-or-stop-an-approval-delegation)
* [Exibir aprovações delegadas](#view-delegated-approvals)

### Delegar suas aprovações a outro usuário {#delegate-your-approvals-to-another-user}

Você pode delegar os seguintes tipos de aprovações, independentemente de como a aprovação foi atribuída a você (se atribuída diretamente a você, a uma equipe da qual você é membro ou à sua função de trabalho):

* Aprovações de projeto
* Aprovações de tarefa
* Emitir aprovações

Não é possível delegar aprovações de folha de ponto e documento. 

Considere o seguinte ao delegar aprovações:

* Quando você delega aprovações, todas elas são delegadas. Não é possível delegar solicitações de aprovação individuais.
* Você pode delegar aprovações a apenas um usuário; não é possível delegar aprovações a vários usuários ao mesmo tempo.\
   Todas as aprovações para todos os projetos, tarefas e problemas são delegadas ao usuário designado.
* No máximo 5 usuários podem delegar aprovações ao mesmo usuário ao mesmo tempo. Em outras palavras, um único usuário não pode ser designado como um aprovador temporário para mais de 5 usuários ao mesmo tempo.
* A atividade relacionada às aprovações é exibida na guia Atualizações . Você deve ativar Mostrar atualizações do sistema. Tanto o usuário que delega a aprovação quanto o usuário para o qual as aprovações estão sendo delegadas recebem uma notificação por email sobre a atividade de aprovação.

Para delegar aprovações a outro usuário:

1. Clique no botão **Início** ícone ![](assets/home-icon-30x29.png) no canto superior esquerdo do Adobe Workfront.

   >[!NOTE]
   O administrador do Workfront pode fazer as seguintes alterações no ícone Início no seu ambiente:
   * Substitua por uma imagem personalizada para ilustrar sua organização. Nesse caso, o ícone terá uma aparência diferente da mostrada neste artigo.
   * Substitua a página vinculada a ela por uma página diferente. Nesse caso, clique no botão **Menu principal** ![](assets/main-menu-icon.png) no canto superior direito da página, em seguida, clique em **Início**.


   Ou

   Clique no botão **Menu principal** ícone > **seu nome** > **Hora de desligar** no painel esquerdo.

1. (Opcional e condicional) Na área Início, clique no botão **Filtro** menu suspenso e, em seguida, clique em **Aprovações**.

1. (Condicional) Clique em **Delegar Minhas Aprovações**

   Ou

   Se o administrador do sistema ou grupo ativou a delegação de tarefas e problemas, clique em **Delegar**, depois clique em **Delegar aprovações**.

   ![](assets/delegate-approvals-nwe.png)

1. Especifique as seguintes informações na seção Delegar minhas aprovações :

   * **Nome**: Comece digitando o nome do usuário para o qual você deseja delegar aprovações e clique no nome quando ele for exibido no menu suspenso.
   * **Data de início**: Selecione a data para as aprovações começarem a ser encaminhadas. O encaminhamento começa às 12:00 da manhã, na data selecionada.\
      A Data de início deve ser a data atual ou uma data futura.
   * **Data final**:execute um dos seguintes procedimentos:

      * Selecione a data em que as aprovações devem parar de ser encaminhadas. O encaminhamento termina às 23:59 na data selecionada.
      * Selecionar **Sem data final** para configurar o Workfront para delegar aprovações indefinidamente.

1. Clique em **Salvar**.

### Atualizar ou parar uma delegação de aprovação {#update-or-stop-an-approval-delegation}

1. Clique no botão **Início** ícone ![](assets/home-icon-30x29.png) no canto superior esquerdo do Adobe Workfront.

   >[!NOTE]
   O administrador do Workfront pode fazer as seguintes alterações no ícone Início no seu ambiente:
   * Substitua por uma imagem personalizada para ilustrar sua organização. Nesse caso, o ícone terá uma aparência diferente da mostrada neste artigo.
   * Substitua a página vinculada a ela por uma página diferente. Nesse caso, clique no botão **Menu principal** ![](assets/main-menu-icon.png) no canto superior direito da página, em seguida, clique em **Início**.


1. Clique no botão **Filtro** menu suspenso e, em seguida, clique em **Aprovações**.

1. (Condicional) Clique em **Editar delegação**

   Ou

   Se a tarefa do sistema ou do administrador de grupo ativou e emitiu a delegação, clique em **Editar delegação**, depois clique em **Delegar aprovações**.

1. (Condicional) Siga um destes procedimentos:

   * Para atualizar a delegação de aprovação existente: Altere as informações exibidas e clique em **Salvar**.

   * Para interromper a delegação existente: Clique em **Parar delegação**, depois clique em **Parar delegação** para confirmar.

      ![](assets/stop-delegation-nwe.png)

### Exibir aprovações delegadas {#view-delegated-approvals}

Você pode exibir somente os seguintes tipos de delegações de aprovação na Lista de Trabalho:

* Aprovações de projeto
* Aprovações de tarefa
* Emitir aprovações

Para exibir aprovações delegadas:

1. Clique no botão **Início** ícone ![](assets/home-icon-30x29.png) no canto superior esquerdo do Adobe Workfront.

   >[!NOTE]
   O administrador do Workfront pode fazer as seguintes alterações no ícone Início no seu ambiente:
   * Substitua por uma imagem personalizada para ilustrar sua organização. Nesse caso, o ícone terá uma aparência diferente da mostrada neste artigo.
   * Substitua a página vinculada a ela por uma página diferente. Nesse caso, clique no botão **Menu principal** ![](assets/main-menu-icon.png) no canto superior direito da página, em seguida, clique em **Início**.


1. Clique no botão **Filtro** menu suspenso e, em seguida, clique em **Aprovações**.\
   Todas as aprovações são exibidas na lista por padrão, incluindo aprovações atribuídas a você e aprovações delegadas a você.

   ![](assets/delegated-to-me-nwe-350x93.png)
