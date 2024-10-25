---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: "Filtro: exibir tarefas pai"
description: Você pode aplicar os filtros de tarefa abaixo para exibir tarefas em execução. Tarefas de trabalho são tarefas que podem ser trabalhadas independentemente e não são tarefas pai de outras tarefas. Em um exemplo, um filtro identifica tarefas filhas que podem ser pais. Nesse caso, elas não são tarefas de trabalho.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 4c3956e1-59e0-4bf2-8739-8064271d6281
source-git-commit: a19668ac2238448010b5a177120f936ef7ba5bba
workflow-type: tm+mt
source-wordcount: '808'
ht-degree: 1%

---

# Filtro: exibir tarefas pai

<!--Audited: 10/2024-->

Você pode aplicar os filtros de tarefa abaixo para exibir tarefas em execução. Tarefas de trabalho são tarefas que podem ser trabalhadas independentemente e não são tarefas pai de outras tarefas. Em um exemplo, um filtro identifica tarefas filhas que podem ser pais. Nesse caso, elas não são tarefas de trabalho.

>[!TIP]
>
>* Se você considerar adicionar mais de um filtro a um relatório, recomendamos adicionar todos os filtros usando a interface do Report Builder e clicando em Alternar para o modo de texto depois que todas as outras regras de filtro tiverem sido adicionadas. Em seguida, é possível adicionar o código do filtro da tarefa pai, conforme observado acima. 
>* Também recomendamos que você adicione um agrupamento para Nome do projeto para facilitar a leitura do relatório. Para obter mais informações sobre como adicionar agrupamentos aos seus relatórios, consulte o artigo [Visão geral de agrupamentos no Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).
>

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> 
    <p>Novo:</p>
   <ul><li><p>Colaborador para modificar um filtro </p></li>
   <li><p>Padrão para modificar um relatório</p></li> </ul>

<p>Atual:</p>
   <ul><li><p>Solicitação para modificar um filtro </p></li>
   <li><p>Planejar a modificação de um relatório</p></li> </ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Editar acesso a relatórios, painéis e calendários para modificar um relatório</p> <p>Editar acesso a Filtros, Visualizações, Agrupamentos para modificar um filtro</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões para um relatório</p>  </td> 
  </tr> 
 </tbody> 
</table>

*Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Exibir tarefas sem filhos (eles podem ter um pai)

Você pode aplicar o filtro a seguir a um relatório de tarefas para exibir tarefas sem filhos. Eles poderiam ter seus próprios pais e serem filhos de outras tarefas.

1. No **Menu Principal** ![](assets/main-menu-icon.png) no canto superior direito ou no **Menu Principal** ![](assets/lines-main-menu.png) no canto superior esquerdo, se disponível, clique em **Relatórios**.

1. Clique em **Novo Relatório**.
1. Selecione um **Relatório de Tarefa**.
1. Clique em **Filtros**.
1. Clique em **Adicionar uma Regra de Filtro**.
1. Na linha **Comece a digitar o nome do campo ...**, comece a digitar **Número de Filhos** e clique em **Tarefa >> Número de Filhos** quando ele for exibido na lista.

1. Selecione **Igual (Diferencia maiúsculas de minúsculas)** para o modificador e digite **0** para o número de filhos.\
   ![](assets/parent-task-filter-from-the-ui-350x76.png)

   Ou

   Clique em **Alternar para Modo de Texto** e, na janela de edição de texto, copie e cole o seguinte texto

   ```
   numberOfChildren=0
   numberOfChildren_Mod=eq
   ```


1. Clique em **Salvar + Fechar**.

   Isso extrai um relatório para todas as tarefas em funcionamento no sistema. Algumas dessas tarefas podem ter um pai, mas não são tarefas pai em si.

## Exibir tarefas com pais (eles podem ter filhos)

Você pode aplicar o filtro a seguir a um relatório de tarefas para exibir tarefas com pais, o que significa que elas são tarefas filhas. No entanto, essas tarefas também podem ter filhos, pois o filtro não exclui os filhos. Tarefas secundárias que também são principais para outras tarefas não são consideradas tarefas de trabalho.

1. No **Menu Principal** ![](assets/main-menu-icon.png) no canto superior direito ou no **Menu Principal** ![](assets/lines-main-menu.png) no canto superior esquerdo, se disponível, clique em **Relatórios**.

1. Clique em **Novo Relatório**.
1. Selecione um **Relatório de Tarefa**.
1. Clique em **Filtros**.
1. Clique em **Adicionar uma Regra de Filtro**.
1. Na linha **Comece a digitar o nome do campo ...**, comece a digitar a **ID do Pai** e selecione a **Tarefa >> ID do Pai** quando ela for exibida na lista.
1. Selecione **Não está em branco** para o modificador.

   ![](assets/filter-parent-id-not-blank-350x100.png)

   Ou

   Clique em **Alternar para Modo de Texto** e, na janela de edição de texto, copie e cole o seguinte texto: 

   `parentID_Mod=notblank`

1. Clique em **Salvar + Fechar**.

   Isso extrai um relatório para todas as tarefas em seu sistema que têm pais e são tarefas filhas desses pais. Algumas dessas tarefas podem ser de responsabilidade principal.

## Exibir tarefas sem filhos e sem pais (tarefas independentes)

Você pode aplicar o filtro a seguir a um relatório de tarefa para exibir tarefas de trabalho independentes. Estas tarefas não têm pais e eles não têm filhos.

1. No **Menu Principal** ![](assets/main-menu-icon.png) no canto superior direito ou no **Menu Principal** ![](assets/lines-main-menu.png) no canto superior esquerdo, se disponível, clique em **Relatórios**.

1. Clique em **Novo Relatório**.
1. Selecione um **Relatório de Tarefa**.
1. Clique em **Filtros**.
1. Clique em **Adicionar uma Regra de Filtro**.
1. Na linha **Comece a digitar o nome do campo ...**, comece a digitar **Número de Filhos** e selecione **Tarefa >> Número de Filhos** na lista.
1. Selecione **Igual (Diferencia maiúsculas de minúsculas)** para o modificador e digite **0** para o número de filhos.
1. Clique em **Adicionar outra regra de filtro**.
1. No campo **Comece a digitar o nome ...**, comece a digitar a **ID do Pai** e selecione **Tarefa >> ID do Pai** na lista.
1. Selecione **Está em Branco** para o modificador.

   ![](assets/filter-parent-id-blank-and-zero-children-350x121.png)

   Ou

   Em vez das etapas 6-10 <!--ensure steps above stay accurate-->, clique em **Alternar para Modo de Texto** e, na janela de edição de texto, copie e cole o seguinte texto:

   ```
   numberOfChildren=0
   numberOfChildren_Mod=eq
   parentID_Mod=isblank
   ```

1. Clique em **Salvar + Fechar**.

   Isso extrai um relatório para todas as tarefas em seu sistema que não têm pais nem filhos. Estas são tarefas de trabalho independentes.
