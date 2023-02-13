---
title: Personalizar o painel esquerdo usando um modelo de layout
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: Em um modelo de layout, é possível personalizar o que os usuários veem na área do painel esquerdo em todo o Adobe Workfront.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: b100ea35-e045-4021-b5be-2c9071b381da
source-git-commit: c0b0102eb1e1f45e794f962f7e905349f9e241eb
workflow-type: tm+mt
source-wordcount: '977'
ht-degree: 0%

---

# Personalizar o painel esquerdo usando um modelo de layout

Em um modelo de layout, é possível personalizar o que os usuários veem na área do painel esquerdo em todo o [!DNL Adobe Workfront].

Por exemplo, você pode determinar qual dos seguintes itens os usuários veem no painel esquerdo ao visualizar uma tarefa:

![](assets/left-panel-adobe-branding.png)

>[!IMPORTANT]
>
>As alterações feitas na ordem e na visibilidade são refletidas no aplicativo móvel.

Para obter informações sobre modelos de layout para grupos, consulte [Criar e modificar modelos de layout de um grupo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plano</td> 
   <td>Qualquer Um</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licença</td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> Para executar essas etapas no nível do sistema, é necessário o nível de acesso [!UICONTROL System Administrator].<p>Para executá-los para um grupo, você deve ser um gerente desse grupo.</p> <p><b>OBSERVAÇÃO</b>: Se ainda não tiver acesso, pergunte ao seu [!DNL Workfront] administrador se eles definirem restrições adicionais em seu nível de acesso. Para obter informações sobre como uma [!DNL Workfront] administrador pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Personalize o painel esquerdo para uma área em [!DNL Workfront]:

1. Comece a trabalhar em um modelo de layout, conforme descrito em [Criar e gerenciar modelos de layout](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
1. Clique na seta para baixo ![](assets/dropdown-arrow.png) under **[!UICONTROL Personalize o que os usuários veem]** e clique no painel esquerdo que deseja personalizar.

   >[!NOTE]
   >
   >Para obter informações sobre o [!UICONTROL Início] nesta lista suspensa, consulte [Personalizar [!UICONTROL Início] e [!UICONTROL Resumo] uso de um modelo de layout](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-home-summary-layout-template.md). Para obter informações sobre a opção Listas , consulte [Personalizar filtros, exibições e agrupamentos usando um modelo de layout](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md).

1. No **[!UICONTROL Painel esquerdo]** , siga um destes procedimentos para determinar o que os usuários verão no painel esquerdo para a opção ([!DNL Workfront] área ou tipo de objeto) que você selecionou:

   * Mostrar ![](assets/add-secondary-nav-item.png) ou ocultar ![](assets/delete-secondary-nav-item.png) itens. Qualquer item sem ![](assets/add-secondary-nav-item.png) ou ![](assets/delete-secondary-nav-item.png) não pode ser oculto.

   * Arrastar itens ![](assets/move-icon---dots.png) para alterar sua ordem no painel esquerdo.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>Opção</th> 
      <th>Quando os usuários clicam no seguinte...</th> 
      <th>Eles veem os itens do painel esquerdo escolhidos dentre os itens a seguir:</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td>[!UICONTROL Project]</td> 
      <td>O nome de um projeto</td> 
      <td>[!UICONTROL Tarefas], [!UICONTROL Detalhes do projeto], [!UICONTROL Caso de negócios], [!UICONTROL Atualizações], [!UICONTROL Documentos], [!UICONTROL Problemas], [!UICONTROL Risks], [!UICONTROL Aprovações], [!UICONTROL Linhas de base], [!UICONTROL Taxas de faturamento], [!UICONTROL Registros de faturamento] , [!UICONTROL Despesas], [!UICONTROL Horas], [!UICONTROL Balanceador de carga de trabalho], [!UICONTROL Pessoas], [!UICONTROL Utilização], [!UICONTROL Detalhes da fila], [!UICONTROL Regras de roteamento], [!UICONTROL Tópico da fila], [!UICONTROL Grupo de tópico], [!UICONTROL Métricas]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Tarefa]</td> 
      <td>O nome de uma tarefa</td> 
      <td> [!UICONTROL Atualizações], [!UICONTROL Documentos], [!UICONTROL Detalhes da tarefa], [!UICONTROL Subtarefa], [!UICONTROL Problemas], [!UICONTROL Horas], [!UICONTROL Aprovações], [!UICONTROL Despesas], [!UICONTROL Predecessores]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Problema]</td> 
      <td>O nome de um problema</td> 
      <td> [!UICONTROL Atualizações], [!UICONTROL Documentos], [!UICONTROL Detalhes da edição], [!UICONTROL Hours], [!UICONTROL Aprovações]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Portfolio]</td> 
      <td>O nome de um portfólio</td> 
      <td>[!UICONTROL Projetos], [!UICONTROL Programas], [!UICONTROL Detalhes do Portfolio], [!UICONTROL Portfolio] [!UICONTROL Otimização], [!UICONTROL Documentos], [!UICONTROL Atualizações]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Program]</td> 
      <td>O nome de um programa</td> 
      <td>[!UICONTROL Projetos], [!UICONTROL Detalhes do programa], [!UICONTROL Atualizações], [!UICONTROL Documentos]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Modelo]</td> 
      <td>O nome de um modelo de projeto</td> 
      <td>[!UICONTROL Tarefas de modelo], [!UICONTROL Detalhes do modelo], [!UICONTROL Atualizações], [!UICONTROL Documentos], [!UICONTROL Risks], [!UICONTROL Despesas], [!UICONTROL Pessoas], [!UICONTROL Aprovações], [!UICONTROL Taxas de faturamento], [!UICONTROL Detalhes da fila], [!UICONTROL Regras de roteamento], [!UICONTROL Tópico da fila], [!UICONTROL Grupo de tópicos]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Tarefa de modelo]</td> 
      <td>O nome de uma tarefa de modelo</td> 
      <td>[!UICONTROL Atualizações], [!UICONTROL Documentos], [!UICONTROL Detalhes da tarefa do modelo], [!UICONTROL Subtarefas], [!UICONTROL Despesas], [!UICONTROL Aprovações], [!UICONTROL Predecessores]</td>
     </tr>
     <!--
      <tr> 
       <td>Document</td> 
       <td>Document Details (for a document uploaded to Workfront)</td> 
       <td>Updates, Approvals, All Versions, Custom Forms</td> 
      </tr>
     --> 
     <tr> 
      <td> [!UICONTROL Registro de Faturamento]</td> 
      <td>O nome de um registro de faturamento de um projeto</td> 
      <td>[!UICONTROL Detalhes do registro de faturamento], [!UICONTROL Horas faturáveis], [!UICONTROL Despesas faturáveis], [!UICONTROL Receitas fixas]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Projetos]</td> 
      <td>Projetos <img src="assets/projects-in-main-menu.png"> no menu principal [!UICONTROL] <img src="assets/main-menu-icon.png"></td> 
      <td>[!UICONTROL Projetos]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Solicitações]</td> 
      <td>O nome de uma solicitação</td> 
      <td>[!UICONTROL Nova solicitação], [!UICONTROL Solicitações enviadas], [!UICONTROL Todas as solicitações], [!UICONTROL Rascunhos]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Painéis]</td> 
      <td>O nome de um painel</td> 
      <td>[!UICONTROL Meus painéis], [!UICONTROL Painéis compartilhados], [!UICONTROL Todos os painéis]<p><b>OBSERVAÇÃO</b>: Se você criou guias personalizadas para a área [!UICONTROL Relatórios] usando um modelo de layout em [!DNL Adobe Workfront Classic], serão exibidos na parte inferior dessa lista. Para usuários, eles são exibidos na parte inferior do painel esquerdo na área [!UICONTROL Painéis] .</p> </td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Equipe de verificação]</td> 
      <td>O nome de uma equipe do Scrum</td> 
      <td><p>[!UICONTROL Iterações], [!UICONTROL iteração atual], [!UICONTROL Backlog], [!UICONTROL Workload Balancer], [!UICONTROL Atualizações], [!UICONTROL Configurações da equipe]</p> <p><strong>OBSERVAÇÃO:</strong> O <strong>[!UICONTROL iteração atual]</strong> item é exibido somente no painel esquerdo quando há pelo menos uma tarefa ou problema na iteração.</p></td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Equipe Kanban]</td> 
      <td>O nome de uma equipe kanban</td> 
      <td>[!UICONTROL Balanceador de carga de trabalho], [!UICONTROL Kanban board], [!UICONTROL Backlog], [!UICONTROL Atualizações], [!UICONTROL Configurações da equipe]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Equipe de cascata]</td> 
      <td>O nome de uma equipe de Quebra d'água</td> 
      <td>[!UICONTROL Balanceador de carga de trabalho], [!UICONTROL Atualizações], [!UICONTROL Solicitações da equipe], [!UICONTROL Configurações da equipe]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Iteration]</td> 
      <td>O nome de uma iteração</td> 
      <td>[!UICONTROL Histórias], [!UICONTROL Problemas], [!UICONTROL Story Board], [!UICONTROL Visão geral], [!UICONTROL Forms personalizado], [!UICONTROL Atualizações] </td> 
     </tr> 
     <!--
      <tr> 
       <td>Company</td> 
       <td>The name of the company</td> 
       <td> <p>People (cannot be hidden), Billing Rates, Custom Forms </p> </td> 
      </tr>
     --> 
     <!--
      <tr> 
       <td>Timesheets</td> 
       <td>The name of the timesheet</td> 
       <td>My Timesheets, Timesheets I Approve, All Timesheets (cannot be hidden) </td> 
      </tr>
     --> 
     <!--
      <tr> 
       <td>Resourcing</td> 
       <td>The name of the resource</td> 
       <td>Planner (cannot be hidden), Workload Balancer, Utilization, Resource Pools </td> 
      </tr>
     --> 
     <!--
      <tr> 
       <td>User Details</td> 
       <td>____________</td> 
       <td>Details (cannot be hidden), Org Chart, Time Off, Custom Forms </td> 
      </tr>
     --> 
    </tbody> 
   </table>

   >[!NOTE]
   >
   >Os últimos 3 itens no **[!UICONTROL Personalize o que os usuários veem]** lista suspensa ([!UICONTROL Listas], [!UICONTROL Início e resumo]e [!UICONTROL Marca]) são para configurar áreas diferentes do painel esquerdo. Para obter informações sobre eles, consulte estes artigos:
>   * [Personalizar filtros, exibições e agrupamentos usando um modelo de layout](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)
>* [Personalizar [!UICONTROL Início] e [!UICONTROL Resumo] uso de um modelo de layout](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-home-summary-layout-template.md)
* [Adobe da marca [!DNL Workfront] uso de um modelo de layout](../../../administration-and-setup/customize-workfront/use-layout-templates/brand-wf-using-a-layout-template.md)



1. (Opcional) Se quiser adicionar um item de painel esquerdo vinculado a um dos painéis de sua organização, clique em **[!UICONTROL Adicionar seção personalizada]**, digite a **[!UICONTROL Título da seção personalizada]** para o item, em seguida, adicione o painel.

   Os itens do painel aparecem na parte inferior do painel esquerdo. Os usuários veem o título da seção Personalizada que você digita ao lado do item do painel ao passar o mouse sobre o painel esquerdo.

   >[!NOTE]
   Os usuários podem adicionar itens personalizados do painel ao seu próprio painel esquerdo. Quando você adiciona itens de painel personalizados em um modelo de layout, seus itens se mesclam aos deles, sem sobrescrever ou redefinir. Isso também acontece se você atribuir usuários a um novo modelo de layout com itens personalizados do painel. Para obter informações sobre como os usuários podem personalizar o painel esquerdo, consulte [Criar guias ou seções personalizadas](../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/create-custom-tabs.md).

   Para obter informações sobre painéis, consulte [Painéis](../../../reports-and-dashboards/dashboards/dashboards-overview.md).

1. Continue personalizando o modelo de layout.

   Ou

   Se tiver terminado de personalizar, clique em **[!UICONTROL Salvar]**.

   >[!TIP]
   Você pode clicar em [!UICONTROL Salvar] a qualquer momento para salvar seu progresso, continue modificando o template posteriormente.
