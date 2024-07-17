---
product-area: projects
navigation-topic: create-projects
title: Criar um projeto conectado ao Frame.io
description: Um projeto é uma grande unidade de trabalho no Adobe Workfront. Você pode criar projetos do zero, usar um modelo ou converter problemas ou tarefas em projetos.
author: Courtney
feature: Work Management
exl-id: 230d8e62-a3c9-4e38-9b26-5ba1c4f56391
source-git-commit: 49bd393af77a67aa1e3a443c4189569178e99ada
workflow-type: tm+mt
source-wordcount: '1169'
ht-degree: 1%

---

# Criar um projeto conectado ao Frame.io

A integração do Workfront e do Frame.io permite criar projetos no Workfront que são espelhados no Frame.io, fornecendo uma experiência contínua de revisão e aprovação.

Quando um projeto do Workfront é conectado com o Frame.io, é possível

* **Atribuir usuários do Frame.io a tarefas**: os usuários habilitados com Frame.io são notificados por email quando são atribuídos a uma tarefa do Workfront, sinalizando que há trabalho a ser concluído.
* **Compartilhar o projeto com usuários do Frame.io**: quando um projeto é compartilhado com usuários habilitados para Frame.io, eles têm acesso ao projeto dentro do Workfront e do Frame.io.
* **Compartilhar materiais criativos com o Frame.io**: os coordenadores de projetos podem enviar instruções e materiais do Workfront diretamente para o usuário criativo no Frame.io usando uma pasta de projeto de sincronização unidirecional. [!BADGE Em breve]{type=Informative}
* **Rastrear o progresso da tarefa**: os criadores podem enviar os ativos concluídos e marcar as tarefas como concluídas, tudo sem sair do Frame.io.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

>[!IMPORTANT]
>
>Essa funcionalidade está disponível somente para organizações que foram integradas ao [!DNL Adobe Admin Console].

Você deve ter o seguinte:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td> <p>Padrão</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Editar acesso a projetos</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Ao criar um projeto, você recebe automaticamente permissões de gerenciamento para o projeto.</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Pré-requisitos

* Configure a conta padrão Frame.io na área de configuração do Workfront
* Habilitar usuários do Frame.io no perfil de usuário do Workfront

Para obter mais informações sobre os pré-requisitos acima, consulte [Configurar a [!DNL Workfront] e [!DNL Frame.io] integração](/help/quicksilver/administration-and-setup/configure-integrations/configure-wf-and-frame.md).


## Criar um novo modelo de projeto

Ao criar um novo modelo, você pode inserir as informações de todas as tarefas e das futuras configurações do projeto. Essas informações serão transferidas para qualquer projeto criado a partir do modelo.

Os projetos no Frame.io são organizados por equipes, que estão conectadas a grupos do Workfront. Recomendamos usar um modelo de projeto para criar projetos conectados, pois você pode definir o grupo de projetos antes de.

Se você optar por criar o projeto do zero, o Workfront adicionará automaticamente o grupo de projeto Padrão, e o projeto espelho Frame.io será criado na equipe padrão no Frame.io.

>[!NOTE]
>
>A atualização do grupo após a criação do projeto não altera a equipe Frame.io.


### Criar o modelo e especificar o grupo de projeto

{{step1-to-templates}}

1. Clique em **Novo Modelo**.
1. Digite um nome para o modelo e pressione **Enter** para salvar o nome.
1. No painel esquerdo, clique em **Detalhes do Modelo**.
1. Na seção **Associação de modelo**, especifique um grupo. Se você não adicionar um grupo, o grupo de projeto padrão será adicionado e o projeto no Frame.io será criado na equipe padrão correspondente no Frame.io.

Continue para a próxima seção.

![](assets/template-group.png)

### Adicionar tarefas e atribuir usuários habilitados para Frame.io

1. No painel esquerdo, clique em **Tarefas de Modelo**.
1. Clique em **Começar a Adicionar Tarefas de Modelo** para adicionar tarefas rapidamente ao seu modelo. Você pode definir configurações adicionais posteriormente.

   Ou

   Clique em **Nova Tarefa de Modelo** para adicionar uma tarefa de cada vez e definir configurações adicionais.
   ![](assets/add-tasks-to-template.png)
1. Adicione um nome de tarefa.
1. Na área **Atribuições**, atribua usuários ou equipes. Se você atribuir um usuário habilitado para Frame.io, individualmente ou em uma equipe, ele receberá acesso de colaborador ao projeto Frame.io e será notificado sobre a tarefa no projeto Frame.io por email. A partir desse email, eles podem ingressar no projeto Frame.io e começar a trabalhar.
1. Repita as etapas 1 e 2 conforme necessário.

Continue para a próxima seção.

### Configurar detalhes adicionais do modelo

O Workfront tem recursos robustos de gerenciamento de projetos. Recomendamos o uso do artigo [Editar modelos de projeto](/help/quicksilver/manage-work/projects/create-and-manage-templates/edit-templates.md) para configurar as seguintes áreas do modelo:

* Visão geral
* Finanças
* Formulários personalizados
* Parâmetros do projeto
* Configurações de tarefas
* Configurações do problema
* Acesso

### Criar um projeto a partir do modelo

Depois de criar um modelo, você pode usá-lo para criar projetos.

{{step1-to-projects}}

1. Clique em **Novo projeto do modelo**.
1. Usando a caixa de pesquisa, comece digitando o nome do template necessário.
1. Selecione o nome do modelo e clique em **Usar modelo**.
   ![](assets/find-your-template.png)
1. Ajuste qualquer configuração de projeto conforme necessário, em seguida clique em **Criar projeto**.
1. No painel esquerdo, clique em **Documentos**.
1. Use a pasta de sincronização unidirecional para compartilhar automaticamente materiais criativos com o Frame.io. [!BADGE Em breve]{type=Informative}

   >[!NOTE]
   >
   >Este recurso está atualmente em desenvolvimento. Para compartilhar informações com usuários no Frame.io, carregue os arquivos na guia Documento. Quando o status do projeto é definido como Atual, esses arquivos são automaticamente enviados para Frame.io.

1. No cabeçalho do projeto, altere o projeto de **Planning** para **Current**.

Depois que o projeto for criado e a criação fizer upload de ativos concluídos, você poderá atribuir um fluxo de trabalho de revisão e aprovação ao ativo no Workfront. Para obter mais informações, consulte [Criar uma revisão de documento ou solicitação de aprovação](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md). <!-- name may need to change -->

## Criar um novo projeto do zero

Você pode criar um novo projeto do zero conforme necessário.

>[!IMPORTANT]
>
>* Os projetos no Frame.io são organizados por equipes, que estão conectadas a grupos do Workfront. Recomendamos usar um modelo de projeto para criar projetos conectados, pois você pode definir o grupo de projetos antes de.
>
>
>* Se você optar por criar o projeto do zero, o Workfront adicionará automaticamente o grupo de projeto Padrão, e o projeto espelho Frame.io será criado na equipe padrão no Frame.io.
>
>A atualização do grupo após a criação do projeto não altera a equipe Frame.io.

### Criar o projeto

{{step1-to-projects}}

1. Clique em **Novo projeto**.
1. Digite um nome para o seu projeto e pressione **Enter** para salvar o nome.

Continue para a próxima seção.

### Adicionar tarefas e atribuir usuários habilitados para Frame.io

1. No painel esquerdo, clique em **Tarefas**.
1. Clique em **Começar a adicionar tarefas** para adicionar tarefas rapidamente ao seu projeto. Você pode definir configurações adicionais posteriormente.

   Ou

   Clique em **Nova tarefa** para adicionar uma tarefa de cada vez e definir configurações adicionais.
   ![](assets/add-project-tasks.png)
1. Adicione um nome de tarefa.
1. Na área **Atribuições**, atribua usuários ou equipes. Se você atribuir um usuário habilitado para Frame.io, individualmente ou em uma equipe, ele receberá acesso de colaborador ao projeto Frame.io e será notificado sobre a tarefa no projeto Frame.io por email. A partir desse email, eles podem ingressar no projeto Frame.io e começar a trabalhar.
1. Repita as etapas 1 e 2 conforme necessário.

Continue para a próxima seção.

### Fazer upload de materiais criativos

1. No painel esquerdo, clique em **Documentos**.
1. Use a pasta de sincronização unidirecional para compartilhar automaticamente materiais criativos com o Frame.io. [!BADGE Em breve]{type=Informative}

   >[!NOTE]
   >
   >Este recurso está atualmente em desenvolvimento. Para compartilhar informações com usuários no Frame.io, carregue os arquivos na guia Documento. Quando o status do projeto é definido como Atual, esses arquivos enviam automaticamente para o Frame.io

Continue para a próxima seção.

### Configurar detalhes adicionais do projeto

O Workfront tem recursos robustos de gerenciamento de projetos. Recomendamos o uso do artigo [Editar projetos](/help/quicksilver/manage-work/projects/manage-projects/edit-projects.md) para configurar as seguintes áreas do projeto:

* Visão geral
* Finanças
* Formulários personalizados
* Parâmetros do projeto
* Configurações de tarefas
* Configurações do problema
* Acesso

### Definir o projeto para o atual

1. No cabeçalho do projeto, altere o projeto de Planejamento para Atual.
Depois que o projeto for criado e a criação fizer upload de ativos concluídos, você poderá atribuir um fluxo de trabalho de revisão e aprovação ao ativo no Workfront.

Depois que o projeto for criado e a criação fizer upload de ativos concluídos, você poderá atribuir um fluxo de trabalho de revisão e aprovação ao ativo no Workfront.

Para obter mais informações, consulte [Criar uma revisão de documento ou solicitação de aprovação](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md). <!-- name may need to change -->
