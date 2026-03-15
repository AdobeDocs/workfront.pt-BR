---
product-area: reporting
navigation-topic: reporting-elements
title: Use curingas baseados em datas para generalizar relatórios
description: É possível generalizar um relatório usando curingas em vez de informações específicas ao criar determinados elementos de relatório.
author: Courtney
feature: Reports and Dashboards
exl-id: 759b0bea-729e-4206-808c-0a7216ded4ff
source-git-commit: 6a6d3d47ed5741e3202c44b7240a2e67b687ea95
workflow-type: tm+mt
source-wordcount: '636'
ht-degree: 10%

---

# Use curingas baseados em datas para generalizar relatórios

<!-- Audited: 11/2024 -->

Você pode generalizar um relatório usando curingas em vez de informações específicas ao criar determinados elementos de relatórios.

Por exemplo, se você quiser criar um relatório que mostre as tarefas com uma Data de início planejada específica, poderá usar o seletor de datas do calendário em um filtro para selecionar uma data específica. No entanto, se quiser criar um relatório que mostre as tarefas que têm a Data de Início Planejada dentro de um determinado período a partir da data em que o relatório é acessado, você pode usar um curinga que indique que, quando alguém exibe o relatório, ele exibe informações para um período relevante para o momento em que o relatório é exibido.

Por exemplo, na última semana, no último ano, nas próximas duas semanas etc. Dessa forma, o relatório é criado uma vez, mas, como você usa um curinga no filtro, ele produz resultados diferentes sempre que alguém o lê, porque se adapta ao dia em que o relatório é executado.

Você pode usar curingas baseados em data ao criar os seguintes elementos de relatório:

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

Você deve criar um relatório antes de adicionar variáveis curingas a ele.

Para obter informações sobre como criar um relatório, consulte [Criar um relatório](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md).

## Etapas de instruções

Para inserir um curinga baseado em data em um relatório:

1. Vá para um relatório no qual você deseja inserir um curinga baseado em data.
1. Clique em **Ações de Relatório** e depois em **Editar**.
1. Clique na guia **Filtros**.
1. Clique em **Adicionar uma Regra de Filtro**.
1. Comece digitando o nome do campo pelo qual deseja filtrar.\
   É necessário digitar campos que façam referência a uma data.
1. Selecione **Igual** no menu suspenso da variável de filtro.

   >[!TIP]
   >
   >Você sempre deve selecionar a variável de filtro **Igual** ao trabalhar com curingas no Adobe Workfront.

1. Clique no botão de alternância **Definir data relativa** e, na caixa de texto exibida, digite: `$$TODAY` se desejar exibir informações sobre algo que ocorra no mesmo dia em que o relatório é executado.

   Ou

   Digite `$$NOW` se quiser exibir informações sobre algo que ocorra na mesma data e hora em que o relatório é executado.

   Essa data é sempre diferente, pois muda com a data em que o relatório é realmente exibido por um usuário. portanto, as informações no relatório são diferentes do dia a dia.

1. (Opcional) Se desejar exibir informações que ocorram em um período após a data em que o relatório é executado, digite `$$TODAY+1w` para exibir informações na semana seguinte ou `$$TODAY+2m` para exibir informações nos próximos dois meses. Você também pode indicar períodos para trimestres, horas, dias ou anos.
1. (Opcional) Se desejar exibir informações sobre algo que ocorreu em um período anterior à data em que o relatório é executado, digite `$$TODAY-1w` para exibir informações da semana anterior, ou `$$TODAY-2m` para exibir informações dos dois meses anteriores. Você também pode indicar períodos de tempo para trimestres, horas, dias ou anos.

   Para obter uma lista completa de atributos, qualificadores e operadores que você pode usar em curingas baseados em data, consulte o artigo [Visão geral das variáveis de filtro de curinga](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).

1. Clique em **Salvar + Fechar**.

## Informações adicionais

Consulte também:

<!--outdated: * [Basic Report Creation Program](https://one.workfront.com/s/basic-report-creation-program) -->
* [Visão geral das variáveis de filtro curinga](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md)
* [Criar ou editar filtros no Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/create-filters.md)
* [Adicionar um prompt a um relatório](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md)
* [Usar formatação condicional nas visualizações](../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md)
