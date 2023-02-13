---
product-area: reporting
navigation-topic: reporting-elements
title: Usar curingas com base em data para generalizar relatórios
description: Você pode generalizar um relatório usando curingas em vez de informações específicas ao criar determinados elementos de relatório.
author: Lisa
feature: Reports and Dashboards
exl-id: 759b0bea-729e-4206-808c-0a7216ded4ff
source-git-commit: 442e0b8fde9e4acaa2686ccd292fb003f72be623
workflow-type: tm+mt
source-wordcount: '686'
ht-degree: 0%

---

# Usar curingas com base em data para generalizar relatórios

Você pode generalizar um relatório usando curingas em vez de informações específicas ao criar determinados elementos de relatório.

Por exemplo, se você quiser criar um relatório que mostre as tarefas que têm uma Data Inicial Planejada específica, poderá usar o seletor de datas do calendário em um filtro para selecionar uma data específica. No entanto, se você quiser criar um relatório que mostre tarefas que tenham a Data inicial planejada em um determinado período a partir da data em que o relatório for acessado, poderá usar um curinga indicando que, quando alguém exibir o relatório, exibirá informações para um período relevante para o momento em que o relatório for visualizado.

Por exemplo, na semana passada, no ano passado, nas próximas duas semanas, etc. Dessa forma, você cria o relatório uma vez, mas como você usa um curinga no filtro, ele produz resultados diferentes sempre que alguém o lê, pois ele se adapta ao dia em que o relatório é executado.

Você pode usar curingas com base em data ao criar os seguintes elementos de relatório:

* Filtros
* Solicitações personalizadas
* Exibições ao adicionar regras para colunas

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Plano Adobe Workfront*</strong></td> 
   <td> <p>Qualquer Um</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Licença da Adobe Workfront*</strong></td> 
   <td> <p>Plano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurações de nível de acesso*</strong></td> 
   <td> <p>Editar acesso a filtros, visualizações, agrupamentos</p> <p>Editar o acesso a Relatórios, Painéis, Calendários para editar elementos de relatório em um relatório</p> <p>Observação: Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Permissões de objeto</strong></td> 
   <td> <p>Gerenciar permissões de um relatório para editar elementos de relatório em um relatório</p> <p>Gerencie permissões em uma visualização ou filtro para editá-las</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

## Pré-requisitos

Você deve criar um relatório antes de poder adicionar variáveis curingas a ele.

Para obter informações sobre como criar um relatório, consulte [Criar um relatório](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md).

## Etapas de instruções

Para inserir um curinga com base em data em um relatório:

1. Vá para um relatório para o qual deseja inserir um curinga com base em data.
1. Clique em **Ações de Relatório**, em seguida **Editar**.

1. Clique no botão **Filtros** guia .
1. Clique em **Adicionar uma regra de filtro**.
1. Comece digitando o nome do campo que deseja filtrar.\
   Você deve digitar os campos que fazem referência a uma data.
1. Selecionar **Igual** no menu suspenso da variável de filtro.

   >[!TIP]
   >
   >Você sempre deve selecionar a variável **Igual** variável de filtro ao trabalhar com curingas no Adobe Workfront.

1. No **Começar a digitar nome ...** caixa, tipo: `$$TODAY` se desejar exibir informações sobre algo que ocorre no mesmo dia em que o relatório é executado.

   Ou

   Tipo `$$NOW` se desejar exibir informações sobre algo que ocorre na mesma data e hora em que o relatório é executado.

   Essa data é sempre diferente, pois é alterada com a data em que o relatório é realmente visualizado por um usuário. assim, as informações no relatório são diferentes do dia para dia.

1. (Opcional) Se desejar exibir informações que ocorrem dentro de um período após a data em que o relatório é executado, digite `$$TODAY+1w` para exibir informações na semana seguinte, ou `$$TODAY+2m` para exibir informações nos próximos dois meses. Você também pode indicar períodos para trimestres, horas, dias ou anos.
1. (Opcional) Se desejar exibir informações sobre algo que ocorreu dentro de um período antes da data em que o relatório foi executado, digite `$$TODAY-1w` para exibir informações da semana anterior, ou `$$TODAY-2m` para exibir informações dos dois meses anteriores. Você também pode indicar períodos para trimestres, horas, dias ou anos.

   Para obter uma lista completa de atributos, qualificadores e operadores que podem ser usados em curingas baseadas em data, consulte o artigo [Variáveis de filtro curinga](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).

   ![](assets/video-date-based-wildcard-in-task-filter-350x81.png)

1. Clique em **Salvar + Fechar**.

## Informações adicionais

Consulte também:

* [Programa básico de criação de relatórios](https://one.workfront.com/s/basic-report-creation-program)
* [Variáveis de filtro curinga](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md)
* [Criar ou editar filtros no Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/create-filters.md)
* [Adicionar um prompt a um relatório](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md)
* [Usar formatação condicional em exibições](../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md)
