---
product-area: reporting
navigation-topic: text-mode-reporting
title: Criar instruções "OU" em filtros de modo de texto
description: É possível incluir várias instruções ao criar um filtro em listas e relatórios.
author: Nolan
feature: Reports and Dashboards
exl-id: be145e22-d66c-4a74-af0e-8bb0598b4d67
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '566'
ht-degree: 0%

---

# Criar instruções &quot;OU&quot; em filtros de modo de texto

É possível incluir várias instruções ao criar um filtro em listas e relatórios.

Para obter informações sobre como criar filtros, consulte os seguintes artigos:

* [Visão geral dos filtros no Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)
* [Editar um filtro usando o modo de texto](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md)

## Operadores de filtro do Modo de texto

Para obter informações sobre operadores de filtro Adobe Workfront na interface de filtro padrão, consulte [Visão geral dos filtros no Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

O Workfront tem 2 operadores de filtro que conectam cada instrução de filtro:

* **E**: Ao unir 2 instrução de filtro pelo operador AND, você indica que deseja que ambas as instruções de filtro sejam atendidas ao mesmo tempo.

   Por padrão, as instruções em um filtro são unidas pelo operador AND .

   Ao criar um filtro AND na interface do modo de texto, não é necessário usar o operador AND . É suposto.

   **Exemplo:** Para filtrar tarefas que têm uma Data de Conclusão Planejada de Hoje e uma Porcentagem de Conclusão menor que 100%, use o seguinte código de modo de texto:

   <pre>planCompletionDate=$$TODAY</pre><pre>planCompletionDate_Mod=eq</pre><pre>percentComplete=100</pre><pre>percentComplete_Mod=lt</pre>

* **OU**: Ao associar duas instruções de filtro pelo operador OR, você indica que deseja que qualquer uma delas seja atendida.

   >[!TIP]
   >
   >Ao alterar suas instruções AND para instruções OR , o número de itens no relatório deve aumentar.

   Ao criar um filtro OU usando a interface do modo de texto, você deve usar o operador OU .

   **Exemplo:** Para filtrar tarefas que têm uma Data de Conclusão Planejada de Hoje ou uma Porcentagem de Conclusão menor que 100%, use o seguinte código de modo de texto:

   <pre>planCompletionDate=$$TODAY</pre><pre>planCompletionDate_Mod=eq</pre><pre>OU:1:percentComplete=100</pre><pre>OU:1:percentComplete_Mod=lt</pre>

## Sintaxe do modo de texto para filtros OU

A sintaxe do modo de texto para um filtro OU deve conter o seguinte:

* O operador OR seguido de dois pontos, um número e outro dois pontos no início de cada linha de filtro que se refere ao objeto na instrução OR. Isso inclui a linha que faz referência ao campo ou atributo de filtro e a linha que faz referência ao modificador de filtro.

   Siga este padrão ao criar um filtro OU:

   <pre><field name in camel case>=<value></pre><pre><field name in camel case>_Mod=<modifier value></pre><pre>OU:1:<field name in camel case>=<value></pre><pre>OU:1:<field name in camel case>_Mod=<modifier value></pre>

   >[!TIP]
   >
   >O operador OR diferencia maiúsculas de minúsculas e sempre está em maiúsculas.

   Você pode ter várias instruções OR em um filtro. Nesse caso, cada instrução OR recebe um número, na ordem em que você deseja que as instruções sejam aplicadas.

   **Exemplo:**  Para filtrar tarefas que têm uma Data de Conclusão Planejada de Hoje OU uma Porcentagem Concluída menor que 100% OU um Status de Novo, use o seguinte código de modo de texto:

   <pre>planCompletionDate=$$TODAY</pre><pre>planCompletionDate_Mod=eq</pre><pre>OU:1:status=NEW</pre><pre>OU:1:status_Mod=in</pre><pre>OU:2:percentComplete=100</pre><pre>OU:2:percentComplete_Mod=lt</pre>

* O nome dos campos ou os atributos que você faz referência em um filtro devem ser escritos em camel case. Para obter informações sobre o caso camel, consulte [Visão geral da sintaxe do modo de texto](../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md).
* Ao se referir a campos personalizados em um filtro OU, você deve inserir DE: entre a sintaxe OR modifier e o nome do campo personalizado. Você deve digitar o nome do campo personalizado como ele aparece na interface do Workfront.

   **Exemplo:** Para filtrar tarefas que têm Status Novo OU Porcentagem Concluída menor que 100% OU um campo personalizado chamado &quot;Tipo de Conta&quot; com um valor de &quot;Igual&quot;, use o seguinte código de modo de texto:

   <pre>status=NEW</pre><pre>status_Mod=in</pre><pre>OU:1:percentComplete=100</pre><pre>OU:1:percentComplete_Mod=lt</pre><pre>OU:2:DE:Tipo de Conta=Capital</pre><pre>OU:2:DE:Account Type_Mod=in</pre>
