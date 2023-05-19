---
product-area: reporting
navigation-topic: reporting-elements
title: Usar curingas com base em data para generalizar relatórios
description: Você pode generalizar um relatório usando curingas em vez de informações específicas ao criar determinados elementos de relatórios.
author: Nolan
feature: Reports and Dashboards
exl-id: 759b0bea-729e-4206-808c-0a7216ded4ff
source-git-commit: 888c938e5d649557df69374a55d4e4ecc2da6f55
workflow-type: tm+mt
source-wordcount: '678'
ht-degree: 0%

---

# Usar curingas com base em data para generalizar relatórios

Você pode generalizar um relatório usando curingas em vez de informações específicas ao criar determinados elementos de relatórios.

Por exemplo, se você quiser criar um relatório que mostre as tarefas com uma Data de início planejada específica, poderá usar o seletor de datas do calendário em um filtro para selecionar uma data específica. No entanto, se você quiser criar um relatório que mostre tarefas com a Data de início planejada dentro de um determinado período a partir da data em que o relatório é acessado, poderá usar um curinga que indique que, quando alguém exibir o relatório, ele exibirá informações de um período relevante para o momento em que o relatório for exibido.

Por exemplo, na semana passada, no ano passado, nas próximas duas semanas etc. Assim, você cria o relatório uma vez, mas como usa um curinga no filtro, ele produz resultados diferentes toda vez que alguém o lê, pois se adapta ao dia em que executam o relatório.

Você pode usar curingas baseados em data ao criar os seguintes elementos de relatório:

* Filtros
* Prompts personalizados
* Exibições ao adicionar regras para colunas

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>plano do Adobe Workfront*</strong></td> 
   <td> <p>Qualquer Um</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Licença da Adobe Workfront*</strong></td> 
   <td> <p>Plano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurações de nível de acesso*</strong></td> 
   <td> <p>Editar acesso a Filtros, Visualizações, Agrupamentos</p> <p>Editar acesso a relatórios, painéis e calendários para editar elementos de relatórios em um relatório</p> <p>Observação: se você ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Permissões de objeto</strong></td> 
   <td> <p>Gerenciar permissões para um relatório para editar elementos de relatórios em um relatório</p> <p>Gerenciar permissões em uma exibição ou um filtro para editá-las</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir seu plano, tipo de licença ou acesso, entre em contato com o administrador do Workfront.

## Pré-requisitos

Você deve criar um relatório antes de adicionar variáveis curingas a ele.

Para obter informações sobre como criar um relatório, consulte [Criar um relatório](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md).

## Etapas passo a passo

Para inserir um curinga com base em data em um relatório:

1. Vá para um relatório para o qual deseja inserir um curinga com base em data.
1. Clique em **Ações de Relatório**, depois **Editar**.

1. Clique em **Filtros** guia.
1. Clique em **Adicionar uma regra de filtro**.
1. Comece digitando o nome do campo pelo qual deseja filtrar.\
   É necessário digitar campos que façam referência a uma data.
1. Selecionar **Igual** no menu suspenso para a variável de filtro.

   >[!TIP]
   >
   >Você sempre deve selecionar o **Igual** ao trabalhar com curingas no Adobe Workfront.

1. No **Comece a digitar o nome...** digite: `$$TODAY` se quiser exibir informações sobre algo que ocorre no mesmo dia em que o relatório é executado.

   Ou

   Tipo `$$NOW` se desejar exibir informações sobre algo que ocorre na mesma data e hora em que o relatório é executado.

   Essa data é sempre diferente, pois muda com a data em que o relatório é realmente visualizado por um usuário. portanto, as informações no relatório são diferentes de dia para dia.

1. (Opcional) Se desejar exibir informações que ocorram em um período posterior à data em que o relatório é executado, digite `$$TODAY+1w` para exibir informações na semana seguinte, ou `$$TODAY+2m` para exibir informações nos próximos dois meses. Você também pode indicar períodos de tempo para trimestres, horas, dias ou anos.
1. (Opcional) Se desejar exibir informações sobre algo que ocorreu em um período anterior à data em que o relatório foi executado, digite `$$TODAY-1w` para exibir informações da semana anterior, ou `$$TODAY-2m` para exibir informações dos dois meses anteriores. Você também pode indicar períodos de tempo para trimestres, horas, dias ou anos.

   Para obter uma lista completa de atributos, qualificadores e operadores que você pode usar em curingas baseados em data, consulte o artigo [Variáveis de filtro curinga](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).

   ![](assets/video-date-based-wildcard-in-task-filter-350x81.png)

1. Clique em **Salvar + Fechar**.

## Informações adicionais

Consulte também:

<!--outdated: * [Basic Report Creation Program](https://one.workfront.com/s/basic-report-creation-program) -->
* [Variáveis de filtro curinga](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md)
* [Criar ou editar filtros no Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/create-filters.md)
* [Adicionar um prompt a um relatório](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md)
* [Usar formatação condicional em exibições](../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md)
