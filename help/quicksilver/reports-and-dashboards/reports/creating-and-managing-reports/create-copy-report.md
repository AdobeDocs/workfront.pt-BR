---
product-area: reporting;user-management
keywords: salvar,novo,relatório,copiar
navigation-topic: create-and-manage-reports
title: Criar uma cópia de um relatório
description: É possível criar uma cópia de qualquer relatório que você tenha acesso a. Você pode criar uma cópia exata de um relatório personalizado ou pode salvar uma nova versão de um relatório padrão. Após copiar um relatório, você se torna o proprietário do relatório copiado e ele é exibido na seção Meus relatórios .
author: Nolan
feature: Reports and Dashboards
exl-id: 84737f48-efc5-45f1-acd1-b9f5d353f80f
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '682'
ht-degree: 0%

---

# Criar uma cópia de um relatório

É possível criar uma cópia de qualquer relatório que você tenha acesso a. Você pode criar uma cópia exata de um relatório personalizado ou pode salvar uma nova versão de um relatório padrão. Após copiar um relatório, você se torna o proprietário do relatório copiado e ele é exibido na seção Meus relatórios .

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plano Adobe Workfront*</td> 
   <td> <p>Qualquer Um</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Plano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a Relatórios, Painéis, Calendários</p> <p>Editar acesso a filtros, visualizações, agrupamentos</p> <p>Observação: Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Exibir permissões para um relatório</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

## Criar uma cópia exata de um relatório

Se você deseja fazer uma cópia de um relatório do qual é proprietário, faça o seguinte:

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront.

1. Clique em **Relatórios**, em seguida **Todos os relatórios**.
1. Abra um relatório.
1. Clique em **Ações de Relatório**, em seguida **Copiar**.

   >[!TIP]
   >
   >Se o relatório for um relatório padrão, a opção Copiar não será exibida no menu Ações de relatório.\
   >Para obter informações sobre como criar uma cópia de um relatório padrão, consulte [Criar uma nova versão de um relatório](#create-a-new-version-of-a-report).

   ![Copiar relatório](assets/nwe-fulllistofreportactions-2022.png)

   Uma cópia do relatório original é criada com o nome padrão de *Cópia de [Nome do relatório original]*. Por exemplo, o relatório &quot;Tarefas concluídas do quarto trimestre&quot; teria &quot;Cópia de tarefas concluídas do quarto trimestre&quot; como o nome.

1. (Opcional) Para renomear o relatório, comece a digitar um novo nome.

   >[!TIP]
   >
   >Se você desmarcar o título antes de digitar o novo nome, selecione o título do relatório, exclua o nome e insira o novo nome.

1. (Opcional) Para compartilhar a nova versão do relatório com outros usuários, clique em **Ações de Relatório**, em seguida **Compartilhamento**.

   >[!NOTE]
   >
   >As informações de compartilhamento não são transferidas para o relatório copiado da versão original.\
   >Para obter informações sobre como ver com quem o relatório anterior foi compartilhado, consulte [Criar um relatório sobre atividades de relatório](../../../reports-and-dashboards/reports/report-usage/create-report-reporting-activities.md#identify).

1. (Opcional) Se você tiver permissões de gerenciamento para o relatório original e o relatório original não for mais necessário, é possível excluí-lo para remover relatórios duplicados desnecessários no Workfront.

   Para excluir o relatório original, faça o seguinte:

   1. Navegue até o relatório .
   1. Clique em **Ações de Relatório**, em seguida **Excluir**.

   1. Clique em **Sim, Excluir** para confirmar que você deseja excluir o relatório.

## Criar uma nova versão de um relatório {#create-a-new-version-of-a-report}

Se quiser criar uma cópia de um relatório padrão, faça o seguinte:

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront.

1. Clique em **Relatórios**, em seguida **Todos os relatórios**.
1. Clique no nome de um relatório padrão para abri-lo.
1. Clique em **Ações de Relatório**, em seguida **Editar**.

   ![Editar relatório](assets/nwe-reportactionsfordefaultreport-2022.png)

1. Faça as modificações necessárias nas guias a seguir do relatório:

   * **Colunas (Exibir)**: Para obter mais informações sobre como personalizar exibições, consulte o artigo [Visão geral das exibições no Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).
   * **Agrupamentos**: Para obter mais informações sobre como personalizar agrupamentos, consulte o artigo [Visão geral dos agrupamentos no Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).
   * **Filtros**: Para obter mais informações sobre como personalizar filtros, consulte o artigo [Visão geral dos filtros no Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).
   * **Gráfico**: Para obter mais informações sobre como personalizar um gráfico de relatório, consulte o artigo [Adicionar um gráfico a um relatório](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md).

1. No canto superior direito, clique em **Configurações do relatório**.
1. No **Título do relatório** , dê um novo nome ao relatório.
1. Clique em **Concluído**.
1. Clique em **Salvar como novo relatório**.

   ![](assets/nwe-save-as-new-report-350x220.png)

1. (Opcional) Para compartilhar a nova versão do relatório com outros usuários, clique em **Ações de Relatório**, em seguida **Compartilhamento**.
