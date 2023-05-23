---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: "Filtro: exibir tarefas pai"
description: Você pode aplicar os filtros de tarefa abaixo para exibir tarefas em execução. Tarefas de trabalho são tarefas que podem ser trabalhadas independentemente e não são tarefas pai de outras tarefas. Em um exemplo, um filtro identifica tarefas filhas que podem ser pais. Nesse caso, elas não são tarefas de trabalho.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 4c3956e1-59e0-4bf2-8739-8064271d6281
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '756'
ht-degree: 0%

---

# Filtro: exibir tarefas pai

Você pode aplicar os filtros de tarefa abaixo para exibir tarefas em execução. Tarefas de trabalho são tarefas que podem ser trabalhadas independentemente e não são tarefas pai de outras tarefas. Em um exemplo, um filtro identifica tarefas filhas que podem ser pais. Nesse caso, elas não são tarefas de trabalho.

>[!TIP]
>
>* Se você considerar adicionar mais de um filtro a um relatório, recomendamos adicionar todos os filtros usando a interface do Report Builder e clicando em Alternar para o modo de texto depois que todas as outras regras de filtro tiverem sido adicionadas. Em seguida, é possível adicionar o código do filtro da tarefa pai, conforme observado acima. 
* Também recomendamos que você adicione um agrupamento para Nome do projeto para facilitar a leitura do relatório. Para obter mais informações sobre como adicionar agrupamentos aos relatórios, consulte o artigo [Visão geral de agrupamentos no Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).
>


## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront*</td> 
   <td> <p>Qualquer Um</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Solicitação para modificar um filtro </p>
   <p>Planejar a modificação de um relatório</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a relatórios, painéis e calendários para modificar um relatório</p> <p>Editar acesso a Filtros, Visualizações, Agrupamentos para modificar um filtro</p> <p><b>Nota</b>

Se você ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td>
</tr>
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões para um relatório</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir seu plano, tipo de licença ou acesso, entre em contato com o administrador do Workfront.

## Exibir tarefas sem filhos (eles podem ter um pai)

Você pode aplicar o filtro a seguir a um relatório de tarefas para exibir tarefas sem filhos. Eles poderiam ter seus próprios pais e serem filhos de outras tarefas.

1. No **Menu principal** ![](assets/main-menu-icon.png), clique em **Relatórios.**

1. Clique em **Novo Relatório**.
1. Selecione um **Relatório de Tarefa**.
1. Clique em **Filtros**.
1. Clique em **Adicionar uma regra de filtro**.
1. No **Comece a digitar o nome do campo...** linha, comece a digitar **Número de Filhos**.

1. Selecionar **Igual (Diferencia Maiúsculas de Minúsculas)** para o modificador, em seguida, informe **0** para o número de filhos.\
   ![](assets/parent-task-filter-from-the-ui-350x76.png)

   Ou

   Clique em **Alternar para modo de texto** e na janela de edição de texto, copie e cole o seguinte texto: 

   ```
   numberOfChildren=0
   numberOfChildren_Mod=eq
   ```


1. Clique em **Salvar + Fechar**.

   Isso extrai um relatório para todas as tarefas em funcionamento no sistema. Algumas dessas tarefas podem ter um pai, mas não são tarefas pai em si.

## Exibir tarefas com pais (eles podem ter filhos)

Você pode aplicar o filtro a seguir a um relatório de tarefas para exibir tarefas com pais, o que significa que elas são tarefas filhas. No entanto, essas tarefas também podem ter filhos, pois o filtro não exclui os filhos. Tarefas secundárias que também são principais para outras tarefas não são consideradas tarefas de trabalho.

1. No **Menu principal** ![](assets/main-menu-icon.png), clique em **Relatórios.
1. Clique em **Novo Relatório**.
1. Selecione um **Relatório de Tarefa**.
1. Clique em **Filtros**.
1. Clique em **Adicionar uma regra de filtro**.
1. No **Comece a digitar o nome do campo...** linha, comece a digitar **ID do Pai**.
1. Selecionar **Não está em branco** para o modificador.

   ![](assets/filter-parent-id-not-blank-350x100.png)

   Ou

   Clique em **Alternar para modo de texto** e na janela de edição de texto, copie e cole o seguinte texto: 

   `parentID_Mod=notblank`

1. Clique em **Salvar + Fechar**.

   Isso extrai um relatório para todas as tarefas em seu sistema que têm pais e são tarefas filhas desses pais. Algumas dessas tarefas podem ser de responsabilidade principal.

## Exibir tarefas sem filhos e sem pais (tarefas independentes)

Você pode aplicar o filtro a seguir a um relatório de tarefa para exibir tarefas de trabalho independentes. Estas tarefas não têm pais e eles não têm filhos.

1. No **Menu principal** ![](assets/main-menu-icon.png), clique em **Relatórios.**
1. Clique em **Novo Relatório**.
1. Selecione um **Relatório de Tarefa**.
1. Clique em **Filtros**.
1. Clique em **Adicionar uma regra de filtro** e no **Comece a digitar o nome do campo...** início de digitação da linha **Número de Filhos** selecionar **Igual (Diferencia Maiúsculas de Minúsculas)** para o modificador, em seguida, informe **0** para o número de filhos.
1. Clique em **Adicionar outra regra de filtro** e no **Comece a digitar o nome do campo...** início de digitação da linha **ID do Pai** e selecione **Está em Branco**.

   ![](assets/filter-parent-id-blank-and-zero-children-350x121.png)

   Ou

   Em vez das etapas 6 a 7, clique em **Alternar para modo de texto** e na janela de edição de texto, copie e cole o seguinte texto: 

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ensure steps above stay accurate)</p>
   -->

   ```
   numberOfChildren=0
   numberOfChildren_Mod=eq
   parentID_Mod=isblank
   ```

1. Clique em **Salvar + Fechar**.

   Isso extrai um relatório para todas as tarefas em seu sistema que não têm pais nem filhos. Estas são tarefas de trabalho independentes.
