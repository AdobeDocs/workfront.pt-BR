---
product-area: agile-and-teams;setup
navigation-topic: create-and-manage-teams
title: Configure o botão Concluído para problemas
description: O botão Concluído pode definir automaticamente o status de uma tarefa ou problema. Por padrão, o Adobe Workfront marca um problema como Resolvido quando um destinatário clica em Concluído em seu item de trabalho.
author: Lisa
feature: People Teams and Groups
exl-id: 2e72854a-2d49-4665-b307-b88f660b141e
source-git-commit: 6c5be4dccff46abbed104f1f1b3c958aaf74d629
workflow-type: tm+mt
source-wordcount: '1115'
ht-degree: 1%

---

# Configure o [!UICONTROL Concluído] botão para problemas

O [!UICONTROL Concluído] pode definir automaticamente o status de uma tarefa ou de um problema. Por padrão, [!DNL Adobe Workfront] marca um problema como [!UICONTROL Resolvido] quando um destinatário clica [!UICONTROL Concluído] no seu item de trabalho.

## Visão geral

Os usuários com certas permissões podem configurar o [!UICONTROL Concluído] para refletir determinados status no sistema. Há 3 maneiras diferentes de [!UICONTROL Concluído] O botão funciona para problemas em [!DNL Workfront]:

* Se o usuário tiver um [!UICONTROL Equipe inicial], a [!DNL Workfront] administrador ou um usuário com uma [!UICONTROL Plano] licença pode configurar o [!UICONTROL Concluído] para refletir determinados status para os membros da equipe. Consulte [Configure o [!UICONTROL Concluído] botão para uma equipe](#configure-the-uicontrol-done-button-for-a-team) neste artigo.
* Se o usuário não tiver uma [!UICONTROL Equipe inicial] atribuído, o [!UICONTROL Concluído] O botão para problemas é vinculado a um sistema [!UICONTROL Resolvido] status que tem o código de três letras [!UICONTROL RLV]. Não há opções de configuração disponíveis neste cenário. O [!UICONTROL Concluído] assume automaticamente esse status como padrão.
* Se a variável [!UICONTROL Resolvido] ([!UICONTROL RLV]) é excluído e o usuário marca o problema como [!UICONTROL Concluído] tem [!UICONTROL Equipe inicial], o status padrão da ocorrência é vinculado ao que for definido como o padrão para [!UICONTROL Fechado] para o grupo atribuído ao projeto, o problema pertence a. O administrador do Workfront pode configurar uma configuração padrão do sistema para o grupo. Consulte [Configure o [!UICONTROL Concluído] quando o botão [!UICONTROL Resolvido] o status foi excluído](#configure-the-uicontrol-done-button-when-the-uicontrol-resolved-status-has-been-deleted) neste artigo.

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] plano*</strong></td> 
   <td> <p>Qualquer Um</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licença*</strong></td> 
   <td> <p>[!UICONTROL Plan] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurações de nível de acesso*</strong></td> 
   <td>O acesso do administrador do sistema é necessário para configurar o botão [!UICONTROL concluído] quando o status [!UICONTROL resolvido] é excluído</td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

## Configure o [!UICONTROL Concluído] botão para uma equipe

Você pode alterar qual status é aplicado ao item de trabalho com a variável [!UICONTROL Concluído] botão. Você também pode definir vários status e permitir que o usuário escolha qual status é apropriado.

1. Clique no botão **[!UICONTROL Menu principal]** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront, em seguida, clique em **[!UICONTROL Equipes]**.

1. Clique no botão **[!UICONTROL Alterar equipe]** em seguida, selecione uma nova equipe no menu suspenso ou pesquise por uma equipe na barra de pesquisa.
1. Clique no botão **[!UICONTROL Mais]** , em seguida, clique em **[!UICONTROL Editar]**.
1. Encontre a **[!UICONTROL Botão Concluído]** na parte inferior do **[!UICONTROL Configurações do grupo]** página.

1. Selecione um status ou mais de um para cada tipo de item de trabalho.

   >[!NOTE]
   >
   >Considere o seguinte ao selecionar os status para tarefas ou problemas:
   >
   >* Quando você seleciona um status para cada tipo de item de trabalho, o status da tarefa ou da emissão é definido para esse status quando um usuário clica em [!UICONTROL Concluído] no seu item. Se você definir vários status para cada tipo de item de trabalho, um menu suspenso será adicionado à variável [!UICONTROL Concluído] e o usuário deve escolher um status para alterar o status no item de trabalho.
   >* Você pode associar somente status de nível de sistema à variável [!UICONTROL Concluído] botão. Não é possível associar status específicos do grupo a status de item de trabalho.
   >* Quando um usuário atribuído ao item coloca o item no status associado ao [!UICONTROL Concluído] botão, o item é exibido como [!UICONTROL Concluído] para esse usuário, independentemente de o status selecionado ser um [!UICONTROL Concluído] ou [!UICONTROL Fechado] status ou status de trabalho.

   >   
   >   
   >  Por exemplo, associar a variável [!UICONTROL Concluído] com Em Andamento faz com que o item de trabalho seja exibido como [!UICONTROL Concluído] para o usuário que altera o status de Novo para Em andamento.
   >   
   >* Os tipos de problemas são personalizáveis e podem ter nomes diferentes dos listados abaixo no seu ambiente.\
      >  A seguir estão as tarefas padrão e os tipos de problema:
      >     
      >   * [!UICONTROL Tarefas]
      >   * [!UICONTROL Problema]
      >   * [!UICONTROL Solicitar]
      >   * [!UICONTROL Pedido de alteração]
      >   * [!UICONTROL Registro de Defeito]


   Se a tarefa ou o problema for atribuído a vários usuários, você verá um &quot;[!UICONTROL Feito com a minha parte]&quot; no menu suspenso, além dos vários status escolhidos para sua equipe.

1. Clique em **[!UICONTROL Salvar alterações]**.

## Associar usuários a uma Equipe Inicial

Para fazer as alterações no [!UICONTROL Concluído] Para tornar a funcionalidade do botão visível para os usuários, é possível tornar a equipe cujas configurações você alterou a Home Team dos usuários.

Para associar usuários a uma Equipe inicial:

1. Clique no botão **[!UICONTROL Menu principal]** ícone ![](assets/main-menu-icon.png) no canto superior direito de [!DNL Adobe Workfront].

1. Clique em **[!UICONTROL Usuários]** e, em seguida, selecione o(s) usuário(s) que deseja associar a uma Equipe Inicial.
1. Clique no botão **[!UICONTROL Mais]** e selecione **[!UICONTROL Editar]**.\
   ![](assets/user-settings-nwe-350x291.png)

1. No **[!UICONTROL Organização]** selecione a **[!UICONTROL Equipe inicial]** campo. Comece a digitar o nome da equipe cujas configurações você deseja associar com os usuários. Clique no nome da equipe quando visualizá-lo na lista.

1. Clique em **[!UICONTROL Salvar alterações]**.\
   Os usuários selecionados agora estão associados a uma Equipe inicial.
Todas as configurações do grupo, incluindo os status associados ao grupo [!UICONTROL Concluído] , agora estão visíveis para esses usuários.

## Configure o [!UICONTROL Concluído] quando o botão [!UICONTROL Resolvido] o status foi excluído

Se um usuário não tiver uma Home Team e o padrão do sistema para [!UICONTROL Resolvido] ([!UICONTROL RLV]) foi excluída, uma [!DNL Workfront] o administrador pode configurar o [!UICONTROL Fechado] status do grupo no projeto. [!DNL Workfront] seleciona esse status para um problema fechado quando o usuário clica no botão [!DNL Done] botão.

### Encontrar o grupo associado ao projeto

Quando um usuário cria um projeto, seu Grupo doméstico é automaticamente atribuído ao projeto. Usuários com [!UICONTROL Gerenciar] o acesso ao projeto pode alterar esse grupo no [!UICONTROL Detalhes do projeto] a qualquer momento. Para entender qual status [!DNL Workfront] O usa para um problema concluído, nesse caso, você deve entender em qual grupo está associado ao projeto o problema e qual é o status padrão de [!UICONTROL Fechado] este grupo tem problemas.

Para localizar o grupo associado ao projeto:

1. Vá para um projeto.
1. No lado esquerdo da página, clique em **[!UICONTROL Detalhes do projeto]**.
1. Localize a variável **[!UICONTROL Associação de projeto]** seção e, em seguida, encontrar **[!UICONTROL Grupo]**.\
   Este é o nome de grupo que você precisa usar para verificar o status na área Configuração. Consulte a seção a seguir para obter instruções sobre como atualizar o status padrão de um grupo específico.

### Atualizar o status padrão de um grupo específico

Como um [!UICONTROL Workfront] administrador, você pode atualizar o status de um grupo específico:

1. Clique no botão **[!UICONTROL Menu principal]** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront, em seguida, clique em **[!UICONTROL Configuração]** ![](assets/gear-icon-settings.png).
1. No painel esquerdo, clique em **[!UICONTROL Preferências do projeto]**, em seguida **[!UICONTROL Status]**.

1. Clique em **[!UICONTROL Problemas]** e digite o nome do grupo no **[!UICONTROL Status do sistema]** caixa de pesquisa localizada à direita.

1. Selecione o grupo.
1. Clique no botão **[!UICONTROL Definir status padrão]** , em seguida, escolha um status padrão para [!UICONTROL Fechado]. [!DNL Workfront] O usa esse status para um problema fechado quando um usuário clica no botão [!UICONTROL Concluído] botão.

   >[!IMPORTANT]
   >
   >Este status é usado somente quando o usuário não tem Equipe Inicial atribuída e a [!UICONTROL RLV] status foi excluído.

1. Clique em **[!UICONTROL Salvar]**.
