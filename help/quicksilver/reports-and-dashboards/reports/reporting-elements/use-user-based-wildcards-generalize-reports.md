---
product-area: reporting
navigation-topic: reporting-elements
title: Use curingas baseados no usuário para generalizar relatórios
description: É possível generalizar um relatório usando curingas em vez de informações específicas ao criar determinados elementos de relatório.
author: Courtney
feature: Reports and Dashboards
exl-id: 216e2869-b4f8-4cc7-9497-a12ebe00fe49
source-git-commit: 6a6d3d47ed5741e3202c44b7240a2e67b687ea95
workflow-type: tm+mt
source-wordcount: '448'
ht-degree: 15%

---

# Use curingas baseados no usuário para generalizar relatórios

<!-- Audited: 11/2024 -->

É possível generalizar um relatório usando curingas em vez de informações específicas ao criar determinados elementos de relatório. Por exemplo, para criar um relatório que mostre as tarefas atribuídas a um usuário específico, você pode usar o nome do usuário no campo Atribuído a do filtro. However, if you want to create a report that shows tasks assigned to the logged in user, regardless of who that user is, you can use a wildcard that indicates that when someone views the report it displays information pertaining only to them. Dessa forma, o relatório é criado uma vez, mas, como você usa um curinga no filtro, ele produz resultados diferentes sempre que outra pessoa o lê.

Você pode usar curingas baseados no usuário ao criar os seguintes elementos de relatório:

* Filtros
* Prompts personalizados
* Exibições ao adicionar regras para colunas

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
   <td role="rowheader">Licença do Adobe Workfront</strong></td> 
   <td> 
    <p>Padrão</p>
    <p>Plano</p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Editar acesso a filtros, exibições e agrupamentos</p> <p>Acesso de edição a Relatórios, Painéis e Calendários para editar elementos de relatórios em um relatório</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
    <td> <p>Gerenciar permissões para um relatório para editar elementos de relatório em um relatório</p> <p>Gerenciar permissões para uma exibição ou filtro para editá-las</p></td> 
   </td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações contidas nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Pré-requisitos

Você deve criar um relatório antes de adicionar uma variável curinga a ele.

For instructions on creating reports, see [Create a report](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md).

## Etapas de instruções

Para inserir um curinga baseado no usuário em um relatório:

1. Vá para um relatório no qual você deseja inserir um curinga baseado no usuário.
1. Clique em **Ações de Relatório** e depois em **Editar**.

1. Clique na guia **Filtros**.
1. Clique em **Adicionar uma Regra de Filtro**.
1. Comece a digitar o nome do campo pelo qual deseja filtrar.\
   Você deve digitar campos que referenciem o objeto de usuário ou informações sobre usuários.
1. Selecione **Igual** no menu suspenso para a variável de filtro.

   >[!TIP]
   >
   >You must always select the **Equal** filter variable when working with wildcards in Adobe Workfront.

1. In the **Start typing name ...** box, type: `$$USER.ID` or `$$USER.name` if you want the report to display information about the user who logs in, based on their name. You can insert other wildcards that refer to the logged-in user&#39;s Group, Team, Company, or other information.

   Para obter uma lista completa de curingas baseados no usuário, consulte [Visão geral das variáveis de filtro de curingas](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).

1. Clique em **Salvar + Fechar**.

## Informações adicionais

Consulte também:

<!--outdated: * [Basic Report Creation Program](https://one.workfront.com/s/basic-report-creation-program) -->
* [Visão geral das variáveis de filtro curinga](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md)
* [Criar ou editar filtros no Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/create-filters.md)
* [Visão geral dos Filtros](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)
* [Adicionar um prompt a um relatório](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md)
* [Usar formatação condicional nas visualizações](../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md)
