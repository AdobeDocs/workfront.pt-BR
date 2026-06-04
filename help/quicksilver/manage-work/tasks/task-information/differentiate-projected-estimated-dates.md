---
content-type: overview
product-area: projects
navigation-topic: task-information
title: Visão geral das datas projetadas e estimadas
description: Há vários tipos de datas que mostram a linha do tempo de tarefas entre o momento em que elas podem ser iniciadas e o momento em que podem ser concluídas.
author: Alina
feature: Work Management
exl-id: 7cc68fc4-5f79-4ce6-a404-737ea8959ec3
TQID: https://experienceleague.adobe.com/H-lO-an4TrEuwNx-l76JFpACJfyM22g36F3pa3aP6EY
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
subfeature_v2: id: b91c0848-76c4-4da4-8b81-3aade0518dd0id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 925
ht-degree: 1%

---

# Visão geral das datas projetadas e estimadas

<!--Audited: 07/2024-->

Há vários tipos de datas que mostram a linha do tempo de tarefas entre o momento em que elas podem ser iniciadas e o momento em que podem ser concluídas. Estas são algumas datas que exibem a linha do tempo de tarefas:

* Datas de Início Planejadas e de Término Planejadas
* Início Projetado e Datas de Término Projetadas
* Datas de Início e Vencimento Estimadas
* Início Efetivo e Datas de Término Efetivo

Este artigo descreve as diferenças entre as Datas estimadas e projetadas dos projetos.

Quando a tarefa é criada pela primeira vez, as Datas Planejadas, Projetadas e Estimadas normalmente devem corresponder. Existem algumas exceções.

Para obter mais informações sobre as datas de projeto, tarefa e problema no Adobe Workfront, consulte [Visão geral das datas de projeto, tarefa e problema no Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/definitions-pti-dates.md).

## Visão Geral das Datas Planejadas

As Datas planejadas são as datas que o Proprietário do projeto define como as datas de início e término das tarefas. Você ou o Proprietário do projeto podem modificar manualmente as Datas planejadas em uma tarefa.

## Visão Geral das Datas Reais

Quando uma tarefa é criada pela primeira vez, ela não tem Datas Reais porque ainda não foi iniciada ou concluída.

## Visão geral das datas projetadas e estimadas

Durante a vida útil de um projeto, as Datas projetada e estimada estão mais alinhadas com a realidade do projeto, pois levam em consideração o que pode influenciar o início e o fim reais de uma tarefa. Isso faz com que elas mudem das Datas planejadas.

Considere o seguinte ao trabalhar com Datas projetadas e estimadas em tarefas:

* Não é possível modificar manualmente as Datas estimadas nem as Datas projetadas das tarefas. Ambos são calculados pela Adobe Workfront.
* Ao criar uma tarefa, as datas Projetado e Estimado devem ser idênticas e devem ilustrar os horários reais em que as tarefas podem começar ou terminar.\
  Certas atualizações feitas nas tarefas afetam diretamente os valores das Datas Projetada e Estimada.

  Por exemplo, se o usuário iniciar ou concluir uma tarefa, a tarefa exibirá as Datas de Início e Término Reais, que influenciam as Datas Projetada e Estimada da tarefa. Além disso, se um designado na tarefa modificar a Data de confirmação, essa data influenciará a Data projetada da tarefa.

## Diferença entre Datas Projetadas e Estimadas

A diferença entre as Datas Projetada e Estimada é:

* As Datas projetadas são afetadas por um usuário que faz as seguintes atualizações na tarefa:

   * Adicionar uma Data de Restrição adicionando uma Restrição de Tarefa fixa
   * Adicionar uma data de compromisso

* As Datas estimadas consideram apenas o progresso real em uma tarefa em um determinado momento.

**Exemplo:** se tivermos uma tarefa com Data de Início Planejada para 20 de setembro e Data de Término Planejada para 24 de setembro, e ela tiver Data de Término Planejada em Restrição, a Data de Término Projetada para 24 de setembro. Esta tarefa tem uma duração de 4 dias.

A Data de conclusão estimada é calculada com base no progresso atual do trabalho na tarefa. Portanto, se hoje for 23 de setembro e a tarefa ainda não tiver sido iniciada, a Data de conclusão estimada será 27 de setembro (ela deve ser concluída após 4 dias, supondo que o trabalho seja iniciado hoje).

Se a tarefa estiver 50% concluída hoje, a Data de conclusão estimada será em 25 de setembro (ela deve ser concluída após 2 dias, que é a metade da Duração da tarefa).


### Entender quando as Datas Projetadas são atualizadas em tarefas {#understand-when-projected-dates-update-on-tasks}

As Datas Projetadas podem corresponder a outras datas de tarefa ou são um cálculo feito pela Workfront que leva em consideração o progresso real da tarefa.

A lista a seguir exibe vários cenários quando as Datas Projetadas das tarefas são alteradas durante a vida útil de um projeto, dependendo do que acontece na vida real com a tarefa:

* Quando uma tarefa está marcada como Concluída:

  `Projected Dates = Estimated Dates = Actual Dates`

* Quando uma tarefa tem uma Data de Início Efetivo:

  `Projected Start Date = Estimated Start Date = Actual Start Date`

* Quando uma tarefa não tem uma Data Inicial Real, mas há uma restrição forçada na Data Inicial Planejada (Deve Iniciar em) que está no futuro:

  `Projected Start Date = Constraint Date`

  Para obter informações sobre a Data de Restrição, consulte [Glossário da terminologia do Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

* Quando uma tarefa não tem uma Data de Início Efetivo e a tarefa não tem uma data de restrição forçada:

  `Projected Start Date = the next available date in the future that falls within working schedule`

* Quando o destinatário atualizar a Data de confirmação:

  `Projected Completion Date = Commit Date`

  Para obter informações sobre a Data de Confirmação, consulte [Visão geral da Data de Confirmação](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md).

* Quando a tarefa não tiver uma Data de Confirmação atualizada e a tarefa tiver uma restrição forçada (Deve Ser Concluída Em) para a Data de Conclusão Planejada que estiver no futuro:

  `Projected Completion Date = Constraint Date`

* Quando uma tarefa não tiver uma Data de Compromisso atualizada, uma data de restrição forçada no futuro ou tiver uma Data de Restrição no passado:

  `Projected Completion Date = system calculation for the Completion Date based on the current progress and the work left to be done`

### Entenda quando as Datas estimadas são atualizadas nas tarefas {#understand-when-the-estimated-dates-update-on-tasks}

Em comparação com os cenários descritos acima para as Datas projetadas, as Datas estimadas sempre refletem a análise real da Workfront de quando a tarefa será iniciada ou concluída, independentemente das Datas de restrição ou confirmação.

## O que influencia a linha do tempo de uma tarefa

Veja a seguir alguns exemplos do que pode influenciar a linha do tempo real de uma tarefa:

* Progresso da tarefa em relação às Datas Planejadas e ao dia atual
* Porcentagem concluída da tarefa até o momento
* Relação predecessora
* Progresso anterior
* Alocação de usuários

  >[!NOTE]
  >
  >A alocação de usuários pode influenciar a Data de conclusão estimada de uma tarefa se eles afetarem a velocidade com que a tarefa pode ser concluída. Por exemplo, se o Tipo de duração da tarefa for Orientado pelo Esforço, você poderá tornar a tarefa concluída mais cedo adicionando atribuídos. Como resultado, a Data de conclusão estimada muda.
