---
product-area: projects
navigation-topic: create-tasks
title: Criar tarefas em um projeto
description: Você só pode criar tarefas em um projeto depois de criá-lo.
author: Alina
feature: Work Management, Tasks
role: User
exl-id: 96f80e7b-6ad5-40ae-861d-8d97c570f2ac
source-git-commit: 4a4efe7d8a354bc9ec22a607fe6e75040e7cca24
workflow-type: tm+mt
source-wordcount: '792'
ht-degree: 1%

---

# Criar tarefas em um projeto

Você só pode criar tarefas em um projeto depois de criá-lo.

Por exemplo, após criar um projeto, você pode adicionar tarefas e modificá-las para organizar o plano do projeto. Para obter mais informações sobre como criar um projeto, consulte [Criar um projeto](../../../manage-work/projects/create-projects/create-project.md).

Para obter informações sobre como criar tarefas pessoais que não estão em um projeto, consulte a seção &quot;Criar uma tarefa pessoal&quot; no artigo [Criar itens de trabalho a partir da Área da página inicial](../../../workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md).

Este artigo descreve como criar tarefas do zero. Você também pode criar tarefas das seguintes maneiras:

* Copiando ou duplicando tarefas existentes. Para obter informações, consulte [Copiar e duplicar tarefas](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md).
* Movendo tarefas de um projeto para outro. Para obter informações, consulte [Mover tarefas](../../../manage-work/tasks/manage-tasks/move-tasks.md).

## Requisitos de acesso

<!--drafted for P&P - replace the table:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p role="rowheader">Adobe Workfront license*</p> </td> 
   <td><p>Current license: Standard</p> 
   Or
   <p>Legacy license: Work or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Tasks and Projects</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information about access to tasks, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md" class="MCXref xref">Grant access to tasks</a>. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Contribute permissions to the project with ability to Add Tasks or higher</p> <p>When you create a task you automatically receive Manage permissions to the task</p> <p> For information about task permissions, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-task.md" class="MCXref xref">Share a task </a>. </p> <p>For information on requesting additional permissions, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->
Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront*</td> 
   <td> <p>Qualquer Um</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p role="rowheader">Licença da Adobe Workfront*</p> </td> 
   <td> <p>Trabalhar ou superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a tarefas e projetos</p> <p>Observação: se você ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre o acesso a tarefas, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md" class="MCXref xref">Conceder acesso a tarefas</a>. Para obter informações sobre como um administrador do Workfront pode alterar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Contribuir com permissões para o projeto com a capacidade de adicionar tarefas ou superior</p> <p>Ao criar uma tarefa, você recebe automaticamente permissões Gerenciar para a tarefa</p> <p> Para obter informações sobre permissões de tarefas, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-task.md" class="MCXref xref">Compartilhar uma tarefa </a>. </p> <p>Para obter informações sobre a solicitação de permissões adicionais, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir seu plano, tipo de licença ou acesso, entre em contato com o administrador do Workfront.

## Criar tarefas em um projeto

1. Vá para o projeto em que deseja criar uma tarefa.
1. Clique em **Tarefas** no painel esquerdo.
1. (Condicional) Se você estiver visualizando a lista de tarefas em uma exibição ágil, clique no link **Exibição de lista** ícone ![](assets/list-view-in-agile-view-for-tasks.png) no canto superior direito para exibir a lista de tarefas.
1. (Opcional) Clique no link **Modo de plano** ícone ![](assets/nwe-plan-mode-icon-task-list.png) e selecione **Salvamento manual** e selecione **Padrão** ou **Planejamento da linha do tempo**. Isso desativa o **Salvamento automático** que está ativada por padrão.

   ![Selecione Salvar manualmente](assets/manual-save-option.png)

   >[!TIP]
   >
   >É possível reverter as alterações ao selecionar Salvar manualmente.

1. Crie uma nova tarefa seguindo um destes procedimentos:

   * Clique em **Nova tarefa** na parte superior da lista de tarefas
   * Clique em **Adicionar mais tarefas** na parte inferior da lista de tarefas

   ![](assets/qs-new-task-or-add-task-buttons-in-list-highlighted-350x242.png)

1. (Condicional) Se você clicou em **Nova tarefa** faça o seguinte:

   1. Especifique qualquer um dos campos na lista limitada de campos dentro do **Nova tarefa** e clique em **Criar tarefa** se quiser criar uma tarefa rapidamente.

      Ou

      Para atualizar todos os campos da tarefa, clique em **Mais opções** para abrir o **Criar tarefa** caixa.

      ![](assets/nwe-create-task-small-screen-350x272.png)

      A variável **Criar tarefa** é aberta.

      ![](assets/create-task-larger-box-nwe-350x244.png)

       

      >[!NOTE]
      >
      >Dependendo de como o administrador do Workfront configura nosso Modelo de layout, os campos na caixa Criar tarefa podem exibir campos diferentes no seu ambiente. Para obter informações, consulte [Personalizar a exibição de Detalhes usando um modelo de layout](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

   1. Especifique informações para as seguintes áreas no painel esquerdo da caixa Criar tarefa:

      * Nome da tarefa
      * Visão geral
      * Atribuições
      * Formulários personalizados
      * Finanças
      * Configurações

        Para obter informações sobre como definir todos os campos relacionados a uma tarefa, consulte [Editar tarefas](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

   1. (Condicional e opcional) Se quiser que a tarefa seja recorrente, atualize o **Frequência de recorrência** campo. Para obter mais informações sobre como criar tarefas recorrentes, consulte [Criar tarefas recorrentes](../../../manage-work/tasks/create-tasks/create-recurring-tasks.md).
   1. (Opcional) Clique em **Documentos** no painel esquerdo para anexar um documento à nova tarefa e clique em **Adicionar ou vincular arquivos** para adicionar um documento à tarefa a partir de seu computador ou outro serviço, ou para vincular documentos e pastas de seu computador ou outro serviço.

1. (Condicional) Se você clicou em **Adicionar mais tarefas** na etapa 5, comece inserindo as informações da tarefa usando a edição em linha e, em seguida, pressione Enter.

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ensure this stays accurate)</p>
   -->

   Recomendamos usar essa opção, especialmente ao adicionar várias tarefas à lista.

   ![](assets/ctp4-350x26.png)

1. (Condicional) Siga um destes procedimentos:

   * Se você clicou em **Nova tarefa** na etapa 5, clique em **Criar tarefa** para salvar as alterações e adicionar a nova tarefa ao projeto.

     <!--   
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: is this step still right?)</p>   
     -->

   * Se você clicou em **Adicionar mais tarefas** na etapa 5, faça o seguinte:

     <!--   
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: is this step still right?) </p>   
     -->

      1. Clique em qualquer lugar no navegador para enviar suas alterações ou pressione Enter.
      1. (Opcional) Na lista de tarefas, selecione a tarefa recém-criada e clique em **Recuar**.

         Isso torna a nova tarefa uma tarefa filha ou subtarefa da tarefa anterior.

         Para obter mais informações sobre tarefas-filho, consulte [Visão geral das tarefas](../../../manage-work/tasks/task-information/tasks-overview.md).

      1. (Condicional) Se você desativou a variável **Salvamento automático** depois de pressionar **Adicionar mais tarefas**, você pode fazer o seguinte:

         * Clique em **Desfazer** a qualquer momento para reverter sua última alteração ou **Cancelar** para reverter todas as alterações feitas na lista de tarefas.
         * Se você clicou anteriormente em **Desfazer**, clique em **Refazer** para reaplicar a última alteração cancelada.
         * Clique em **Salvar** para salvar as alterações na lista de tarefas.
