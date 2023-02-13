---
title: 21.3 Melhorias do projeto
description: 21.3 Melhorias do projeto
author: Luke
draft: Probably
feature: Product Announcements
exl-id: 1df4ccdb-5b74-414c-a622-b0a5ed30a8c4
source-git-commit: 665732453b33b49421108791a560ab84d51280b9
workflow-type: tm+mt
source-wordcount: '1122'
ht-degree: 0%

---

# 21.3 Melhorias do projeto

Esta página descreve todas as melhorias do projeto feitas com a versão 21.3 para o ambiente de Visualização. Esses aprimoramentos foram disponibilizados no ambiente de Produção na semana de 21 de julho de 2021.

Para obter uma lista de todas as alterações disponíveis com a versão 21.3, consulte [Visão geral da versão 21.3](../../../product-announcements/product-releases/21.3-release-activity/21-3-release-overview.md).

## Associar um modelo a um grupo

>[!NOTE]
>
>Esse recurso está disponível somente na nova experiência do Adobe Workfront.

Para ajudar você a simplificar o processo de criação do projeto, e para ajudá-lo a identificar e relatar mais facilmente quais grupos possuem quais modelos de projeto, adicionamos a capacidade de atribuir um grupo a um modelo de projeto.

Quando você atribui um grupo a um modelo de projeto, todos os projetos criados a partir do modelo são associados automaticamente ao grupo do modelo. Para obter mais informações, consulte [Editar modelos de projeto](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).

Além disso, é possível anexar um processo de aprovação de grupo a um modelo e suas tarefas de modelo se o modelo estiver associado ao grupo. Para obter mais informações, consulte [Associar um processo de aprovação novo ou existente ao trabalho](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).

## Edição mais fácil de campos na seção Detalhes

>[!NOTE]
>
>Esse recurso está disponível somente na nova experiência do Adobe Workfront.

As melhorias a seguir permitem editar informações com mais facilidade na seção Detalhes de qualquer objeto:

* Um contorno cinza em torno de um campo ao passar o mouse sobre ele indica que ele é editável.
* Você pode editar os campos clicando neles uma vez.

Antes desse aprimoramento, não estava claro quais campos eram editáveis e você tinha que clicar duas vezes para editar um campo.

## Considere predecessores entre projetos ao calcular datas de handoff

Com uma nova melhoria na maneira como o Adobe Workfront calcula as datas de handoff para tarefas, as dependências entre projetos agora são consideradas.

Anteriormente, as datas de handoff eram calculadas somente com base nos antecessores da tarefa do mesmo projeto.

Agora, para garantir que você sempre tenha uma data de handoff precisa para uma tarefa com um antecessor entre projetos, você deve recalcular a linha do tempo do projeto da tarefa sucessora. Após recalcular a linha do tempo, as datas de handoff da tarefa são calculadas levando em conta as dependências entre projetos das tarefas.

Para obter mais informações sobre datas de handoff, consulte [Visão geral da Data de Entrega da Tarefa](../../../manage-work/tasks/task-information/handoff-task-date.md).

## Adicionar histórias e problemas existentes no Scrum Board

>[!NOTE]
>
>Esse recurso está disponível somente na nova experiência do Adobe Workfront.

Agora é possível adicionar uma história ou edição existente diretamente do quadro de controle. Isso facilita adicionar histórias existentes à sua iteração atual sem precisar ir para a página de backlog.

Para obter mais informações, consulte [Adicionar histórias e problemas do Scrum Board](../../../agile/use-scrum-in-an-agile-team/scrum-board/add-story-from-scrum-board.md).

## Adicionar novas histórias e problemas do quadro de controle

>[!NOTE]
>
>Esse recurso está disponível somente na nova experiência do Adobe Workfront.

Agora você pode criar uma nova história ou edição diretamente do quadro de controle. Isso facilita adicionar rapidamente uma nova história à sua iteração atual.

Para obter mais informações, consulte [Adicionar histórias e problemas do Scrum Board](../../../agile/use-scrum-in-an-agile-team/scrum-board/add-story-from-scrum-board.md).

## Excluir história ou problema do quadro Kanban

>[!NOTE]
>
>Esse recurso está disponível somente na nova experiência do Adobe Workfront.

Agora é possível excluir uma história ou um problema diretamente do quadro Kanban clicando no ícone Mais em uma história ou cartão de edição e selecionando Excluir. Ao excluir uma história ou problema, ela é movida para a Lixeira por 30 dias e pode ser recuperada somente pelo administrador do sistema.

Para obter mais informações, consulte [Excluir histórias ou problemas do quadro Kanban](../../../agile/use-kanban-in-an-agile-team/delete-story-from-kanban-board.md).

## Atualizações do cabeçalho de cartão ágil e da placa de história

>[!NOTE]
>
>Esse recurso está disponível somente na nova experiência do Adobe Workfront.

Em quadros Kanban e Scrum, os seguintes aprimoramentos já estão disponíveis:

* Os cartões de história e as colunas do quadro têm uma largura fixa, de modo que os tamanhos dos cartões não serão alterados se você ajustar o tamanho da janela do navegador.
* A coluna Histórias foi renomeada para História principal.
* Cada cartão tem um rótulo na parte superior para identificá-lo como uma história principal, subtarefa (associada a uma história principal), história (não associada a um pai) ou problema.
* O sombreamento do plano de fundo separa visualmente as colunas.

Para obter mais informações, consulte [Visão geral das iterações](../../../agile/use-scrum-in-an-agile-team/iterations/iterations-overview.md).

## Agrupar projeto, tarefa e emitir preferências

Conforme nos comunicamos anteriormente, lançamos personalizações no nível do grupo para projetos, tarefas e emitir preferências em fases que levaram até 24 de junho de 2021. Agora, a implantação foi concluída e está disponível em Produção para todos os clientes.

Para obter mais informações, consulte os seguintes artigos:

* [Configurar preferências de projeto para um grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md)
* [Configurar preferências de tarefa e emissão para um grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md)

## Permitir que usuários externos aprovem um documento

>[!NOTE]
>
>Esse recurso está disponível somente na nova experiência do Adobe Workfront.

Agora é possível usar endereços de email externos para atribuir aprovadores a um documento na nova experiência do Workfront.

Anteriormente, você podia adicionar usuários externos por endereço de email somente no Workfront Classic.

Para obter mais informações, consulte [Solicitar aprovações de documento](../../../review-and-approve-work/manage-approvals/request-document-approvals.md).

## Exportar informações da seção Detalhes de um portfólio ou programa

>[!NOTE]
>
>Esse recurso foi lançado no ambiente de visualização em 20 de maio de 2021. Ele será lançado para o ambiente de produção em 3 de junho de 2021.

>[!NOTE]
>
>Esse recurso está disponível somente na nova experiência do Adobe Workfront.

Agora é possível exportar para um arquivo .pdf informações da seção Detalhes de portfólios e programas. Antes desse aprimoramento, você podia exportar informações da seção Detalhes somente de projetos, tarefas e problemas.

Para obter informações sobre como exportar formulários personalizados de um objeto, consulte [Exportar formulários personalizados e detalhes do objeto](../../../workfront-basics/work-with-custom-forms/export-custom-forms-details.md).

## Adição do carimbo de data e hora da Data de conclusão planejada no cabeçalho do objeto

>[!NOTE]
>
>Esse recurso está disponível somente na nova experiência do Adobe Workfront.

Para facilitar o acesso, a conveniência e a precisão, adicionamos a opção de selecionar um carimbo de data e hora na Data de conclusão planejada do cabeçalho de projetos, tarefas ou problemas.

Antes desse aprimoramento, quando você atualizava a Data de conclusão planejada de um objeto, a Workfront selecionava meia-noite como o horário padrão. Agora, você pode personalizar a hora, bem como a data de conclusão.

Para obter informações sobre os cabeçalhos de objetos na nova experiência do Workfront, consulte [Novos cabeçalhos de objeto](../../../workfront-basics/the-new-workfront-experience/new-object-headers.md).

## Adicionar um formulário personalizado a um objeto sem editá-lo

>[!NOTE]
>
>Esse recurso está disponível somente na nova experiência do Adobe Workfront.

Facilitamos a adição de um formulário personalizado que outra pessoa preencherá (ou que preencherá posteriormente) a um objeto. O formulário não entra mais no modo de edição automaticamente quando você o adiciona. Basta salvar o formulário vazio no objeto.

Anteriormente, ao adicionar um formulário personalizado a um objeto, a página entrava no modo de edição e era necessário preencher os campos obrigatórios do formulário antes de poder salvá-lo no objeto. Isso era inconveniente quando o formulário era destinado a outro usuário preenchê-lo ou quando você ainda não sabia o que colocar em um campo obrigatório no formulário.

Para obter informações sobre como adicionar um formulário personalizado a um objeto, consulte [Adicionar um formulário personalizado a um objeto](../../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

