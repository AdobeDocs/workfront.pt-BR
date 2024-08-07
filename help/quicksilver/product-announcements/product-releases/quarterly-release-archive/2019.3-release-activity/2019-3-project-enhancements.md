---
content-type: release-notes
navigation-topic: 2019-3-release-activity
title: Aprimoramentos do projeto 2019.3
description: Esta página descreve todas as alterações que o Project aprimorou com a versão 2019.3. Ele foi disponibilizado no ambiente de Produção na semana de 19 de agosto de 2019.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 127d695c-74e4-45f9-b5f6-55c1d05935cf
source-git-commit: dd718ff8f497065018cdfb9592ff0804d7668bf8
workflow-type: tm+mt
source-wordcount: '1340'
ht-degree: 0%

---

# Aprimoramentos do projeto 2019.3

Esta página descreve todas as alterações que o Project aprimorou com a versão 2019.3. Ele foi disponibilizado no ambiente de Produção na semana de 19 de agosto de 2019.

Para obter uma lista de todas as alterações feitas em 2019.3, consulte a [visão geral da atividade da versão 2019.3](../../../../product-announcements/product-releases/quarterly-release-archive/2019.3-release-activity/2019-3-release-activity-overview.md).

## Alterar o tipo de exibição de um campo em um formulário personalizado

Agora é possível alterar o tipo de exibição de um campo em um formulário personalizado.

Por exemplo, se você criou um campo Checkboxes, é possível alterá-lo para um campo Suspenso ou um campo Radio Buttons. Esses três tipos de exibição de campo são intercambiáveis.

Ou, se você tiver criado um Campo de texto de linha única, poderá alterá-lo para um campo de texto de parágrafo. Esses dois tipos de exibição de campo são intercambiáveis.

Anteriormente, para alterar o tipo de exibição de um campo personalizado, era necessário criar um novo campo e excluir o antigo. Isso exigia a transferência de dados, o que geralmente era demorado.

>[!NOTE]
>
>Disponibilidade de visualização: 9 de agosto de 2019
>
>Disponibilidade de produção: 30 de agosto de 2019

## Criar calendários e relatórios de folga

Agora você pode ver a folga do usuário para melhorar o planejamento e a execução. Você também pode adicionar novos relatórios e calendários de folga aos seus painéis para obter uma visualização em tempo real da disponibilidade do usuário.

>[!NOTE]
>
>Disponibilidade de visualização: 9 de agosto de 2019
>
>Disponibilidade de produção: 30 de agosto de 2019

## O filtro Abrir agora mostra mais resultados em uma lista de Problemas

Quando você aplica o filtro Abrir a uma lista de problemas, a lista inclui problemas que:

* Está em um status Fechado - Pendente de Aprovação
* Estão associados a um objeto de resolução

Antes dessa alteração, esses problemas não eram incluídos na lista ao aplicar o filtro Abrir.

## Nova experiência ao editar informações em linha em listas

Quando você editar as informações em linha nas novas listas, as linhas que foram editadas ficarão esmaecidas, mas as informações permanecerão visíveis. Antes dessa alteração, as linhas editadas estavam esmaecidas e as informações não estavam visíveis.

Você pode encontrar as novas listas nas seguintes áreas do Workfront:

* Listas de projetos e tarefas
* Guia Horas para projetos, tarefas e problemas

## Listas atualizadas para as guias de horas de projetos, tarefas e problemas

As exibições de lista aprimoradas agora estão disponíveis nas guias Horas para projetos, tarefas e problemas.

Antes desse aprimoramento, as novas listas eram aplicadas apenas ao seguinte:

* Uma lista de tarefas
* Uma lista de projetos

Para obter informações sobre como visualizar itens em uma lista, consulte [Introdução a listas no Adobe Workfront](../../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

## Editar Gantt sem Ativar um Modo de Edição Especial

Agora você pode editar o gráfico de Gantt da lista de tarefas quando o salvamento automático estiver ativado ou não. Não é possível desfazer alterações quando o botão está ativado. Nesse caso, as alterações feitas no projeto são salvas automaticamente.

Para obter informações sobre como editar o gráfico de Gantt da lista de tarefas, consulte [Atualizar informações no Gráfico de Gantt da lista de tarefas](../../../../manage-work/gantt-chart/use-the-gantt-chart/update-info-task-list-gantt.md).

## Remoção da guia Problemas do quadro Kanban

Estamos removendo a guia Problemas do quadro Kanban na versão de Produção 19.3. Você ainda pode acessar a subguia Problemas no Backlog do quadro Kanban.

## Remoção das guias Documentos e Problemas da página de detalhes da iteração

>[!NOTE]
>
>Essa alteração ocorrerá na Produção com a versão 2019.3. Ele não será feito no ambiente de Pré-visualização antes da versão de Produção.

Estamos removendo as guias Documentos e Problemas da página de detalhes da iteração do Agile:

* **Documentos:** todos os documentos armazenados na guia Documentos devem ser movidos antes da versão de produção. Se você não conseguir mover seus documentos, não terá mais acesso a eles.
* **Problemas:** esta guia geralmente está localizada no menu suspenso Mais. Você ainda pode acessar a subguia Problemas na guia Itens de trabalho na iteração.

## Considerar ou ignorar o tempo de folga do usuário nas datas da tarefa

Agora você pode decidir se permite que o horário de folga do Principal responsável por uma tarefa ajuste as datas planejadas.

Você pode tomar essa decisão no nível do sistema, como administrador do Workfront ou no nível do projeto, como gerente de projeto.

Antes dessa alteração, o tempo de folga do Destinatário principal sempre ajustava as datas planejadas da tarefa, se a Restrição da tarefa permitisse a modificação das datas.

Para obter informações sobre a configuração de Tempo Livre do Usuário no nível do sistema, consulte [Configurar preferências de projeto do sistema](../../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

Para obter informações sobre a configuração de Tempo livre do usuário no nível do projeto, consulte [Editar projetos](../../../../manage-work/projects/manage-projects/edit-projects.md).

>[!NOTE]
>
>Disponibilidade de visualização: 22 de julho de 2019
>
>Disponibilidade de produção: 9 de agosto de 2019

## Condições personalizadas

Agora você pode fazer o seguinte para personalizar as Condições que usa para projetos, tarefas e problemas e atender melhor às necessidades da sua organização:

* Crie condições personalizadas com seus próprios rótulos e cores.
* Altere a ordem das Condições nas listas suspensas em que os usuários as selecionam.
* Use as Condições personalizadas que você cria no lugar das Condições padrão integradas que o Workfront atribui automaticamente aos itens de trabalho.
* Altere os nomes e as cores das Condições padrão incorporadas para projetos, tarefas e problemas.

Além disso, se você tiver direitos para editar uma tarefa ou problema, mas não estiver atribuído a ele (talvez por estar supervisionando-o), agora é possível alterar sua Condição usando a coluna Condições em uma exibição de lista.

Anteriormente, as Condições não podiam ser personalizadas ou alteradas e somente os usuários podiam alterar a Condição de uma tarefa ou problema se fossem atribuídos a ela.

Para obter mais informações, consulte [Condições personalizadas](../../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/custom-conditions.md).

>[!NOTE]
>
>Disponibilidade de visualização: 4 de julho de 2019
>
>Disponibilidade de produção: final de setembro ou início de outubro

## Nova notificação por email para Equipes

Há uma nova notificação de evento por email para equipes. Os membros da equipe recebem uma notificação por email quando um projeto com tarefas atribuídas à sua equipe se torna ativo. Esta configuração é desativada por padrão.

Anteriormente, os membros da equipe não podiam ser notificados quando os projetos em que estavam se tornavam ativos.

Para obter mais informações, consulte Notificações: informações sobre projetos em que estou.

>[!NOTE]
>
>Disponibilidade de visualização: 4 de julho de 2019
>
>Disponibilidade de produção: 18 de julho de 2019

## Atualizações de documento agora aparecem no objeto e projeto associados

Quando você comenta em um documento, a atualização agora aparece na guia Atualizações para o documento e para o objeto ao qual o documento está anexado.

Se o objeto fizer parte de um projeto, seu comentário no documento também aparecerá na guia Atualizações do projeto.

Anteriormente, os comentários de atualização apareciam somente na guia Atualizações do documento.

Para obter mais informações, consulte a seção [Atualizar trabalho](../../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#updates) no artigo [Atualizar trabalho](../../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

>[!NOTE]
>
>Disponibilidade de pré-visualização: 6 de junho de 2019
>
>Disponibilidade de produção: 20 de junho de 2019

## Visibilidade sobre a programação de folga de um usuário ao atribuí-lo a tarefas e problemas

Ao atribuir um usuário a uma tarefa ou um problema, agora é possível ver um aviso em linha se o usuário selecionado tiver uma folga programada a qualquer momento entre as datas planejadas da tarefa ou problema.

Para obter informações sobre atribuição de tarefas, consulte [Atribuir tarefas](../../../../manage-work/tasks/assign-tasks/assign-tasks-1.md)

Para obter informações sobre folga, consulte [Configurar folga pessoal](../../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/personal-time-overview.md).

>[!NOTE]
>
>Disponibilidade de visualização: 30 de maio de 2019
>
>Disponibilidade de produção: 13 de junho de 2019

## Adicionar campos que representam objetos no Forms personalizado

Criamos um novo tipo de campo no construtor de formulários personalizado chamado Digitação antecipada. Este campo permite adicionar campos que representam objetos aos seus formulários personalizados. Atualmente, o objeto Usuário está habilitado com Digitação antecipada e outros objetos estão chegando no futuro.

Anteriormente, os administradores precisavam manter os usuários manualmente como opções individuais nos menus suspensos de formulários personalizados.

>[!NOTE]
>
>Disponibilidade de visualização: 30 de maio de 2019
>
>Disponibilidade de produção: 13 de junho de 2019
>
>Antes da data de lançamento da Produção, os novos campos personalizados não eram compatíveis com o Mobile, Outlook, MS Teams e com a integração nativa do Salesforce.
>
>Na produção, o Outlook e o MS Teams agora são compatíveis. O Mobile é compatível desde o final de junho ou início de julho; as integrações do Salesforce são compatíveis a partir de junho.

## O novo campo &quot;Assunto&quot; da solicitação foi renomeado para &quot;Nome&quot;

>[!NOTE]
>
>Este recurso foi removido e não será incluído na versão 2019.3.

Agora, ao submeter uma nova solicitação a uma Fila de solicitações, você informa o nome da solicitação no campo &quot;Nome&quot; do novo formulário de solicitação.

Antes dessa alteração, você digitaria o nome da solicitação no campo &quot;Assunto&quot;.

Para obter informações sobre como criar solicitações, consulte [Criar e enviar solicitações do Workfront](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md).

