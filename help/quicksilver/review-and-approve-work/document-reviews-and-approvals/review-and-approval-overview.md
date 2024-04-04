---
product-area: documents
navigation-topic: approvals
title: Visão geral da revisão e aprovação de ativos
description: Saiba mais sobre o processo formal de revisão e aprovação no Workfront.
author: Courtney
feature: Work Management, Digital Content and Documents
hide: true
hidefromtoc: true
recommendations: noDisplay, noCatalog
exl-id: 68b91aad-af76-473f-861d-da846fdfb84c
source-git-commit: 7e970f4f707937a62f68c191a7cbd5dfa26e471c
workflow-type: tm+mt
source-wordcount: '909'
ht-degree: 0%

---

# Visão geral da revisão e aprovação de ativos

O novo fluxo de trabalho de revisão e aprovação de ativos é construído em torno de uma estreita integração entre o Workfront e o Frame.io. Essa integração tira o melhor proveito do que cada produto tem a oferecer e a combina para criar uma experiência que permite que todas as pessoas envolvidas na criação de conteúdo trabalhem em suas ferramentas de escolha, enquanto têm acesso a comentários, arquivos e atualizações de status sincronizados em ambos os sistemas em tempo real.

Para obter mais informações sobre o Frame.io, consulte [Introdução ao Frame.io](https://support.frame.io/en/collections/49298-getting-started).

## Iniciação e planejamento do trabalho no Workfront

O administrador do Workfront habilita a integração entre o Workfront e o Frame.io, configurando a conta padrão Frame.io na área Configuração e designando os usuários do Frame.io no Workfront. Isso permite que o coordenador planeje e inicie o trabalho usando o Workfront Projects e a revisão e aprovação formais.

### Configurar uma conta padrão do Frame.io

Os administradores do Workfront iniciam a integração do Workfront e do Frame.io adicionando uma conta padrão do Frame.io na área Configuração do Workfront. Depois que uma conta padrão Frame.io é configurada, a integração cria projetos conectados entre o Workfront e o Frame.io.

Para obter mais informações, consulte [].

<!-- in procedure article we need to cover how groups work with projects and how the frame account is associated with a group. And that accounts other than the default can be added on a 1:1 basis using the dev token. -->

### Habilitar usuários do Frame.io

Os usuários do Workfront que usam regularmente o Frame.io devem ser marcados como usuários do Frame.io. Os administradores do Workfront podem designar usuários do Frame.io no Perfil de usuário do Workfront.

Quando um usuário é marcado como um usuário do Frame.io no Workfront e adicionado a um projeto,

* Eles são adicionados como um Colaborador no Frame.io
* Eles podem enviar ativos do Frame.io para o Workfront para revisão e aprovação formais

>[!TIP]
>
>Recomendamos permitir que os usuários que trabalham regularmente em ferramentas criativas e fazem upload de ativos para revisão e aprovação como usuários do Frame.io.


Para obter mais informações, consulte [].

![](assets/Frame-enabled-user.png)


### Criar um projeto conectado ao Frame.io

Depois que a conta padrão Frame.io é adicionada e os usuários do Frame.io são designados, os coordenadores de projeto podem criar projetos do Workfront conectados ao Frame.io. Ao criar um projeto conectado, você pode

* **Atribuir usuários do Frame.io a tarefas**: os usuários habilitados com Frame.io são notificados por email quando são atribuídos a uma tarefa, sinalizando que há trabalho a ser concluído.
* **Compartilhar o projeto com usuários do Frame.io**: Projetos compartilhados com usuários habilitados para Frame.io concede a eles acesso ao projeto dentro do Frame.io.
* **Compartilhar materiais criativos com o Frame.io**: você pode enviar instruções e materiais do Workfront diretamente para o usuário criativo no Frame.io usando uma pasta de projeto de sincronização unidirecional.
* **Rastrear o progresso da tarefa**: os criadores podem enviar ativos concluídos e marcar tarefas como concluídas sem sair do Frame.io.

Para obter mais informações, consulte [].

<!--Preassign approval templates to tasks coming in the future-->


## Criação de conteúdo e colaboração no Frame.io

Os criativos podem permanecer em suas ferramentas de escolha e ter a liberdade de criar, iterar e realizar revisões por pares dentro do Frame.io.

Quando um criativo é adicionado a um projeto conectado, ele pode fazer o seguinte sem sair do Frame.io:

* Acessar instruções do coordenador do projeto
* Realizar avaliações informais pelos pares
* Enviar ativos concluídos para a Workfront para revisão e aprovação formais
* Alterar o status de uma tarefa ou marcá-la como concluída
<!-- * Notification of decision
* Upload new versions of connected assets marked as needs more work < will automatically connect>-->

Para obter mais informações sobre a revisão de ativos no Frame.io, consulte

## Revisar e aprovar ativos

Depois que um criativo envia um ativo concluído para o Workfront do Frame.io, o coordenador do projeto pode iniciar o processo formal de revisão e aprovação no Workfront.

Após a criação da aprovação, os usuários retornam ao Frame.io para comentar e marcar o ativo. Eles também podem tomar a decisão de aprovação no visualizador Frame.io.

### Iniciar revisões e aprovações formais no Workfront

Os coordenadores de projetos podem criar revisões e aprovações únicas ou Modelos de aprovação reutilizáveis na área Configuração do Workfront. Todas as atividades de revisão e aprovação feitas no Frame.io também são registradas no Workfront.

Os coordenadores de projeto têm a opção de atribuir revisores, aprovadores ou uma combinação de ambos:

* **Revisores** podem comentar e marcar ativos. Depois de concluído, eles podem marcar sua revisão como concluída. <!--example of when to add reviewers-->
* **Aprovadores** é possível comentar em ativos de marcação. Eles devem tomar a decisão de mover o processo de aprovação para frente.



Todos os comentários feitos no Frame.io são refletidos na guia Atualizações no Workfront. As respostas feitas no Workfront não são refletidas no Frame.io.

Comentários marcados Somente para equipes não aparecerão na guia Atualizações do Workfront.

Revisores e aprovadores podem ser adicionados a modelos de uso único ou de aprovação:

<!--can also assign teams and set deadline-->

* **Aprovações de uso único**: Definir prazos de aprovação

* **Modelos de aprovação**
Na área Configuração do Workfront, os usuários com uma licença Standard podem criar Modelos de aprovação reutilizáveis. Em um modelo, os usuários podem especificar um período e adicionar revisores e aprovadores. <!--do we want to mention any upcoming plans here? -->

  Depois que um modelo é criado, ele pode ser aplicado a ativos enviados do Frame.io para iniciar o processo formal de revisão e aprovação no Workfront.
  ![](assets/assign-template.png)

<!-- can set timreframe which calculates deadline once approval is started. >

    For more information, see [Create and manage Approval Templates](/)<!--don't forget link-->

* Faça upload de um ativo do Workfront e envie-o para o quadro para revisão e aprovação - Em breve?

### Aprovar ativos no Frame.io

As partes interessadas do ativo conectado ao Frame.io podem revisar e aprovar no visualizador Frame.io com comentários sincronizados com o fluxo de atualização do Workfront, decisões etc.

<!-- include screenshot from frame.io-->

Se trabalhar exclusivamente no Frame, você pode ser notificado de uma solicitação por email.

Se você trabalhar exclusivamente no Workfront, poderá usar o widget de aprovação na página inicial.

você pode acessar o visualizador Frame.io do sempre que trabalhar

**Aprovar ativos do Frame.io**
como são notificados

tomar uma decisão - aprovar, aprovar com alterações, precisa de trabalho

**Aprovar ativos do Workfront**
como são notificados

Página inicial Aguardando meu widget de aprovação

Email - emails do prazo 72, 24 e no prazo.

Os usuários externos do WF serão solicitados a criar um login para o quadro

Se o ativo não estiver conectado ao quadro, ele poderá visualizar a miniatura no WF e usar a transmissão de comentários. É possível tomar decisões de revisão e aprovação.

<!-- upload assets directly to workfront to be reviewed in Frame.io/ Will have to send manually at first

Reviewer/approver needs to go through email to get to frame vier
-->


### Rastrear métricas de revisão e aprovação

Widgets no relatório Velocidade de aprovação da página inicial?

<!--
### Published approved assets to Adobe Experience Manager Assets

Use the native integration to send approved assets to AEM.
-->


## Exemplo de fluxo de trabalho de aprovação de ativo de campanha

introdução para?

![](assets/example-workflow.png) <!-- probbly need a different version of this but add something similar rather than typing all out?-->
