---
navigation-topic: use-the-gantt-chart
title: Exportar o Gráfico de Gantt para o PDF
description: É possível exportar o Diagrama de Gantt para uma PDF. Posteriormente, você pode imprimi-lo ou anexá-lo a um email para compartilhá-lo com outros usuários.
author: Alina
feature: Work Management
exl-id: 91aad9e0-25c9-4eae-aa66-8aab763d3b76
source-git-commit: c8987d036e1c1324618cb53ebcbb8fd7e4bcc6a4
workflow-type: tm+mt
source-wordcount: '979'
ht-degree: 2%

---

# Exportar o [!UICONTROL Gráfico de Gantt] para o PDF

<!--Audited: 08/2025-->

Você pode exportar o [!UICONTROL Gráfico de Gantt] para um PDF. Posteriormente, você pode imprimi-lo ou anexá-lo a um email para compartilhá-lo com outros usuários.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacote [!UICONTROL Adobe Workfront]</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da [!UICONTROL Adobe Workfront]</td> 
   <td> <p>[!UICONTROL Light] ou superior</p>
   <p>[!UICONTROL Review] ou superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>[!UICONTROL Exibir] ou superior acesso a Projetos e Tarefas</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>[!UICONTROL Exibir] ou superior acesso ao projeto e às tarefas</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront] plan</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront] license</td> 
   <td> <p>New:[!UICONTROL Light] or higher</p>
   <p>Current:[!UICONTROL Review] or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>[!UICONTROL View] or higher access to Projects and Tasks</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>[!UICONTROL View] or higher access to the project</p> </td> 
  </tr> 
 </tbody> 
</table>

-->

## Exportar o [!UICONTROL Gráfico de Gantt]

1. Acesse o [!UICONTROL Gráfico de Gantt] que você deseja exportar para o PDF, conforme descrito em [Introdução ao [!UICONTROL Gráfico de Gantt]](../../../manage-work/gantt-chart/use-the-gantt-chart/get-started-with-gantt.md).
1. Configure o [!UICONTROL Gráfico de Gantt] para exibir as informações apropriadas que você deseja exportar.

   >[!NOTE]
   >
   >Se você exportar o [!UICONTROL Gráfico de Gantt] de uma lista de projetos, o arquivo PDF conterá apenas os projetos da lista, não as tarefas de cada projeto. Se você deseja exportar uma lista de tarefas, é possível fazer isso a partir do projeto ao qual estão associadas, criando um relatório de tarefas e exibindo os resultados do relatório na [!UICONTROL Exibição de Gantt].

   Configure qualquer uma das seguintes informações:

   * Clique nos ícones **Filtros**, **Exibir** e **Agrupamento** acima do [!UICONTROL Gráfico de Gantt] e adicione ou edite o filtro, a exibição ou o agrupamento existente aplicado à lista de itens no [!UICONTROL Gráfico de Gantt].

     Quaisquer filtros e agrupamentos selecionados na exibição de lista são mantidos durante a exibição do [!UICONTROL Gráfico de Gantt]. As exibições são refletidas no [!UICONTROL Gráfico de Gantt] exportado somente na lista exibida ao lado do [!UICONTROL Gráfico de Gantt] na primeira página. Os modos de exibição não são exibidos no próprio [!UICONTROL Gráfico de Gantt].

     >[!TIP]
     >
     >Para permitir mais espaço para o [!UICONTROL Gráfico de Gantt], aplique um modo de exibição que contenha o menor número possível de colunas.

   * Selecione a opção **Alternar para Datas Projetadas** para exibir Datas Projetadas em vez de Planejadas. Por padrão, Datas planejadas são exibidas.

   * Clique no ícone **Configurações** ![Ícone Configurações](assets/settings-icon.png) no canto superior direito do gráfico de Gantt e selecione quais informações você deseja exibir. Depois de selecionadas, essas informações são incluídas no arquivo PDF de Gantt exportado.

     Selecione entre as seguintes opções:

      * Datas Efetivas
      * Atribuições
      * Linha de base
      * Data de confirmação
      * % concluído
      * Caminho Crítico
      * Etapas como diamantes
      * Linhas de etapas
      * Predecessoras
      * Status do Progresso
      * Datas Planejadas (Condicionais)
      * Datas Projetadas (Condicionais)

     Para obter mais informações, consulte   [Configure como as informações são exibidas no [!UICONTROL Gráfico de Gantt]](../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md).

     >[!NOTE]
     >
     > As atribuições não são exibidas no [!UICONTROL Gráfico de Gantt] quando o [!UICONTROL Gráfico de Gantt] é exportado para o PDF. Depois de exportadas, as atribuições são exibidas somente na exibição de lista.

   * O período exibido no [!UICONTROL Gráfico de Gantt]. A maneira como isso é exibido no arquivo de exportação depende se você selecionou **[!UICONTROL O que vejo]** ou **[!UICONTROL Várias páginas]** em uma etapa posterior.

     Para obter mais informações, consulte [Exibindo Informações no [!UICONTROL Gráfico de Gantt]](../../../manage-work/gantt-chart/use-the-gantt-chart/view-info-in-gantt.md).



1. (Opcional) Para incluir apenas determinadas tarefas no PDF exportado, selecione as tarefas que deseja incluir. Se você não selecionar nenhuma tarefa, todas as tarefas serão incluídas no PDF exportado.

   Por exemplo, se você estiver exibindo o [!UICONTROL Gráfico de Gantt] de um projeto que contém 50 tarefas, mas quiser exibir apenas 10 tarefas no [!UICONTROL Gráfico de Gantt] exportado, selecione as 10 tarefas que deseja exibir.

1. Clique no ícone da impressora ![Ícone da impressora](assets/printer-icon.png) no canto superior direito do Diagrama de Gantt.
A caixa de diálogo **[!UICONTROL Exportar para o PDF]** é exibida.

   ![Caixa de diálogo Exportar para o PDF](assets/exported-gantt-ui-350x225.png)

1. Na seção **Exportar**, selecione uma das opções a seguir para indicar se deseja exportar apenas o que você vê ou todo o [!UICONTROL Gráfico de Gantt]:

   * **[!UICONTROL O que vejo]:** exporta todas as tarefas (incluindo todas as subtarefas) exibidas na tela antes de exportar até 500 itens. (Não é o que é exibido na seção **[!UICONTROL Visualização]**; a seção **Visualização** contém apenas dados de exemplo.)

     As subtarefas são incluídas no PDF exportado mesmo se a tarefa pai for recolhida e as subtarefas não estiverem visíveis. Para incluir somente tarefas pai, selecione as tarefas pai que deseja incluir e deixe qualquer subtarefa desmarcada.

     >[!TIP]
     >
     >Você pode usar a ferramenta de zoom ou controle deslizante para exibir apenas uma parte do [!UICONTROL Gráfico de Gantt], conforme descrito em [Exibindo Informações no [!UICONTROL Gráfico de Gantt]](../../../manage-work/gantt-chart/use-the-gantt-chart/view-info-in-gantt.md). Selecione uma opção mais granular para exibir mais páginas para exportar ou selecione uma opção menos granular para exibir menos páginas para exportar.


   * **[!UICONTROL Várias páginas]:** exporta todo o [!UICONTROL Gráfico de Gantt] (até 500 itens), incluindo itens que não estão visíveis na tela atual.

     >[!NOTE]
     >
     >* Se você precisar exportar um [!UICONTROL Gráfico de Gantt] que contenha mais de 500 itens, aplique um filtro à lista antes de exibir o [!UICONTROL Gráfico de Gantt] para que menos de 500 itens ou 250 páginas sejam exibidos. Para obter informações sobre como aplicar um filtro, consulte [Visão geral dos filtros](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).
     >
     >
     >* Não é possível exportar todo o Diagrama de Gantt nas seguintes circunstâncias:
     >   
     >   * Quando abrange mais de 250 páginas.
     >   * Quando contiver mais de 500 itens.


1. Se a PDF for impressa depois de ser exportada para o PDF, selecione o tamanho do papel no qual deseja imprimir no menu suspenso **[!UICONTROL Tamanho da página]**.
Você pode selecionar entre as opções a seguir:

   * **[!UICONTROL Carta]**
   * **[!UICONTROL Assuntos legais]**
   * **[!UICONTROL Razão]**
   * **[!UICONTROL A1]**
   * **[!UICONTROL A2]**
   * **[!UICONTROL A3]** (disponível somente para alguns idiomas)
   * **[!UICONTROL A4]**
1. Na seção **[!UICONTROL Orientação da página]**, selecione se deseja que a PDF seja exportada na orientação paisagem ou retrato.
1. Selecione **[!UICONTROL Mostrar legenda]** se desejar incluir a legenda no PDF exportado.
1. Clique em **[!UICONTROL Exportar]**. O pdf é criado e baixado no computador.

   A legenda na parte inferior do arquivo exportado explica apenas as opções que você habilitou no [!UICONTROL Gráfico de Gantt] e que estão disponíveis na sua lista de tarefas. Por exemplo, marcos são exibidos na legenda somente se você tiver pelo menos uma tarefa associada a um marco.

   ![gráfico_de_gantt_com_legenda_limitada_atualizada.png](assets/gantt-chart-with-updated--limited--legend-350x271.png)
