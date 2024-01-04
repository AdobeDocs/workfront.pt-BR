---
product-area: reporting
navigation-topic: text-mode-reporting
title: Criar instruções "OR" em filtros do modo de texto
description: É possível incluir várias instruções ao criar um filtro em listas e relatórios.
author: Nolan
feature: Reports and Dashboards
exl-id: be145e22-d66c-4a74-af0e-8bb0598b4d67
source-git-commit: 548e713700fda79070f59f3dc3457410d2c50133
workflow-type: tm+mt
source-wordcount: '561'
ht-degree: 0%

---

# Criar instruções &quot;OR&quot; em filtros do modo de texto

É possível incluir várias instruções ao criar um filtro em listas e relatórios.

Para obter informações sobre como criar filtros, consulte os seguintes artigos:

* [Visão geral dos filtros](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)
* [Editar um filtro usando o modo de texto](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md)

## Operadores de filtro do Modo de texto

Para obter informações sobre operadores de filtro Adobe Workfront na interface de filtro padrão, consulte [Visão geral dos filtros](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

O Workfront tem dois operadores de filtro que conectam cada instrução de filtro:

* **E**: ao unir a instrução de filtro 2 pelo operador AND, você indica que deseja que ambas as instruções de filtro sejam atendidas ao mesmo tempo.

  Por padrão, as instruções em um filtro são unidas pelo operador AND.

  Ao criar um filtro AND na interface do modo de texto, não é necessário usar o operador AND. É presumido.

  **Exemplo:** Para filtrar tarefas com uma Data de Conclusão Planejada de Hoje e uma Porcentagem Concluída inferior a 100%, use o seguinte código de modo de texto:

  <pre>plannedCompletionDate=$$TODAY</pre><pre>plannedCompletionDate_Mod=eq</pre><pre>percentComplete=100</pre><pre>percentComplete_Mod=lt</pre>

* **OU**: ao unir duas instruções de filtro pelo operador OR, você indica que deseja que uma delas seja atendida.

  >[!TIP]
  >
  >Ao alterar as instruções AND para instruções OR, o número de itens no relatório deve aumentar.

  Ao criar um filtro OR usando a interface de modo de texto, é necessário usar o operador OR.

  **Exemplo:** Para filtrar tarefas com uma Data de Conclusão Planejada de Hoje ou uma Porcentagem Concluída inferior a 100%, use o seguinte código de modo de texto:

  <pre>plannedCompletionDate=$$TODAY</pre><pre>plannedCompletionDate_Mod=eq</pre><pre>OU:1:percentComplete=100</pre><pre>OU:1:percentComplete_Mod=lt</pre>

## Sintaxe do modo de texto para filtros OR

A sintaxe do modo de texto para um filtro OR deve conter o seguinte:

* O operador OR seguido por dois pontos, um número e outro sinal de dois pontos no início de cada linha de filtro que se refere ao objeto na instrução OR. Isso inclui a linha que faz referência ao campo de filtro ou atributo e a linha que faz referência ao modificador de filtro.

  Siga este padrão ao criar um filtro OR:

  <pre><field name in camel case>=<value></pre><pre><field name in camel case>_Mod=<modifier value></pre><pre>OU:1:<field name in camel case>=<value></pre><pre>OU:1:<field name in camel case>_Mod=<modifier value></pre>

  >[!TIP]
  >
  >O operador OR diferencia maiúsculas de minúsculas, e está sempre em maiúsculas.

  Você pode ter várias instruções OR em um filtro. Nesse caso, cada instrução OR recebe um número, na ordem em que você deseja que as instruções sejam aplicadas.

  **Exemplo:**  Para filtrar tarefas com uma Data de conclusão planejada de Hoje OU um Percentual concluído inferior a 100% OU um Status de Novo, use o seguinte código de modo de texto:

  <pre>plannedCompletionDate=$$TODAY</pre><pre>plannedCompletionDate_Mod=eq</pre><pre>OU:1:status=NOVO</pre><pre>OU:1:status_Mod=in</pre><pre>OU:2:percentComplete=100</pre><pre>OU:2:percentComplete_Mod=lt</pre>

* O nome dos campos ou dos atributos aos quais você faz referência em um filtro deve ser escrito em camel case. Para obter informações sobre camel case, consulte [Visão geral da sintaxe do modo de texto](../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md).
* Quando você faz referência a campos personalizados em um filtro OR, deve inserir DE: entre a sintaxe do modificador OR e o nome do campo personalizado. Você deve digitar o nome do campo personalizado como ele aparece na interface do Workfront.

  **Exemplo:** Para filtrar tarefas com um Status de Novo OU uma Porcentagem Concluída inferior a 100% OU um campo personalizado chamado &quot;Tipo de conta&quot; com um valor de &quot;Igual&quot;, use o seguinte código de modo de texto:

  <pre>status=NOVO</pre><pre>status_Mod=in</pre><pre>OU:1:percentComplete=100</pre><pre>OU:1:percentComplete_Mod=lt</pre><pre>OU:2:DE:Tipo de Conta=Capital</pre><pre>OU:2:DE:Tipo de Conta_Mod=in</pre>
