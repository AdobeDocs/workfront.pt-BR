---
product-previous: workfront-goals
navigation-topic: goal-management
title: Visão geral do progresso e da condição da meta no Adobe Workfront Goals
description: O progresso da meta é orientado por indicadores de progresso como atividades, resultados ou metas secundárias. A condição da meta é determinada pelo progresso da meta no momento atual.
author: Alina
feature: Workfront Goals
exl-id: 3050f7ff-a579-4fb8-82fd-bef850f27c20
source-git-commit: 09e34ecdfeec531ebbaaba4fb8682496c53d86bf
workflow-type: tm+mt
source-wordcount: '820'
ht-degree: 0%

---

# Visão geral do progresso e da condição da meta no Adobe Workfront Goals

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
>Sua organização deve ter as seguintes opções para usar a funcionalidade descrita neste artigo:
>
>* A Pro ou superior [plano do Adobe Workfront](https://www.workfront.com/plans).
>* Uma licença do Adobe Workfront Goals, além de uma licença da Workfront.
>
>Entre em contato com o gerente de conta da Workfront para saber mais sobre uma licença do Workfront Goals.
>Para obter informações adicionais sobre o acesso ao Workfront Goals, consulte [Requisitos para usar as metas do Workfront](../../workfront-goals/goal-management/access-needed-for-wf-goals.md).

O Adobe Workfront calcula o progresso da meta automaticamente, com base no progresso de seus indicadores de progresso.

## Pré-requisitos

Você deve ter o seguinte antes de iniciar:

* Um Modelo de layout que inclui a área Metas no Menu principal.

## Visão geral do progresso e limite da meta

Depois de ativar uma meta, o Workfront Goals começa a calcular seu progresso e condição e exibe os seguintes indicadores quando você passa o mouse sobre o campo Progresso:

| Indicador | Descrição do indicador |
|---|---|
| Percentual concluído real | Quanto da meta foi realmente concluída até agora. O Workfront Goals calcula esse valor calculando a média do percentual concluído de todos os indicadores de progresso associados à meta. |
| Porcentagem concluída esperada | Quanto da meta deve ser concluída até o momento para que seja concluída no prazo. O Workfront Goals calcula esse valor observando a Duração da meta e o momento atual no tempo. A meta deve exibir esse valor no horário atual, se for concluído a tempo. |
| Progresso | Um rótulo que indica se a meta está no público alvo para ser concluída no prazo, ou se está em risco ou em problema de não ser concluída. |

![](assets/in-trouble-goal-progress-expanded.png)

<!--drafted for the redesign: replace the screen shot above with the redesigned one which is white, not black-->

* [Percentual concluído real](#actual-percent-complete)
* [Porcentagem concluída esperada](#expected-percent-complete)
* [Progresso e condição](#progress)

### Percentual concluído real {#actual-percent-complete}

As Metas do Workfront calculam automaticamente o percentual de conclusão real de uma meta com base na média do percentual de conclusão dos indicadores de progresso da meta.

Os itens a seguir são considerados indicadores de progresso para metas:

* Resultados

  Para obter informações sobre como adicionar resultados às metas, consulte [Adicionar resultados às metas no Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-results-to-goals.md).

* Atividades

  Para obter informações sobre como adicionar atividades, incluindo projetos às metas, consulte [Adicionar atividades às metas no Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-activities-to-goals.md).

* Metas secundárias alinhadas

  Para obter informações sobre metas pai e filho, consulte [Alinhar metas ao conectá-las às Metas do Adobe Workfront](../../workfront-goals/goal-alignment/align-goals-by-connecting-them.md).

  O Workfront Goals calcula o percentual de conclusão real usando a seguinte fórmula:

  ```
  Actual percent complete of goal = SUM(Percent complete of goal progress indicators)* 100 / Number of progress indicators
  ```

  Por exemplo, se uma meta tiver um Resultado que esteja 20% concluído, uma Barra de progresso manual que esteja 30% concluída, um projeto que esteja 10% concluído e uma meta secundária que esteja 40% concluída, a porcentagem concluída será de 25%.

### Porcentagem concluída esperada {#expected-percent-complete}

O Workfront Goals calcula automaticamente a porcentagem concluída esperada de uma meta com base no número total de dias na duração da meta, bem como no número de dias decorridos desde a data de início da meta.

O Workfront Goals calcula o percentual de conclusão esperado usando a seguinte fórmula:

```
Expected percent complete of goal = Number of days since the goal start date * 100/ Number of days in the goal duration
```

Por exemplo, se uma meta tiver de ser concluída em 90 dias e hoje for o 45º dia dessa duração, o percentual de conclusão esperado será de 50%.

### Progresso e condição {#progress}

O Workfront Goals calcula uma porcentagem de progresso e atribui um rótulo de progresso às metas com base na porcentagem esperada de conclusão atingida no momento atual. A cor da barra de porcentagem concluída da meta muda para indicar o progresso da meta.

A Condição da meta também é atualizada, de acordo, para indicar se a meta está no destino para ser concluída no prazo ou se está atrasada.

O Workfront Goals calcula a porcentagem de progresso de uma meta usando a seguinte fórmula:

```
Goal progress percentage = Actual percent complete * 100 / Expected percent complete
```

Por exemplo, se o percentual de conclusão esperado for 53% no momento atual e o percentual de conclusão real for 30%, o percentual de progresso de conclusão meta será 56%. O Workfront Goals rotula essa meta com uma Condição de &quot;Com Problemas&quot;.

O gráfico a seguir ilustra a relação entre os rótulos de condição e a porcentagem de progresso:

![](assets/progress-status-labels-charted-after-match-with-project-condition-350x147.png)

A tabela abaixo lista os rótulos de condição de meta e as porcentagens de progresso da meta associadas a cada rótulo.

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
   <td><b>Definição do progresso da meta</b></td> 
   <td><b>Porcentagem de progresso da meta</b></td> 
   <td><b>Cor da barra de porcentagem concluída</b></td> 
   <td><b>Ícone do indicador de condição</b></td> 
  </tr> 
  <tr> 
   <td>Novo(a)</td> 
   <td> <p>A meta é recém-criada e ainda não está registrando o progresso. Um progresso da meta é exibido como Novo até que alguém atualize seu progresso pela primeira vez. </p> <p>Para obter informações sobre como atualizar o progresso da meta, consulte <a href="../../workfront-goals/goal-review-and-workfront-goals-sections/check-in-goals.md" class="MCXref xref">Atualizar progresso da meta nas Metas do Adobe Workfront</a>.</p> </td> 
   <td>Nenhuma porcentagem</td> 
   <td>Sem barra</td> 
   <td><img src="assets/new-goal-icon-condition.png" alt="new_goal_icon_condition.png"></td>
  </tr> 
  <tr> 
   <td> <p><span>No Destino</span> </p> </td> 
   <td>A meta está funcionando como esperado e há uma grande probabilidade de ser concluída a tempo. </td> 
   <td>90-100%</td> 
   <td>Verde</td> 
    <td><img src="assets/on-target-icon-condition.png" alt="on_target_icon_condition.png"></td>
  </tr> 
  <tr> 
   <td> <p><span>Em Risco</span> </p> </td> 
   <td>A meta está atrasada, mas ainda pode ser possível concluí-la no prazo. </td> 
   <td>70-89,99%</td> 
   <td>Amarelo</td>
   <td><img src="assets/at-risk-icon-condition.png" alt="at_risk_icon_condition.png"></td> 
  </tr> 
  <tr> 
   <td> <p><span>Com Problemas</span> </p> </td> 
   <td> <p>É muito provável que a meta não seja concluída a tempo. </p> </td> 
   <td>0-69,99%</td> 
   <td>Vermelho</td> 
   <td><img src="assets/in-trouble-icon-condition.png" alt="in_problem_icon_condition.png"></td> 
  </tr> 
 </tbody> 
</table>