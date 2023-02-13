---
product-previous: workfront-goals
navigation-topic: goal-management
title: Visão geral do progresso e condição da meta nas Metas da Adobe Workfront
description: O progresso de metas é orientado por indicadores de progresso como atividades, resultados ou metas secundárias. A condição da meta é determinada pelo progresso da meta no momento atual.
author: Alina
feature: Workfront Goals
exl-id: 3050f7ff-a579-4fb8-82fd-bef850f27c20
source-git-commit: 1d221d10e5845e477dff825f853330b9b4df0adf
workflow-type: tm+mt
source-wordcount: '821'
ht-degree: 1%

---

# Visão geral do progresso e condição da meta nas Metas da Adobe Workfront

<!--drafted for P&P release: the note at the top will need to be replaced with this:

Your organization must have the following to use the functionality described in this article:

* For the legacy plan and license structure: 

  * A Pro or higher [Adobe Workfront plan](https://www.workfront.com/plans). 
  * An Adobe Workfront Goals license in addition to a Workfront license.

* For the current plan and license structure:

  * An Ultimate plan 
    
    Or
    
    An additional license for Adobe Workfront Goals for the Prime or Select Adobe Workfront plans. <is there a link we can add here for the plans and what they contain?!>

Contact your Workfront account manager to learn about a Workfront Goals license.

For additional information about access to Workfront Goals, see [Requirements to use Workfront Goals](../../workfront-goals/goal-management/access-needed-for-wf-goals.md).
-->

>[!NOTE]
>
>Sua organização deve ter o seguinte para usar a funcionalidade descrita neste artigo:
>
>* Um Pro ou superior [Plano Adobe Workfront](https://www.workfront.com/plans).
>* Uma licença do Adobe Workfront Metas além de uma licença da Workfront.
>
>Entre em contato com o gerente de conta da Workfront para saber mais sobre uma licença do Workfront Metas.
>Para obter informações adicionais sobre o acesso às Metas da Workfront, consulte [Requisitos para usar as metas do Workfront](../../workfront-goals/goal-management/access-needed-for-wf-goals.md).

O Adobe Workfront calcula o progresso da meta automaticamente, com base no progresso de seus indicadores de progresso.

## Pré-requisitos

Você deve ter o seguinte antes de começar:

* Um modelo de layout que inclui a área Metas no Menu principal.

## Visão geral do progresso e do limite da meta

Após ativar uma meta, as Metas do Workfront começam a calcular seu progresso e condição e exibem os seguintes indicadores quando você passa o mouse sobre o campo Andamento:

| Indicador | Descrição do indicador |
|---|---|
| Porcentagem real concluída | Até agora, a percentagem do objetivo foi efetivamente alcançada. As Metas da Workfront calculam esse valor ao calcular a média da porcentagem completa de todos os indicadores de progresso associados à meta. |
| Porcentagem esperada concluída | Quanta meta deve ser concluída até agora para que a meta seja concluída a tempo. As Metas da Workfront calculam esse valor observando a Duração da meta e o momento atual no tempo. O objetivo deve exibir esse valor no momento atual, se ele for concluído no momento. |
| Progresso | Um rótulo que indica se a meta está no target para ser concluída a tempo ou se está em risco ou com problemas de não conclusão. |

![](assets/in-trouble-goal-progress-expanded.png)

<!--drafted for the redesign: replace the screen shot above with the redesigned one which is white, not black-->

* [Porcentagem real concluída](#actual-percent-complete)
* [Porcentagem esperada concluída](#expected-percent-complete)
* [Progresso e condição](#progress)

### Porcentagem real concluída {#actual-percent-complete}

As Metas do Workfront calculam automaticamente a porcentagem completa real de uma meta com base na média de porcentagem completa dos indicadores de progresso da meta.

Os itens a seguir são considerados indicadores de progresso para metas:

* Resultados

   Para obter informações sobre como adicionar resultados às metas, consulte [Adicionar resultados às metas em Metas da Adobe Workfront](../../workfront-goals/results-and-activities/add-results-to-goals.md).

* Atividades

   Para obter informações sobre como adicionar atividades, incluindo projetos, a metas, consulte [Adicionar atividades às metas em Metas da Adobe Workfront](../../workfront-goals/results-and-activities/add-activities-to-goals.md).

* Objetivos de crianças alinhadas

   Para obter informações sobre metas pai e filho, consulte [Alinhar metas ao conectá-las às metas da Adobe Workfront](../../workfront-goals/goal-alignment/align-goals-by-connecting-them.md).

   As Metas do Workfront calculam a porcentagem total real usando a seguinte fórmula:

   ```
   Actual percent complete of goal = SUM(Percent complete of goal progress indicators)* 100 / Number of progress indicators
   ```

   Por exemplo, se uma meta tiver um Resultado 20% concluído, uma barra de progresso manual que esteja 30% concluída, um projeto 10% concluído e uma meta para crianças que esteja 40% concluída, a porcentagem de meta concluída será 25%.

### Porcentagem esperada concluída {#expected-percent-complete}

As Metas do Workfront calculam automaticamente a porcentagem completa esperada de uma meta com base no número total de dias na duração da meta, bem como no número de dias que passaram desde a data de início da meta.

As Metas do Workfront calculam a porcentagem completa esperada usando a seguinte fórmula:

```
Expected percent complete of goal = Number of days since the goal start date * 100/ Number of days in the goal duration
```

Por exemplo, se uma meta deve ser concluída em 90 dias e hoje é o 45º dia dessa duração, a porcentagem esperada de conclusão é 50%.

### Progresso e condição {#progress}

As Metas do Workfront calculam uma porcentagem de progresso e atribuem um rótulo de progresso a metas, com base na porcentagem da porcentagem esperada concluída que foi alcançada no momento atual. A cor da barra de porcentagem de meta concluída muda para indicar o progresso da meta.

A condição da meta também é atualizada, de acordo, para indicar se a meta está no target para ser concluída a tempo ou se está ficando para trás.

As Metas do Workfront calculam a porcentagem de progresso de uma meta usando a seguinte fórmula:

```
Goal progress percentage = Actual percent complete * 100 / Expected percent complete
```

Por exemplo, se a porcentagem esperada de conclusão for de 53% no momento atual e a porcentagem real de conclusão for de 30%, a porcentagem de progresso da meta será de 56%. O Workfront Metas rotula essa meta com uma Condição de &quot;Em problemas&quot;.

O gráfico a seguir ilustra a relação entre os rótulos de condição e a porcentagem de progresso:

![](assets/progress-status-labels-charted-after-match-with-project-condition-350x147.png)

A tabela abaixo lista os rótulos de condição da meta e as porcentagens de progresso da meta associadas a cada rótulo.

>[!TIP]
>
>Os rótulos de condição de meta correspondem ao nome e à cor da condição do projeto do Workfront.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><b>Nome do progresso da meta</b></td> 
   <td><b>Definição de progresso de meta</b></td> 
   <td><b>Porcentagem de progresso do objetivo</b></td> 
   <td><b>Cor da barra de porcentagem concluída</b></td> 
   <td><b>Ícone Indicador de condição</b></td> 
  </tr> 
  <tr> 
   <td>Novo(a)</td> 
   <td> <p>O objetivo é recém-criado e ainda não está registrando progresso. Um progresso de meta é exibido como Novo até que alguém atualize seu progresso pela primeira vez. </p> <p>Para obter informações sobre como atualizar o progresso da meta, consulte <a href="../../workfront-goals/goal-review-and-workfront-goals-sections/check-in-goals.md" class="MCXref xref">Atualizar o progresso da meta nas Metas da Adobe Workfront</a>.</p> </td> 
   <td>Sem porcentagem</td> 
   <td>Sem barra</td> 
   <td><img src="assets/new-goal-icon-condition.png" alt="new_gol_icon_condition.png"></td>
  </tr> 
  <tr> 
   <td> <p><span>No Prazo</span> </p> </td> 
   <td>A meta está funcionando como esperado e há uma grande probabilidade de ser concluída a tempo. </td> 
   <td>90-100%</td> 
   <td>Verde</td> 
    <td><img src="assets/on-target-icon-condition.png" alt="on_target_icon_condition.png"></td>
  </tr> 
  <tr> 
   <td> <p><span>Em Risco</span> </p> </td> 
   <td>A meta está atrasada, mas ainda pode ser possível concluí-la a tempo. </td> 
   <td>70-89.99%</td> 
   <td>Amarelo</td>
   <td><img src="assets/at-risk-icon-condition.png" alt="at_risk_icon_condition.png"></td> 
  </tr> 
  <tr> 
   <td> <p><span>Com problemas</span> </p> </td> 
   <td> <p>É muito provável que a meta não seja concluída a tempo. </p> </td> 
   <td>0-69.99%</td> 
   <td>Vermelho</td> 
   <td><img src="assets/in-trouble-icon-condition.png" alt="in_trouble_icon_condition.png"></td> 
  </tr> 
 </tbody> 
</table>