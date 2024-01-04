---
navigation-topic: use-the-gantt-chart
title: Exporte o Gráfico de Gantt para o PDF
description: Você pode exportar o Diagrama de Gantt para um PDF.
author: Alina
feature: Work Management
exl-id: 91aad9e0-25c9-4eae-aa66-8aab763d3b76
source-git-commit: 548e713700fda79070f59f3dc3457410d2c50133
workflow-type: tm+mt
source-wordcount: '967'
ht-degree: 0%

---

# Exportar o [!UICONTROL Gráfico de Gantt] para PDF

Você pode exportar o [!UICONTROL Gráfico de Gantt] para um PDF.

Após exportar o [!UICONTROL Gráfico de Gantt] para o PDF, você pode imprimi-lo ou anexá-lo a um email, para compartilhá-lo com outros usuários.

## Requisitos de acesso

Você deve ter o seguinte para seguir as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plano [!UICONTROL Adobe Workfront]*</td> 
   <td> <p>Qualquer </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da [!UICONTROL Adobe Workfront]*</td> 
   <td> <p>[!UICONTROL Review] ou superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>[!UICONTROL Exibir] ou superior acesso a Projetos e Tarefas</p> <p>Observação: se você ainda não tiver acesso, pergunte ao seu [!DNL Workfront] administrador se eles definirem restrições adicionais no seu nível de acesso. Para obter informações sobre como uma [!DNL Workfront] administrador pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>[!UICONTROL Exibir] ou superior acesso ao projeto</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir que plano, tipo de licença ou acesso você tem, entre em contato com o [!DNL Workfront] administrador.

## Exportar o [!UICONTROL Gráfico de Gantt]

1. Acesse o [!UICONTROL Gráfico de Gantt] que você deseja exportar para o PDF, conforme descrito em [Introdução ao [!UICONTROL Gráfico de Gantt]](../../../manage-work/gantt-chart/use-the-gantt-chart/get-started-with-gantt.md).
1. Verifique se você configurou o [!UICONTROL Gráfico de Gantt] para exibir as informações apropriadas antes de exportá-las.

   >[!NOTE]
   >
   >Se você exportar a variável [!UICONTROL Gráfico de Gantt] a partir de uma lista de projetos, o arquivo PDF contém apenas os projetos na lista, não as tarefas em cada projeto. Se quiser exportar uma lista de tarefas, faça isso a partir do projeto ao qual estão associadas ou criando um relatório de tarefa e exibindo os resultados do relatório na [!UICONTROL Visualização de Gantt].

   Você pode configurar as seguintes informações:

   * Filtros, Visualizações e Agrupamentos conforme desejado na lista de tarefas. Quaisquer Filtros e Agrupamentos selecionados na exibição de lista são mantidos ao visualizar o [!UICONTROL Gráfico de Gantt]. As exibições são refletidas na página exportada [!UICONTROL Gráfico de Gantt] somente na lista exibida ao lado da variável [!UICONTROL Gráfico de Gantt] na primeira página. As exibições não são exibidas na [!UICONTROL Gráfico de Gantt] próprio.

     >[!TIP]
     >
     >Para permitir mais espaço para o [!UICONTROL Gráfico de Gantt] Aplique uma visualização que contenha o menor número de colunas possível.

   * Opções de configuração no [!UICONTROL Gráfico de Gantt]. Por exemplo, você pode ativar marcos, datas, [!UICONTROL linhas de base]ou [!UICONTROL porcentagem concluída] para aparecer no [!UICONTROL Gráfico de Gantt].

     Para obter mais informações, consulte   [Configure como as informações são exibidas na [!UICONTROL Gráfico de Gantt]](../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md).

     >[!NOTE]
     >
     > As atribuições não são exibidas na [!UICONTROL Gráfico de Gantt] quando a variável [!UICONTROL Gráfico de Gantt] é exportado para o PDF. Quando a variável [!UICONTROL Gráfico de Gantt] for exportado para PDF, as atribuições serão exibidas somente na exibição em lista.

   * O período exibido no [!UICONTROL Gráfico de Gantt].\

     Para obter mais informações, consulte [Exibindo Informações na [!UICONTROL Gráfico de Gantt]](../../../manage-work/gantt-chart/use-the-gantt-chart/view-info-in-gantt.md).

     A forma como o período de tempo é exibido no arquivo de exportação depende se você seleciona **[!UICONTROL O que vejo]** ou **[!UICONTROL Várias páginas]** em uma etapa posterior.

1. (Opcional) Para incluir apenas determinadas tarefas no PDF exportado, selecione as tarefas que deseja incluir.

   Se você não selecionar nenhuma tarefa, todas as tarefas serão incluídas no PDF exportado.

   Por exemplo, se você estiver exibindo a variável [!UICONTROL Gráfico de Gantt] para um projeto que contém 50 tarefas, mas você deseja exibir apenas 10 tarefas no [!UICONTROL Gráfico de Gantt], selecione as 10 tarefas que deseja exibir.

1. Clique no ícone da impressora.\
   A variável **[!UICONTROL Exportar para PDF]** é exibida.\
   ![export_gantt_UI.png](assets/exported-gantt-ui-350x225.png)

1. Selecione se deseja exportar apenas o que vê ou o conteúdo [!UICONTROL Gráfico de Gantt]:

   * **[!UICONTROL O que vejo]:** Exporta todas as tarefas (incluindo qualquer subtarefa) exibidas na tela antes de exportar até 500 itens. (Isso não é o que é exibido no **[!UICONTROL Visualizar]** seção; a [!UICONTROL Visualizar] contém apenas dados de exemplo.)

     As subtarefas são incluídas no PDF exportado mesmo se a tarefa pai estiver recolhida e as subtarefas não estiverem visíveis. Para incluir somente tarefas pai, selecione as tarefas pai que deseja incluir e deixe qualquer subtarefa desmarcada.

     Você pode usar o **[!UICONTROL Zoom para]** menu suspenso ou na ferramenta controle deslizante para exibir apenas uma parte do [!UICONTROL Gráfico de Gantt], conforme descrito em [Exibindo Informações na [!UICONTROL Gráfico de Gantt]](../../../manage-work/gantt-chart/use-the-gantt-chart/view-info-in-gantt.md) .

   * **[!UICONTROL Várias páginas]:** Exporta todo o [!UICONTROL Gráfico de Gantt], mesmo o que não estiver visível na tela atual, até 500 itens.\

     Você pode usar o **[!UICONTROL Zoom para]** menu suspenso ou a ferramenta controle deslizante para determinar quantas informações são exibidas em cada página, conforme descrito em [Configure como as informações são exibidas na [!UICONTROL Gráfico de Gantt]](../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md). Selecione uma opção mais granular para exibir mais páginas para exportar ou selecione uma opção menos granular para exibir menos páginas para exportar.

     >[!NOTE]
     >
     >Se precisar exportar um [!UICONTROL Gráfico de Gantt] que contenha mais de 500 itens, aplique um Filtro à lista antes de visualizar o [!UICONTROL Gráfico de Gantt] para que menos de 500 itens ou 250 páginas sejam exibidos. Para obter informações sobre como aplicar um filtro, consulte  [Visão geral dos filtros](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).
     >
     >
     >Não é possível exportar todo o Diagrama de Gantt nas seguintes circunstâncias:
     >
     >   
     >   
     >   * Quando abrange mais de 250 páginas
     >   * Quando contiver mais de 500 itens




1. Se o PDF for impresso depois de ser exportado para o PDF, na **[!UICONTROL Tamanho da página]** selecione o tamanho do papel no qual deseja imprimir.\
   É possível selecionar **[!UICONTROL Carta]**, **[!UICONTROL Legal]**, **[!UICONTROL Ledger]**, **[!UICONTROL A1]**, **[!UICONTROL A2]**, **[!UICONTROL A3]** (disponível somente para alguns idiomas) ou **[!UICONTROL A4]**.
1. No **[!UICONTROL Orientação da página]** selecione se deseja que o PDF seja exportado na orientação paisagem ou retrato.
1. Selecionar **[!UICONTROL Mostrar legenda]** se desejar incluir a Legenda no PDF exportado.
1. Clique em **[!UICONTROL Exportar]**.

   O pdf da [!UICONTROL Gráfico de Gantt] O foi criado e baixado no computador.

   Observe a legenda na parte inferior do arquivo exportado. Ele explica apenas as opções que você ativou no [!UICONTROL Gráfico de Gantt] e que estão disponíveis na lista de tarefas.

   Por exemplo, marcos são exibidos na legenda somente se você tiver pelo menos uma tarefa associada a um marco.

   ![gantt_chart_with_updated_limit_legend.png](assets/gantt-chart-with-updated--limited--legend-350x271.png)
