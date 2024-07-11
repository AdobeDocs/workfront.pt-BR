---
product-area: documents
navigation-topic: approvals
title: Introdução à revisão e aprovação de ativos com Frame.io
description: Saiba mais sobre o processo formal de revisão e aprovação no uso do Workfront e Frame.io.
author: Courtney
feature: Work Management, Digital Content and Documents
recommendations: noDisplay, noCatalog
exl-id: 68b91aad-af76-473f-861d-da846fdfb84c
source-git-commit: d01a26eaa43b264d11faa88c750f48f0ef1272c4
workflow-type: tm+mt
source-wordcount: '1152'
ht-degree: 0%

---

# Introdução à revisão e aprovação de ativos com Frame.io

O novo fluxo de trabalho de revisão e aprovação de ativos é construído em torno de uma estreita integração entre o Workfront e o Frame.io. Essa integração tira o melhor proveito do que cada produto tem a oferecer e combina-os para criar uma experiência que permita que todos os envolvidos na criação de conteúdo trabalhem com suas ferramentas de escolha, enquanto tenham acesso a comentários, arquivos e atualizações de status — tudo sincronizado em ambos os sistemas em tempo real.

Para obter mais informações sobre o Frame.io, consulte [Introdução ao Frame.io](https://support.frame.io/en/collections/49298-getting-started).

## Iniciação e planejamento do trabalho no Workfront

O administrador do Workfront habilita a integração entre o Workfront e o Frame.io, configurando a conta padrão Frame.io na área Configuração e designando os usuários do Frame.io no Workfront. Isso permite que o coordenador planeje e inicie o trabalho usando projetos do Workfront e workflows formais de revisão e aprovação.

### Configurar a conta padrão do Frame.io [!BADGE Em breve]{type=Informative}

Os administradores do Workfront iniciam a integração do Workfront e do Frame.io adicionando uma conta padrão do Frame.io na área Configuração do Workfront. Uma vez configurada a conta padrão Frame.io, todos os projetos criados no Workfront têm um projeto espelho criado no Frame.io.

>[!IMPORTANT]
>
>Esse recurso será adicionado em breve. Por enquanto, contas Frame.io são adicionadas manualmente pela equipe do Workfront. Entre em contato com o representante de conta Adobe para obter ajuda.

<!--For more information, see [Configure the [!DNL Workfront] and [!DNL Frame.io] integration](/help/quicksilver/administration-and-setup/configure-integrations/configure-wf-and-frame.md).

 in procedure article we need to cover how groups work with projects and how the frame account is associated with a group. And that accounts other than the default can be added on a 1:1 basis using the dev token. -->

### Habilitar usuários do Frame.io Disponível agora

Os usuários do Workfront que usam regularmente o Frame.io devem ser marcados como usuários do Frame.io. Os administradores do Workfront podem designar usuários do Frame.io no Perfil de usuário do Workfront.

>[!TIP]
>
>Recomendamos permitir que os usuários que trabalham regularmente em ferramentas criativas e fazem upload de ativos para revisão e aprovação como usuários do Frame.io.

Quando um usuário é marcado como um usuário do Frame.io no Workfront e adicionado a um projeto:

* Eles são adicionados como um Colaborador no Frame.io.
* Eles podem enviar ativos do Frame.io para o Workfront para revisão e aprovação formais.
* Eles podem exibir informações na pasta de sincronização unidirecional do Workfront. [!BADGE Em breve]{type=Informative}

Para obter mais informações, consulte [Configure o [!DNL Workfront] e [!DNL Frame.io] integração](/help/quicksilver/administration-and-setup/configure-integrations/configure-wf-and-frame.md).

![](assets/Frame-enabled-user.png)


### Criar um projeto conectado ao Frame.io

Depois que a conta padrão Frame.io é adicionada e os usuários do Frame.io são designados, os coordenadores de projeto podem criar projetos do Workfront conectados ao Frame.io. Ao criar um projeto conectado, você pode

* **Atribuir usuários do Frame.io a tarefas**: os usuários habilitados com Frame.io são notificados por email quando são atribuídos a uma tarefa do Workfront, sinalizando que há trabalho a ser concluído.
* **Compartilhar o projeto com usuários do Frame.io**: quando um projeto é compartilhado com usuários habilitados para Frame.io, eles têm acesso ao projeto dentro do Workfront e do Frame.io.
* **Compartilhar materiais criativos com o Frame.io**: os coordenadores de projetos podem enviar instruções e materiais do Workfront diretamente para o usuário criativo no Frame.io usando uma pasta de projeto de sincronização unidirecional. [!BADGE Em breve]{type=Informative}
* **Rastrear o progresso da tarefa**: os criadores podem enviar ativos concluídos e marcar tarefas como concluídas, tudo sem sair do Frame.io.

Para obter mais informações, consulte [Criar um projeto conectado ao Frame.io](/help/quicksilver/manage-work/projects/create-projects/create-frame-connected-project.md).


## Criação de conteúdo e colaboração no Frame.io

Os criativos podem permanecer em suas ferramentas de escolha e ter a liberdade de criar, iterar e realizar revisões por pares dentro do Frame.io.

Quando um criativo é adicionado a um projeto conectado, ele pode fazer o seguinte no Frame.io:

<!--* Access instructions from the project coordinator -->
* Realizar avaliações informais pelos pares
* Enviar ativos concluídos para a Workfront para revisão e aprovação formais
* Alterar o status de uma tarefa ou marcá-la como concluída
* Fazer upload de novas versões e reenviá-las para aprovação <!--do they have to send to frame.io again?-->

Para obter mais informações sobre o Frame.io, consulte [Fui convidado para colaborar em um projeto](https://support.frame.io/en/articles/11125-i-ve-been-invited-to-collaborate-on-a-project).

## Revisar e aprovar ativos

Depois que um criativo envia um ativo concluído para o Workfront do Frame.io, o coordenador do projeto pode iniciar o processo formal de revisão e aprovação no Workfront.

Após a criação do fluxo de trabalho de aprovação, os revisores e aprovadores retornam ao Frame.io para adicionar comentários e marcar o ativo. Eles também podem tomar a decisão de aprovação no visualizador Frame.io.

### Iniciar revisões e aprovações formais no Workfront

Os coordenadores de projetos podem criar revisões e aprovações únicas ou modelos de aprovação reutilizáveis. Todas as atividades de revisão e aprovação no Frame.io também são registradas no Workfront.

Os coordenadores de projeto têm a opção de atribuir revisores, aprovadores ou uma combinação de ambos:

* **Revisores** O pode adicionar comentários e marcar ativos. Depois de concluído, eles podem marcar sua revisão como concluída. Não é necessário marcar a revisão como concluída para que o ativo possa avançar no processo de aprovação.
* **Aprovadores** O pode adicionar comentários e marcar ativos. Eles devem tomar a decisão de mover o processo de aprovação para frente.


#### Criar um fluxo de trabalho de revisão e aprovação

Revisores e aprovadores podem ser adicionados a um fluxo de trabalho de aprovação de uso único ou a um modelo de aprovação reutilizável:

* **Aprovações de uso único**: no projeto ou tarefa em que o ativo reside, o coordenador do projeto pode atribuir revisores e aprovadores e definir um prazo de conclusão. Revisores e aprovadores são lembrados por e-mail 72 e 24 horas antes do prazo, bem como sobre o próprio prazo.

  Para obter mais informações, consulte * [Criar uma solicitação de revisão ou aprovação para um ativo Frame.io](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-request-for-frame-asset.md).

* **Modelos de aprovação**: na área Configuração do Workfront, os coordenadores de projetos podem criar Modelos de aprovação reutilizáveis. Em um modelo, os usuários podem adicionar revisores e aprovadores e especificar um período de conclusão. Quando o modelo de aprovação é aplicado a um ativo, o prazo é calculado a partir do período especificado.

  Depois que um modelo é criado, ele pode ser aplicado a ativos enviados do Frame.io para iniciar o processo formal de revisão e aprovação no Workfront.

  Para obter mais informações, consulte [Criar um modelo de aprovação](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md)


![](assets/assign-template.png)


#### Acessar o visualizador Frame.io

Os usuários podem acessar o visualizador Frame.io das seguintes maneiras:

* Notificações por email do Workfront
* O widget Aguardando minha aprovação na nova área Página inicial do Workfront
  ![](assets/awaiting-my-approval.png)

>[!NOTE]
>
>Os usuários externos do Workfront são notificados por email e serão solicitados a criar um logon Frame.io para revisar e aprovar ativos.

#### Adicionar comentários e marcar ativos

Todos os comentários feitos no visualizador Frame.io também são registrados na guia Atualizações do Workfront. As respostas feitas no Workfront não aparecem no Frame.io. Se os comentários forem marcados como &quot;Somente equipe&quot; no visualizador do Frame.io, eles não aparecerão na guia Atualizações do Workfront.

#### Tomar uma decisão

Quando toda a atividade de revisão estiver concluída, os aprovadores deverão tomar uma das seguintes decisões:

* **Aprovar**: o ativo não precisa de alterações e está pronto para uso.
* **Aprovar com alterações**: o ativo precisa de alterações e está pronto para uso depois de feito. Aprovação adicional não é necessária.
* **Precisa do trabalho**: o ativo precisa de alterações e não está pronto para uso. Depois que as alterações especificadas forem feitas, o ativo deverá ser carregado como uma nova versão e passar por outra rodada de aprovações. <!--is the same approval workflow automatically applied? Does the coordinator have to do anything to get the approval going? -->

Os revisores podem marcar sua revisão como concluída dentro do visualizador Frame.io, mas isso não é necessário para que o ativo avance no processo de aprovação.

Para obter mais informações sobre decisões no Workfront, consulte [Visão geral do status de decisão do documento](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/document-approval-status.md).

![](assets/frame-viewer-and-decision.png)


<!-- upload assets directly to workfront to be reviewed in Frame.io/ Will have to send manually at first

Reviewer/approver needs to go through email to get to frame vier
-->

### Rastrear métricas de revisão e aprovação

Os coordenadores de projetos podem monitorar o progresso em todas as aprovações em andamento na área da página inicial da Workfront com o seguinte widget:

* **Todas as aprovações**: exibe dois gráficos com informações sobre o tempo médio de aprovação e as decisões, bem como exibições de lista de aprovações pendentes e vencidas.
  ![](assets/all-approvals.png)