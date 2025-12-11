---
product-area: reporting
navigation-topic: reporting-elements
title: Criar ou editar exibições no Adobe Workfront
description: Você pode personalizar o tipo de informação exibida na tela usando visualizações. Você pode usar vários tipos de visualizações no Adobe Workfront.
author: Nolan
feature: Reports and Dashboards
exl-id: 8fcd6320-c939-4195-8972-5c31575f78cb
source-git-commit: 0c0ffbeefb0eed8d1ca2a6e68ed19b40080726df
workflow-type: tm+mt
source-wordcount: '898'
ht-degree: 4%

---

# Criar ou editar exibições no Adobe Workfront

<!-- Audited: 11/2024 -->

Você pode personalizar o tipo de informação exibida na tela usando visualizações. Você pode usar vários tipos de visualizações no Adobe Workfront.

Este artigo descreve como criar e editar exibições padrão para listas e relatórios.

Para obter mais informações, consulte [Visão geral na Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacote do Adobe Workfront</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</strong></td> 
   <td> 
    <p>Colaborador ou superior</p>
    <p>Solicitação ou superior</p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Editar acesso a Filtros, Visualizações, Agrupamentos</p> <p>Editar acesso a Relatórios, Painéis, Calendários para criar uma visualização em um relatório</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões para um relatório para criar ou editar uma visualização em um relatório</p> <p>Gerenciar permissões em uma exibição para editá-la</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).
+++

## Criar ou personalizar um modo de exibição

O processo de criação ou personalização de uma view difere dependendo se você está criando ou personalizando uma view padrão ou uma view Agile ou Board.

* [Criar ou personalizar um modo de exibição padrão](#create-or-customize-a-standard-view)
* [Criar ou personalizar uma visualização Agile](#create-or-customize-an-agile-view)

### Criar ou personalizar um modo de exibição padrão {#create-or-customize-a-standard-view}

Você pode criar uma nova view-padrão ou personalizar uma view-padrão existente criada anteriormente.

1. Clique no menu suspenso **Exibir** em qualquer lista em que deseje criar ou personalizar um modo de exibição.

1. Clique no botão **+ Nova Exibição** para criar uma nova exibição.
Ou
Clique no ícone **Editar** ![Ícone Editar](assets/edit-icon.png) que aparece ao passar o mouse à direita de um modo de exibição existente que você deseja editar.
A caixa de diálogo **Personalizar exibição** é exibida.

1. Na seção **Visualização da coluna**, siga um destes procedimentos:

   * Modifique o valor de qualquer coluna clicando no título da coluna e selecionando um novo campo.
   * Adicione uma coluna clicando em **Adicionar coluna**, comece digitando o nome da coluna que deseja adicionar e clique nela quando ela aparecer na lista suspensa.
   * Ajuste a ordem em que as colunas aparecem arrastando o título da coluna para um novo local.

   * Na área **Configurações de Coluna**, clique em **Resumir esta coluna por** e escolha como deseja que os dados sejam exibidos na coluna. Essa opção está disponível para os seguintes tipos de coluna:
     <table style="table-layout:auto"> 
         <col> 
         <col> 
         <tbody> 
          <tr> 
           <td role="rowheader"><strong>Campos de data</strong></td> 
           <td><ul>
           <li>Máximo</li>
         <li>Mínimo</li>
           </ul></td> 
          </tr> 
          <tr>
           <td role="rowheader"><strong>Campos de moeda</strong></td> 
           <td><ul>
           <li>Contagem</li>
         <li>Sum</li>
           <li>Média</li>
         <li>Máximo</li>
           <li>Mínimo</li>
         </ul></td> 
          </tr> 
         <tr>
           <td role="rowheader"><strong>Campos de string e booleanos</strong></td> 
           <td><ul><li>Contagem</li></ul>
           <p>Observação: geralmente, o Workfront não recomenda o resumo de um campo booleano por contagem, pois o valor sempre será verdadeiro/falso.</p></td> 
          </tr> 
         </tbody> 
        </table>

     >[!NOTE]
     >
     >As exceções a seguir se aplicam a objetos pai (por exemplo, tarefas pai) quando você está resumindo valores para os seguintes campos em agrupamentos:
     >   
     > * Todos os campos de número e moeda, exceto Horas Reais (por exemplo, Custo de Trabalho Planejado/Efetivo, Custo de Despesas Planejado/Efetivo, Custo Planejado/Efetivo, Horas Planejadas) resumem os valores apenas para tarefas filhas e tarefas independentes. Eles não resumem os valores das tarefas pai ou pais dos pais.
     > * As Horas Reais resumem os valores das tarefas principais principal e independente; elas não resumem os números das tarefas principais ou secundárias.
     > * Os campos de dados personalizados para valores de número e moeda resumem todas as tarefas: pais, filhos, pais dos pais e tarefas independentes.
     >
     >Para obter mais informações sobre como usar agrupamentos em um relatório, consulte o artigo [Visão geral sobre agrupamentos no Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

      * (Opcional) Clique em **Opções Avançadas** para especificar as seguintes informações para a coluna:

        <table style="table-layout:auto"> 
         <col> 
         <col> 
         <tbody> 
          <tr> 
           <td role="rowheader"><strong>Personalizar rótulo da coluna</strong></td> 
           <td><p>Especifique um rótulo personalizado para a coluna. Esse rótulo substitui o rótulo padrão. Recomendamos usar somente caracteres UTF-8 para evitar problemas de compatibilidade.</p></td> 
          </tr> 
          <tr> 
           <td role="rowheader"><strong>Formato do campo</strong></td> 
           <td>Selecione o formato no qual deseja que os valores sejam exibidos para os campos na coluna.</td> 
          </tr> 
          <tr> 
           <td role="rowheader"><strong>Mostrar esta coluna quando estiver em um Painel</strong></td> 
           <td><p>Selecione essa opção para mostrar essa coluna em um painel, quando o relatório for exibido lado a lado com outro relatório. Quando essa opção não está selecionada, essa coluna não é exibida ao visualizar o relatório em um painel em que os relatórios são exibidos lado a lado.</p></td> 
          </tr> 
          <tr> 
           <td role="rowheader"><strong>Regras de colunas</strong></td> 
           <td><p>Clique em <strong>+ Adicionar uma Regra para esta Coluna</strong> para definir uma regra para a coluna. Após adicionar uma regra, é possível definir estilos de campo e texto para a forma como os campos que correspondem a essa regra são exibidos. Clique em <strong>Adicionar regra</strong> depois que terminar de definir a regra.</p></td> 
          </tr> 
         </tbody> 
        </table>

        Para obter mais informações sobre modos de exibição de formatação condicional nos relatórios, consulte o artigo [Usar formatação condicional no Modo de Texto](../../../reports-and-dashboards/reports/text-mode/use-conditional-formatting-text-mode.md).

1. (Condicional) Se você clicou em **Opções Avançadas**, clique em **Concluído**.

1. Clique em **Salvar exibição** para criar um novo modo de exibição ou substituir o modo de exibição atual por suas alterações.\
   Ou\
   Clique em **Salvar como Novo Modo de Exibição** para salvar suas alterações como um novo modo de exibição.

   >[!TIP]
   >
   >A **Salvar como Nova Exibição** é a única opção disponível ao personalizar uma exibição interna do Workfront.

   Seu acesso determina como a visualização é salva. Se você criou a visualização originalmente, é possível salvar as alterações; caso contrário, será solicitado que você salve uma versão. Lembre-se de que as alterações feitas na exibição afetam os usuários com os quais a exibição foi compartilhada.

### Criar ou personalizar uma visualização Agile {#create-or-customize-an-agile-view}

As exibições Agile, também chamadas de exibições de Quadro, são exibidas somente para listas de tarefas e problemas em um projeto.

Eles são pré-configurados, mas você pode modificar determinadas configurações para eles.

Para obter mais informações sobre exibições Agile ou Board, consulte o artigo [Gerenciar um projeto na Exibição Agile](../../../manage-work/projects/manage-projects/manage-projects-in-agile-view.md).

<!-- Legacy Agile views were deprecated with 25.3. This is old: 

>[!NOTE]
>
>This procedure only applies to the legacy Agile view, not to the board view of a project.

To create or customize an Agile view:

1. Go to the list of tasks on a project.
1. Click the **Board** icon ![Board icon](assets/board-icon-for-agile-view.png), and then click **Use legacy agile** on the board view.

1. (Conditional) To customize an existing Agile view:

   1. Click the **View** drop-down menu, then select the Agile view you want to customize.  
      You cannot customize the default Agile view.
   
   1. Click the **View** drop-down menu again, then click **Customize View**.  
      ![Customize view](assets/view-agile-customize.png)

1. (Conditional) To create a new Agile view, click **New View**.  
   The **Customize Agile View** dialog box displays.  

1. In the **Customize Agile View** dialog box, specify a name for the Agile view.  
   We recommend that you include the word "Agile" in your view name, so users know this is an Agile view.  
   This name is displayed in the **View** drop-down menu when selecting a view.

1. Define the status columns to display on the story board in the agile view. These are the task statuses that are defined by the Workfront administrator, as described in [Create or edit a status](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

   Only system statuses are available to use on the Agile story board. If a status is available only for an individual group you are a member of, the status is not available on the agile story board. Furthermore, tasks that are in a status that is available only to a custom group are not visible when viewing the project in an Agile view.

   Users can move stories among these status columns on the Agile story board.  
   When defining status columns, you can do the following:

   <table style="table-layout:auto"> 
    <col> 
    <col>
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Reorder status columns:</strong> </td> 
      <td> Drag a status column to the order where you want it to appear.<br><img src="assets/agile-project-reorderstatuses-350x141.png" alt="" style="width: 350;height: 141;"></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Remove status columns:</strong> </td> 
      <td>Click the (x) icon on the column that you want to remove.<br>You cannot remove the "New" status unless a custom status has been added to the view and that custom status equates with "New."<br>For information about creating a custom status, see <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md" class="MCXref xref">Create or edit a status</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Add status columns:</strong> </td> 
      <td> <p>Click the <strong>Plus</strong> icon, then select the status you want to add.<br>All default system statuses are displayed, as well as any custom statuses that have been shared with you.<br>You can configure up to 10 statuses to display.</p></td> 
     </tr> 
    </tbody> 
   </table>

   *********   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE FOR ADD STATUS COLUMNS: research this and add: [! What if the status has been shared with me or a group I'm in (so I can see it here), but the status hasn't been shared with another user who also has access to a project where I later apply this view? Can that user still see this status on the project?]) </p>
       *************

1. In the **Associate Card Color to** area, select from the following options:

   <table style="table-layout:auto"> 
    <col> 
    <col>
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Story:</strong> </td> 
      <td>Any subtasks match the color of the parent task, so that the colors of all stories in any given swimlane are the same.<br>Colors are randomly assigned to tasks when they are created if the task does not have any subtasks or does not have a parent task.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Free Form:</strong> </td> 
      <td> All cards are displayed as blue by default until a user changes the color manually, as described in the article <a href="../../../agile/use-scrum-in-an-agile-team/scrum-board/categorize-stories-by-color.md" class="MCXref xref">Categorize stories by color on the Scrum board</a>. </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Priority:</strong> </td> 
      <td> <p> Colors are associated with the story priority, as follows:</p> 
       <ul> 
        <li>High = Red</li> 
        <li>Medium = Yellow</li> 
        <li>Low = Green<br>If your Workfront administrator has configured custom priorities for your Workfront system, the highest priority is red, the second-highest is yellow, and the remaining are green.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Task Owner:</strong> </td> 
      <td> All stories with the same primary assignee are the same color.<br>The primary assignee is the user who was first assigned to the task. </td> 
     </tr> 
    </tbody> 
   </table>

1. In the **Additional Fields** area, click **Add Field**, then select the field you want to add to story cards. (These are the same fields you can add when creating customizing a view or creating columns for a report.)  
   Repeat this process to add up to three additional fields to the story cards.  
   When you add fields to story cards, fields are view-only and display only when the field is populated.

   By default, the following types of data is displayed on the story card:

   * Story name with a link directly to the task
   * The project name with a link directly to the project  
     This link is displayed only when using the agile view on an iteration; it is not displayed when using an Agile view on a project.
   * The task description
   * Current commitment
   * View and edit the percent complete either by adjusting the percent complete itself or by adjusting the number of points or hours that are complete
   * Assigned Users

   You can display additional data (including custom data) on story cards. You might want to display additional fields on story cards for any number of reasons. For example, you might want to display the Customer ID if you are working on stories for multiple customers within the project, or you might want to display the Task Start Date.

1. Click **Save**.  
   Your access dictates how the view is saved. If you created the view originally, you can save the changes; otherwise, you are prompted to save a version. Keep in mind that changes you make to the view impact users with whom the view has been shared.

1. (Optional) Click the **List** icon to return to the list of tasks.

-->
