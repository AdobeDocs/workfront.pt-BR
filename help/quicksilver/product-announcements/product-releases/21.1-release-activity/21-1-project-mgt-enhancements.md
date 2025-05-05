---
content-type: release-notes
keywords: notas,trimestral,atualizar
navigation-topic: product-releases
title: 21.1 Aprimoramentos no gerenciamento de projetos
description: Esta página descreve todas as melhorias de Gerenciamento de projetos feitas com a versão 21.1 para o ambiente de Pré-visualização. Essas melhorias serão disponibilizadas no ambiente de Produção na semana de 15 de fevereiro de 2021.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 95e75a28-5ac2-4d1d-acc3-dbc0b295b28f
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '956'
ht-degree: 1%

---

# 21.1 Aprimoramentos no gerenciamento de projetos

Esta página descreve todas as melhorias de Gerenciamento de projetos feitas com a versão 21.1 para o ambiente de Pré-visualização. Essas melhorias serão disponibilizadas no ambiente de Produção na semana de 15 de fevereiro de 2021.

Para obter uma lista de todas as alterações disponíveis com a versão 21.1, consulte a [visão geral da versão 21.1](../../../product-announcements/product-releases/21.1-release-activity/21-1-release-overview.md).

## Exportar agora disponível na seção Métricas em um projeto

Para compartilhar mais facilmente o status e o progresso de um projeto, você pode exportar todo o painel na seção Métricas de um projeto para um arquivo .png.

Para obter mais informações, consulte [Visão geral das métricas do projeto](../../../manage-work/projects/manage-projects/project-metrics.md).

Este recurso agora está incluído nos [Fundamentos do planejador para a nova experiência do Workfront, Parte 3: Gerenciar um caminho de aprendizado do Projeto](https://experienceleague.adobe.com/pt-br/docs/workfront-learn/tutorials-workfront/home) no Workfront One.

## Atualizar percentual concluído de problema quando o projeto ou tarefa convertido a partir da atualização de problema

Atualizamos a forma como a porcentagem concluída dos problemas funciona para problemas que foram convertidos em projetos ou tarefas. Com a nova funcionalidade, quando um problema é convertido em uma tarefa ou um projeto, o percentual concluído do problema é atualizado em sincronia com o percentual concluído da tarefa ou do projeto de resolução quando a configuração &quot;Atualizar automaticamente o status de um problema resolvível quando o status do Objeto de resolução é alterado&quot; é ativada na configuração.

Para obter informações sobre como converter problemas, consulte [Visão Geral de Objetos Resolventes e Resolvíveis](../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md).

## Nova lista de solicitações enviadas

Para permitir que você gerencie suas Solicitações enviadas de uma maneira mais fácil e consistente, removemos as seções Solicitações que enviei e Todas as solicitações na área Solicitações e as substituímos por uma nova Lista enviada. A lista tem uma aparência familiar que corresponde a todas as outras listas do sistema, permitindo filtrar por diferentes categorias de solicitações enviadas e pesquisar rapidamente por uma solicitação que pode ser difícil de encontrar.

Para obter informações sobre como localizar solicitações enviadas, consulte [Localizar solicitações enviadas](../../../manage-work/requests/create-requests/locate-submitted-requests.md).

Este recurso agora está incluído nos [Fundamentos do Collaborator para o novo caminho de aprendizado da Workfront Experience](https://experienceleague.adobe.com/pt-br/docs/workfront-learn/tutorials-workfront/manage-work/issues-requests/make-a-request) no Workfront One.

Este recurso agora está incluído nas [Solicitações no novo caminho de aprendizado da experiência de Workfront](https://experienceleague.adobe.com/pt-br/docs/workfront-learn/tutorials-workfront/manage-work/request-queues/understand-request-queues) no Workfront One.

## Campos removidos da página Nova solicitação

>[!NOTE]
>
>Removido da versão.

Como parte do redesign da página Nova solicitação, atualizamos os Campos de novo problema configurados na seção Configuração da fila de um projeto.

Os seguintes campos Novo problema são exibidos somente ao criar um problema na seção Problemas do projeto. Eles não são exibidos ao enviar um problema usando uma fila de solicitações na área Solicitações:

* Severidade
* Horas planejadas
* Data de início planejado
* URL
* Atribuído para
* Função no trabalho
* Equipe

Substituímos os campos Atribuído a, Função de trabalho e Equipe pelo novo campo Atribuições na página Nova solicitação para designar com eficiência um usuário, função de trabalho ou equipe em um campo comum à medida que você envia uma nova solicitação.

Para obter informações sobre como definir Campos de Novo Problema para um projeto, consulte [Criar uma Fila de Solicitações](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

## Nova experiência ao enviar solicitações na área Solicitações

>[!NOTE]
>
>Removido da versão; permanecerá em Pré-visualização e versão para Produção com 21.2.

Para manter a consistência com a nova experiência do Workfront e criar eficiência para você ao enviar solicitações, reprojetamos a caixa Nova solicitação na área Solicitações. Estas são algumas das melhorias:

* Uma interface de usuário composta com o restante da nova experiência do Workfront
* Eliminação da área Novas solicitações para uma experiência mais fácil e intuitiva
* Uma maneira nova e mais eficiente de anexar documentos às suas solicitações

Capacidade de compartilhar um link para a fila de solicitações, o grupo de tópicos ou o tópico da fila conforme você insere a solicitação.

Para obter informações sobre o envio de solicitações, consulte [Criar e enviar solicitações do Workfront](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md).

## Compartilhar um link para uma fila de solicitações ao enviar uma solicitação

>[!NOTE]
>
>Removido da versão; permanecerá em Pré-visualização e versão para Produção com 21.2.

Agora, tornamos possível compartilhar um link para um tópico de fila de solicitações, grupo de tópicos ou fila ao criar uma solicitação.

Antes de submeter uma nova solicitação, você pode copiar um link para a fila de solicitações, grupo de tópicos ou tópico da fila da solicitação e compartilhá-lo com outros usuários ou incorporá-lo em um painel.

Para obter informações sobre como compartilhar um link com uma fila de solicitações ao enviar uma solicitação, consulte [Compartilhar um link com uma fila de solicitações](../../../manage-work/requests/create-requests/share-link-to-request-queue.md).

## Procure um grupo que você deseja atribuir a um projeto e visualize seus detalhes

Agora é mais fácil garantir que você identifique o grupo correto ao atribuir um grupo a um projeto. Passe o mouse sobre o nome de um grupo encontrado na caixa Grupo, em seguida, clique no ícone de informações que é exibido ao lado do nome para exibir a dica de ferramenta Detalhes do grupo.

Esta dica de ferramenta inclui a hierarquia de grupos acima do grupo, se houver, e os administradores do grupo.

Dependendo dos detalhes configurados para o grupo, você também pode ver o Líder de negócios e a descrição do grupo.

Com essas informações, você pode ter certeza de que está selecionando o grupo correto para atribuir ao projeto.

Para obter mais informações, consulte [Gerenciar informações na área Visão Geral do projeto](../../../manage-work/projects/manage-projects/understand-project-overview-area.md).

## Novo relatório de delegação de usuários

Anteriormente, as informações para as delegações de tarefas, problemas e aprovações de projetos só podiam ser visualizadas pelo delegado na área Página inicial. Para permitir que outros usuários vejam essas informações, os usuários do Plano agora podem criar o relatório Delegação de usuários, que informa a você:

* Quem delegou essas aprovações a outro usuário
* A qual usuário foram delegadas essas aprovações
* A data de início e de termo dessas delegações

Para saber mais, consulte [Criar um relatório de delegação de usuário](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-user-delegation-report.md).
