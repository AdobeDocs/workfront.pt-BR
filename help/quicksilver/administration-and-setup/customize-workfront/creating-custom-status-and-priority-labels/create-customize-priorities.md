---
title: Criar e personalizar prioridades
description: Você pode controlar as prioridades de projetos, tarefas e problemas na área Configuração do Workfront. As prioridades dão importância aos seus projetos, tarefas ou problemas no Adobe Workfront.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 6e7952cf-f07a-412b-9f9a-623cdba46849
source-git-commit: e20934501c2117455ca7950834d868f78576dee7
workflow-type: tm+mt
source-wordcount: '735'
ht-degree: 2%

---

# Criar e personalizar prioridades

<!--
DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.
-->

Você pode controlar as prioridades de projetos, tarefas e problemas na área Configuração do Workfront. As prioridades dão importância aos seus projetos, tarefas ou problemas no Adobe Workfront.

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plano Adobe Workfront</td> 
   <td>Qualquer Um</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença Adobe Workfront</td> 
   <td>Plano</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Você deve ser um administrador do Workfront.</p> <p><b>OBSERVAÇÃO</b>: Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Personalização das prioridades existentes

Como administrador do Workfront, você pode fazer as seguintes modificações nas prioridades padrão fornecidas no Workfront:

* Renomeie as prioridades.
* Reordene as prioridades.

   Para obter mais informações sobre como reorganizar prioridades, consulte [Criar uma prioridade para uma tarefa do projeto ou um problema](#create-a-priority-for-a-project-task-or-issue).

* Altere a prioridade padrão.

   Para obter mais informações sobre a funcionalidade de alterar a prioridade padrão, consulte [Criar uma prioridade para uma tarefa do projeto ou um problema](#create-a-priority-for-a-project-task-or-issue).

* Edite a descrição das prioridades.
* Defina uma cor para cada prioridade.

   A cor da prioridade é usada nos relatórios do gráfico, ao agrupar os resultados por **Prioridade**.

   Para obter mais informações sobre relatórios de gráfico, consulte [Adicionar um gráfico a um relatório](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md).

* Excluir prioridades.

   Ao excluir uma prioridade existente, você deve selecionar uma prioridade de substituição.

* Ocultar prioridades.

   Para obter mais informações sobre a funcionalidade de ocultar prioridades, consulte [Criar uma prioridade para uma tarefa do projeto ou um problema](#create-a-priority-for-a-project-task-or-issue).

   >[!NOTE]
   >
   >Você deve ter pelo menos uma prioridade na conta do Workfront para cada objeto.

As prioridades fornecidas por padrão para cada tipo de objeto (projeto, tarefa e problema) são idênticas:

* Nenhum(a)
* Baixa
* Normal
* Alta
* Urgente

## Criar uma prioridade para uma tarefa do projeto ou um problema {#create-a-priority-for-a-project-task-or-issue}

Além das prioridades padrão fornecidas no Workfront, você pode adicionar suas próprias prioridades para refletir as necessidades da organização.

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront, em seguida, clique em **Configuração** ![](assets/gear-icon-settings.png).

1. No painel esquerdo, clique em **Preferências do projeto** > **Prioridades**.

1. Clique na guia referente ao tipo de objeto para o qual deseja criar uma prioridade (**Projeto**, **Tarefa** ou **Problema**).
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
      <td> <p>Ao adicionar uma nova prioridade, um número é atribuído a ele por padrão. Edite esse número se ele não corresponder às suas necessidades.</p> <p>O <strong>Importância</strong> número para cada prioridade deve ser exclusivo para o objeto selecionado.<br>O número da prioridade reflete a importância do projeto, tarefa ou problema: o número mais alto corresponde à prioridade mais alta.</p> <p><b>OBSERVAÇÃO</b>: Não é possível editar o número de Importância depois de salvar a prioridade. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Cor</td> 
      <td> <p>Escolha uma cor para a sua prioridade.</p> <p>A cor da prioridade é usada nos relatórios do gráfico e nas Configurações do grupo ágil. Para obter mais informações sobre relatórios de gráfico, consulte <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md" class="MCXref xref">Adicionar um gráfico a um relatório</a>.</p> <p>Para obter mais informações sobre as Configurações da equipe ágil, consulte em .</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Prioridade Padrão</td> 
      <td> <p>Decida se essa deve ser uma prioridade padrão ou não, selecionando o botão de opção .</p> <p>Se uma prioridade for designada como <strong>Prioridade padrão</strong>, ele é selecionado automaticamente para todos os projetos, tarefas ou problemas no Workfront. <strong>Normal</strong> é a prioridade padrão para todos os objetos no Workfront.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Descrição</td> 
      <td>Adicione uma descrição para sua prioridade para explicar sua função.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ocultar</td> 
      <td> <p>Selecione essa caixa se desejar ocultar a prioridade.</p><p>Ao selecionar a variável <b>Ocultar</b> , a prioridade não é exibida em nenhum lugar do Workfront e os usuários não podem escolhê-la para seus projetos, tarefas e problemas.</p> 
      <p><b>IMPORTANTE</b>: Recomendamos que você oculte as prioridades que não deseja mais usar, em vez de excluí-las. Ao ocultá-los, você ainda mantém todos os seus dados históricos, de objetos que foram completados com essa prioridade, enquanto impede que as pessoas escolham essa prioridade no futuro. </p>
      <p>Como opção, você pode alterar a ordem de listagem de suas prioridades arrastando-as e soltando-as na ordem desejada. Isso altera a ordem em que são exibidos para projetos, tarefas e problemas. Isso não altera a variável <b>Importância</b> número. </p></td> 
     </tr> 
    </tbody> 
   </table>

1. Clique em **Salvar**.

Para obter instruções sobre como aplicar prioridades a projetos, tarefas e questões, consulte os seguintes artigos:

* [Compreender e atualizar as prioridades do projeto](../../../manage-work/projects/planning-a-project/project-priority.md)
* [Atualizar Prioridade da Tarefa](../../../manage-work/tasks/task-information/task-priority.md)
* [Atualizar prioridade do problema](../../../manage-work/issues/issue-information/update-issue-priority.md)
