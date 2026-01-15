---
title: Personalizar o painel esquerdo usando um modelo de layout
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: Em um modelo de layout, você pode personalizar o que os usuários veem na área do painel esquerdo em todo o Adobe Workfront.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: b100ea35-e045-4021-b5be-2c9071b381da
source-git-commit: c037b4f9e5530d8dd796bed25021f7073f16061f
workflow-type: tm+mt
source-wordcount: '1095'
ht-degree: 2%

---

# Personalizar o painel esquerdo usando um modelo de layout

<!--Audited: 10/2024-->

Em um modelo de layout, você pode personalizar o que os usuários veem na área do painel esquerdo no [!DNL Adobe Workfront].

Por exemplo, você pode determinar quais dos seguintes itens os usuários veem no painel esquerdo ao visualizar um projeto:

![Painel esquerdo de um projeto](assets/left-panel-in-project.png)

>[!IMPORTANT]
>
>As alterações feitas no pedido e na visibilidade são refletidas no aplicativo móvel.

Para obter informações sobre como criar modelos de layout, consulte [Criar e gerenciar modelos de layout](../use-layout-templates/create-and-manage-layout-templates.md).

Para obter informações sobre modelos de layout para grupos, consulte [Criar e modificar modelos de layout de um grupo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

Após configurar um modelo de layout, você deve atribuí-lo aos usuários para que as alterações feitas fiquem visíveis para outros usuários. Para obter informações sobre como atribuir um modelo de layout aos usuários, consulte [Atribuir usuários a um modelo de layout](../use-layout-templates/assign-users-to-layout-template.md).

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Pacote do Adobe Workfront</td> 
   <td><p>Qualquer</p>
       <p>Adicionar aplicativos personalizados ao menu principal só está disponível para organizações licenciadas para o Adobe App Builder.</p></td> 
  </tr> 
  <tr> 
   <td>Licença do Adobe Workfront</td> 
   <td><p>Padrão</p>
       <p>Plano</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td>Configurações de nível de acesso</td> 
   <td> <p>Para executar essas etapas no nível do sistema, você precisa do nível de acesso Administrador do sistema.</p>
        <p>Para executá-las para um grupo, você deve ser um gerente desse grupo.</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Personalizar o painel esquerdo para uma área em [!DNL Workfront]:

1. Comece a trabalhar em um modelo de layout, conforme descrito em [Criar e gerenciar modelos de layout](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
1. Clique na seta para baixo ![Seta para baixo](assets/dropdown-arrow.png) em **[!UICONTROL Personalize o que os usuários veem]** e clique no nome de um tipo de objeto ou de uma área [!DNL Workfront] cujo painel esquerdo você deseja personalizar.

   Os tipos de objetos e as áreas [!DNL Workfront] cujo painel esquerdo você pode personalizar estão listados na tabela a seguir:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>Tipo de objeto ou área [!DNL Workfront]</th> 
      <th>Quando os usuários clicarem no seguinte...</th> 
      <th>Seções no painel esquerdo que os usuários veem depois que você as mostra no modelo de layout:</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td>[!UICONTROL Projeto]</td> 
      <td>O nome de um projeto</td> 
      <td>[!UICONTROL Tarefas], [!UICONTROL Detalhes do Projeto], [!UICONTROL Business Case], [!UICONTROL Atualizações], [!UICONTROL Documentos], [!UICONTROL Problemas], [!UICONTROL Riscos], [!UICONTROL Aprovações], [!UICONTROL Linhas de Base], [!UICONTROL Taxas de Cobrança], [!UICONTROL Registros de Cobrança], [!UICONTROL Despesas], [!UICONTROL Horas], [!UICONTROL Balanceador de Carga de Trabalho], [!UICONTROL Pessoas], [!UICONTROL Utilização], [!UICONTROL Detalhes da Fila], [!UICONTROL Regras de Roteamento], [!UICONTROL Tópico de Fila], [!UICONTROL Grupo de Tópicos], [!UICONTROL Métricas], [!UICONTROL Planning]*, [!UICONTROL Aplicativo personalizado]**</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Tarefa]</td> 
      <td>O nome de uma tarefa</td> 
      <td> [!UICONTROL Atualizações], [!UICONTROL Documentos], [!UICONTROL Detalhes da Tarefa], [!UICONTROL Subtarefa], [!UICONTROL Problemas], [!UICONTROL Horas], [!UICONTROL Aprovações], [!UICONTROL Despesas], [!UICONTROL Predecessoras], [!UICONTROL Aplicativo Personalizado]**</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Problema]</td> 
      <td>O nome de um problema</td> 
      <td> [!UICONTROL Atualizações], [!UICONTROL Documentos], [!UICONTROL Detalhes do Problema], [!UICONTROL Horas], [!UICONTROL Aprovações], [!UICONTROL Aplicativo Personalizado]**</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Portfolio]</td> 
      <td>O nome de um portfólio</td> 
      <td>[!UICONTROL Projetos], [!UICONTROL Programas], [!UICONTROL Detalhes do Portfolio], [!UICONTROL Portfolio] [!UICONTROL Otimização], [!UICONTROL Documentos], [!UICONTROL Atualizações], [!UICONTROL Planejamento]*, [!UICONTROL Aplicativo Personalizado]**</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Program]</td> 
      <td>O nome de um programa</td> 
      <td>[!UICONTROL Projetos], [!UICONTROL Detalhes do Programa], [!UICONTROL Atualizações], [!UICONTROL Documentos], [!UICONTROL Planejamento]*, [!UICONTROL Aplicativo Personalizado]**</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Modelo]</td> 
      <td>O nome de um modelo de projeto</td> 
      <td>[!UICONTROL Tarefas de Modelo], [!UICONTROL Detalhes de Modelo], [!UICONTROL Atualizações], [!UICONTROL Documentos], [!UICONTROL Riscos], [!UICONTROL Despesas], [!UICONTROL Pessoas], [!UICONTROL Aprovações], [!UICONTROL Taxas de Cobrança], [!UICONTROL Detalhes da Fila], [!UICONTROL Regras de Roteamento], [!UICONTROL Tópico de Fila], [!UICONTROL Grupo de Tópicos]</td> 
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
      <td>[!UICONTROL Projects]</td> 
      <td>Projetos <img src="assets/projects-in-main-menu.png"> no menu principal  <img src="assets/main-menu-icon.png"></td> 
      <td>[!UICONTROL Projects]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Solicitações]</td> 
      <td>O nome de uma solicitação</td> 
      <td>[!UICONTROL Nova Solicitação], [!UICONTROL Solicitações Enviadas], [!UICONTROL Todas as Solicitações], [!UICONTROL Rascunhos]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Painéis]</td> 
      <td>O nome de um painel</td> 
      <td>[!UICONTROL Meus Painéis], [!UICONTROL Painéis Compartilhados], [!UICONTROL Todos os Painéis]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Equipe de Scrum]</td> 
      <td>O nome de uma equipe Scrum</td> 
      <td><p>[!UICONTROL Iterações], [!UICONTROL Iteração atual], [!UICONTROL Lista de Pendências], [!UICONTROL Balanceador de Carga de Trabalho], [!UICONTROL Atualizações], [!UICONTROL Configurações de Equipe]</p> <p><strong>OBSERVAÇÃO:</strong> o item <strong>[!UICONTROL Iteração atual]</strong> só é exibido no painel esquerdo quando há pelo menos uma tarefa ou problema na iteração.</p></td> 
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

   *Sua empresa deve comprar uma licença adicional para que o Workfront Planning possa adicionar essa área ao painel esquerdo de projetos, portfólios e programas. Para obter mais informações, consulte [Introdução ao Adobe Workfront Planning](/help/quicksilver/planning/general/planning-overview.md)

   **Os aplicativos personalizados devem ser criados separadamente antes de serem disponibilizados como opções do Menu principal. Para obter mais informações, consulte [Criar um aplicativo personalizado para o Workfront com o Adobe App Builder](/help/quicksilver/app-builder/app-builder.md).


1. Na lista **[!UICONTROL Painel esquerdo]**, siga um destes procedimentos para determinar o que os usuários verão no painel esquerdo para a área [!DNL Workfront] ou o tipo de objeto selecionado:

   * Clique nos ícones **Mostrar** ![Mostrar ícone](assets/add-secondary-nav-item.png) ou **Ocultar** ![Ocultar ícone](assets/delete-secondary-nav-item.png) para exibir ou ocultar seções no painel esquerdo. Você não pode ocultar itens que não tenham um ícone **Mostrar** ou **Ocultar**.

   * Arraste os itens ![ícone Mover](assets/move-icon---dots.png) para alterar sua ordem no painel esquerdo.

   >[!NOTE]
   >
   >Os seguintes itens da **[!UICONTROL Personalize o que os usuários veem]** na lista suspensa se referem a áreas diferentes do painel esquerdo:
   >* [!UICONTROL Listas]
   >* [!UICONTROL Painel de resumo]
   >* [!UICONTROL Página inicial]
   >* [!UICONTROL Identidade visual]
   > 
   >Para obter informações sobre como personalizar as áreas adicionais, consulte os seguintes artigos:
   >
   >* [Personalizar Filtros, Modos de Exibição e Agrupamentos usando um modelo de layout](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)
   >* [Personalizar o [!UICONTROL Painel de resumo] usando um modelo de layout](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-home-summary-layout-template.md)
   >* [Personalizar Página Inicial usando um modelo de layout](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-new-home-layout-template.md)
   >* [Brand Adobe [!DNL Workfront] usando um modelo de layout](../../../administration-and-setup/customize-workfront/use-layout-templates/brand-wf-using-a-layout-template.md)


1. (Opcional) Se você deseja adicionar um item do painel esquerdo que se vincula a um dos painéis da sua organização, clique em **[!UICONTROL Adicionar painel]**, digite o **[!UICONTROL Nome rápido do link]** para o item e escolha o painel.

   Você deve criar o painel antes que ele apareça na lista.

   Os itens do painel são exibidos na parte inferior do painel esquerdo.

   >[!NOTE]
   >
   >Os usuários podem adicionar itens personalizados do painel a seu próprio painel esquerdo. Ao adicionar itens personalizados do painel em um modelo de layout, seus itens são exibidos além daqueles que adicionam, sem substituí-los ou redefini-los. Isso também é verdadeiro se você atribuir usuários a um novo modelo de layout com itens de painel personalizados. Para obter informações sobre como os usuários podem personalizar o painel esquerdo, consulte [Adicionar um painel no painel esquerdo de um objeto ou área do Workfront](../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/create-custom-tabs.md).
   >
   >Para obter informações sobre painéis, consulte [Painéis](../../../reports-and-dashboards/dashboards/dashboards-overview.md).

1. Continue personalizando o modelo de layout. Você pode clicar em **Aplicar** a qualquer momento para salvar seu progresso.

   Ou

   Se tiver terminado de personalizar, clique em **Salvar e Fechar**.
