---
content-type: overview
product-area: projects
navigation-topic: task-information
title: Diferenciar entre datas projetadas e estimadas
description: Há vários tipos de datas que mostram a linha do tempo das tarefas entre quando elas podem iniciar e quando podem concluir.
author: Alina
feature: Work Management
exl-id: 7cc68fc4-5f79-4ce6-a404-737ea8959ec3
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '996'
ht-degree: 0%

---

# Diferenciar entre datas projetadas e estimadas

Há vários tipos de datas que mostram a linha do tempo das tarefas entre quando elas podem iniciar e quando podem concluir. 

A seguir estão algumas datas que exibem a linha do tempo das tarefas:

* Datas de Início e Conclusão Planejadas
* Datas de início e conclusão previstas
* Datas Estimadas de Início e Vencimento Estimadas
* Datas de início e conclusão reais

Este artigo descreve as diferenças entre as Datas estimada e prevista dos projetos. Quando a tarefa é criada pela primeira vez, as Datas Planejada, Projetada e Estimada normalmente devem corresponder. Existem algumas exceções. 

Para obter mais informações sobre o projeto, a tarefa e as datas de edição no Adobe Workfront, consulte [Visão geral do projeto, tarefa e datas de ocorrência no Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/definitions-pti-dates.md).

## Visão geral das datas planejadas

As Datas Planejadas são as datas que o Proprietário do Projeto define como as datas inicial e final das tarefas. 

Você ou o Proprietário do projeto podem modificar manualmente as Datas planejadas em uma tarefa.

## Visão geral das datas reais

Quando uma tarefa é criada pela primeira vez, ela não tem Datas reais, pois ainda não foi iniciada nem concluída.

## Visão geral das datas projetadas e estimadas

Durante a vida de um projeto, as Datas Projetadas e Estimadas estão mais de acordo com a realidade do projeto, pois levam em conta o que pode influenciar o início e o fim real de uma tarefa. Isso faz com que eles mudem das Datas Planejadas.

Considere o seguinte ao trabalhar com datas projetadas e estimadas em tarefas:

* Não é possível modificar manualmente as Datas Estimadas ou Projetadas das tarefas. Ambos são calculados pela Adobe Workfront.
* Ao criar uma tarefa, as datas Projetado e Estimado devem ser idênticas e devem ilustrar os horários reais em que as tarefas podem iniciar ou terminar.\
   Certas atualizações feitas em tarefas afetam diretamente os valores das Datas Projetada e Estimada. 

   Por exemplo, se o usuário iniciar ou concluir uma tarefa, ela exibirá Datas de Início e Conclusão Reais que influenciam as Datas Projetada e Estimada da tarefa. Além disso, se um destinatário na tarefa modificar a Data de confirmação, essa data influenciará a Data de projeção da tarefa.

## Diferença entre datas projetadas e estimadas

A diferença entre Datas Projetadas e Estimadas é:

* As Datas projetadas são afetadas por um usuário que faz as seguintes atualizações na tarefa:

   * Adicionar uma Data de Restrição adicionando uma Restrição de Tarefa fixa
   * Adicionar uma Data de Confirmação

* As Datas estimadas levam em consideração apenas o progresso real em uma tarefa em um determinado ponto no tempo.

**Exemplo:** Se tivermos uma tarefa que tenha uma Data de Início Planejada de 20 de setembro e uma Data de Conclusão Planejada de 24 de setembro, e tiver que Concluir na Restrição, a Data de Conclusão Projetada de 24 de setembro. Esta tarefa tem uma Duração de 4 dias.

A Data Estimada de Conclusão é calculada com base no progresso atual do trabalho na tarefa. Portanto, se hoje for 23 de setembro e a tarefa ainda não tiver sido iniciada, a Data de Conclusão Estimada será 27 de setembro (deverá ser concluída após 4 dias, supondo que o trabalho tenha sido iniciado hoje).

Se a tarefa estiver 50% concluída hoje, a Data de conclusão estimada será em 25 de setembro (ela deverá ser concluída após 2 dias, que é a metade da Duração da tarefa).

* [Entender quando as Datas Projetadas são atualizadas nas tarefas](#understand-when-projected-dates-update-on-tasks)
* [Entender quando as Datas estimadas são atualizadas nas tarefas](#understand-when-the-estimated-dates-update-on-tasks)

### Entender quando as Datas Projetadas são atualizadas nas tarefas {#understand-when-projected-dates-update-on-tasks}

As Datas Projetadas podem corresponder a outras datas de tarefa ou são um cálculo feito pela Workfront que leva em consideração o progresso da vida real da tarefa.

A lista a seguir exibe vários cenários quando as Datas projetadas das tarefas são alteradas durante a vida de um projeto, dependendo do que acontece na vida real à tarefa:

* Quando uma tarefa é marcada como Concluída:

   *Datas Projetadas = Datas Estimadas = Datas Reais*

* Quando uma tarefa tem uma Data de Início Real:

   *Data Inicial Projetada = Data Inicial Estimada = Data Inicial Real*

* Quando uma tarefa não tiver uma Data de Início Real, mas houver uma restrição forçada na Data de Início Planejada (Deve Iniciar Em) que esteja no futuro:

   *Data Inicial Projetada = Data da Restrição*

   Para obter informações sobre a Data da Restrição, consulte [Glossário da terminologia do Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

* Quando uma tarefa não tiver uma Data de Início Real e a tarefa não tiver uma data de restrição forçada:

   *Data Inicial Projetada = a próxima data disponível no futuro que se enquadra no cronograma de trabalho*

* Quando o destinatário atualiza a Data da confirmação:

   *Data de Conclusão Projetada = Data de Confirmação*

   Para obter informações sobre a Data da Confirmação, consulte [Visão geral da data de confirmação](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md).

* Quando a tarefa não tiver uma Data de Confirmação atualizada e tiver uma restrição forçada (Deve Concluir em) para a Data de Conclusão Planejada que está no futuro:

   *Data de Conclusão Projetada = Data de Restrição*

* Quando uma tarefa não tiver uma Data de Confirmação atualizada, uma data de restrição forçada no futuro ou tiver uma Data de Restrição no passado:

   *Data de Conclusão Projetada = cálculo do sistema para a Data de Conclusão com base no progresso atual e no trabalho a ser feito*

### Entender quando as Datas estimadas são atualizadas nas tarefas {#understand-when-the-estimated-dates-update-on-tasks}

Em comparação com os cenários descritos acima para as Datas Projetadas, as Datas Estimadas sempre refletem a análise real da Workfront de quando a tarefa será iniciada ou concluída independentemente das Datas de Restrição ou Confirmação.

## O que influencia a linha do tempo de uma tarefa

A seguir estão alguns exemplos do que pode influenciar a linha do tempo real de uma tarefa: 

* progresso da tarefa em relação às Datas Planejadas e ao dia atual
* porcentagem concluída da tarefa até o momento
* relação antecessora
* progresso do antecessor
* alocação de usuários

   >[!NOTE]
   >
   >A alocação do usuário pode influenciar a Data estimada de conclusão de uma tarefa se afetar a velocidade com que a tarefa pode ser concluída. Por exemplo, se o Tipo de duração da tarefa for Orientado ao esforço, você poderá concluir a tarefa mais cedo adicionando destinatários. Como resultado, a Data estimada de conclusão é alterada.
