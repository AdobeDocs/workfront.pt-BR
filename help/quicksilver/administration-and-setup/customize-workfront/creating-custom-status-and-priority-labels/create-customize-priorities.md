---
title: Criar e personalizar prioridades
description: Você pode controlar as prioridades de projetos, tarefas e problemas na área Configuração do Workfront. As prioridades dão importância aos seus projetos, tarefas ou problemas no Adobe Workfront.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 6e7952cf-f07a-412b-9f9a-623cdba46849
source-git-commit: 0bc2817255b8879de377c3916bb36be760f28f4c
workflow-type: tm+mt
source-wordcount: '708'
ht-degree: 2%

---

# Criar e personalizar prioridades

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

  Para obter mais informações sobre como reordenar prioridades, consulte [Criar uma prioridade para uma tarefa de projeto ou problema](#create-a-priority-for-a-project-task-or-issue).

* Altere a prioridade padrão.

  Para obter mais informações sobre a funcionalidade de alterar a prioridade padrão, consulte [Criar uma prioridade para uma tarefa de projeto ou problema](#create-a-priority-for-a-project-task-or-issue).

* Edite a descrição das prioridades.
* Defina uma cor para cada prioridade.

  A cor da prioridade é usada nos relatórios de gráfico, quando você agrupa seus resultados por **Prioridade**.

  Para obter mais informações sobre relatórios de gráficos, consulte [Adicionar um gráfico a um relatório](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md).

* Excluir prioridades.

  Quando você exclui uma prioridade existente, deve selecionar uma prioridade substituta.

* Ocultar prioridades.

  Para obter mais informações sobre a funcionalidade de ocultar prioridades, consulte [Criar uma prioridade para uma tarefa de projeto ou problema](#create-a-priority-for-a-project-task-or-issue).

  >[!NOTE]
  >
  >Você deve ter pelo menos uma prioridade em sua conta do Workfront para cada objeto.

As prioridades fornecidas por padrão para cada tipo de objeto (projeto, tarefa e problema) são idênticas:

* Nenhum(a)
* Baixa
* Normal
* Alta
* Urgente

## Criar uma prioridade para uma tarefa de projeto ou problema {#create-a-priority-for-a-project-task-or-issue}

Além das prioridades padrão fornecidas no Workfront, você pode adicionar suas próprias prioridades para refletir as necessidades de sua organização.

{{step-1-to-setup}}

1. No painel esquerdo, clique em **Preferências do projeto** > **Prioridades**.

1. Clique na guia do tipo de objeto para o qual você deseja criar uma prioridade (**Projeto**, **Tarefa** ou **Problema**).
1. Clique em **Adicionar uma nova prioridade**.
1. Especifique as seguintes informações para a nova prioridade:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Nome da Prioridade</td> 
      <td>Digite um nome para sua prioridade.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Chave</td> 
      <td> <p>Ao adicionar uma nova prioridade, um número é atribuído a ele por padrão. Edite esse número se ele não corresponder às suas necessidades.</p> <p>O número de <strong>Importância</strong> para cada prioridade deve ser exclusivo para o objeto selecionado.<br>O número da prioridade reflete a importância do projeto, tarefa ou problema: o número mais alto corresponde à prioridade mais alta.</p> <p><b>OBSERVAÇÃO</b>: não é possível editar o número de importância depois de salvar a prioridade. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Cor</td> 
      <td> <p>Escolha uma cor para sua prioridade.</p> <p>A cor da prioridade é usada em relatórios de gráfico e Configurações de Equipe Agile. Para obter mais informações sobre relatórios de gráficos, consulte <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md" class="MCXref xref">Adicionar um gráfico a um relatório</a>.</p> <p>Para obter mais informações sobre as Configurações de Equipe Agile, consulte em .</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Prioridade Padrão</td> 
      <td> <p>Decida se essa deve ser uma prioridade padrão ou não, selecionando o botão de opção.</p> <p>Se uma prioridade for designada como a <strong>Prioridade Padrão</strong>, ela será selecionada automaticamente para todos os projetos, tarefas ou problemas na Workfront. <strong>Normal</strong> é a prioridade padrão para todos os objetos no Workfront.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Descrição</td> 
      <td>Adicione uma descrição para a prioridade para explicar sua função.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ocultar</td> 
      <td> <p>Selecione esta caixa se desejar ocultar a prioridade.</p><p>Ao selecionar a opção <b>Ocultar</b>, a prioridade não é exibida em nenhum lugar do Workfront e os usuários não podem escolhê-la para seus projetos, tarefas e problemas.</p> 
      <p><b>IMPORTANTE</b>: recomendamos que você oculte as prioridades que não deseja mais usar, em vez de excluí-las. Ao ocultá-los, você ainda mantém todos os dados históricos dos objetos que foram concluídos com essa prioridade, enquanto impede que as pessoas escolham essa prioridade no futuro. </p>
      <p>Opcionalmente, é possível alterar a ordem de listagem das prioridades arrastando-as e soltando-as na ordem desejada. Isso altera a ordem em que são exibidos para projetos, tarefas e problemas. Isso não altera o número de <b>Importância</b>. </p></td> 
     </tr> 
    </tbody> 
   </table>

1. Clique em **Salvar**.

Para obter instruções sobre como aplicar prioridades a projetos, tarefas e problemas, consulte os seguintes artigos:

* [Compreender e atualizar as prioridades de projeto](../../../manage-work/projects/planning-a-project/project-priority.md)
* [Atualizar Prioridade da Tarefa](../../../manage-work/tasks/task-information/task-priority.md)
* [Atualizar prioridade do problema](../../../manage-work/issues/issue-information/update-issue-priority.md)
