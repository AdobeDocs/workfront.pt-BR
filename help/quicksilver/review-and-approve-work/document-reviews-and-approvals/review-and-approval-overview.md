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
source-git-commit: 63160895fc77994fdecd7aca8769b7d236d285d6
workflow-type: tm+mt
source-wordcount: '813'
ht-degree: 0%

---


# Visão geral da revisão e aprovação de ativos

O novo fluxo de trabalho de revisão e aprovação de ativos é construído em torno de uma estreita integração entre o Workfront e o Frame.io. Essa integração tira o melhor proveito do que cada produto tem a oferecer e a combina para criar uma experiência que permite que todas as pessoas envolvidas na criação de conteúdo trabalhem em suas ferramentas de escolha, enquanto têm acesso a comentários, arquivos e atualizações de status sincronizados em ambos os sistemas em tempo real.

<!-- link to frame docs-->

## Iniciação e planejamento do trabalho no Workfront

O coordenador do projeto começa no Workfront. O projeto é criado, as tarefas são atribuídas e as instruções são enviadas.

O coordenador do projeto cria o projeto WF, usa a pasta de projeto sincronizada para enviar informações e materiais de suporte para criações dentro do Frame.io

Configurar o fluxo de trabalho de aprovação do zero ou por meio de modelos

Atribuir tarefas

Define o projeto como Atual ou igual para criar o projeto de quadro e criações de alerta

### Configurar uma conta padrão do Frame.io

Os administradores do Workfront iniciam a integração do Workfront e do Frame.io adicionando uma conta padrão do Frame.io na área Configuração do Workfront. Depois que uma conta padrão do Frame.io é configurada, isso permite que a integração crie projetos conectados entre o Workfront e o Frame.io.

Para obter mais informações, consulte [].


<!-- in procedure article we need to cover how groups work with projects and how the frame account is associated with a group. And that accounts other than the default can be added on a 1:1 basis using the dev token. -->


### Habilitar usuários do Frame.io

Os usuários do Workfront que usam regularmente o Frame.io devem ser marcados como usuários do Frame.io. Os administradores do Workfront podem designar usuários do Frame.io no Perfil de usuário do Workfront.

Quando um usuário é marcado como um usuário do Frame.io no Workfront e adicionado a um projeto:

* Eles são adicionados como um Colaborador no Frame.io
* Eles podem enviar ativos do Frame.io para o Workfront para revisão e aprovação formais

Para obter mais informações, consulte [].

![](assets/Frame-enabled-user.png)

>[!TIP]
>
>Recomendamos permitir que os usuários que trabalham regularmente em ferramentas criativas e fazem upload de ativos para revisão e aprovação como usuários do Frame.io.

### Criar um projeto conectado ao Frame.io

Os coordenadores de projetos podem criar projetos do Workfront conectados ao Frame.io. Ao criar um projeto conectado, você pode

* **Atribuir usuários do Frame.io a tarefas**: os usuários habilitados com Frame.io são notificados por email quando são atribuídos a uma tarefa, sinalizando para eles que há trabalho a ser concluído.
* **Compartilhar o projeto com usuários do Frame.io**: Projetos compartilhados com usuários habilitados para Frame.io concede a eles acesso ao projeto dentro do Frame.io.
* **Compartilhar materiais criativos com o Frame.io**: você pode enviar instruções e materiais do Workfront diretamente para o usuário criativo no Frame.io usando uma pasta de projeto de sincronização unidirecional.
* **Rastrear o progresso da tarefa**: os criadores podem enviar ativos concluídos e marcar tarefas como concluídas sem sair do Frame.io.

Para obter mais informações, consulte [].

<!--Preassign approval templates to asks coming in the future-->


## Criação de conteúdo e colaboração no Frame.io

Os criativos podem permanecer em suas ferramentas de escolha e ter a liberdade de criar, iterar e realizar revisões por pares dentro do Frame.io.

Quando um criativo é adicionado a um projeto integrado, ele pode fazer tudo o que segue sem sair do Frame.io:

* Acessar instruções do coordenador do projeto
* Realizar avaliações informais pelos pares
* Enviar ativos concluídos para a Workfront para revisão e aprovação formais
* Alterar o status de uma tarefa ou marcá-la como concluída
<!-- * Notification of decision
* Upload new versions of connected assets marked as needs more work < will automatically connect>-->


## Revisar e aprovar ativos no Workfront

Depois que um criativo envia um ativo concluído para o Workfront do Frame.io, o coordenador do projeto pode dar início ao processo formal de revisão e aprovação no Workfront. Todas as atividades de revisão e aprovação são registradas no Workfront.

Todos os comentários feitos no Frame.io também são refletidos na guia Atualizações no Workfront. As respostas feitas no Workfront não são refletidas no Frame.io.

Comentários marcados Somente para equipes não aparecerão na guia Atualizações do Workfront.

### Iniciar revisões e aprovações formais

Você pode criar revisões e aprovações ocasionais ou criar Modelos de aprovação reutilizáveis na área Configuração do workfront:

Você tem a opção de atribuir revisores, aprovadores ou uma combinação de ambos:

* **Revisores** é possível comentar e marcar ativos. Depois de concluído, eles podem marcar sua revisão como concluída. <!--example of when to add reviewers-->
* **Aprovadores** Podem comentar, marcar ativos e devem tomar a decisão de mover o processo de aprovação para frente.

Revisores e aprovadores podem ser adicionados a modelos de uso único ou de aprovação:

<!--can also assign teams and set deadline-->

* **Aprovações de uso único**: Definir prazos de aprovação

* **Modelos de aprovação**
Na área Configuração do Workfront, os usuários com uma licença Standard podem criar Modelos de aprovação reutilizáveis. Em um modelo, os usuários podem especificar um período e adicionar revisores e aprovadores. <!--do we want to mention any upcoming plans here? -->

  Depois que um modelo é criado, ele pode ser aplicado a ativos enviados do Frame.io para iniciar o processo formal de revisão e aprovação no Workfront.
  ![](assets/assign-template.png)

<!-- can set timreframe which calculates deadline once approval is started. >

    For more information, see [Create and manage Approval Templates](/)<!--don't forget link-->

### Notificações de revisão e aprovação

Combinar com outras seções?

Página inicial Aguardando meu email do widget de aprovação - emails do prazo 72, 24 e no prazo.

<!-- upload assets directly to workfront to be reviewed in Frame.io/ Will have to send manually at first

Reviewer/approver needs to go through email to get to frame vier
-->

### Revisar e aprovar ativos

As partes interessadas do ativo conectado ao Frame.io podem revisar e aprovar dentro do visualizador de quadros com comentários sincronizados com o fluxo de atualização do Workfront, decisões etc

<!-- include screenshot from frame.io-->

Os usuários externos do WF serão solicitados a criar um login para o quadro

Se o ativo não estiver conectado ao quadro, ele poderá visualizar a miniatura no WF e usar a transmissão de comentários. decisões de revisão e aprovação podem ser tomadas.

### Rastrear métricas de revisão e aprovação

Widget no relatório inicial de velocidade de aprovação

<!--
### Published approved assets to Adobe Experience Manager Assets

Use the native integration to send approved assets to AEM.
-->


* Faça upload de um ativo do Workfront e envie-o para o quadro para revisão e aprovação - Em breve?

## Exemplo de fluxo de trabalho de aprovação de ativo de campanha

introdução para?

![](assets/example-workflow.png) <!-- probbly need a different version of this but add something similar rather than typing all out?-->