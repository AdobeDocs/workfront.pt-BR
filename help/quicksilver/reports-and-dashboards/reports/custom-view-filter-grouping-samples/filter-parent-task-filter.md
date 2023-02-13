---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '"Filtro: exibir tarefas pai'''
description: Você pode aplicar os filtros de tarefa abaixo para exibir tarefas de trabalho. As tarefas de trabalho são tarefas que podem ser trabalhadas independentemente e que não são tarefas pai de outras tarefas. Em um exemplo, um filtro identifica tarefas secundárias que podem ser os próprios pais. Nesse caso, elas não são tarefas de trabalho.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 4c3956e1-59e0-4bf2-8739-8064271d6281
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '739'
ht-degree: 0%

---

# Filtro: exibir tarefas pai

Você pode aplicar os filtros de tarefa abaixo para exibir tarefas de trabalho. As tarefas de trabalho são tarefas que podem ser trabalhadas independentemente e que não são tarefas pai de outras tarefas. Em um exemplo, um filtro identifica tarefas secundárias que podem ser os próprios pais. Nesse caso, elas não são tarefas de trabalho.

>[!TIP]
>
>* Se você considerar adicionar mais de um filtro a um relatório, recomendamos adicionar todos os seus filtros usando a interface do Report Builder e clicando em Alternar para o modo de texto depois que todas as outras regras de filtro tiverem sido adicionadas. Em seguida, é possível adicionar o código do filtro de tarefa pai, conforme observado acima. 
* Também recomendamos adicionar um agrupamento para Nome do projeto para facilitar a leitura do relatório. Para obter mais informações sobre como adicionar agrupamentos aos seus relatórios, consulte o artigo [Visão geral dos agrupamentos no Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).
>


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
   <td> <p>Gerenciar permissões de um relatório</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

## Exibir tarefas sem filhos (elas podem ter um pai)

Você pode aplicar o seguinte filtro a um relatório de tarefa para exibir tarefas sem filhos. Poderiam ter pais próprios e ser filhos de outras tarefas.

1. No **Menu principal** ![](assets/main-menu-icon.png), clique em **Relatórios.**

1. Clique em **Novo relatório**.
1. Selecione um **Relatório de tarefa**.
1. Clique em **Filtros**.
1. Clique em **Adicionar uma regra de filtro**.
1. No **Começar a digitar o nome do campo ...** linha, comece a digitar **Número de filhos**.

1. Selecionar **Igual (Diferencia Maiúsculas De Minúsculas)** para o modificador, insira **0** para o número de filhos.\
   ![](assets/parent-task-filter-from-the-ui-350x76.png)

   Ou

   Clique em **Alternar para o modo de texto** e, na janela de edição de texto, copie e cole o seguinte texto: 

   ```
   numberOfChildren=0
   numberOfChildren_Mod=eq
   ```


1. Clique em **Salvar + Fechar**.

   Isso extrai um relatório para todas as tarefas que estão funcionando no seu sistema. Algumas dessas tarefas podem ter um pai, mas não são tarefas pai em si.

## Exibir tarefas com pais (eles podem ter filhos)

Você pode aplicar o seguinte filtro a um relatório de tarefa para exibir tarefas com pais, o que significa que elas são tarefas secundárias. No entanto, essas tarefas também podem ter filhos próprios porque o filtro não exclui seus filhos. As tarefas filho que também são pais para outras tarefas não são consideradas tarefas de trabalho.

1. No **Menu principal** ![](assets/main-menu-icon.png), clique em **Relatórios.
1. Clique em **Novo relatório**.
1. Selecione um **Relatório de tarefa**.
1. Clique em **Filtros**.
1. Clique em **Adicionar uma regra de filtro**.
1. No **Começar a digitar o nome do campo ...** linha, comece a digitar **ID principal**.
1. Selecionar **Não está em Branco** para o modificador.

   ![](assets/filter-parent-id-not-blank-350x100.png)

   Ou

   Clique em **Alternar para o modo de texto** e, na janela de edição de texto, copie e cole o seguinte texto: 

   `parentID_Mod=notblank`

1. Clique em **Salvar + Fechar**.

   Isso obtém um relatório para todas as tarefas em seu sistema que têm pais e são tarefas filhas desses pais. Algumas dessas tarefas poderiam ser um pai.

## Exibir tarefas sem filhos e sem pais (tarefas independentes)

Você pode aplicar o seguinte filtro a um relatório de tarefa para exibir tarefas de trabalho independentes. Essas tarefas não têm um pai e não têm filhos próprios.

1. No **Menu principal** ![](assets/main-menu-icon.png), clique em **Relatórios.**
1. Clique em **Novo relatório**.
1. Selecione um **Relatório de tarefa**.
1. Clique em **Filtros**.
1. Clique em **Adicionar uma regra de filtro** e na **Começar a digitar o nome do campo ...** digitação de início de linha **Número de filhos** select **Igual (Diferencia Maiúsculas De Minúsculas)** para o modificador, insira **0** para o número de filhos.
1. Clique em **Adicionar outra regra de filtro** e na **Começar a digitar o nome do campo ...** digitação de início de linha **ID principal**, em seguida selecione **Está em Branco**.

   ![](assets/filter-parent-id-blank-and-zero-children-350x121.png)

   Ou

   Em vez das etapas 6 a 7, clique em **Alternar para o modo de texto** e na janela de edição de texto, copie e cole o seguinte texto: 

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
