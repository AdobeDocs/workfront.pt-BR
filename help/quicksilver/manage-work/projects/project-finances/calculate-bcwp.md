---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: Calcular o custo orçado do trabalho realizado (BCWP)
description: Também conhecido como Valor Agregado, o Custo Orçado do Trabalho Realizado (COTR) é uma métrica de desempenho do projeto que representa a quantidade da tarefa que foi realmente concluída no momento em que essa métrica é calculada.
author: Lisa
feature: Work Management
exl-id: 203709a7-e522-4875-b3eb-40b967a938ec
TQID: https://experienceleague.adobe.com/ahGgQPcR7LoWSLthsvYytqMIyoVcE86N2A3kAflYS2I
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40cid: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 573
ht-degree: 10%

---

# Calcular o custo orçado do trabalho realizado (BCWP)

## Visão Geral do Custo Orçado do Trabalho Executado (COTR)

Também conhecido como Valor Agregado, o Custo Orçado do Trabalho Realizado (COTR) é uma métrica de desempenho do projeto que representa a quantidade da tarefa que foi realmente concluída no momento em que essa métrica é calculada.

O Adobe Workfront calcula o COTR (Custo Orçado do Trabalho Executado) para projetos e tarefas.

Considere o seguinte ao revisar os valores para o COTR em uma tarefa ou projeto:

* O Workfront calcula o COTR de uma tarefa com base na sua configuração para o Método de indexação de desempenho (PMI) do projeto.

  Você pode configurar seu projeto para calcular a PMI usando horas ou custo e a BCWP também é calculada usando os mesmos valores.

  Para obter informações sobre como configurar o cálculo do COTR, consulte a seção [Configurar como o COTR é calculado](#configure-how-bcwp-is-calculated) neste artigo.

* O Workfront calcula o COTR de um projeto adicionando todos os valores do COTR de todas as tarefas pai e tarefas individuais do projeto.

  Os valores de tarefas filhas não são adicionados ao COTR do projeto.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Pacote do Adobe Workfront</td> 
   <td>Qualquer</td> 
  </tr> 
  <tr> 
   <td>Licença do Adobe Workfront</td> 
   <td>
   <p>Padrão</p>
   <p>Plano</p></td> 
  </tr> 
  <tr> 
   <td>Configurações de nível de acesso</td> 
   <td>Editar acesso a projetos</td> 
  </tr> 
  <tr> 
   <td>Permissões de objeto</td> 
   <td>Gerenciar permissões do projeto</td> 
  </tr> 
 </tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Configurar como o COTR é calculado {#configure-how-bcwp-is-calculated}

Você pode configurar se o COTR é calculado em horas ou em custos, configurando como o Método de Índice de Desempenho (PIM) do projeto é calculado.

1. Vá para um projeto e expanda **Detalhes do projeto** no painel esquerdo.
1. Na área **Finanças**, localize o campo **Método de Índice de Desempenho** e clique duas vezes nele para editá-lo.

   ![Opções de PIM](assets/pim-options-hour-cost-based-nwe.png)

1. Selecione entre as seguintes opções:

   | Opção | Como o cálculo é executado |
   |---|---|
   | Baseado em Hora | O Workfront calcula o COTR usando as Horas planejadas das tarefas. |
   | Baseado em Custo | O Workfront calcula o COTR usando o Custo Planejado das tarefas. |

1. Clique em **Salvar alterações**.

   O COTR das tarefas no projeto é calculado usando horas ou custos.

## Calcular COTR

O Workfront calcula o COTR (Custo Orçado do Trabalho Executado) de uma tarefa ou projeto usando as seguintes fórmulas:

```
Task BCWP = Actual Percent Complete x Task Budget
```

```
Project BCWP = SUM(BCWP values of all parent and individual tasks)
```

Os seguintes valores são usados nesses cálculos:

| Valor usado | Descrição do valor usado |
|---|---|
| Percentual de Término Efetivo | Este é o percentual de conclusão real da tarefa, conforme exibido no Workfront. |
| Orçamento da tarefa | Esse é o valor para as Horas planejadas ou o Custo planejado da tarefa. |

Por exemplo, se o percentual de conclusão real da tarefa for de 25% e o Orçamento da Tarefa ou o Custo Planejado for de $10.000, o COTR da tarefa será:

```
BCWP = 25% x $10,000 = $2,500
```

## Localizar o COTR de um projeto ou de uma tarefa

Você pode exibir o valor do Custo Orçado do Trabalho Executado em um relatório ou lista adicionando a coluna COTR à exibição.

1. Ir para uma lista de tarefas ou projetos.
1. Expanda o menu **Exibir** e selecione **Nova Exibição** ou **Personalizar Exibição**.

1. Clique em **Adicionar coluna**.
1. No campo **Mostrar nesta coluna:**, comece digitando **BCWP** e clique para selecioná-lo quando ele for exibido na lista.

   ![COTR no modo de exibição de projeto](assets/bcwp-project-view.png)

1. Clique em **Salvar visualização**.
1. O campo COTR é exibido na exibição.
