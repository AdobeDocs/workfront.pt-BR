---
product-area: reporting
navigation-topic: reporting-elements
title: Usar curingas com base em data para generalizar relatórios
description: Você pode generalizar um relatório usando curingas em vez de informações específicas ao criar determinados elementos de relatórios.
author: Nolan
feature: Reports and Dashboards
exl-id: 759b0bea-729e-4206-808c-0a7216ded4ff
source-git-commit: 3cee374b68b26f2a423d41101300ec8b6685fadd
workflow-type: tm+mt
source-wordcount: '644'
ht-degree: 1%

---

# Usar curingas com base em data para generalizar relatórios

<!-- Audited: 11/2024 -->

Você pode generalizar um relatório usando curingas em vez de informações específicas ao criar determinados elementos de relatórios.

Por exemplo, se você quiser criar um relatório que mostre as tarefas com uma Data de início planejada específica, poderá usar o seletor de datas do calendário em um filtro para selecionar uma data específica. No entanto, se você quiser criar um relatório que mostre tarefas com a Data de início planejada dentro de um determinado período a partir da data em que o relatório é acessado, poderá usar um curinga que indique que, quando alguém exibir o relatório, ele exibirá informações de um período relevante para o momento em que o relatório for exibido.

Por exemplo, na semana passada, no ano passado, nas próximas duas semanas etc. Assim, você cria o relatório uma vez, mas como usa um curinga no filtro, ele produz resultados diferentes toda vez que alguém o lê, pois se adapta ao dia em que executam o relatório.

Você pode usar curingas baseados em data ao criar os seguintes elementos de relatório:

* Filtros
* Prompts personalizados
* Exibições ao adicionar regras para colunas

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>plano do Adobe Workfront*</strong></td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Licença da Adobe Workfront*</strong></td> 
   <td> 
      <p>Novo:</p>
         <ul>
         <li><p>Padrão</p></li>
         </ul>
      <p>Atual:</p>
         <ul>
         <li><p>Plano</p></li>
         </ul>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurações de nível de acesso*</strong></td> 
   <td> <p>Editar acesso a Filtros, Visualizações, Agrupamentos</p> <p>Editar acesso a relatórios, painéis e calendários para editar elementos de relatórios em um relatório</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Permissões de objeto</strong></td> 
   <td> <p>Gerenciar permissões para um relatório para editar elementos de relatórios em um relatório</p> <p>Gerenciar permissões em uma exibição ou um filtro para editá-las</p></td> 
  </tr> 
 </tbody> 
</table>

*Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Pré-requisitos

Você deve criar um relatório antes de adicionar variáveis curingas a ele.

Para obter informações sobre como criar um relatório, consulte [Criar um relatório](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md).

## Etapas passo a passo

Para inserir um curinga com base em data em um relatório:

1. Vá para um relatório para o qual deseja inserir um curinga com base em data.
1. Clique em **Ações de Relatório** e depois em **Editar**.
1. Clique na guia **Filtros**.
1. Clique em **Adicionar uma Regra de Filtro**.
1. Comece digitando o nome do campo pelo qual deseja filtrar.\
   É necessário digitar campos que façam referência a uma data.
1. Selecione **Igual** no menu suspenso da variável de filtro.

   >[!TIP]
   >
   >Você sempre deve selecionar a variável de filtro **Igual** ao trabalhar com curingas no Adobe Workfront.

1. Clique no botão **Definir data relativa** e, na caixa de texto exibida, digite: `$$TODAY` se desejar exibir informações sobre algo que ocorra no mesmo dia em que o relatório for executado.

   Ou

   Digite `$$NOW` se desejar exibir informações sobre algo que ocorre na mesma data e hora em que o relatório é executado.

   Essa data é sempre diferente, pois muda com a data em que o relatório é realmente visualizado por um usuário. portanto, as informações no relatório são diferentes de dia para dia.

1. (Opcional) Se desejar exibir informações que ocorrem dentro de um período de tempo após a data em que o relatório é executado, digite `$$TODAY+1w` para exibir informações na semana seguinte, ou `$$TODAY+2m` para exibir informações nos próximos dois meses. Você também pode indicar períodos de tempo para trimestres, horas, dias ou anos.
1. (Opcional) Se desejar exibir informações sobre algo que ocorreu em um período anterior à data em que o relatório é executado, digite `$$TODAY-1w` para exibir informações da semana anterior, ou `$$TODAY-2m` para exibir informações dos dois meses anteriores. Você também pode indicar períodos de tempo para trimestres, horas, dias ou anos.

   Para obter uma lista completa de atributos, qualificadores e operadores que você pode usar em curingas baseados em data, consulte o artigo [Visão geral das variáveis de filtro de curinga](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).

1. Clique em **Salvar + Fechar**.

## Informações adicionais

Consulte também:

<!--outdated: * [Basic Report Creation Program](https://one.workfront.com/s/basic-report-creation-program) -->
* [Visão geral das variáveis de filtro curinga](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md)
* [Criar ou editar filtros no Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/create-filters.md)
* [Adicionar um prompt a um relatório](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md)
* [Usar formatação condicional em exibições](../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md)
