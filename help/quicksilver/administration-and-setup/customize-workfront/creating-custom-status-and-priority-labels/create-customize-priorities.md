---
title: Criar e personalizar prioridades
description: Você pode controlar as prioridades de projetos, tarefas e problemas na área Configuração do Workfront. As prioridades dão importância aos seus projetos, tarefas ou problemas no Adobe Workfront.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 6e7952cf-f07a-412b-9f9a-623cdba46849
source-git-commit: 7db80f5bacf52b7bbe540f4e38e88853af86a5e2
workflow-type: tm+mt
source-wordcount: '761'
ht-degree: 1%

---

# Criar e personalizar prioridades

{{highlighted-preview}}

<!--
DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.
-->

Você pode controlar as prioridades de projetos, tarefas e problemas na área Configuração do Workfront. As prioridades dão importância aos seus projetos, tarefas ou problemas no Adobe Workfront.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte acesso para executar as etapas deste artigo:

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
   <td>
     <p>Novo: Padrão</p>
     <p>ou</p>
     <p>Atual: Plano</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td>[!UICONTROL Administrador do Sistema]</td>
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Personalização de prioridades existentes

Como administrador do Workfront, você pode fazer as seguintes modificações nas prioridades padrão fornecidas no Workfront:

* Renomear prioridades.
* Reordene as prioridades.

  Para obter mais informações sobre como reordenar prioridades, consulte [Criar uma prioridade para um projeto, tarefa ou problema](#create-a-priority-for-a-project-task-or-issue).

* Altere a prioridade padrão.

  Para obter mais informações sobre a funcionalidade de alterar a prioridade padrão, consulte [Criar uma prioridade para um projeto, tarefa ou problema](#create-a-priority-for-a-project-task-or-issue).

* Edite a descrição das prioridades.
* Defina uma cor para cada prioridade.

  A cor da prioridade é usada nos relatórios de gráfico, quando você agrupa seus resultados por **Prioridade**.

  Para obter mais informações sobre relatórios de gráficos, consulte [Adicionar um gráfico a um relatório](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md).

* Excluir prioridades.

  Quando você exclui uma prioridade existente, deve selecionar uma prioridade substituta.

* Ocultar prioridades.

  Para obter mais informações sobre a funcionalidade de ocultar prioridades, consulte [Criar uma prioridade para um projeto, tarefa ou problema](#create-a-priority-for-a-project-task-or-issue).

  >[!NOTE]
  >
  >Você deve ter pelo menos uma prioridade em sua conta do Workfront para cada objeto.

As prioridades fornecidas por padrão para cada tipo de objeto (projeto, tarefa e problema) são idênticas:

* Nenhum(a)
* Baixa
* Normal
* Alta
* Urgente

## Criar uma prioridade para um projeto, tarefa ou problema {#create-a-priority-for-a-project-task-or-issue}

Além das prioridades padrão fornecidas no Workfront, você pode adicionar suas próprias prioridades para refletir as necessidades de sua organização.

{{step-1-to-setup}}

1. No painel esquerdo, clique em **Preferências do projeto** > **Prioridades**.

1. Clique na guia do tipo de objeto para o qual você deseja criar uma prioridade (**Projeto**, **Tarefa** ou **Problema**).
1. Clique em <span class="preview">**Nova linha** na parte inferior da tabela</span> ou **Adicionar uma Nova Prioridade**.
1. Configure as seguintes opções para a prioridade:

   * **Nome da Prioridade**: digite um nome para a prioridade.
   * **Importância**: ao adicionar uma nova prioridade, um número é atribuído a ela por padrão. Edite esse número se ele não corresponder às suas necessidades.

     O número de importância de cada prioridade deve ser exclusivo. O número da prioridade reflete a importância do projeto, tarefa ou problema: o número mais alto corresponde à prioridade mais alta.

     Não é possível editar esse número depois de salvar a prioridade.

   * **Cor**: escolha uma cor para a prioridade.

     A cor da prioridade é usada em relatórios de gráfico e Configurações de Equipe Agile. Para obter informações sobre relatórios de gráficos, consulte [Adicionar um gráfico a um relatório](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md). Para obter informações sobre Configurações de Equipe Agile, consulte [Criar uma Equipe Agile](/help/quicksilver/agile/get-started-with-agile-in-workfront/create-an-agile-team.md).

   * **Prioridade padrão**: selecione a prioridade que deseja que o Workfront aplique automaticamente a todos os projetos, tarefas ou problemas recém-criados.

     **Normal** é a prioridade padrão para todos os objetos no Workfront.

     Não é possível definir uma prioridade oculta como padrão.

     <div class="preview">

     A prioridade padrão é indicada com um ícone ![Ícone de prioridade padrão](assets/default-icon.png). Para escolher um novo padrão, siga um destes procedimentos:

      * Marque a caixa de seleção ao lado do nome da prioridade e selecione **Tornar padrão** na barra de ações, na parte inferior da tela.
      * Passe o mouse sobre o nome da prioridade e clique no menu **Mais** que é exibido. Em seguida, selecione **Tornar Padrão**.

        A nova prioridade padrão é rotulada com o ícone.

     </div>

   * **Descrição**: digite uma descrição para a prioridade para explicar sua função.
   * <span class="preview">**Ocultar Opção**</span> ou **Ocultar**: <span class="preview">Escolha **Sim**</span> ou marque a caixa de seleção para ocultar uma prioridade que não é mais necessária.

     Uma prioridade oculta não é exibida em nenhum lugar do Workfront, portanto, os usuários não podem escolhê-la para seus projetos, tarefas ou problemas.

     >[!IMPORTANT]
     >
     >Em vez de excluir prioridades que você não deseja mais usar, sugerimos que você as oculte. Dessa forma, você mantém todos os dados históricos em objetos já concluídos com a prioridade, impedindo que as pessoas usem a prioridade no futuro.

1. (Opcional) Altere a ordem de listagem de suas prioridades arrastando e soltando na ordem desejada.

   Isso altera a ordem em que são exibidos para projetos, tarefas ou problemas. Isso não altera o número de **Importância**.

1. Clique em **Salvar**.

Para obter instruções sobre como aplicar prioridades a projetos, tarefas e problemas, consulte os seguintes artigos:

* [Compreender e atualizar as prioridades de projeto](../../../manage-work/projects/planning-a-project/project-priority.md)
* [Atualizar Prioridade da Tarefa](../../../manage-work/tasks/task-information/task-priority.md)
* [Atualizar prioridade do problema](../../../manage-work/issues/issue-information/update-issue-priority.md)
