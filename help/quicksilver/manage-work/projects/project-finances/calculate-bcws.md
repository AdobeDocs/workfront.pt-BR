---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: Calcular o Custo do Trabalho Programado Orçado (BCWS)
description: Também conhecido como Valor Planejado, o Custo do Trabalho Programado Orçado (BCWS) é uma métrica de desempenho do projeto que representa a quantidade da tarefa que deve ter sido concluída no momento em que essa métrica é calculada.
author: Alina
feature: Work Management
exl-id: b9a36333-9430-42bd-99dd-3ad82803b633
source-git-commit: 1d5de5ff0ebebd84482507c71730cfbd05c513a5
workflow-type: tm+mt
source-wordcount: '644'
ht-degree: 0%

---

# Calcular o Custo do Trabalho Programado Orçado (BCWS)

## Visão Geral do Custo do Trabalho Programado Orçado (BCWS)

Também conhecido como Valor Planejado, o Custo do Trabalho Programado Orçado (BCWS) é uma métrica de desempenho do projeto que representa a quantidade da tarefa que deve ter sido concluída no momento em que essa métrica é calculada.

O Adobe Workfront calcula o Custo do Trabalho Programado Orçado (BCWS) para projetos e tarefas.

Considere o seguinte ao revisar os valores do BCWS em uma tarefa ou projeto:

* A Workfront calcula o BCWS para uma tarefa com base na sua configuração do Método de Índice de Desempenho (PIM) do projeto.

   Você pode configurar seu projeto para calcular o PIM usando horas ou custo e o BCWS também é calculado usando os mesmos valores.

   Para obter informações sobre como configurar como o BCWS é calculado, consulte a seção [Configurar como o BCWS é calculado](#configure-how-bcws-is-calculated) neste artigo.

* O Workfront calcula o BCWS para um projeto adicionando todos os valores BCWS de todas as tarefas pai e tarefas individuais no projeto.

   Os valores das tarefas filho não são adicionados ao BCWS do projeto.

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
   <td> <p>Editar acesso a Projetos</p> <p>Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões do projeto</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

## Configurar como o BCWS é calculado {#configure-how-bcws-is-calculated}

Você pode configurar se o BCWS é calculado em horas ou custos configurando como o Método de Índice de Desempenho (PIM) do projeto é calculado.

1. Vá para um projeto e clique em **Detalhes do projeto** no painel esquerdo.
1. No **Finanças** localize a **Método do Índice de Desempenho** e clique duas vezes nele para editá-lo.

   ![](assets/pim-options-hour-cost-based-nwe.png)

1. Selecione dentre as seguintes opções:

   | Opção | Como o cálculo é executado |
   |---|---|
   | Baseado em Hora | O Workfront calcula o BCWS usando as Horas Planejadas das tarefas. |
   | Baseado em Custo | O Workfront calcula o BCWS usando o Custo planejado das tarefas. |


1. Clique em **Salvar alterações**.

   O BCWS das tarefas no projeto é calculado usando horas ou custos.

## Calcular BCWS

O Workfront calcula o Custo do Trabalho Programado Orçado (BCWS) para tarefas ou projetos usando as seguintes fórmulas:

```
Task BCWS = Planned Percent Complete x Task Budget
```

```
Project BCWS = SUM(BCWS values of all parent and individual tasks)
```

Os seguintes valores são usados neste cálculo:

| Valor usado | Descrição do valor utilizado |
|---|---|
| Porcentagem Planejada Concluída | Isso é o percentual de conclusão da tarefa que deve ser observando a quantidade de tempo decorrido entre o início da tarefa e hoje. |
| Orçamento da Tarefa | Esse é o valor para as Horas Planejadas ou o Custo Planejado da tarefa. |

Por exemplo, se hoje for 12 de fevereiro e uma tarefa estiver agendada para durar de 10 de fevereiro a 20 de fevereiro, a tarefa deverá estar 20% concluída hoje. Se o Orçamento da Tarefa (Custo Planejado) for de US$ 10.000, o BCWS para a tarefa será:

```
Task BCWS = 20% x $10,000 = $2,000
```

## Localize o BCWS para um projeto ou tarefa

Você pode exibir o valor do Custo do Trabalho Programado Orçado em um relatório ou lista, adicionando a coluna BCWS à sua visualização.

1. Vá para uma lista de tarefas ou projetos.
1. Expanda o **Exibir** e selecione **Nova exibição** ou **Personalizar exibição**.

1. Clique em **Adicionar coluna**.
1. No **Mostrar nesta coluna:** digitação de início de campo **BCWS** e clique em para selecioná-lo quando for exibido na lista.

   ![](assets/bcws-in-project-view.png)

1. Clique em **Salvar exibição**.
1. O **BCWS** é exibido na exibição.
