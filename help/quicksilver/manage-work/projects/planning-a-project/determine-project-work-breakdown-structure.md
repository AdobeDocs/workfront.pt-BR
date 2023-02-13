---
product-area: projects
navigation-topic: plan-a-project
title: Determinar a estrutura de detalhamento de trabalho em um projeto
description: Definir uma Estrutura de Detalhamento de Trabalho (WBS) para um projeto é um conjunto de atividades que, em última análise, delineia o plano do projeto. A WBS divide o resultado do projeto em elementos de trabalho gerenciáveis, que podem ser usados para definir marcos e organizar atribuições de trabalho.
author: Alina
feature: Work Management
exl-id: a76c468d-6373-4dab-93ff-a0b3734f368c
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '1737'
ht-degree: 1%

---

# Determinar a estrutura de detalhamento de trabalho em um projeto

Definir uma Estrutura de Detalhamento de Trabalho (WBS) para um projeto é um conjunto de atividades que, em última análise, delineia o plano do projeto. A WBS divide o resultado do projeto em elementos de trabalho gerenciáveis, que podem ser usados para definir marcos e organizar atribuições de trabalho.

Você deve ter uma licença do Plano com Editar acesso a Projetos para criar a Estrutura de Detalhamento do Trabalho de um projeto. Pode ser necessário acesso adicional a outras áreas do Adobe Workfront, dependendo de quantas atividades você executa ao criar a WBS.

Recomendamos que você mantenha o projeto em um status de Planejamento enquanto faz alterações na Estrutura de Detalhamento do Trabalho, para evitar notificações para acionar usuários na Equipe do Projeto.

## Definir os resultados do projeto

O objetivo de um projeto é fornecer resultados tangíveis às partes interessadas internas e externas. Os resultados de um projeto são os que você deseja alcançar ao concluir o projeto. Os resultados estão quase sempre associados a pelo menos um deliverables, e todos os deliverables devem ser associados a um projeto.

Os resultados do projeto podem ser bens de consumo, produção intelectual (como relatórios) ou serviços. Por exemplo, se o escopo do projeto for criar uma casa, alguns dos produtos podem incluir:

* criação de planos de arquitetura
* conclusão da canalização
* trabalhos elétricos
* derramamento da fundação
* trabalho de enquadramento
* fechando a venda da casa.

Dependendo do tamanho e do escopo, um projeto pode ser composto de vários deliveries.

Depois de identificar os resultados, você pode começar a dividi-los em tarefas. As tarefas são o resultado alcançado para fornecer o resultado geral do projeto. Ao definir suas tarefas, você considera os seguintes parâmetros:

* Tempo necessário para conclusão.
* Orçamento necessário para completar o trabalho.
* Os recursos necessários para concluir o trabalho.
* Agendamento dos recursos com base na linha do tempo lógico das tarefas.

Conforme você define tarefas, certifique-se de não planejar muito trabalho para uma tarefa individual. Se o trabalho necessário em uma tarefa for superior a 40 horas (uma semana de trabalho típica), talvez seja necessário dividir essa quantidade de trabalho em subtarefas. A conclusão de todas as subtarefas concluirá a tarefa principal.

Para definir os resultados e resultados da WBS no Workfront, recomendamos que você execute as seguintes atividades para criar uma exibição hierárquica das tarefas do projeto:

* Se ainda não tiver feito isso, crie um novo projeto.\
   Para obter informações sobre como criar um projeto, consulte o artigo [Criar um projeto](../../../manage-work/projects/create-projects/create-project.md).

* Crie tarefas para todos os itens de ação necessários para concluir cada resultado e entregável.\
   Para obter informações sobre como criar tarefas, consulte o artigo [Criar tarefas em um projeto](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md) .

* A partir das tarefas que você acabou de criar, identifique quais são resultados importantes e associe-os aos marcos.\
   Para obter informações sobre como criar tarefas de marco, consulte os artigos [Criar um caminho de marco](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md) e [Associar marcos a tarefas](../../../manage-work/tasks/manage-tasks/associate-milestones-with-tasks.md).

* Analise as tarefas com um escopo muito grande em subtarefas. Associe-os ao pai que define seu delivery .\
   Para obter informações sobre como criar subtarefas, consulte o artigo [Criar subtarefas](../../../manage-work/tasks/create-tasks/create-subtasks.md).

* Identificar relacionamentos de dependência entre subtarefas e entre etapas.\
   Em um relacionamento de dependência, o início de uma tarefa depende da conclusão de outra tarefa ou grupo de tarefas.\
   Para obter informações sobre dependências de tarefas, consulte os artigos [Visão geral dos antecessores de tarefas](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md) e [Criar uma relação de antecessor na lista de tarefas](../../../manage-work/tasks/use-prdcssrs/create-predecessors-on-task-list.md).

* Determine se, em qualquer ponto da vida útil do projeto, são necessárias aprovações e revisões. Crie processos de aprovação para atender a essa necessidade.\
   Para obter informações sobre aprovações, consulte o artigo [Criar um processo de aprovação para itens de trabalho](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

## Estimar programação de trabalho e restrições de programação

Depois de criar o marco básico e a estrutura de tarefas do projeto, você pode estimar o tempo que levará para concluir o projeto geral definindo as restrições e durações da tarefa.

Considere o seguinte:

* As restrições de tarefa definem quando o trabalho em uma tarefa deve começar ou terminar.

   Para obter informações sobre como definir restrições de tarefa, consulte o artigo [Visão geral da restrição de tarefa](../../../manage-work/tasks/task-constraints/task-constraint-overview.md).

* A Duração de uma tarefa é o período disponível para concluir uma tarefa. Ao estimar a Duração, convém inserir um valor que considere a possibilidade de um atraso. Se projetos semelhantes tiverem sido concluídos no passado, você pode ter uma boa ideia de onde definir esse valor.

   Como a duração é uma estimativa, certifique-se de definir valores de tempo otimistas para levar em conta fatores que podem afetar a tarefa, como tempo, falta de energia, dificuldades do fornecedor ou outros eventos imprevistos. Além disso, considere se há algum antecessor associado ou tarefas de dependência e como eles podem colocar restrições no trabalho e afetar a conclusão da tarefa.

   Dependendo do Tipo de duração da tarefa, é possível modificar a duração de uma tarefa durante a vida útil de um projeto, mas isso também afetará a linha do tempo do projeto. Para obter informações sobre a Duração de uma tarefa, consulte o artigo [Visão Geral da Duração da Tarefa e do Tipo de Duração](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md) .

## Atribuir tarefas

Após definir a duração e as restrições de cada tarefa, você pode determinar quem tem o tempo e as habilidades para realizar o trabalho. Você pode atribuir tarefas às seguintes entidades no Workfront:

* Usuários\
   Somente usuários com nível de acesso do Planejador ou do Trabalhador podem ser atribuídos a tarefas. Embora você possa atribuir tarefas a Solicitantes e Revisores, eles não podem concluí-las. Por isso, não recomendamos atribuir tarefas a eles.

   Para obter informações sobre os níveis de acesso e como eles definem o que os usuários podem fazer com objetos Workfront, consulte [Visão geral dos níveis de acesso](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

* Função no trabalho
* Equipes

Para obter informações sobre como atribuir tarefas, consulte os artigos na seção [Atribuir tarefas](../../../manage-work/tasks/assign-tasks/assign-tasks-1.md) seção.

## Gerenciar recursos

O Gerenciamento de recursos no Workfront permite determinar se há equipe adequada para concluir o projeto. Quando os usuários são adicionados a um projeto, o Workfront mostra a utilização de cada usuário. Os Gerentes de Recursos podem ver o número total de horas em que a pessoa é atribuída a outros projetos durante o período do projeto.

>[!NOTE]
>
>Desde que o projeto tenha um status de Planejamento, as tarefas atribuídas aos usuários não aparecerão em suas listas de tarefas.

No início de um ano fiscal ou trimestre, você pode gerenciar seus recursos em um nível superior, em vários projetos, sem o conhecimento de uma estrutura específica de Detalhamento de trabalho.\
Para obter informações sobre o planejamento do uso de seus recursos em um nível superior, consulte o artigo [Introdução ao planejamento de recursos](../../../resource-mgmt/resource-planning/get-started-resource-planning.md).

Ao gerenciar os recursos no contexto da criação da Estrutura de Detalhamento do Trabalho de um projeto e garantir que cada tarefa seja atribuída ao recurso correto, você estará pronto para agendar os recursos para o trabalho que precisa ser feito.\
Para obter informações sobre como programar seus recursos, consulte os artigos na [Agendamento de recursos](../../../resource-mgmt/resource-scheduling/resource-scheduling-overview.md) seção.

## Estimativa das finanças dos projetos

A Workfront calculará os custos planejados para cada tarefa e os custos gerais de um projeto. Os custos planejados de uma tarefa incluem todas as despesas da tarefa mais o custo do funcionário ou da função atribuída à tarefa. As taxas por hora para a tarefa, a função e o funcionário são atribuídas durante a tarefa, a função e a criação do usuário.

Para obter informações sobre as finanças do projeto, consulte a seção [Finanças dos projetos](../../../manage-work/projects/project-finances/project-finances-overview.md) .

## Determinar pontos de aprovação do projeto

Ao criar Processos de aprovação no Workfront, é possível estabelecer pontos de revisão para o projeto a fim de monitorar o progresso e as possíveis áreas problemáticas. Por meio do processo de aprovação, os Proprietários do projeto podem discernir quais tarefas estão atrasadas e antecipadas, exibir trilhas de auditoria que listam quem alterou o status de uma tarefa e ver históricos de problemas, incluindo como os problemas foram resolvidos e quando foram fechados. Após revisar um projeto, os Proprietários do projeto podem determinar quais etapas tomar e atualizar o plano do projeto, se necessário.

Para obter informações sobre aprovações, consulte o artigo [Criar um processo de aprovação para itens de trabalho](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md)

## Exibir sua WBS

Para entender a WBS de um projeto, você deseja exibir os seguintes elementos de tarefa:

* Sequência de tarefas e linha do tempo (Datas de Início e Conclusão Planejadas e Duração da tarefa)
* Dependências do antecessor
* Relação filho e pai
* Atribuições

Após concluir a WBS, é possível exibi-la em uma lista de tarefas no nível do projeto ou em um relatório.

* [Exibir o WBS em uma lista de tarefas](#view-the-wbs-in-a-task-list)
* [Exibir o WBS em um relatório de tarefa](#view-the-wbs-in-a-task-report)

### Exibir o WBS em uma lista de tarefas {#view-the-wbs-in-a-task-list}

Você pode exibir a lista de tarefas no nível do projeto.

1. Vá para o projeto para o qual deseja ver a Estrutura de Detalhamento do Trabalho.
1. Selecione o **Tarefas** guia .
1. (Opcional) Selecione **Nada** no **Agrupamento** menu suspenso.

   A Estrutura de detalhamento de trabalho não exibe o recuo das tarefas na WBS.

1. No **Exibir** e selecione o **Detalhamento do trabalho** exibir.

   A estrutura de Detalhamento do trabalho é exibida na segunda coluna da exibição selecionada.

   ![](assets/wbs-view-on-task-list-nwe-350x87.png)

### Exibir o WBS em um relatório de tarefa {#view-the-wbs-in-a-task-report}

Você pode criar um relatório de tarefa e exibir o WBS das tarefas seguindo um destes procedimentos:

* Aplique a exibição da Estrutura de Detalhamento de Trabalho existente ao relatório.
* Adicione a coluna Estrutura de análise de trabalho a qualquer relatório personalizado.

>[!TIP]
>
>Recomendamos adicionar um grupo de projetos para esclarecer a quais projetos as tarefas pertencem. O recuo das tarefas não é exibido em um relatório de tarefa.

Para obter informações sobre como criar relatórios, consulte o artigo [Criar um relatório personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

## Salvar o WBS de um projeto como um modelo

Se você trabalhar em outros projetos que seguem agendamentos de trabalho semelhantes à WBS que acabou de criar, poderá salvar o projeto como um modelo. Um modelo economizará tempo e esforço ao criar projetos relacionados ao futuro.

Se sua organização tiver pouco faturamento, considere aguardar até que as atribuições de usuário sejam feitas para salvar o modelo. Independentemente de quando um projeto é salvo como modelo, atribuições de usuário ou tarefas específicas podem ser removidas durante a anexação do modelo a um novo projeto.

Os seguintes elementos de uma estrutura de detalhamento de trabalho podem ser salvos em um modelo, para uso futuro com outro projeto:

* Dependências do antecessor
* Atribuições (incluindo Proprietário do projeto, Patrocinador e Gerenciador de Recursos)
* Processos de Aprovação
* Restrições de tarefa
* Documentos
* Despesas e outras Informações Financeiras
* Metas
* Tipos de Hora
* Estrutura da fila de solicitações
* Notificações de Lembrete
* Riscos
* Preços
* Compartilhamento de informações
* Formulários personalizados

Para obter informações sobre como salvar projetos como modelos, consulte o artigo [Criar modelo a partir do projeto](../../../manage-work/projects/create-and-manage-templates/create-template-from-project.md) .
