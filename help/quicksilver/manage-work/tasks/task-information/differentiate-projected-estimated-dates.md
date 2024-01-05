---
content-type: overview
product-area: projects
navigation-topic: task-information
title: Diferenciar entre datas projetadas e estimadas
description: Há vários tipos de datas que mostram a linha do tempo de tarefas entre o momento em que elas podem ser iniciadas e o momento em que podem ser concluídas.
author: Alina
feature: Work Management
exl-id: 7cc68fc4-5f79-4ce6-a404-737ea8959ec3
source-git-commit: 8764de907f49260908911ca393c1173b66dbb065
workflow-type: tm+mt
source-wordcount: '991'
ht-degree: 0%

---

# Diferenciar entre datas projetadas e estimadas

Há vários tipos de datas que mostram a linha do tempo de tarefas entre o momento em que elas podem ser iniciadas e o momento em que podem ser concluídas. Estas são algumas datas que exibem a linha do tempo de tarefas:

* Datas de Início Planejadas e de Término Planejadas
* Início Projetado e Datas de Término Projetadas
* Datas de Início e Vencimento Estimadas
* Início Efetivo e Datas de Término Efetivo

Este artigo descreve as diferenças entre as Datas estimadas e projetadas dos projetos.

Quando a tarefa é criada pela primeira vez, as Datas Planejadas, Projetadas e Estimadas normalmente devem corresponder. Existem algumas exceções. 

Para obter mais informações sobre projeto, tarefa e datas de problemas no Adobe Workfront, consulte [Visão geral das datas de Projeto, Tarefa e Problema no Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/definitions-pti-dates.md).

## Visão Geral das Datas Planejadas

As Datas planejadas são as datas que o Proprietário do projeto define como as datas de início e término das tarefas. Você ou o Proprietário do projeto podem modificar manualmente as Datas planejadas em uma tarefa.

## Visão Geral das Datas Reais

Quando uma tarefa é criada pela primeira vez, ela não tem Datas Reais porque ainda não foi iniciada ou concluída.

## Visão Geral das Datas Projetadas e Estimadas

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

**Exemplo:** Se houver uma tarefa com uma Data de Início Planejada de 20 de setembro e uma Data de Conclusão Planejada de 24 de setembro e ela tiver a opção Precisa Ser Concluída na Restrição, a Data de Conclusão Projetada será 24 de setembro. Esta tarefa tem uma duração de 4 dias.

A Data de conclusão estimada é calculada com base no progresso atual do trabalho na tarefa. Portanto, se hoje for 23 de setembro e a tarefa ainda não tiver sido iniciada, a Data de conclusão estimada será 27 de setembro (ela deve ser concluída após 4 dias, supondo que o trabalho seja iniciado hoje).

Se a tarefa estiver 50% concluída hoje, a Data de conclusão estimada será em 25 de setembro (ela deve ser concluída após 2 dias, que é a metade da Duração da tarefa).


### Entender quando as Datas Projetadas são atualizadas em tarefas {#understand-when-projected-dates-update-on-tasks}

As Datas Projetadas podem corresponder a outras datas de tarefa ou são um cálculo feito pela Workfront que leva em consideração o progresso real da tarefa.

A lista a seguir exibe vários cenários quando as Datas Projetadas das tarefas são alteradas durante a vida útil de um projeto, dependendo do que acontece na vida real com a tarefa:

* Quando uma tarefa está marcada como Concluída:

  *Datas Projetadas = Datas Estimadas = Datas Reais*

* Quando uma tarefa tem uma Data de Início Efetivo:

  *Data Inicial Projetada = Data Inicial Estimada = Data Inicial Real*

* Quando uma tarefa não tem uma Data Inicial Real, mas há uma restrição forçada na Data Inicial Planejada (Deve Iniciar em) que está no futuro:

  *Data Inicial Projetada = Data de Restrição*

  Para obter informações sobre Data de Restrição, consulte [Glossário da terminologia do Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

* Quando uma tarefa não tem uma Data de Início Efetivo e a tarefa não tem uma data de restrição forçada:

  *Data Inicial Projetada = a próxima data disponível no futuro que se enquadra na programação de trabalho*

* Quando o destinatário atualizar a Data de confirmação:

  *Data de conclusão projetada = Data de confirmação*

  Para obter informações sobre a Data de confirmação, consulte [Visão geral da data de compromisso](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md).

* Quando a tarefa não tiver uma Data de Confirmação atualizada e a tarefa tiver uma restrição forçada (Deve Ser Concluída Em) para a Data de Conclusão Planejada que estiver no futuro:

  *Data de Término Projetada = Data de Restrição*

* Quando uma tarefa não tiver uma Data de Compromisso atualizada, uma data de restrição forçada no futuro ou tiver uma Data de Restrição no passado:

  *Data de Término Projetada = cálculo do sistema para a Data de Término com base no andamento atual e no trabalho a ser concluído*

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
