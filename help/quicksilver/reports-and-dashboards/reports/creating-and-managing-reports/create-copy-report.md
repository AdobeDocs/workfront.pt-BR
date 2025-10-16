---
product-area: reporting;user-management
keywords: salvar,novo,relatório,copiar
navigation-topic: create-and-manage-reports
title: Criar uma cópia de um relatório
description: É possível criar uma cópia de qualquer relatório ao qual você tenha acesso. Você pode criar uma cópia exata de um relatório personalizado ou salvar uma nova versão de um relatório padrão. Depois de copiar um relatório, você se torna o proprietário do relatório copiado e ele é exibido na seção Meus relatórios.
author: Nolan
feature: Reports and Dashboards
exl-id: 84737f48-efc5-45f1-acd1-b9f5d353f80f
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '641'
ht-degree: 0%

---

# Criar uma cópia de um relatório

<!-- Audited: 11/2024 -->

É possível criar uma cópia de qualquer relatório ao qual você tenha acesso. Você pode criar uma cópia exata de um relatório personalizado ou salvar uma nova versão de um relatório padrão. Depois de copiar um relatório, você se torna o proprietário do relatório copiado e ele é exibido na seção Meus relatórios.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacote do Adobe Workfront</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td> 
      <p>Standard</p>
      <p>Plano</p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Configuração do nível de acesso</td> 
   <td> <p>Editar acesso a relatórios, painéis, calendários</p> <p>Editar acesso a Filtros, Visualizações, Agrupamentos</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Exibir permissões para um relatório</p>  </td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Criar uma cópia exata de um relatório

Se quiser fazer uma cópia de um relatório personalizado, faça o seguinte:

1. Clique no ícone **[!UICONTROL Menu Principal]** ![Menu Principal](/help/_includes/assets/main-menu-icon.png) no canto superior direito do Adobe Workfront ou (se disponível) clique no ícone **[!UICONTROL Menu Principal]** ![Menu Principal](/help/_includes/assets/main-menu-icon-left-nav.png) no canto superior esquerdo e clique em **[!UICONTROL Relatórios]**.

1. Clique em **Todos os relatórios** e abra um relatório.

1. Clique em **Ações de Relatório** e em **Copiar**.

   >[!TIP]
   >
   >Se o relatório for um relatório padrão, a opção Copiar não aparecerá no menu Ações de Relatório.\
   >Para obter informações sobre como criar uma cópia de um relatório padrão, consulte [Criar uma nova versão de um relatório](#create-a-new-version-of-a-report).

   ![Copiar relatório](assets/unshimmed-report-actions-copy.png)

   Uma cópia do relatório original é criada com o nome padrão de _[Nome do relatório original] (Cópia)_. Por exemplo, uma cópia do relatório &quot;Tarefas concluídas do quarto trimestre&quot; seria nomeada &quot;Tarefas concluídas do quarto trimestre (Cópia)&quot;.

1. (Opcional) Para renomear o relatório, clique em **Ações de Relatório** e em **Editar**. Digite um novo nome na caixa de texto no canto superior esquerdo e clique em **Salvar + Fechar** quando terminar.

1. (Opcional) Para compartilhar a nova versão do relatório com outros usuários, clique em **Ações de Relatório** e depois em **Compartilhamento**.

   >[!NOTE]
   >
   >As informações de compartilhamento não são transferidas para o relatório copiado da versão original.\
   >Para obter informações sobre como ver com quem o relatório anterior foi compartilhado, consulte [Criar um relatório sobre atividades de relatório](../../../reports-and-dashboards/reports/report-usage/create-report-reporting-activities.md#identify).

1. (Opcional) Se você tiver Gerenciar permissões para o relatório original e o relatório original não for mais necessário, você poderá excluí-lo para remover relatórios duplicados desnecessários no Workfront.

   Para excluir o relatório original, faça o seguinte:

   1. Navegue até o relatório.

   1. Clique em **Ações de Relatório** e depois em **Excluir**.

   1. Clique em **Sim, exclua-o** para confirmar que deseja excluir o relatório.

## Criar uma nova versão de um relatório {#create-a-new-version-of-a-report}

Se quiser criar uma cópia de um relatório incorporado, faça o seguinte:

1. Clique no ícone **Menu Principal** ![Ícone do Menu Principal](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront.

1. Clique em **Relatórios** e depois em **Todos os Relatórios**.
1. Clique no nome de um relatório integrado para abri-lo.
1. Clique em **Ações de Relatório** e depois em **Editar**.

   ![Editar relatório](assets/unshimmed-report-actions-default-report.png)

1. Faça as modificações necessárias nas seguintes guias do relatório:

   * **Colunas (Modo de Exibição)**: Para obter mais informações sobre como personalizar modos de exibição, consulte o artigo [Visão geral dos modos de exibição no Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).
   * **Agrupamentos**: para obter mais informações sobre como personalizar agrupamentos, consulte o artigo [Visão geral de agrupamentos no Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).
   * **Filtros**: para obter mais informações sobre como personalizar filtros, consulte o artigo [Visão geral dos filtros](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).
   * **Gráfico**: para obter mais informações sobre como personalizar um gráfico de relatório, consulte o artigo [Adicionar um gráfico a um relatório](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md).

1. No canto superior direito, clique em **Configurações do relatório**.
1. No campo **Título do relatório**, dê um novo nome ao relatório.
1. Clique em **Concluído**.
1. Clique em **Salvar como Novo Relatório**.

   ![Salvar como novo relatório](assets/unshimmed-save-as-new-report.png)

1. (Opcional) Para compartilhar a nova versão do relatório com outros usuários, clique em **Ações de Relatório** e depois em **Compartilhamento**.
