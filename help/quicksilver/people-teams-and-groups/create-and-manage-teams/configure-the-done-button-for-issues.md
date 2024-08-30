---
product-area: agile-and-teams;setup
navigation-topic: create-and-manage-teams
title: Configurar o botão Concluído para Problemas
description: O botão Concluído pode definir automaticamente o status de uma tarefa ou problema. Por padrão, o Adobe Workfront marca um problema como Resolvido quando um destinatário clica em Concluído no item de trabalho.
author: Lisa
feature: People Teams and Groups
exl-id: 2e72854a-2d49-4665-b307-b88f660b141e
source-git-commit: dfd5c7423b65e6065ab9c2094578443b81189abd
workflow-type: tm+mt
source-wordcount: '1170'
ht-degree: 1%

---

# Configure o botão [!UICONTROL Concluído] para problemas

O botão [!UICONTROL Concluído] pode definir automaticamente o status de uma tarefa ou problema. Por padrão, [!DNL Adobe Workfront] marca um problema como [!UICONTROL Resolvido] quando um destinatário clica em [!UICONTROL Concluído] em seu item de trabalho.

## Visão geral

Os usuários com determinadas permissões podem configurar o botão [!UICONTROL Concluído] para refletir determinados status no sistema. Há 3 maneiras diferentes de o botão [!UICONTROL Concluído] funcionar para problemas no [!DNL Workfront]:

* Se o usuário tiver uma [!UICONTROL Equipe interna] atribuída, um administrador [!DNL Workfront] ou um usuário com uma licença [!UICONTROL Plano] poderá configurar o botão [!UICONTROL Concluído] para refletir determinados status para os membros da equipe. Consulte [Configurar o botão [!UICONTROL Concluído] para uma Equipe](#configure-the-uicontrol-done-button-for-a-team) neste artigo.
* Se o usuário não tiver uma [!UICONTROL Equipe interna], mas tiver [!UICONTROL Outras equipes] em seu perfil, a Workfront procurará a configuração do botão [!UICONTROL Concluído] em qualquer uma das equipes associadas ao usuário. A seleção é aleatória e o status associado a qualquer uma das equipes é usado para o problema.
* Se o usuário não tiver uma [!UICONTROL Equipe interna] atribuída, o botão [!UICONTROL Concluído] para problemas estará vinculado a um status gerado pelo sistema [!UICONTROL Resolvido] com o código de três letras [!UICONTROL RLV]. Não há opções de configuração disponíveis neste cenário. O botão [!UICONTROL Concluído] define automaticamente este status como padrão.
* Se o status de [!UICONTROL Resolvido] ([!UICONTROL RLV]) for excluído e o usuário que estiver marcando o problema como [!UICONTROL Concluído] não tiver nenhuma [!UICONTROL Equipe Doméstica], o status padrão do problema será vinculado ao que for definido como o padrão para [!UICONTROL Fechado] para o grupo atribuído ao projeto ao qual o problema pertence. O administrador do Workfront pode definir uma configuração padrão em todo o sistema para o grupo. Consulte [Configurar o botão [!UICONTROL Concluído] quando o status [!UICONTROL Resolvido] for excluído](#configure-the-uicontrol-done-button-when-the-uicontrol-resolved-status-has-been-deleted) neste artigo.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>plano do Adobe Workfront</p> </td> 
   <td>Qualquer</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td>
   <p>Novo: Padrão</p>
   <p>ou</p>
   <p>Atual: Plano</p></td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>É necessário acesso de administrador do sistema para configurar o botão Concluído quando o status Resolvido for excluído</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Configurar o botão [!UICONTROL Concluído] para uma equipe

Você pode alterar o status aplicado ao item de trabalho com o botão [!UICONTROL Concluído]. Você também pode definir vários status e permitir que o usuário escolha qual status é apropriado.

{{step1-to-team}}

1. Clique no ícone **[!UICONTROL Trocar equipe]** e selecione uma nova equipe no menu suspenso ou procure uma equipe na barra de pesquisa.
1. Clique no menu **[!UICONTROL Mais]** e em **[!UICONTROL Editar]**.
1. Localize a seção **[!UICONTROL Botão Concluído]** na parte inferior da página **[!UICONTROL Configurações de Equipe]**.

1. Selecione um ou mais status para cada tipo de item de trabalho.

   >[!NOTE]
   >
   >Considere o seguinte ao selecionar status para tarefas ou problemas:
   >
   >* Quando você seleciona um status para cada tipo de item de trabalho, o status da tarefa ou problema é definido para esse status quando um usuário clica em [!UICONTROL Concluído] no item. Se você definir vários status para cada tipo de item de trabalho, um menu suspenso será adicionado ao botão [!UICONTROL Concluído] e o usuário deverá escolher um status para alterar o status no item de trabalho.
   >* Você pode associar somente os status de nível de sistema ao botão [!UICONTROL Concluído]. Você não pode associar status específicos de Grupo a status de item de trabalho.
   >* Quando um usuário atribuído ao item coloca o item no status associado ao botão [!UICONTROL Concluído], o item é exibido como [!UICONTROL Concluído] para esse usuário, independentemente do status selecionado ser [!UICONTROL Concluído] ou [!UICONTROL Fechado] ou um status de trabalho.
   >   
   >   
   >  Por exemplo, associar o botão [!UICONTROL Concluído] a Em andamento faz com que o item de trabalho seja exibido como [!UICONTROL Concluído] para o usuário que altera o status de Novo para Em andamento.
   >   
   >* Os tipos de problemas são personalizáveis e podem ter nomes diferentes dos listados abaixo em seu ambiente.\
   >  A seguir estão as tarefas padrão e os tipos de problemas:
   >     
   >   * [!UICONTROL Tarefas]
   >   * [!UICONTROL Problema]
   >   * [!UICONTROL Solicitar]
   >   * [!UICONTROL Pedido de alteração]
   >   * [!UICONTROL Relatório de erro]

   Se a tarefa ou problema for atribuído a vários usuários, você verá a opção &quot;[!UICONTROL Concluído com minha parte]&quot; no menu suspenso, além dos vários status escolhidos para sua equipe.

1. Clique em **[!UICONTROL Salvar alterações]**.

## Associar usuários a uma Equipe interna

Para tornar as alterações na funcionalidade de botão [!UICONTROL Concluído] visíveis para os usuários, você pode tornar a equipe cujas configurações você alterou a Equipe inicial dos usuários.

Para associar usuários a uma Equipe da Página Inicial:

1. Clique no ícone ![](assets/main-menu-icon.png) do **[!UICONTROL Menu Principal]** no canto superior direito de [!DNL Adobe Workfront].

1. Clique em **[!UICONTROL Usuários]** e selecione o(s) usuário(s) que deseja associar a uma Equipe interna.
1. Clique no menu **[!UICONTROL Mais]** e selecione **[!UICONTROL Editar]**.\
   ![](assets/user-settings-nwe-350x291.png)

1. Na seção **[!UICONTROL Organização]**, selecione o campo **[!UICONTROL Equipe interna]**. Comece digitando o nome da equipe cujas configurações você deseja associar aos usuários. Clique no nome da equipe ao ser exibido na lista.

1. Clique em **[!UICONTROL Salvar alterações]**.\
   Os usuários selecionados agora estão associados a uma Equipe interna.
Todas as configurações do grupo, incluindo os status associados ao botão [!UICONTROL Concluído], agora estão visíveis para esses usuários.

## Configure o botão [!UICONTROL Concluído] quando o status [!UICONTROL Resolvido] for excluído

Se um usuário não tiver uma Equipe Inicial e o padrão em todo o sistema para [!UICONTROL Resolvido] ([!UICONTROL RLV]) tiver sido excluído, um administrador [!DNL Workfront] poderá configurar o status [!UICONTROL Fechado] para o grupo no projeto. [!DNL Workfront] seleciona este status para um problema encerrado quando o usuário clica no botão [!DNL Done].

### Localizar o grupo associado ao projeto

Quando um usuário cria um projeto, seu Grupo inicial é automaticamente atribuído ao projeto. Usuários com acesso de [!UICONTROL Gerenciar] ao projeto podem alterar este grupo na seção [!UICONTROL Detalhes do Projeto] a qualquer momento. Para entender qual status [!DNL Workfront] usa para um problema concluído neste caso, você deve entender qual grupo está associado ao projeto em que o problema está e qual é o status padrão para [!UICONTROL Fechado] este grupo tem para problemas.

Para localizar o grupo associado ao projeto:

1. Ir para um Projeto.
1. No lado esquerdo da página, clique em **[!UICONTROL Detalhes do projeto]**.
1. Localize a seção **[!UICONTROL Associação do projeto]** e, em seguida, localize o **[!UICONTROL Grupo]**.\
   Esse é o nome do grupo que você precisa usar para verificar o status na área Configuração. Consulte a seção a seguir para obter instruções sobre como atualizar o status padrão de um grupo específico.

### Atualizar o status padrão de um grupo específico

Como administrador do [!UICONTROL Workfront], você pode atualizar o status de um grupo específico:

1. Clique no ícone ![](assets/main-menu-icon.png) do **[!UICONTROL Menu Principal]** no canto superior direito do Adobe Workfront e em **[!UICONTROL Configurar]** ![](assets/gear-icon-settings.png).
1. No painel esquerdo, clique em **[!UICONTROL Preferências do projeto]** e em **[!UICONTROL Status]**.

1. Clique em **[!UICONTROL Problemas]** e digite o nome do grupo na caixa de pesquisa **[!UICONTROL Status do sistema]**, localizada à direita.

1. Selecione o grupo.
1. Clique no menu suspenso **[!UICONTROL Definir Status Padrão]** e escolha um status padrão para [!UICONTROL Fechado]. [!DNL Workfront] usa este status para um problema encerrado quando um usuário clica no botão [!UICONTROL Concluído].

   >[!IMPORTANT]
   >
   >Este status é usado somente quando o usuário não tem nenhuma Equipe Inicial atribuída e o status [!UICONTROL RLV] foi excluído.

1. Clique em **[!UICONTROL Salvar]**.
