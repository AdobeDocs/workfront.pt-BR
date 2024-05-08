---
product-area: projects
navigation-topic: approvals
title: Conectar o Workfront e o Frame.io
description: O Workfront usa o Frame.io no processo de revisão e aprovação para atender às pessoas onde elas desejam trabalhar. O processo de gerenciamento e aprovação de projetos é gerenciado no Workfront e o processo de revisão é feito no Frame.io.
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: 8529b4d5-9732-4dd6-bf81-191aea1ed68c
source-git-commit: a8a5205616a0bf30c5ba4b27a2ffb9fae4d52ac4
workflow-type: tm+mt
source-wordcount: '633'
ht-degree: 0%

---

# Conectar o Workfront e o Frame.io

>[!IMPORTANT]
>
>O conteúdo deste artigo se refere à funcionalidade atualizada de aprovação de documentos, disponível somente para contas específicas. Para obter informações sobre processos de aprovação padrão, consulte os artigos listados em [Aprovações de trabalho](/help/quicksilver/review-and-approve-work/manage-approvals/manage-approvals.md).

O Workfront usa o Frame.io no processo de revisão e aprovação para atender às pessoas onde elas desejam trabalhar. O processo de gerenciamento e aprovação de projetos é gerenciado no Workfront e o processo de revisão é concluído no Frame.io. Você deve concluir todas as seções a seguir para configurar a integração com êxito:

* [Conectar um grupo do Workfront a uma equipe do Frame.io](#connect-a-workfront-group-to-a-frameio-team)
* [Criar um projeto do Workfront e adicionar um grupo conectado](#create-a-workfront-project-and-add-a-connected-group)



## Requisitos de acesso

* Sua organização deve ser integrada manualmente à versão beta para usar a funcionalidade descrita neste artigo. Para obter mais informações, consulte [Integração nativa do Adobe Workfront e Frame.io beta](/help/quicksilver/review-and-approve-work/Documents/wf-frame-alpha.md).


## Conectar um grupo do Workfront a uma equipe do Frame.io

Estamos aprimorando ativamente esse recurso para disponibilidade geral em maio.

### Pré-requisitos

* Crie uma equipe do Frame.io para mapear para um grupo do Workfront.
* Encontre o token de desenvolvedor da API da equipe. Para obter mais informações, consulte [Tokens de desenvolvedor](https://developer.frame.io/docs/getting-started/authentication#developer-tokens) no site do desenvolvedor Frame.io.

### Conectar um grupo do Workfront a uma equipe do Frame.io

{{step-1-to-setup}}

1. No painel esquerdo, clique em **Grupos**.
1. Escolha um grupo existente ou clique em **Criar grupo**.
1. No painel esquerdo, clique em **Conectar ao Frame.io**.
   ![](assets/connect-frame-group.png)
1. Insira o token do desenvolvedor de API.
1. Clique em **Iniciar conexão**.
1. (Condicional) Se você for o administrador de mais de uma conta Frame.io, selecione a conta que deseja usar.

## Criar um projeto do Workfront e adicionar um grupo conectado

Depois de conectar um Grupo Workfront a uma equipe Frame.io, você deve criar um projeto com esse grupo conectado.

### Pré-requisitos

* Você deve ter um grupo do Workfront conectado a uma equipe do Frame.io, conforme explicado na seção anterior.

### Criar um projeto do Workfront e adicionar um grupo conectado

{{step1-to-projects}}

1. Crie um novo projeto do zero ou um modelo. Para obter informações sobre como criar um projeto, consulte [Criar um projeto](/help/quicksilver/manage-work/projects/create-projects/create-project.md).

1. No painel esquerdo, localize **Detalhes do projeto**.

1. Localize o **Grupo** no lado direito da tela e remova o grupo Padrão.

1. No menu suspenso, localize o grupo desejado. Grupos conectados ao Frame.io exibem o ícone Frame.io.
   ![](assets/add-frame-group.png)

1. Faça qualquer outra alteração de configuração de projeto.

1. Clique em **Salvar alterações**.

1. Continue para a próxima seção.

### Adicione uma tarefa e defina o status de integração como Ativo

>[!NOTE]
>
>Atualmente, as subtarefas não são suportadas em projetos Frame.io conectados.


1. Crie as tarefas que você precisa preencher no Frame.io

1. Selecione as tarefas necessárias e clique em **Editar**.

1. Role para a **Forms personalizado** e localize o formulário de integração Frame.io.

   >[!IMPORTANT]
   >
   >Um grupo Frame.io conectado deve ser atribuído na área Detalhes do projeto para que este formulário seja exibido. Para obter mais informações, consulte [Criar um projeto do Workfront e adicionar um grupo conectado](#create-a-workfront-project-and-add-a-connected-group) neste artigo.


1. Ativar o **Status de integração desta tarefa** e escolha **Ativo**.
   ![](assets/frame-custom-form.png)

1. Clique em **Salvar alterações**. Um ícone Frame.io é exibido ao lado do nome do projeto.

1. Atribuir usuários ou equipes a tarefas.

   >[!NOTE]
   >
   >Usuários ou equipes adicionados às tarefas também são adicionados ao projeto Frame.io.

1. Faça upload de qualquer documento ou resumo criativo na área Documentos do projeto.

O projeto ainda não está conectado. Você deve continuar com a próxima seção para concluir a integração.

### Habilitar o projeto no Frame.io

1. Alterar o status do projeto de **Planejamento** para **Atual** ou um status personalizado igual ao atual. Isso conclui a integração e gera o projeto, as tarefas e quaisquer documentos no Frame.io.

O ícone Frame.io ao lado do nome do projeto fica roxo, sinalizando que a integração foi bem-sucedida. Os usuários recebem um email convidando-os para o projeto Frame.io.

>[!IMPORTANT]
>
>Uma vez que o projeto esteja conectado ao Frame.io, as alterações feitas no grupo do projeto não são refletidas no Frame.io.
