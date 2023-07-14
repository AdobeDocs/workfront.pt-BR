---
title: Personalizar o painel esquerdo usando um modelo de layout
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: Em um modelo de layout, você pode personalizar o que os usuários veem na área do painel esquerdo em todo o Adobe Workfront.
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: b100ea35-e045-4021-b5be-2c9071b381da
source-git-commit: 7ee96045e5673c51c3ce348f395226857686a923
workflow-type: tm+mt
source-wordcount: '1025'
ht-degree: 0%

---

# Personalizar o painel esquerdo usando um modelo de layout

Em um modelo de layout, você pode personalizar o que os usuários veem na área do painel esquerdo em todo o [!DNL Adobe Workfront].

Por exemplo, você pode determinar qual dos seguintes itens os usuários veem no painel esquerdo ao visualizar uma tarefa:

![](assets/left-panel-adobe-branding.png)

>[!IMPORTANT]
>
>As alterações feitas no pedido e na visibilidade são refletidas no aplicativo móvel.

Para obter informações sobre como criar modelos de layout, consulte [Criar e gerenciar modelos de layout](../use-layout-templates/create-and-manage-layout-templates.md).

Para obter informações sobre modelos de layout para grupos, consulte [Criar e modificar os modelos de layout de um grupo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

Após configurar um modelo de layout, você deve atribuí-lo aos usuários para que as alterações feitas fiquem visíveis para outros usuários. Para obter informações sobre como atribuir um modelo de layout aos usuários, consulte [Atribuir usuários a um modelo de layout](../use-layout-templates/assign-users-to-layout-template.md).

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas deste artigo:

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
   <td>[!UICONTROL Plano]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> Para executar essas etapas no nível do sistema, você precisa do nível de acesso [!UICONTROL Administrador do Sistema].<p>Para executá-las para um grupo, você deve ser um gerente desse grupo.</p> <p><b>NOTA</b>: Se ainda não tiver acesso, pergunte ao seu [!DNL Workfront] administrador se eles definirem restrições adicionais no seu nível de acesso. Para obter informações sobre como uma [!DNL Workfront] administrador pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Personalizar o painel esquerdo para uma área no [!DNL Workfront]:

1. Comece a trabalhar em um modelo de layout, conforme descrito em [Criar e gerenciar modelos de layout](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
1. Clique na seta para baixo ![](assets/dropdown-arrow.png) em **[!UICONTROL Personalize o que os usuários veem]** e, em seguida, clique no painel esquerdo que deseja personalizar.

   >[!NOTE]
   >
   >Para obter informações sobre o [!UICONTROL Início] nesta lista suspensa, consulte [Personalizar [!UICONTROL Início] e [!UICONTROL Resumo] uso de um modelo de layout](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-home-summary-layout-template.md). Para obter informações sobre a opção Listas, consulte [Personalizar filtros, visualizações e agrupamentos usando um modelo de layout](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md).

1. No **[!UICONTROL Painel esquerdo]** faça o seguinte para determinar o que os usuários verão no painel esquerdo para a opção ([!DNL Workfront] tipo de objeto) que você selecionou:

   * Mostrar ![](assets/add-secondary-nav-item.png) ou ocultar ![](assets/delete-secondary-nav-item.png) itens. Qualquer item sem ![](assets/add-secondary-nav-item.png) ou ![](assets/delete-secondary-nav-item.png) não pode ser oculto.

   * Arrastar itens ![](assets/move-icon---dots.png) para alterar a ordem no painel esquerdo.
   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>Opção</th> 
      <th>Quando os usuários clicarem no seguinte...</th> 
      <th>Eles verão os itens do painel esquerdo que você escolher entre os seguintes:</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td>[!UICONTROL Projeto]</td> 
      <td>O nome de um projeto</td> 
      <td>[!UICONTROL Tarefas], [!UICONTROL Detalhes do Projeto], [!UICONTROL Business Case], [!UICONTROL Atualizações], [!UICONTROL Documentos], [!UICONTROL Problemas], [!UICONTROL Riscos], [!UICONTROL Aprovações], [!UICONTROL Linhas de Base], [!UICONTROL Taxas de Cobrança], [!UICONTROL Registros de Cobrança], [!UICONTROL Despesas], [!UICONTROL CONTROL Hours, [!UICONTROL Balanceador de Carga de Trabalho], [!UICONTROL People], [!UICONTROL Utilização], [!UICONTROL Detalhes da Fila], [!UICONTROL Regras de Roteamento], [!UICONTROL Tópico de Fila], [!UICONTROL Grupo de Tópicos], [!UICONTROL Métricas]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Tarefa]</td> 
      <td>O nome de uma tarefa</td> 
      <td> [!UICONTROL Atualizações], [!UICONTROL Documentos], [!UICONTROL Detalhes da Tarefa], [!UICONTROL Subtarefa], [!UICONTROL Problemas], [!UICONTROL Horas], [!UICONTROL Aprovações], [!UICONTROL Despesas], [!UICONTROL Predecessoras]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Problema]</td> 
      <td>O nome de um problema</td> 
      <td> [!UICONTROL Atualizações], [!UICONTROL Documentos], [!UICONTROL Detalhes do Problema], [!UICONTROL Horas], [!UICONTROL Aprovações]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Portfolio]</td> 
      <td>O nome de um portfólio</td> 
      <td>[!UICONTROL Projetos], [!UICONTROL Programas], [!UICONTROL Detalhes do Portfolio], [!UICONTROL Portfolio] [!UICONTROL Otimização], [!UICONTROL Documentos], [!UICONTROL Atualizações]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Programa]</td> 
      <td>O nome de um programa</td> 
      <td>[!UICONTROL Projetos], [!UICONTROL Detalhes do Programa], [!UICONTROL Atualizações], [!UICONTROL Documentos]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Modelo]</td> 
      <td>O nome de um modelo de projeto</td> 
      <td>[!UICONTROL Tarefas de Modelo], [!UICONTROL Detalhes de Modelo], [!UICONTROL Atualizações], [!UICONTROL Documentos], [!UICONTROL Riscos], [!UICONTROL Despesas], [!UICONTROL Pessoas], [!UICONTROL Aprovações], [!UICONTROL Taxas de Cobrança], [!UICONTROL Detalhes da Fila], [!UICONTROL Regras de Roteamento], [!UICONTROL Tópico de Fila], [!UICONTROL!UICONTROL Grupo de Tópicos]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Modelo de Tarefa]</td> 
      <td>O nome de uma tarefa de modelo</td> 
      <td>[!UICONTROL Atualizações], [!UICONTROL Documentos], [!UICONTROL Detalhes da Tarefa de Modelo], [!UICONTROL Subtarefas], [!UICONTROL Despesas], [!UICONTROL Aprovações], [!UICONTROL Predecessoras]</td>
     </tr>
     <!--
      <tr> 
       <td>Document</td> 
       <td>Document Details (for a document uploaded to Workfront)</td> 
       <td>Updates, Approvals, All Versions, Custom Forms</td> 
      </tr>
     --> 
     <tr> 
      <td> [!UICONTROL Registro de Cobrança]</td> 
      <td>O nome de um registro de cobrança para um projeto</td> 
      <td>[!UICONTROL Detalhes de Registro de Cobrança], [!UICONTROL Horas Faturáveis], [!UICONTROL Despesas Faturáveis], [!UICONTROL Receitas Fixas]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Projetos]</td> 
      <td>Projetos <img src="assets/projects-in-main-menu.png"> no menu principal [!UICONTROL] <img src="assets/main-menu-icon.png"></td> 
      <td>[!UICONTROL Projetos]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Solicitações]</td> 
      <td>O nome de uma solicitação</td> 
      <td>[!UICONTROL Nova Solicitação], [!UICONTROL Solicitações Enviadas], [!UICONTROL Todas as Solicitações], [!UICONTROL Rascunhos]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Painéis]</td> 
      <td>O nome de um painel</td> 
      <td>[!UICONTROL Meus Painéis], [!UICONTROL Painéis Compartilhados], [!UICONTROL Todos os Painéis]<p><b>NOTA</b>: se você criou guias personalizadas para a área [!UICONTROL Reports] usando um modelo de layout em [!DNL Adobe Workfront Classic], elas são exibidas na parte inferior desta lista. Para usuários, eles são exibidos na parte inferior do painel esquerdo na área [!UICONTROL Dashboards].</p> </td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Equipe de Scrum]</td> 
      <td>O nome de uma equipe Scrum</td> 
      <td><p>[!UICONTROL Iterações], [!UICONTROL Iteração atual], [!UICONTROL Lista de Pendências], [!UICONTROL Balanceador de Carga de Trabalho], [!UICONTROL Atualizações], [!UICONTROL Configurações de Equipe]</p> <p><strong>NOTA:</strong> A variável <strong>[!UICONTROL Iteração atual]</strong> o item só é exibido no painel esquerdo quando há pelo menos uma tarefa ou problema na iteração.</p></td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Equipe Kanban]</td> 
      <td>O nome de uma equipe Kanban</td> 
      <td>[!UICONTROL Balanceador de Carga], [!UICONTROL Quadro Kanban], [!UICONTROL Lista de Pendências], [!UICONTROL Atualizações], [!UICONTROL Configurações de Equipe]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Equipe de Cascata]</td> 
      <td>O nome de uma equipe do Waterfall</td> 
      <td>[!UICONTROL Balanceador de Carga], [!UICONTROL Atualizações], [!UICONTROL Solicitações de Equipe], [!UICONTROL Configurações de Equipe]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Iteração]</td> 
      <td>O nome de uma iteração</td> 
      <td>[!UICONTROL Histórias], [!UICONTROL Problemas], [!UICONTROL Story Board], [!UICONTROL Visão Geral], [!UICONTROL Custom Forms], [!UICONTROL Atualizações] </td> 
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
   >Os últimos 3 itens na **[!UICONTROL Personalize o que os usuários veem]** lista suspensa ([!UICONTROL Listas], [!UICONTROL Página inicial e resumo], e [!UICONTROL Marcas]) são para configurar áreas diferentes do painel esquerdo. Para obter informações sobre eles, consulte estes artigos:
>   >   
* [Personalizar filtros, visualizações e agrupamentos usando um modelo de layout](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)
>* [Personalizar [!UICONTROL Início] e [!UICONTROL Resumo] uso de um modelo de layout](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-home-summary-layout-template.md)
* [Adobe da marca [!DNL Workfront] uso de um modelo de layout](../../../administration-and-setup/customize-workfront/use-layout-templates/brand-wf-using-a-layout-template.md)


1. (Opcional) Se quiser adicionar um item do painel esquerdo que se vincule a um dos painéis de sua organização, clique em **[!UICONTROL Adicionar seção personalizada]**, digite um **[!UICONTROL Título da seção personalizada]** para o item, em seguida, adicione o painel.

   Os itens do painel são exibidos na parte inferior do painel esquerdo. Os usuários veem o título da seção Personalizada que você digita ao lado do item do painel quando passam o mouse sobre o painel esquerdo.

   >[!NOTE]
   >
   Os usuários podem adicionar itens personalizados do painel a seu próprio painel esquerdo. Quando você adiciona itens personalizados do painel em um modelo de layout, seus itens são mesclados com os deles, sem substituir ou redefini-los. Isso também é verdadeiro se você atribuir usuários a um novo modelo de layout com itens de painel personalizados. Para obter informações sobre como os usuários podem personalizar o painel esquerdo, consulte [Criar guias ou seções personalizadas](../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/create-custom-tabs.md).

   Para obter informações sobre painéis, consulte [Painéis](../../../reports-and-dashboards/dashboards/dashboards-overview.md).

1. Continue personalizando o modelo de layout.

   Ou

   Se tiver terminado de personalizar, clique em **[!UICONTROL Salvar]**.

   >[!TIP]
   >
   Você pode clicar em [!UICONTROL Salvar] a qualquer momento para salvar seu progresso e, em seguida, continuar modificando o modelo posteriormente.
