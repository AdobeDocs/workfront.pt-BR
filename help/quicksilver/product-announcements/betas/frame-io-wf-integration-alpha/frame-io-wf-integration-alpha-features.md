---
content-type: reference
navigation-topic: betas
title: "Integração nativa alfa: recursos do Adobe Workfront e Frame.io"
description: Recursos planejados para a integração nativa do Adobe Workfront e Frame.io alpha
author: Nolan
feature: Product Announcements
hide: true
hidefromtoc: true
source-git-commit: 0ad33f377086f71699c550e2300731056a834e72
workflow-type: tm+mt
source-wordcount: '845'
ht-degree: 0%

---


# Integração nativa alfa do Adobe Workfront e Frame.io: recursos

## Casos de uso e teste de recursos

Com essa integração, nosso objetivo é permitir que os criadores permaneçam em sua ferramenta de escolha (CC ou Frame.io) para conduzir a criação de conteúdo e revisões por pares, enquanto os gerentes de projeto coordenam o trabalho e inicializam e monitoram o processo de revisão formal dentro do Workfront. Isso pode ser feito utilizando o melhor das duas soluções: as novas aprovações de documentos do Workfront para gerenciar aprovações de conteúdo, juntamente com os recursos de revisão de conteúdo oferecidos pelo Frame.io. Coletivamente, as novas aprovações de documentos e o Frame.io vão formar nossa nova experiência completa de revisão e aprovação de conteúdo. 

Para saber mais sobre como o alfa funcionará e como você poderá participar, consulte [Integração do Adobe Workfront e do Frame.io alfa: visão geral](/help/quicksilver/product-announcements/betas/frame-io-wf-integration-alpha/frame-io-wf-integration-alpha-overview.md)


>[!NOTE]
>
>Caso você tenha encontrado essas páginas sem que sua empresa participe desse programa alfa, certifique-se de tratar as informações aqui com cuidado e entre em contato com o administrador do Workfront ou Frame.io para obter mais informações.

<!--Initial setup and basic test scenario 

As part of the alpha program, we've provisioned a new test Frame.io account for you and connected it to a new group "Frame.io alpha testing" in your existing Workfront Preview or Sandbox environment. To test the delivered functionality please log in to your Workfront Preview or Sandbox instance and  perform the following steps: 

Coordinators: Within Workfront, create a project with the "Frame.io alpha testing" group assigned as project group 

Coordinators: Within Workfront, assign your creatives to the project or Frame enabled tasks and change the project status to "Current" 

Creatives: Check your emails for an invite to the newly created Frame.io project 

Creatives: Click on the "Join project" button within the invitation email to join the Frame.io project, review the creative brief within the project and start your content creation within your CC tool of choice 

Creatives: Upload your created assets to Frame.io and add them to the linked Workfront project (or assigned Frame enabled tasks)  

Coordinators: Within Workfront, see the linked Frame.io assets in your project and assign reviewers / approvers (new document approvals: More help on this feature) 

Stakeholders: Withing Workfront, view your approval request in Workfront Home or Document Details and review the Frame connected document in the Frame.io Viewer. Leave a comment feedback 

Coordinators: Within Workfront, view the stakeholder created comments within the Updates section of the Frame.io connected document in Workfront 

Stakeholders: Make a decision from within the Frame.io Viewer 

Creatives: Within Frame.io, notice the overall approval decision made for your assets 

Creatives: Within Frame.io, Apply the requested changes by adding the updated version to the version stack of the connected asset 

Coordinators: Within Workfront, assign approvers / reviewers to the new version upload and monitor the progress until it reaches sign-off-->

## Planos de recursos

Abaixo estão informações sobre os casos de uso principais que estamos procurando solucionar e os recursos que planejamos fazer no momento. <!--, along with documentation to get you started testing.-->


### Os administradores do Workfront podem configurar uma conexão entre grupos do Workfront e contas Frame.io

* _No Workfront, você pode conectar um grupo do Workfront a uma conta Frame.io_

* Uma nova equipe do Frame.io será criada no Frame.io representando o grupo conectado do Workfront

**Possíveis melhorias em versões futuras:**

* Desconectar um grupo Workfront de uma conta Frame.io

* Conectar um grupo Workfront a uma equipe Frame.io existente

### Os coordenadores de projetos podem configurar quais projetos do Workfront são enviados para o Frame.io e ter o Creatives in Workfront atribuído adicionado a ele no projeto no Frame.io

* Capacidade de marcar projetos do Workfront como Frame.io ativado ao atribuir um grupo conectado ao Quadro

* _Aprimoramento: capacidade de alternar tarefas dentro de projetos Workfront como tarefas Quadro que, por sua vez, criará pastas de tarefas dentro do Frame.io_

* Quando o status de um projeto do Workfront é definido como Atual, um projeto conectado correspondente é criado no Quadro, os usuários atribuídos do Workfront são adicionados ao projeto do Quadro e uma notificação por email é enviada a eles do Frame.io

   * Todos os membros do Projeto do Workfront (usuários e equipes) serão adicionados como Colaboradores ao projeto Frame.io (na criação do projeto e posteriormente)

   * _Alteração: os usuários e as equipes atribuídos às tarefas do Workfront ativadas por Quadro serão adicionados como Colaboradores ao projeto Frame.io e notificados (na criação do projeto e posteriormente)_

* Os documentos (Creative Briefs) adicionados ao projeto e as tarefas ativadas por Quadro serão encaminhadas para o projeto Frame.io (dentro da respectiva pasta de trabalho) quando o projeto for criado (acionador: status do projeto definido como Atual)

   * Recomendamos que você limite a quantidade de documentos adicionados ao seu projeto antes de se tornar ativo apenas para seus resumos criativos, para evitar o envio de vários documentos desnecessários para o Frame.io

* _Aprimoramento: a tarefa do Workfront de usuários/equipes explicitamente desatribuídas de um quadro ativado será removida do projeto Frame.io_

**Possíveis melhorias em versões futuras:**

* Tarefas com quadros ativados podem ser configuradas em modelos de projeto

* Os uploads da nova versão para instruções criativas serão encaminhados para o Quadro

* Sincronização otimizada de projetos (desconexão de projetos, ressincronização de projetos e documentos etc.)

### No Frame.io, os profissionais de criação podem enviar ativos criados para o projeto do Workfront para revisão formal

* Capacidade de conectar um único ativo Frame.io a um projeto ou tarefa do WF. Uma referência de ativo será criada no Workfront

* Os uploads de nova versão dentro do Frame.io criarão automaticamente uma nova versão de documento dentro do Workfront em ativos conectados

* _Aprimoramento: capacidade de marcar as tarefas referenciadas do Workfront como concluídas no Frame.io_

* _Aprimoramento: caso o documento do Workfront conectado seja excluído, ele permanecerá no Frame.io e poderá ser reconectado à mesma tarefa de projeto ou a outra_

**Possíveis melhorias em versões futuras:**

* Capacidade de enviar vários ativos do Frame.io para o Workfront de uma só vez

* Registro de tempo em projetos/tarefas do Workfront no Frame.io

### Os coordenadores de projetos podem atribuir o processo de aprovação formal a documentos vinculados do Frame.io

* Usuários e equipes do Workfront podem ser adicionados a novas aprovações de documentos para documentos conectados ao Frame.io

* _Aprimoramento: quando um usuário/equipe não é compartilhado de um documento habilitado para Frame, ele também perderá o acesso ao ativo no Visualizador Frame.io_

**Possíveis melhorias em versões futuras:**

* Enviar vários ativos como uma única revisão

* Atribuição em massa de aprovadores/revisores a documentos do Workfront

### As partes interessadas podem realizar sua análise e aprovação no Frame.io Viewer

* As partes interessadas serão notificadas e poderão exibir o documento conectado ao Quadro no Visualizador Frame.io

* O Visualizador Frame.io pode ser acessado de diferentes locais dentro do Workfront, por exemplo, Lista de documentos, Detalhes do documento, Página inicial do Workfront

* Capacidade de aproveitar os recursos existentes de revisão e comentário fornecidos pelo Visualizador Frame.io que será sincronizado com o Fluxo de atualização do Workfront

* _Capacidade de tomar uma nova decisão de aprovação de documento dentro do Visualizador Frame.io_

### No Frame.io, a Equipe de criação será informada sobre a decisão geral tomada no ativo Frame.io conectado

* _Aprimoramento: o status de aprovação geral do documento será exibido no ativo dentro do Frame.io_

### Os coordenadores de projetos podem enviar ativos finais para o AEM

* _Aprimoramento: documentos conectados a quadros, incluindo metadados, podem ser enviados ao AEM usando o conector Workfront + AEM Asset CS existente_