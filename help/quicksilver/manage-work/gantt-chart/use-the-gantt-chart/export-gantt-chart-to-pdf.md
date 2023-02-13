---
navigation-topic: use-the-gantt-chart
title: Exportar o Gráfico de Gantt para o PDF
description: Você pode exportar o gráfico de Gantt para um PDF.
author: Alina
feature: Work Management
exl-id: 91aad9e0-25c9-4eae-aa66-8aab763d3b76
source-git-commit: 2db4a79cad71b550b7de573c5b27293b6582858f
workflow-type: tm+mt
source-wordcount: '965'
ht-degree: 0%

---

# Exporte o [!UICONTROL Gráfico de Gantt] para PDF

É possível exportar a variável [!UICONTROL Gráfico de Gantt] para um PDF.

Após exportar o [!UICONTROL Gráfico de Gantt] para o PDF, você pode imprimi-lo ou anexá-lo a um email, para compartilhá-lo com outros usuários.

## Requisitos de acesso

Você deve ter o seguinte para seguir as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plano da [!UICONTROL Adobe Workfront]*</td> 
   <td> <p>Qualquer Um </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da [!UICONTROL Adobe Workfront]*</td> 
   <td> <p>[!UICONTROL Review] ou superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>[!UICONTROL View] ou acesso superior a Projetos e tarefas</p> <p>Observação: Se ainda não tiver acesso, pergunte ao seu [!DNL Workfront] administrador se eles definirem restrições adicionais em seu nível de acesso. Para obter informações sobre como uma [!DNL Workfront] administrador pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>[!UICONTROL View] ou acesso superior ao projeto</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com seu [!DNL Workfront] administrador.

## Exporte o [!UICONTROL Gráfico de Gantt]

1. Acesse o [!UICONTROL Gráfico de Gantt] que você deseja exportar para o PDF, conforme descrito em [Introdução ao [!UICONTROL Gráfico de Gantt]](../../../manage-work/gantt-chart/use-the-gantt-chart/get-started-with-gantt.md).
1. Certifique-se de ter configurado a variável [!UICONTROL Gráfico de Gantt] para exibir as informações apropriadas antes de exportá-las.

   >[!NOTE]
   >
   >Se você exportar a variável [!UICONTROL Gráfico de Gantt] de uma lista de projetos, o arquivo PDF contém apenas os projetos da lista, não as tarefas de cada projeto. Se quiser exportar uma lista de tarefas, faça isso a partir do projeto ao qual elas estão associadas ou criando um relatório de tarefa e exibindo os resultados do relatório na [!UICONTROL Exibição de Gantt].

   Você pode configurar as seguintes informações:

   * Filtros, Exibições e Agrupamentos, conforme desejado na lista de tarefas. Todos os Filtros e Agrupamentos selecionados na exibição em lista são mantidos ao visualizar o [!UICONTROL Gráfico de Gantt]. As exibições são refletidas no exportado [!UICONTROL Gráfico de Gantt] somente na lista exibida ao lado do [!UICONTROL Gráfico de Gantt] na primeira página. As exibições não são exibidas na página [!UICONTROL Gráfico de Gantt] próprio.

      >[!TIP]
      >
      >Para permitir mais espaço para a variável [!UICONTROL Gráfico de Gantt] aplique uma visualização que contenha o menor número possível de colunas.

   * Opções de configuração no [!UICONTROL Gráfico de Gantt]. Por exemplo, você pode ativar marcos, datas, [!UICONTROL linhas de base]ou [!UICONTROL porcentagem concluída] para aparecer no [!UICONTROL Gráfico de Gantt].

      Para obter mais informações, consulte   [Configure como as informações são exibidas no [!UICONTROL Gráfico de Gantt]](../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md).

      >[!NOTE]
      >
      > As atribuições não são exibidas no [!UICONTROL Gráfico de Gantt] quando a variável [!UICONTROL Gráfico de Gantt] é exportado para PDF. Quando a variável [!UICONTROL Gráfico de Gantt] for exportado para o PDF, as atribuições serão exibidas somente na exibição de lista.

   * O período exibido na [!UICONTROL Gráfico de Gantt].\

      Para obter mais informações, consulte [Exibindo informações na [!UICONTROL Gráfico de Gantt]](../../../manage-work/gantt-chart/use-the-gantt-chart/view-info-in-gantt.md).

      A forma como o período de tempo é exibido no arquivo de exportação depende da seleção **[!UICONTROL O que vejo]** ou **[!UICONTROL Várias páginas]** em uma etapa posterior.

1. (Opcional) Para incluir somente determinadas tarefas no PDF exportado, selecione as tarefas que deseja incluir.

   Se não selecionar nenhuma tarefa, todas as tarefas serão incluídas no PDF exportado.

   Por exemplo, se você estiver visualizando a variável [!UICONTROL Gráfico de Gantt] para um projeto que contém 50 tarefas, mas você deseja exibir apenas 10 tarefas no arquivo exportado [!UICONTROL Gráfico de Gantt], selecione as 10 tarefas que deseja exibir.

1. Clique no ícone da impressora.\
   O **[!UICONTROL Exportar para PDF]** será exibida.\
   ![export_gantt_UI.png](assets/exported-gantt-ui-350x225.png)

1. Selecione se deseja exportar apenas o que está vendo ou o [!UICONTROL Gráfico de Gantt]:

   * **[!UICONTROL O que vejo]:** Exporta todas as tarefas (incluindo quaisquer subtarefas) exibidas na tela antes da exportação de até 500 itens. (Não é o que é exibido na variável **[!UICONTROL Visualizar]** seção; o [!UICONTROL Visualizar] contém apenas dados de amostra.)

      As subtarefas são incluídas no PDF exportado mesmo se a tarefa pai for recolhida e as subtarefas não estiverem visíveis. Para incluir apenas tarefas pai, selecione as tarefas pai que deseja incluir e deixe qualquer subtarefa desmarcada.

      Você pode usar o **[!UICONTROL Zoom]** menu suspenso ou a ferramenta de controle deslizante para exibir apenas uma parte do [!UICONTROL Gráfico de Gantt], conforme descrito em [Exibindo informações na [!UICONTROL Gráfico de Gantt]](../../../manage-work/gantt-chart/use-the-gantt-chart/view-info-in-gantt.md) .

   * **[!UICONTROL Várias páginas]:** Exporta o todo [!UICONTROL Gráfico de Gantt], mesmo que não esteja visível na tela atual até 500 itens.\

      Você pode usar o **[!UICONTROL Zoom]** menu suspenso ou a ferramenta controle deslizante para determinar quantas informações são exibidas em cada página, conforme descrito em [Configure como as informações são exibidas no [!UICONTROL Gráfico de Gantt]](../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md). Selecione uma opção mais granular para exibir mais páginas para exportar ou selecione uma opção menos granular para exibir menos páginas para exportar.

      >[!NOTE]
      >
      >Se precisar exportar um [!UICONTROL Gráfico de Gantt] que contenha mais de 500 itens, aplique um Filtro à lista antes de visualizar o [!UICONTROL Gráfico de Gantt] para que menos de 500 itens ou 250 páginas sejam exibidos. Para obter informações sobre como aplicar um filtro, consulte  [Visão geral dos filtros em [!DNL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).
      >
      >
      >Não é possível exportar o gráfico de Gantt inteiro nas seguintes circunstâncias:
      >
      >   
      >   
      >   * Quando se expande por mais de 250 páginas
      >   * Quando contém mais de 500 itens





1. Se a PDF for impressa depois de exportada para o PDF, na **[!UICONTROL Tamanho da página]** no menu suspenso , selecione o tamanho do papel para o qual deseja imprimir.\
   Você pode selecionar **[!UICONTROL Letra]**, **[!UICONTROL Legal]**, **[!UICONTROL Razão]**, **[!UICONTROL A1]**, **[!UICONTROL A2]**, **[!UICONTROL A3]** (disponível apenas para alguns idiomas), ou **[!UICONTROL A4]**.
1. No **[!UICONTROL Orientação da página]** selecione se deseja que o PDF seja exportado em orientação paisagem ou retrato.
1. Selecionar **[!UICONTROL Mostrar legenda]** se desejar incluir a legenda no PDF exportado.
1. Clique em **[!UICONTROL Exportar]**.

   O pdf do [!UICONTROL Gráfico de Gantt] O é criado e baixado no computador.

   Observe a legenda na parte inferior do arquivo exportado. Ela explica somente as opções ativadas em [!UICONTROL Gráfico de Gantt] e que estão disponíveis na lista de tarefas.

   Por exemplo, os marcos são exibidos na legenda somente se você tiver pelo menos uma tarefa associada a um marco.

   ![gantt_chart_with_update__limited_legend.png](assets/gantt-chart-with-updated--limited--legend-350x271.png)
