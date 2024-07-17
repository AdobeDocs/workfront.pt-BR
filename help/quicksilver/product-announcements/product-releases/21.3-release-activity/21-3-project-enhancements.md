---
title: 21.3 Aprimoramentos do projeto
description: 21.3 Aprimoramentos do projeto
author: Luke
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 1df4ccdb-5b74-414c-a622-b0a5ed30a8c4
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '1129'
ht-degree: 0%

---

# 21.3 Aprimoramentos do projeto

Esta página descreve todas as melhorias feitas no Project com a versão 21.3 para o ambiente de Pré-visualização. Essas melhorias foram disponibilizadas no ambiente de Produção na semana de 21 de julho de 2021.

Para obter uma lista de todas as alterações disponíveis com a versão 21.3, consulte a [Visão geral da versão 21.3](../../../product-announcements/product-releases/21.3-release-activity/21-3-release-overview.md).

## Associar um modelo a um grupo

>[!NOTE]
>
>Esse recurso está disponível somente na nova experiência do Adobe Workfront.

Para ajudar você a simplificar o processo de criação de projetos e identificar e relatar com mais facilidade quais grupos são proprietários de cada modelo de projeto, adicionamos a capacidade de atribuir um grupo a um modelo de projeto.

Quando você atribui um grupo a um modelo de projeto, todos os projetos criados a partir do modelo são automaticamente associados ao grupo do modelo. Para obter mais informações, consulte [Editar modelos de projeto](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).

Além disso, você pode anexar um processo de aprovação de grupo a um modelo e suas tarefas de modelo se o modelo estiver associado ao seu grupo. Para obter mais informações, consulte [Associar um processo de aprovação novo ou existente a um trabalho](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).

## Edição mais fácil de campos na seção Detalhes

>[!NOTE]
>
>Esse recurso está disponível somente na nova experiência do Adobe Workfront.

As seguintes melhorias permitem editar mais facilmente as informações na seção Detalhes de qualquer objeto:

* Um contorno cinza ao redor de um campo, ao passar o mouse sobre ele, indica que ele é editável.
* Você pode editar campos clicando neles uma vez.

Antes desse aprimoramento, não estava claro quais campos eram editáveis e você tinha que clicar duas vezes para editar um campo.

## Considerar predecessoras entre projetos ao calcular datas de entrega

Com uma nova melhoria na maneira como o Adobe Workfront calcula datas de entrega para tarefas, as dependências entre projetos agora são consideradas.

Anteriormente, as datas de transferência eram calculadas com base apenas nos predecessores da tarefa no mesmo projeto.

Agora, para garantir que você sempre tenha uma data de entrega precisa para uma tarefa com um predecessor de projeto cruzado, você deve recalcular a linha do tempo do projeto da tarefa sucessora. Depois de recalcular a linha do tempo, as datas de entrega da tarefa são calculadas levando em conta as dependências entre projetos das tarefas.

Para obter mais informações sobre datas de transferência, consulte [Visão geral da Data de Transferência da Tarefa](../../../manage-work/tasks/task-information/handoff-task-date.md).

## Adicionar histórias e problemas existentes do quadro Scrum

>[!NOTE]
>
>Esse recurso está disponível somente na nova experiência do Adobe Workfront.

Agora é possível adicionar uma história ou problema existente diretamente do quadro Scrum. Isso facilita adicionar histórias existentes à iteração atual sem precisar ir para a página de backlog.

Para obter mais informações, consulte [Adicionar histórias e problemas do quadro Scrum](../../../agile/use-scrum-in-an-agile-team/scrum-board/add-story-from-scrum-board.md).

## Adicione novas histórias e problemas do quadro Scrum

>[!NOTE]
>
>Esse recurso está disponível somente na nova experiência do Adobe Workfront.

Agora você pode criar uma nova história ou problema diretamente do quadro Scrum. Isso facilita adicionar rapidamente uma nova história à iteração atual.

Para obter mais informações, consulte [Adicionar histórias e problemas do quadro Scrum](../../../agile/use-scrum-in-an-agile-team/scrum-board/add-story-from-scrum-board.md).

## Excluir história ou problema do quadro Kanban

>[!NOTE]
>
>Esse recurso está disponível somente na nova experiência do Adobe Workfront.

Agora é possível excluir uma história ou problema diretamente do quadro Kanban, clicando no ícone Mais em uma história ou cartão de problema e selecionando Excluir. Ao excluir uma história ou problema, ele é movido para a Lixeira por 30 dias e pode ser recuperado somente pelo administrador do sistema.

Para obter mais informações, consulte [Excluir histórias ou problemas do quadro Kanban](../../../agile/use-kanban-in-an-agile-team/delete-story-from-kanban-board.md).

## Atualizações do cabeçalho do cartão Agile e do storyboard

>[!NOTE]
>
>Esse recurso está disponível somente na nova experiência do Adobe Workfront.

Nos quadros Kanban e Scrum, as seguintes melhorias estão disponíveis:

* Os cartões de história e as colunas do quadro têm uma largura fixa, de modo que os tamanhos dos cartões não serão alterados se você ajustar o tamanho da janela do navegador.
* A coluna Histórias foi renomeada para História principal.
* Cada cartão tem um rótulo na parte superior para identificá-lo como uma matéria principal, subtarefa (associada a uma matéria principal), matéria (não associada a uma matéria principal) ou ocorrência.
* O sombreamento do plano de fundo separa visualmente as colunas.

Para obter mais informações, consulte [Visão geral das iterações](../../../agile/use-scrum-in-an-agile-team/iterations/iterations-overview.md).

## Preferências de projetos, tarefas e problemas do grupo

Conforme comunicamos anteriormente, implantamos personalizações em nível de grupo para preferências de projeto, tarefa e problema nas fases que antecedem 24 de junho de 2021. Agora a implantação foi concluída e elas estão disponíveis na Produção para todos os clientes.

Para obter mais informações, consulte os seguintes artigos:

* [Configurar preferências de projeto para um grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md)
* [Configurar preferências de tarefas e problemas para um grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md)

## Permitir que usuários externos aprovem um documento

>[!NOTE]
>
>Esse recurso está disponível somente na nova experiência do Adobe Workfront.

Agora você pode usar endereços de email externos para atribuir aprovadores a um documento na nova experiência do Workfront.

Anteriormente, só era possível adicionar usuários externos por endereço de email no Workfront Classic.

Para obter mais informações, consulte [Solicitar aprovações de documentos](../../../review-and-approve-work/manage-approvals/request-document-approvals.md).

## Exportar informações da seção Detalhes de um portfólio ou programa

>[!NOTE]
>
>Esse recurso foi lançado no ambiente de Pré-visualização em 20 de maio de 2021. Ele será lançado no ambiente de Produção em 3 de junho de 2021.

>[!NOTE]
>
>Esse recurso está disponível somente na nova experiência do Adobe Workfront.

Agora é possível exportar para um arquivo .pdf as informações da seção Detalhes de portfólios e programas. Antes desse aprimoramento, você poderia exportar informações da seção Detalhes somente de projetos, tarefas e problemas.

Para obter informações sobre como exportar formulários personalizados de um objeto, consulte [Exportar formulários personalizados e detalhes do objeto](../../../workfront-basics/work-with-custom-forms/export-custom-forms-details.md).

## Adição do carimbo de data e hora da Data de conclusão planejada no cabeçalho do objeto

>[!NOTE]
>
>Esse recurso está disponível somente na nova experiência do Adobe Workfront.

Para facilitar o acesso fácil, a conveniência e a precisão, adicionamos a opção de selecionar um carimbo de data e hora na Data de conclusão planejada do cabeçalho de projetos, tarefas ou problemas.

Antes dessa melhoria, quando você atualizava a Data de conclusão planejada de um objeto, a Workfront selecionava meia-noite como o horário padrão. Agora, você pode personalizar a hora, bem como a data de conclusão.

Para obter informações sobre os cabeçalhos de objetos na nova experiência do Workfront, consulte [Novos cabeçalhos de objetos](../../../workfront-basics/the-new-workfront-experience/new-object-headers.md).

## Adicionar um formulário personalizado a um objeto sem editá-lo

>[!NOTE]
>
>Esse recurso está disponível somente na nova experiência do Adobe Workfront.

Facilitamos a adição de um formulário personalizado que outra pessoa preencherá, ou que você preencherá posteriormente, a um objeto. O formulário não entra mais no modo de edição automaticamente quando adicionado. Você pode simplesmente salvar o formulário vazio no objeto.

Anteriormente, ao adicionar um formulário personalizado a um objeto, a página entrava no modo de edição e você tinha que preencher todos os campos obrigatórios no formulário antes de salvá-lo no objeto. Isso era inconveniente quando o formulário deveria ser preenchido por outro usuário ou quando você ainda não sabia o que colocar em um campo obrigatório no formulário.

Para obter informações sobre como adicionar um formulário personalizado a um objeto, consulte [Adicionar um formulário personalizado a um objeto](../../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

