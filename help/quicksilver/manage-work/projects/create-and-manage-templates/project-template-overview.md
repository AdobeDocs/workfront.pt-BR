---
product-area: templates
navigation-topic: templates-navigation-topic
title: Visão geral do modelo de projeto
description: Você pode usar modelos de projeto para capturar a maioria dos processos, informações e configurações repetíveis associados aos projetos em sua organização.
author: Alina
feature: Work Management
exl-id: cac7662f-f2ae-44f0-a0bb-1569c03d172e
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '613'
ht-degree: 1%

---

# Visão geral do modelo de projeto

Você pode usar modelos de projeto para capturar a maioria dos processos, informações e configurações repetíveis associados aos projetos em sua organização.

Você pode definir tarefas, tópicos de fila, formulários personalizados, anexar documentos ao seu modelo.

Depois de criar modelos, você pode anexá-los a projetos existentes ou usá-los para criar novos projetos. Todas as informações no modelo são transferidas para os projetos criados usando ele.

## Benefícios do uso de modelos no Adobe Workfront

Estes são alguns dos benefícios de usar modelos para criar seus projetos:

* Ele economiza tempo e esforço ao criar novos projetos que são repetitivos.
* Você tem informações consistentes em todos os projetos que são semelhantes em escopo.
* Isso é útil ao criar relatórios sobre projetos. Por exemplo, é possível criar relatórios sobre projetos que compartilham o mesmo modelo, comparar o progresso e encontrar melhorias na maneira como eles poderiam ser concluídos.
* Além de definir as configurações futuras do projeto, você pode adicionar as seguintes informações para o projeto futuro em um modelo:

   * Tarefas
   * Documentos
   * Aprovações
   * Detalhes da fila
   * Enfileirar tópicos
   * Grupos de tópicos
   * Regras de Encaminhamento
   * Forms personalizada
   * Informações da empresa e do grupo

## Práticas recomendadas para criação de modelos

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:this is not an extensive list, but we are updating it as we go.)</p>
-->

Considere o seguinte ao criar modelos:

* Não atribuir usuários a tarefas de modelo. Embora seja possível deixar as tarefas desatribuídas, recomendamos que você atribua funções de trabalho a tarefas. Isso lhe dará uma ideia de quais usuários podem ser atribuídos às tarefas ao criar o projeto usando o modelo .
* Sempre dê às suas tarefas de modelo um valor de Duração e Horas Planejadas . Cada tarefa no projeto deve ser associada a uma duração de quanto tempo a tarefa pode permanecer aberta e a um valor de Hora planejada por quanto tempo realmente levará para que a tarefa seja concluída. As tarefas sem essas informações não podem ser orçamentadas corretamente para recursos ao usar ferramentas de gerenciamento de recursos no Workfront.

   Para obter informações sobre a Duração, consulte os seguintes artigos:

   * [Visão Geral da Duração da Tarefa e do Tipo de Duração](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md)
   * [Visão geral da duração do projeto](../../../manage-work/projects/planning-a-project/project-duration.md)

   Para obter informações sobre Horas Planejadas, consulte [Visão geral das Horas Planejadas](../../../manage-work/tasks/task-information/planned-hours.md).

* Adicione as relações do antecessor entre as tarefas no final, quando você tiver uma compreensão clara do futuro plano de projeto em sua totalidade. Adicionar predecessores às tarefas do modelo é semelhante a adicionar predecessores às tarefas em um projeto.

   Para obter informações sobre como adicionar predecessores às tarefas, consulte [Visão geral dos antecessores de tarefas](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

* Indique com quem o modelo deve ser compartilhado para uso futuro e com quem os projetos que serão criados a partir do modelo devem ser compartilhados. Para obter informações sobre compartilhamento de modelos, consulte [Compartilhar modelos de projeto](../../../manage-work/projects/create-and-manage-templates/share-project-template.md).
* Use processos de aprovação global e adicione-os às tarefas do modelo e do modelo, se possível. Isso economizará tempo quando as tarefas ou o projeto futuro precisarem passar pelas mesmas aprovações.

   Para obter informações sobre como criar aprovações, consulte [Criar um processo de aprovação para itens de trabalho](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

   Para obter informações sobre como associar um processo de aprovação a um item de trabalho, consulte [Associar um processo de aprovação novo ou existente ao trabalho](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).

## Formas de criar modelos

Você pode criar um novo template das seguintes maneiras:

* Do zero.\
   Para obter mais informações sobre como criar um novo modelo do zero, consulte [Criar um modelo de projeto](../../../manage-work/projects/create-and-manage-templates/create-template.md).

* A partir de projetos existentes, salvando um projeto como modelo.\
   Para obter mais informações sobre como criar modelos a partir de projetos existentes, consulte [Criar modelo a partir do projeto](../../../manage-work/projects/create-and-manage-templates/create-template-from-project.md).

* Copiando de outro modelo.\
   Para obter mais informações sobre cópia de um modelo existente, consulte [Copiar um modelo de projeto](../../../manage-work/projects/create-and-manage-templates/copy-template.md).

* Usando nossos modelos de exemplo.\
   Para obter mais informações sobre como criar seus modelos usando nossos modelos de exemplo, consulte [Criar modelos de projeto a partir de exemplos](../../../manage-work/projects/create-and-manage-templates/create-templates-from-examples.md).
