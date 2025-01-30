---
product-area: reporting
navigation-topic: text-mode-reporting
title: Criar instruções "OR" em filtros do modo de texto
description: É possível incluir várias instruções ao criar um filtro em listas e relatórios.
author: Nolan
feature: Reports and Dashboards
exl-id: be145e22-d66c-4a74-af0e-8bb0598b4d67
source-git-commit: af4a82ad11b57c7a7457d5d7ee74ee18494a1dc0
workflow-type: tm+mt
source-wordcount: '503'
ht-degree: 0%

---

# Criar instruções &quot;OR&quot; em filtros do modo de texto

É possível incluir várias instruções ao criar um filtro em listas e relatórios.

Para obter informações sobre como criar filtros, consulte os seguintes artigos:

* [Visão geral dos filtros](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/filters-overview.md)
* [Editar um filtro usando o modo de texto](/help/quicksilver/reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md)

## Operadores de filtro do Modo de texto

Para obter informações sobre operadores de filtro Adobe Workfront na interface de filtro padrão, consulte [Visão geral dos filtros](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/filters-overview.md).

O Workfront tem dois operadores de filtro que conectam cada instrução de filtro:

* **AND**: ao unir 2 instruções de filtro pelo operador AND, você indica que deseja que ambas as instruções de filtro sejam atendidas ao mesmo tempo.

  Por padrão, as instruções em um filtro são unidas pelo operador AND.

  Ao criar um filtro AND na interface do modo de texto, não é necessário usar o operador AND. É presumido.

  **Exemplo:** Para filtrar tarefas com uma Data de Conclusão Planejada de Hoje e uma Porcentagem Concluída inferior a 100%, use o seguinte código de modo de texto:

  ```
  plannedCompletionDate=$$TODAY
  plannedCompletionDate_Mod=eq 
  percentComplete=100 percent
  Complete_Mod=lt
  ```

* **OR**: ao unir duas instruções de filtro pelo operador OR, você indica que deseja que qualquer uma delas seja atendida.

  >[!TIP]
  >
  >Ao alterar as instruções AND para instruções OR, o número de itens no relatório deve aumentar.

  Ao criar um filtro OR usando a interface de modo de texto, é necessário usar o operador OR.

  **Exemplo:** Para filtrar tarefas com uma Data de Conclusão Planejada de Hoje ou uma Porcentagem Concluída inferior a 100%, use o seguinte código de modo de texto:

  ```
  plannedCompletionDate=$$TODAY
  plannedCompletionDate_Mod=eq
  OR:1:percentComplete=100
  OR:1:percentComplete_Mod=lt
  ```

## Sintaxe do modo de texto para filtros OR

A sintaxe do modo de texto para um filtro OR deve conter o seguinte:

* O operador OR seguido por dois pontos, um número e outro sinal de dois pontos no início de cada linha de filtro que se refere ao objeto na instrução OR. Isso inclui a linha que faz referência ao campo de filtro ou atributo e a linha que faz referência ao modificador de filtro.

  Siga este padrão ao criar um filtro OR:

  ```
  <field name in camel case>=<value>
  <field name in camel case>_Mod=<modifier value>
  OR:1:<field name in camel case>=<value>
  OR:1:<field name in camel case>_Mod=<modifier value>
  ```

  >[!TIP]
  >
  >O operador OR diferencia maiúsculas de minúsculas, e está sempre em maiúsculas.

  Você pode ter várias instruções OR em um filtro. Nesse caso, cada instrução OR recebe um número, na ordem em que você deseja que as instruções sejam aplicadas.

  **Exemplo:** Para filtrar tarefas com uma Data de Conclusão Planejada de Hoje OU uma Porcentagem Concluída inferior a 100% OU um Status de Novo, use o seguinte código de modo de texto:

  ```
  plannedCompletionDate=$$TODAY
  plannedCompletionDate_Mod=eq
  OR:1:status=NEW
  OR:1:status_Mod=in
  OR:2:percentComplete=100
  OR:2:percentComplete_Mod=lt
  ```

* O nome dos campos ou dos atributos aos quais você faz referência em um filtro deve ser escrito em camel case. Para obter informações sobre camel case, consulte [Visão geral da sintaxe do modo texto](../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md).
* Quando você faz referência a campos personalizados em um filtro OR, deve inserir DE: entre a sintaxe do modificador OR e o nome do campo personalizado. Você deve digitar o nome do campo personalizado como ele aparece na interface do Workfront.

  **Exemplo:** Para filtrar tarefas com status Novo OU Porcentagem Concluída inferior a 100% OU um campo personalizado chamado &quot;Tipo de Conta&quot; com valor &quot;Igual&quot;, use o seguinte código de modo de texto:

  ```
  status=NEW
  status_Mod=in
  OR:1:percentComplete=100
  OR:1:percentComplete_Mod=lt
  OR:2:DE:Account Type=Capital
  OR:2:DE:Account Type_Mod=in
  ```
