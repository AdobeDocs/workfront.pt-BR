---
product-area: projects
navigation-topic: create-tasks
title: Criar tarefas em um projeto
description: Você só pode criar tarefas em um projeto depois de criá-lo.
author: Alina
feature: Work Management, Tasks
role: User
exl-id: 96f80e7b-6ad5-40ae-861d-8d97c570f2ac
source-git-commit: a92c85ad5f58700138d7750423cc3d134d980a9e
workflow-type: tm+mt
source-wordcount: '1041'
ht-degree: 0%

---

# Criar tarefas em um projeto

<!-- Audited: 10/2024 -->

Você pode criar tarefas no Adobe Workfront das seguintes maneiras:

* Crie uma tarefa em um projeto do zero, após a criação do projeto.

  Depois de criar um projeto, você pode adicionar tarefas e modificá-las para organizar o plano do projeto. Para obter mais informações sobre como criar um projeto, consulte [Criar um projeto](../../../manage-work/projects/create-projects/create-project.md).

* Crie tarefas adicionando um modelo a um projeto.

  Para obter informações, consulte [Anexar um modelo a um projeto](/help/quicksilver/manage-work/projects/create-and-manage-templates/attach-template-to-project.md).

* Criar tarefas pessoais e movê-las para um projeto.

  Você pode criar tarefas pessoais seguindo um destes procedimentos:

   * Criar uma solicitação de trabalho ad hoc e enviá-la a um usuário
   * Criar um item de tarefa pendente na área Página inicial

  Para obter informações sobre como criar tarefas pessoais que não estão em um projeto, consulte [Criar tarefas pessoais](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/create-personal-tasks.md).

  Você pode mover tarefas pessoais para um projeto e elas se tornam tarefas de trabalho.

Este artigo descreve como criar tarefas do zero e como mover tarefas pessoais para um projeto.

Você também pode criar tarefas das seguintes maneiras:

* Copiando ou duplicando tarefas existentes. Para obter informações, consulte [Copiar e duplicar tarefas](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md).
* Movendo tarefas de um projeto para outro. Para obter informações, consulte [Mover tarefas](../../../manage-work/tasks/manage-tasks/move-tasks.md).

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p role="rowheader">Licença do Adobe Workfront</p> </td> 
   <td><p>Padrão</p> 
   <p>Trabalhar ou superior</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a tarefas e projetos</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Contribuir com permissões para o projeto com a capacidade de adicionar tarefas ou superior</p> <p>Ao criar uma tarefa, você recebe automaticamente permissões Gerenciar para a tarefa</p> <p> Para obter informações sobre permissões de tarefas, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-task.md" class="MCXref xref">Compartilhar uma tarefa </a>. </p> <p>Para obter informações sobre como solicitar permissões adicionais, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos. </a></p> </td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Criar tarefas em um projeto

Criar tarefas em um projeto é semelhante a criar tarefas em um modelo. Você pode seguir as etapas descritas abaixo ao adicionar tarefas de modelo a um modelo.

Para criar tarefas em um projeto:

1. Vá para o projeto em que deseja criar uma tarefa.
1. Clique em **Tarefas** no painel esquerdo.
1. (Condicional) Se você estiver visualizando a lista de tarefas em um modo de exibição ágil, clique no ícone **do** Modo de Exibição de Lista![](assets/list-view-in-agile-view-for-tasks.png) no canto superior direito para exibir a lista de tarefas.
1. (Opcional) Clique no ícone **do** Modo de Plano![](assets/nwe-plan-mode-icon-task-list.png) e selecione **Salvar Manualmente**. Em seguida, selecione **Padrão** ou **Planejamento de Linha do Tempo**. Isso desabilita a opção **Salvamento automático**, que é habilitada por padrão.

   ![Selecionar Salvamento Manual](assets/manual-save-option.png)

   >[!TIP]
   >
   >É possível reverter as alterações ao selecionar Salvar manualmente.

1. Crie uma nova tarefa seguindo um destes procedimentos:

   * Clique em **Nova tarefa** na parte superior da lista de tarefas.
   * Clique em **Adicionar mais tarefas** na parte inferior da lista de tarefas.

   ![](assets/qs-new-task-or-add-task-buttons-in-list-highlighted-350x242.png)

1. (Condicional) Se você clicou em **Nova tarefa**, faça o seguinte:

   1. Especifique qualquer um dos campos na lista limitada de campos dentro da caixa **Nova tarefa** e clique em **Criar tarefa** se desejar criar uma tarefa rapidamente.

      Ou

      Para atualizar todos os campos da tarefa, clique em **Mais Opções** para abrir a caixa **Criar Tarefa**.

      ![](assets/nwe-create-task-small-screen-350x272.png)

      A caixa **Criar tarefa** é aberta.

      ![](assets/create-task-larger-box-nwe-350x244.png)


      >[!NOTE]
      >
      >Dependendo de como o administrador do Workfront configura nosso Modelo de layout, os campos na caixa Criar tarefa podem exibir campos diferentes no seu ambiente. Para obter informações, consulte [Personalizar o modo de exibição de Detalhes usando um modelo de layout](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

   1. Especifique informações para as seguintes áreas no painel esquerdo da caixa Criar tarefa:

      * Nome da tarefa
      * Visão geral
      * Atribuições
      * Formulários personalizados
      * Finanças
      * Configurações

        Para obter informações sobre como definir todos os campos relacionados a tarefas em uma tarefa, consulte [Editar tarefas](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

   1. (Condicional e opcional) Se quiser que a tarefa seja recorrente, atualize o campo **Frequência de recorrência**. Para obter mais informações sobre como criar tarefas recorrentes, consulte [Criar tarefas recorrentes](../../../manage-work/tasks/create-tasks/create-recurring-tasks.md).
   1. (Opcional) Clique em **Documentos** no painel esquerdo para anexar um documento à nova tarefa e em **Adicionar ou vincular arquivos** para adicionar um documento à tarefa a partir de seu computador, de outro serviço ou para vincular documentos e pastas a partir de seu computador ou de outro serviço.

1. (Condicional) Se você clicou em **Adicionar mais tarefas** na etapa 5, comece a inserir as informações da tarefa usando a edição em linha e, em seguida, pressione Enter.

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ensure this stays accurate)</p>
   -->

   Recomendamos usar essa opção, especialmente ao adicionar várias tarefas à lista.

   ![](assets/add-more-tasks-inline.png)

1. (Condicional) Siga um destes procedimentos:

   * Se você clicou em **Nova tarefa** na etapa 5, clique em **Criar tarefa** para salvar suas alterações e adicionar a nova tarefa ao seu projeto.

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

         Para obter mais informações sobre tarefas filhas, consulte a seção &quot;Criar subtarefas da seção de subtarefas de tarefas&quot; no artigo [Criar subtarefas](/help/quicksilver/manage-work/tasks/create-tasks/create-subtasks.md).

      1. (Condicional) Se você desabilitou a opção **Salvar automaticamente** depois de pressionar **Adicionar mais tarefas**, poderá fazer o seguinte:

         * Clique em **Desfazer** a qualquer momento para reverter a última alteração ou em **Cancelar** para reverter todas as alterações feitas na lista de tarefas.
         * Se você clicou anteriormente em **Desfazer**, clique em **Refazer** para reaplicar a última alteração que você cancelou.
         * Clique em **Salvar** para salvar suas alterações na lista de tarefas.
   1. (Opcional) Em uma lista de tarefas, clique na seção **Predecessor** para adicionar predecessores à tarefa. Para obter mais informações, consulte [Criar uma relação predecessora usando a área Predecessoras](/help/quicksilver/manage-work/tasks/use-prdcssrs/create-predecessors-in-predecessors-area.md).
   1. (Opcional) Em uma lista de tarefas, clique na seção **Subtarefas** para adicionar tarefas filhas. Para obter mais informações, consulte [Criar subtarefas](/help/quicksilver/manage-work/tasks/create-tasks/create-subtasks.md).

## Criar tarefas movendo uma tarefa pessoal para um projeto

1. (Condicional) Certifique-se de que você ou outros usuários criaram tarefas pessoais.

   Para obter informações, consulte [Criar tarefas pessoais](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/create-personal-tasks.md).
1. Crie um filtro de tarefa pessoal e aplique-o a um relatório ou lista de tarefas.

   Para obter informações, consulte [Filtro: tarefas pessoais](/help/quicksilver/reports-and-dashboards/reports/custom-view-filter-grouping-samples/filter-personal-tasks.md).

   ![](assets/personal-tasks-report.png)
1. Clique em um nome de tarefa no relatório de tarefa pessoal para abri-lo.

   O Workfront salva tarefas pessoais em um projeto pessoal não listado que é sempre nomeado de acordo com este padrão: &quot;Tarefas do > nome completo do usuário. Por exemplo, um projeto pessoal poderia ser chamado de &quot;Tarefas de Rick&quot;.

1. Na página de tarefas, clique no **menu Mais** ![](assets/more-icon.png) e em **Mover**. Para obter mais informações sobre como mover tarefas, consulte [Mover tarefas](/help/quicksilver/manage-work/tasks/manage-tasks/move-tasks.md).

   Depois que você terminar de mover a tarefa, ela será exibida no projeto selecionado. A linha do tempo do projeto pode ser afetada pela linha do tempo da nova tarefa.
