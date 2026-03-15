---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Filtro: exibir tarefas principais'
description: Você pode aplicar os filtros de tarefa abaixo para exibir as tarefas de trabalho. As tarefas de trabalho são tarefas que podem ser trabalhadas independentemente e não são tarefas pai de outras tarefas. Em um exemplo, um filtro identifica tarefas filhas que podem ser pais. Nesse caso, eles não são tarefas de trabalho.
author: Lisa and Courtney
feature: Reports and Dashboards
exl-id: 4c3956e1-59e0-4bf2-8739-8064271d6281
source-git-commit: 4261febe4af8628508083fa18e4767e3fd3e1136
workflow-type: tm+mt
source-wordcount: '827'
ht-degree: 7%

---

# Filtro: exibir tarefas principais

<!--Audited: 10/2024-->

Você pode aplicar os filtros de tarefa abaixo para exibir as tarefas de trabalho. As tarefas de trabalho são tarefas que podem ser trabalhadas independentemente e não são tarefas pai de outras tarefas. Em um exemplo, um filtro identifica tarefas filhas que podem ser pais. Nesse caso, eles não são tarefas de trabalho.

>[!TIP]
>
>* Se você considerar adicionar mais de um filtro a um relatório, recomendamos que adicione todos os filtros usando a interface do Construtor de relatórios e clicando em Alternar para Modo de Texto depois de adicionar todas as outras regras de filtro. Em seguida, você pode adicionar o código do filtro da tarefa-pai conforme observado acima. 
>* Recomendamos também adicionar um agrupamento de Nome do projeto para facilitar a leitura do relatório. Para obter mais informações sobre como adicionar agrupamentos aos relatórios, consulte o artigo [Visão geral de agrupamentos no Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).
>

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
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td> 
   <p>Colaborador ou solicitação para modificar um filtro </p>
   <p>Padrão ou Plano para modificar um relatório</p>
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Acesso de edição a relatórios, painéis e calendários para modificar um relatório</p> <p>Editar acesso a Filtros, Visualizações, Agrupamentos para modificar um filtro</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões para um relatório</p>  </td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações contidas nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Exibir tarefas sem filhos (eles podem ter um pai)

Você pode aplicar o filtro a seguir a um relatório de tarefas para exibir tarefas sem filhos. Eles poderiam ter pais próprios e serem filhos de outras tarefas.

1. No **Ícone do** Menu Principal![ do Menu Principal](assets/main-menu-icon.png) no canto superior direito, ou no **Menu Principal** nas ![linhas do Menu Principal](assets/lines-main-menu.png) no canto superior esquerdo, se disponível, clique em **Relatórios**.

1. Clique em **Novo Relatório**.
1. Selecione um **Relatório de Tarefas**.
1. Clique em **Filtros**.
1. Clique em **Adicionar uma Regra de Filtro**.
1. Na linha **Iniciar a digitar o nome do campo ...**, comece a digitar **Número de Filhos** e clique em **Tarefa ” Número de Filhos** quando ele for exibido na lista.

1. Selecione **Igual (Diferencia maiúsculas de minúsculas)** para o modificador e digite **0** para o número de filhos.\
   ![Filtro de tarefa pai](assets/parent-task-filter-from-the-ui-350x76.png)

   Ou

   Clique em **Alternar para Modo de Texto** e, na janela de edição de texto, copie e cole o seguinte texto

   ```
   numberOfChildren=0
   numberOfChildren_Mod=eq
   ```


1. Clique em **Salvar + Fechar**.

   Isso extrai um relatório para todas as tarefas em funcionamento no sistema. Algumas dessas tarefas podem ter um pai, mas elas não são tarefas pai em si.

## Exibir tarefas com pais (eles podem ter filhos)

Você pode aplicar o seguinte filtro a um relatório de tarefas para exibir tarefas com pais, o que significa que são tarefas filhas. No entanto, essas tarefas também podem ter filhos, pois o filtro não exclui os filhos. As tarefas filhas que também são pai de outras tarefas não são consideradas tarefas de trabalho.

1. No **Menu Principal** ![Ícone do Menu Principal](assets/main-menu-icon.png) no canto superior direito ou no **Menu Principal** ![Linhas do Menu Principal](assets/lines-main-menu.png) no canto superior esquerdo, se disponível, clique em **Relatórios**.

1. Clique em **Novo Relatório**.
1. Selecione um **Relatório de Tarefas**.
1. Clique em **Filtros**.
1. Clique em **Adicionar uma Regra de Filtro**.
1. Na linha **Começar a digitar o nome do campo ...**, comece a digitar a **ID pai** e selecione a **Tarefa ” ID pai** quando ela for exibida na lista.
1. Selecione **Não Está em Branco** para o modificador.

   ![A ID do pai não está em branco](assets/filter-parent-id-not-blank-350x100.png)

   Ou

   Clique em **Alternar para Modo de Texto** e, na janela de edição de texto, copie e cole o seguinte texto: 

   `parentID_Mod=notblank`

1. Clique em **Salvar + Fechar**.

   Isso extrai um relatório para todas as tarefas em seu sistema que têm pais e são tarefas filhas desses pais. Algumas dessas tarefas podem ser de responsabilidade principal.

## Exibir tarefas sem filhos e sem pais (tarefas autônomas)

Você pode aplicar o filtro a seguir a um relatório de tarefas para exibir tarefas de trabalho independentes. Essas tarefas não têm um pai nem filhos próprios.

1. No **Ícone do** Menu Principal![ do Menu Principal](assets/main-menu-icon.png) no canto superior direito, ou no **Menu Principal** nas ![linhas do Menu Principal](assets/lines-main-menu.png) no canto superior esquerdo, se disponível, clique em **Relatórios**.

1. Clique em **Novo Relatório**.
1. Selecione um **Relatório de Tarefas**.
1. Clique em **Filtros**.
1. Clique em **Adicionar uma Regra de Filtro**.
1. Na linha **Começar a digitar o nome do campo ...**, comece a digitar **Número de Filhos** e selecione **Tarefa ” Número de Filhos** na lista.
1. Selecione **Igual (Diferencia maiúsculas de minúsculas)** para o modificador e digite **0** para o número de filhos.
1. Clique em **Adicionar outra Regra de Filtro**.
1. Na linha **Começar a digitar o nome do campo ...**, comece a digitar a **ID do Pai** e selecione **Tarefa ” ID do Pai** na lista.
1. Selecione **Está em Branco** para o modificador.

   ![A ID do pai está em branco e não tem filhos](assets/filter-parent-id-blank-and-zero-children-350x121.png)

   Ou

   Em vez das etapas 6 a 10 <!--ensure steps above stay accurate-->, clique em **Alternar para o Modo de Texto** e, na janela de edição de texto, copie e cole o seguinte texto:

   ```
   numberOfChildren=0
   numberOfChildren_Mod=eq
   parentID_Mod=isblank
   ```

1. Clique em **Salvar + Fechar**.

   Isso extrai um relatório para todas as tarefas em seu sistema que não têm pais nem filhos. Estas são tarefas de trabalho independentes.
