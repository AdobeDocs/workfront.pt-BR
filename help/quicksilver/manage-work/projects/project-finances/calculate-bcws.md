---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: Calcular o Custo Orçado do Trabalho Agendado (BCWS)
description: Também conhecido como Valor Planejado, o Custo Orçado do Trabalho Agendado (BCWS) é uma métrica de desempenho do projeto que representa a quantidade da tarefa que deveria ter sido concluída no momento em que essa métrica é calculada.
author: Alina
feature: Work Management
exl-id: b9a36333-9430-42bd-99dd-3ad82803b633
source-git-commit: 1d5de5ff0ebebd84482507c71730cfbd05c513a5
workflow-type: tm+mt
source-wordcount: '649'
ht-degree: 2%

---

# Calcular o Custo Orçado do Trabalho Agendado (BCWS)

## Visão Geral do Custo Orçado do Trabalho Agendado (BCWS)

Também conhecido como Valor Planejado, o Custo Orçado do Trabalho Agendado (BCWS) é uma métrica de desempenho do projeto que representa a quantidade da tarefa que deveria ter sido concluída no momento em que essa métrica é calculada.

O Adobe Workfront calcula o BCWS (Custo Orçado do Trabalho Agendado) para projetos e tarefas.

Considere o seguinte ao revisar os valores para o BCWS em uma tarefa ou projeto:

* O Workfront calcula o BCWS de uma tarefa com base na sua configuração para o Método de Índice de Desempenho (PIM) do projeto.

  Você pode configurar seu projeto para calcular o PIM usando horas ou custo e o BCWS também é calculado usando os mesmos valores.

  Para obter informações sobre como configurar o BCWS, consulte a seção [Configurar como o BCWS é calculado](#configure-how-bcws-is-calculated) neste artigo.

* O Workfront calcula o BCWS de um projeto adicionando todos os valores BCWS de todas as tarefas pai e tarefas individuais do projeto.

  Os valores de tarefas filhas não são adicionados ao BCWS do projeto.

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront*</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Plano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a projetos</p> <p>Se você ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões do projeto</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso aos objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qual plano, tipo de licença ou acesso você tem, contate o administrador do Workfront.

## Configurar como o BCWS é calculado {#configure-how-bcws-is-calculated}

Você pode configurar se o BCWS é calculado em horas ou em custos, configurando como o Método de Índice de Desempenho (PIM) do projeto é calculado.

1. Vá para um projeto e clique em **Detalhes do projeto** no painel esquerdo.
1. Na área **Finanças**, localize o campo **Método de Índice de Desempenho** e clique duas vezes nele para editá-lo.

   ![](assets/pim-options-hour-cost-based-nwe.png)

1. Selecione entre as seguintes opções:

   | Opção | Como o cálculo é executado |
   |---|---|
   | Baseado em Hora | O Workfront calcula o BCWS usando as Horas planejadas das tarefas. |
   | Baseado em Custo | O Workfront calcula o BCWS usando o Custo Planejado das tarefas. |


1. Clique em **Salvar alterações**.

   O BCWS das tarefas no projeto é calculado usando horas ou custos.

## Calcular BCWS

O Workfront calcula o BCWS (Custo Orçado do Trabalho Agendado) para tarefas ou projetos usando as seguintes fórmulas:

```
Task BCWS = Planned Percent Complete x Task Budget
```

```
Project BCWS = SUM(BCWS values of all parent and individual tasks)
```

Os seguintes valores são usados neste cálculo:

| Valor usado | Descrição do valor usado |
|---|---|
| Percentual Concluído Planejado | Isso é o que a porcentagem concluída da tarefa deve ser observando a quantidade de tempo decorrido entre o início da tarefa e hoje. |
| Orçamento da tarefa | Esse é o valor para as Horas planejadas ou o Custo planejado da tarefa. |

Por exemplo, se hoje for 12 de fevereiro e uma tarefa estiver programada para durar de 10 a 20 de fevereiro, a tarefa deverá estar 20% concluída hoje. Se o Orçamento da Tarefa (Custo Planejado) for de $10.000, o COTA da tarefa será:

```
Task BCWS = 20% x $10,000 = $2,000
```

## Localizar o COTA de um projeto ou de uma tarefa

Você pode exibir o valor do Custo orçado do trabalho agendado em um relatório ou lista adicionando a coluna BCWS à exibição.

1. Ir para uma lista de tarefas ou projetos.
1. Expanda o menu **Exibir** e selecione **Nova Exibição** ou **Personalizar Exibição**.

1. Clique em **Adicionar coluna**.
1. No campo **Mostrar nesta coluna:**, comece digitando **BCWS** e clique para selecioná-lo quando ele for exibido na lista.

   ![](assets/bcws-in-project-view.png)

1. Clique em **Salvar visualização**.
1. O campo **BCWS** é exibido no modo de exibição.
