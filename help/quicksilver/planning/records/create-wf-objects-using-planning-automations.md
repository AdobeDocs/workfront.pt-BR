---
title: Criar Objetos Workfront usando as automações de registro do Workfront Planning
description: Você pode configurar automações no Workfront Planning que, quando ativadas, criam objetos no Workfront.
feature: Workfront Planning
role: User, Admin
author: Alina, Becky
recommendations: noDisplay, noCatalog
source-git-commit: d8631e16234486479aa70233aa3770b28ea0d218
workflow-type: tm+mt
source-wordcount: '386'
ht-degree: 1%

---


# Criar Objetos Workfront usando as automações de registro do Workfront Planning

Você pode configurar automações no Workfront Planning que, quando ativadas, criam objetos no Workfront.

Ative a automação em registros. O objeto no Workfront é conectado ao registro de Planejamento no qual você ativou a automação.

Por exemplo, você pode criar uma automação que use uma campanha do Workfront Planning e crie um projeto no Workfront para rastrear o progresso dessa campanha. O projeto seria conectado à campanha de Planejamento do Workfront.

Para obter mais informações sobre registros conectados, consulte [Visão geral dos registros conectados](/help/quicksilver/planning/records/connected-records-overview.md).


## Configurar uma automação no Workfront Planning

Você deve configurar uma automação no Workfront Planning antes de usá-la para criar objetos do Workfront.

1. Clique no menu ![](assets/more-menu.png) **Mais** e selecione **Automações**.

   A lista de automações disponíveis é aberta.

1. Clique em **Criar nova automação** no canto superior direito da tela.
1. No campo **Texto do Botão**, digite o texto que você deseja exibir no botão. Os usuários clicarão nesse botão ao usar a automação para criar um objeto do Workfront.
1. (Opcional) Para adicionar um ícone ao botão, selecione um ícone nas opções disponíveis.
1. No campo **Criar um tipo de**, selecione o objeto que deseja que a automação crie.

   Os objetos disponíveis são:

   * Projeto
   * Portfólio
   * Programa
   * Grupo

1. No campo **Selecione o campo a ser usado no nome do projeto**, selecione um campo de registro. O novo projeto no Workfront terá o conteúdo desse campo como seu nome.
1. No campo **Selecione o campo para vincular o projeto criado novamente**, selecione um campo de registro. O novo projeto no Workfront aparecerá nesse campo ao exibir o registro no Workfront Planning.
1. Selecione outras opções como disponíveis para o tipo de objeto que você está criando.
1. Clique em **Criar**

A automação aparece na lista de automações e está disponível para uso em registros.

## Usar uma automação do Workfront Planning para criar um objeto do Workfront

1. No Workfront Planning, abra a página tipo de registro que contém os registros que você deseja usar para criar objetos do Workfront.
1. Selecione um ou mais registros.
1. Clique no botão de automação próximo ao canto inferior direito da tela.

   Neste exemplo, é o botão Criar projeto.

   ![Botão de automação](assets/automation-custom-button.png)

>[!NOTE]
>
>Recomendamos verificar se o objeto foi criado e conectado conforme esperado.

