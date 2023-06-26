---
product-area: agile-and-teams;setup
navigation-topic: create-and-manage-teams
title: Configurar o botão Concluído para problemas
description: O botão Concluído pode definir automaticamente o status de uma tarefa ou problema. Por padrão, o Adobe Workfront marca um problema como Resolvido quando um destinatário clica em Concluído no item de trabalho.
author: Lisa
feature: People Teams and Groups
exl-id: 2e72854a-2d49-4665-b307-b88f660b141e
source-git-commit: 1f749ba9a54ce75a917e4b1e95713ac7abeaa66b
workflow-type: tm+mt
source-wordcount: '1168'
ht-degree: 1%

---

# Configure o [!UICONTROL Concluído] botão para problemas

A variável [!UICONTROL Concluído] pode definir automaticamente o status de uma tarefa ou problema. Por padrão, [!DNL Adobe Workfront] marca um problema como [!UICONTROL Resolvido] quando um destinatário clicar [!UICONTROL Concluído] em seu item de trabalho.

## Visão geral

Os usuários com determinadas permissões podem configurar o [!UICONTROL Concluído] para refletir determinados status no sistema. Existem 3 maneiras diferentes de [!UICONTROL Concluído] botão funciona para problemas no [!DNL Workfront]:

* Se o usuário tiver um atribuído [!UICONTROL Equipe interna], um [!DNL Workfront] administrador ou um usuário com uma [!UICONTROL Plano] a licença pode configurar o [!UICONTROL Concluído] para refletir determinados status para os membros da equipe. Consulte [Configure o [!UICONTROL Concluído] botão para uma Equipe](#configure-the-uicontrol-done-button-for-a-team) neste artigo.
* Se o usuário não tiver uma [!UICONTROL Equipe interna], mas eles têm [!UICONTROL Outras equipes] em seu perfil, o Workfront procura a configuração da variável [!UICONTROL Concluído] em qualquer equipe associada ao usuário. A seleção é aleatória e o status associado a qualquer uma das equipes é usado para o problema.
* Se o usuário não tiver uma [!UICONTROL Equipe interna] atribuído, o [!UICONTROL Concluído] para problemas está vinculado a um evento gerado pelo sistema [!UICONTROL Resolvido] status que tem o código de três letras [!UICONTROL RLV]. Não há opções de configuração disponíveis neste cenário. A variável [!UICONTROL Concluído] automaticamente assume esse status como padrão.
* Se a variável [!UICONTROL Resolvido] ([!UICONTROL RLV]) for excluído e o usuário marcar o problema como [!UICONTROL Concluído] não tem [!UICONTROL Equipe interna], o status padrão do problema será vinculado ao que for definido como o padrão para [!UICONTROL Fechado] para o grupo atribuído ao projeto ao qual o problema pertence. O administrador do Workfront pode definir uma configuração padrão em todo o sistema para o grupo. Consulte [Configure o [!UICONTROL Concluído] botão quando a variável [!UICONTROL Resolvido] O status foi excluído](#configure-the-uicontrol-done-button-when-the-uicontrol-resolved-status-has-been-deleted) neste artigo.

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas deste artigo:

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
   <td> <p>[!UICONTROL Plano] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurações de nível de acesso*</strong></td> 
   <td>O acesso de administrador do sistema é necessário para configurar o botão [!UICONTROL Concluído] quando o status [!UICONTROL Resolvido] for excluído</td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir seu plano, tipo de licença ou acesso, entre em contato com o administrador do Workfront.

## Configure o [!UICONTROL Concluído] botão para uma Equipe

Você pode alterar qual status é aplicado ao item de trabalho com o [!UICONTROL Concluído] botão. Você também pode definir vários status e permitir que o usuário escolha qual status é apropriado.

1. Clique em **[!UICONTROL Menu principal]** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront e clique em **[!UICONTROL Equipes]**.

1. Clique em **[!UICONTROL Trocar equipe]** , selecione uma nova equipe no menu suspenso ou procure uma equipe na barra de pesquisa.
1. Clique em **[!UICONTROL Mais]** e clique em **[!UICONTROL Editar]**.
1. Localize o **[!UICONTROL Botão Concluído]** na parte inferior do **[!UICONTROL Configurações da equipe]** página.

1. Selecione um ou mais status para cada tipo de item de trabalho.

   >[!NOTE]
   >
   >Considere o seguinte ao selecionar status para tarefas ou problemas:
   >
   >* Quando você seleciona um status para cada tipo de item de trabalho, o status da tarefa ou do problema é definido para esse status quando um usuário clica em [!UICONTROL Concluído] em seu item. Se você definir vários status para cada tipo de item de trabalho, um menu suspenso será adicionado à [!UICONTROL Concluído] e o usuário deve escolher um status para alterar o status no item de trabalho.
   >* Você pode associar somente os status de nível de sistema com o [!UICONTROL Concluído] botão. Você não pode associar status específicos de Grupo a status de item de trabalho.
   >* Quando um usuário atribuído ao item coloca o item no status associado à [!UICONTROL Concluído] , o item é exibido como [!UICONTROL Concluído] para esse usuário, independentemente de o status selecionado ser um [!UICONTROL Concluído] ou [!UICONTROL Fechado] ou um estado de trabalho.
   >   
   >   
   >  Por exemplo, associar a variável [!UICONTROL Concluído] botão com Em andamento faz com que o item de trabalho seja exibido como [!UICONTROL Concluído] para o usuário que altera o status de Novo para Em andamento.
   >   
   >* Os tipos de problemas são personalizáveis e podem ter nomes diferentes dos listados abaixo em seu ambiente.\
   >  A seguir estão as tarefas padrão e os tipos de problemas:
   >     
   >   * [!UICONTROL Tarefas]
   >   * [!UICONTROL Problema]
   >   * [!UICONTROL Solicitar]
   >   * [!UICONTROL Pedido de alteração]
   >   * [!UICONTROL Registro de Defeito]

   Se a tarefa ou o problema for atribuído a vários usuários, você verá um &quot;[!UICONTROL Pronto com minha parte]&quot; no menu suspenso, além dos vários status escolhidos para sua equipe.

1. Clique em **[!UICONTROL Salvar alterações]**.

## Associar usuários a uma Equipe interna

Para fazer as alterações no [!UICONTROL Concluído] funcionalidade de botão visível para os usuários, você pode tornar a equipe cujas configurações você alterou a Equipe inicial dos usuários.

Para associar usuários a uma Equipe da Página Inicial:

1. Clique em **[!UICONTROL Menu principal]** ícone ![](assets/main-menu-icon.png) no canto superior direito de [!DNL Adobe Workfront].

1. Clique em **[!UICONTROL Usuários]**, em seguida, selecione o(s) usuário(s) que deseja associar a uma Equipe interna.
1. Clique em **[!UICONTROL Mais]** e selecione **[!UICONTROL Editar]**.\
   ![](assets/user-settings-nwe-350x291.png)

1. No **[!UICONTROL Organização]** , selecione a **[!UICONTROL Equipe interna]** campo. Comece digitando o nome da equipe cujas configurações você deseja associar aos usuários. Clique no nome da equipe ao ser exibido na lista.

1. Clique em **[!UICONTROL Salvar alterações]**.\
   Os usuários selecionados agora estão associados a uma Equipe interna.
Quaisquer configurações do grupo, incluindo os status associados à [!UICONTROL Concluído] agora estão visíveis para esses usuários.

## Configure o [!UICONTROL Concluído] botão quando a variável [!UICONTROL Resolvido] O status foi excluído

Se um usuário não tiver uma Equipe interna e o padrão em todo o sistema para [!UICONTROL Resolvido] ([!UICONTROL RLV]) foi excluída, uma [!DNL Workfront] o administrador pode configurar o [!UICONTROL Fechado] status do grupo no projeto. [!DNL Workfront] seleciona este status para um problema encerrado quando o usuário clica em [!DNL Done] botão.

### Localizar o grupo associado ao projeto

Quando um usuário cria um projeto, seu Grupo inicial é automaticamente atribuído ao projeto. Usuários com [!UICONTROL Gerenciar] o acesso ao projeto pode alterar esse grupo no [!UICONTROL Detalhes do projeto] a qualquer momento. Para entender qual status [!DNL Workfront] O usa para um problema concluído neste caso, você deve entender em qual grupo está associado ao projeto o problema e qual é o status padrão [!UICONTROL Fechado] este grupo tem problemas.

Para localizar o grupo associado ao projeto:

1. Ir para um Projeto.
1. No lado esquerdo da página, clique em **[!UICONTROL Detalhes do projeto]**.
1. Localize o **[!UICONTROL Associação de projeto]** seção e, em seguida, localizar **[!UICONTROL Grupo]**.\
   Esse é o nome do grupo que você precisa usar para verificar o status na área Configuração. Consulte a seção a seguir para obter instruções sobre como atualizar o status padrão de um grupo específico.

### Atualizar o status padrão de um grupo específico

Como um [!UICONTROL Workfront] administrador, você pode atualizar o status de um grupo específico:

1. Clique em **[!UICONTROL Menu principal]** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront e clique em **[!UICONTROL Configuração]** ![](assets/gear-icon-settings.png).
1. No painel esquerdo, clique em **[!UICONTROL Preferências do projeto]**, depois **[!UICONTROL Status]**.

1. Clique em **[!UICONTROL Problemas]**, em seguida, digite o nome do grupo no campo **[!UICONTROL Status do sistema]** caixa de pesquisa localizada à direita.

1. Selecione o grupo.
1. Clique em **[!UICONTROL Definir status padrão]** e escolha um status padrão para [!UICONTROL Fechado]. [!DNL Workfront] O usa esse status para um problema encerrado quando um usuário clica em [!UICONTROL Concluído] botão.

   >[!IMPORTANT]
   >
   >Esse status é usado somente quando o usuário não tem nenhuma Equipe inicial atribuída e a [!UICONTROL RLV] O status de foi excluído.

1. Clique em **[!UICONTROL Salvar]**.
