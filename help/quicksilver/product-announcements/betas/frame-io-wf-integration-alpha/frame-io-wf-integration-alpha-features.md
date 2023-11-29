---
content-type: reference
navigation-topic: betas
title: "Integração nativa alfa: recursos do Adobe Workfront e Frame.io"
description: Recursos planejados para a integração nativa do Adobe Workfront e Frame.io alpha
author: Nolan
feature: Product Announcements
hide: true
hidefromtoc: true
exl-id: a1603a06-957b-4d52-89f3-f0cec1a4e02c
source-git-commit: 02e55be36d3b649aeb5b81d185538f77ac3d4ec7
workflow-type: tm+mt
source-wordcount: '1183'
ht-degree: 0%

---

# Integração nativa do Adobe Workfront e Frame.io alfa: recursos e testes

Com essa integração, nosso objetivo é permitir que os criadores permaneçam em sua ferramenta de escolha (CC ou Frame.io) para conduzir a criação de conteúdo e revisões por pares, enquanto os gerentes de projeto coordenam o trabalho e inicializam e monitoram o processo de revisão formal dentro do Workfront. Isso pode ser feito utilizando o melhor das duas soluções: as novas aprovações de documentos do Workfront para gerenciar aprovações de conteúdo, juntamente com os recursos de revisão de conteúdo oferecidos pelo Frame.io. Coletivamente, as novas aprovações de documentos e o Frame.io vão formar nossa nova experiência completa de revisão e aprovação de conteúdo. 

Para saber mais sobre como o alfa funcionará e como você poderá participar, consulte [Integração do Adobe Workfront e do Frame.io alfa: visão geral](/help/quicksilver/product-announcements/betas/frame-io-wf-integration-alpha/frame-io-wf-integration-alpha-overview.md)


>[!NOTE]
>
>Caso você tenha encontrado essas páginas sem que sua empresa participe desse programa alfa, certifique-se de tratar as informações aqui com cuidado e entre em contato com o administrador do Workfront ou Frame.io para obter mais informações.

## Cenário de teste básico

Para permitir que você teste facilmente os novos recursos do programa alfa, criamos uma nova conta Frame.io de teste e a conectamos a um novo grupo chamado `Frame.io alpha testing` em seu ambiente Workfront Preview ou Sandbox existente.

Para testar a funcionalidade, faça logon na instância de Visualização do Workfront ou Sandbox e execute as seguintes etapas:

1. **Coordenadores:** No Workfront, crie um projeto com o `Frame.io alpha testing` grupo atribuído como o grupo de projeto.

1. **Coordenadores:** No Workfront, atribua suas criações ao projeto ou às tarefas ativadas por Quadro e altere o status do projeto para &quot;Atual&quot;.

1. **Criativos:** Verifique se seus emails contêm um convite para o projeto Frame.io recém-criado

1. **Criativos:** Clique no botão &quot;Unir projeto&quot; no email de convite para participar do projeto Frame.io, revise o resumo criativo no projeto e inicie a criação de conteúdo na ferramenta Creative Cloud de escolha.

1. **Criativos:** Faça upload dos ativos criados no Frame.io e adicione-os ao projeto vinculado do Workfront (ou às tarefas ativadas por Quadro atribuídas).

1. **Coordenadores:** No Workfront, localize os ativos vinculados do Frame.io no seu projeto e atribua revisores/aprovadores (para obter mais informações sobre como atribuir revisões/aprovadores, consulte [Adicionar aprovadores ou revisores adicionais a um documento](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/add-additional-reviewers-or-approvers.md)).

1. **Partes interessadas:** No Workfront, visualize sua solicitação de aprovação na Página inicial ou em Detalhes do documento, revise o Documento conectado ao quadro no Visualizador Frame.io e deixe um comentário contendo feedback.

1. **Coordenadores:** No Workfront, visualize os comentários criados pela parte interessada na seção Atualizações do documento conectado ao Frame.io.

1. **Partes interessadas:** Tome uma decisão no Visualizador Frame.io.

1. **Criativos:** No Frame.io, observe a decisão geral de aprovação tomada para seus ativos.

1. **Criativos:** No Frame.io, aplique as alterações solicitadas adicionando a versão atualizada à pilha de versão do ativo conectado.

1. **Coordenadores:** No Workfront, atribua aprovadores/revisores à versão recém-carregada e monitore o progresso até que ele atinja a aprovação.

## Planos de recursos

Abaixo estão informações sobre os casos de uso principais que estamos procurando solucionar e os recursos que planejamos fazer no momento. <!--, along with documentation to get you started testing.-->

>[!NOTE]
>
><span class="preview">Texto destacado</span> abaixo refere-se aos recursos que ainda não foram implementados, mas serão incluídos em uma versão posterior.
>
>Marcadores em a **&quot;Possíveis melhorias em versões futuras&quot;** o cabeçalho pode ou não ser incluído em uma versão futura, dependendo do feedback alfa e de nossos planos de desenvolvimento em evolução.
>


### Os administradores do Workfront podem configurar uma conexão entre grupos do Workfront e contas Frame.io

* <span class="preview">No Workfront, você pode conectar um grupo do Workfront a uma conta Frame.io</span>

* Uma nova equipe do Frame.io será criada no Frame.io representando o grupo conectado do Workfront

**Possíveis melhorias em versões futuras:**

* Desconectar um grupo Workfront de uma conta Frame.io

* Conectar um grupo Workfront a uma equipe Frame.io existente

### Os coordenadores de projetos podem configurar quais projetos do Workfront são enviados para o Frame.io e ter o Creatives in Workfront atribuído adicionado a ele no projeto no Frame.io

* Capacidade de marcar projetos do Workfront como Frame.io ativado ao atribuir um grupo conectado ao Quadro

* <span class="preview">Aprimoramento: capacidade de alternar tarefas dentro de projetos Workfront como tarefas Quadro que, por sua vez, criará pastas de tarefas dentro do Frame.io</span>

* Quando o status de um projeto do Workfront é definido como Atual, um projeto conectado correspondente é criado no Quadro, os usuários atribuídos do Workfront são adicionados ao projeto do Quadro e uma notificação por email é enviada a eles do Frame.io

   * Todos os membros do Projeto do Workfront (usuários e equipes) serão adicionados como Colaboradores ao projeto Frame.io (na criação do projeto e posteriormente)

   * <span class="preview">Alteração: os usuários e as equipes atribuídos às tarefas do Workfront ativadas por Quadro serão adicionados como Colaboradores ao projeto Frame.io e notificados (na criação do projeto e posteriormente)</span>

* Os documentos (Creative Briefs) adicionados ao projeto e as tarefas ativadas por Quadro serão encaminhadas para o projeto Frame.io (dentro da respectiva pasta de trabalho) quando o projeto for criado (acionador: status do projeto definido como Atual)

   * Recomendamos que você limite a quantidade de documentos adicionados ao seu projeto antes de se tornar ativo apenas para seus resumos criativos, para evitar o envio de vários documentos desnecessários para o Frame.io

* <span class="preview">Aprimoramento: a tarefa do Workfront de usuários/equipes explicitamente desatribuídas de um quadro ativado será removida do projeto Frame.io</span>

**Possíveis melhorias em versões futuras:**

* Tarefas com quadros ativados podem ser configuradas em modelos de projeto

* Os uploads da nova versão para instruções criativas serão encaminhados para o Quadro

* Sincronização otimizada de projetos (desconexão de projetos, ressincronização de projetos e documentos etc.)

### No Frame.io, os profissionais de criação podem enviar ativos criados para o projeto do Workfront para revisão formal

* Capacidade de conectar um único ativo Frame.io a um projeto ou tarefa do WF. Uma referência de ativo será criada no Workfront

* Os uploads de nova versão dentro do Frame.io criarão automaticamente uma nova versão de documento dentro do Workfront em ativos conectados

* <span class="preview">Aprimoramento: capacidade de marcar as tarefas referenciadas do Workfront como concluídas no Frame.io</span>

* <span class="preview">Aprimoramento: caso o documento do Workfront conectado seja excluído, ele permanecerá no Frame.io e poderá ser reconectado à mesma tarefa de projeto ou a outra</span>

**Possíveis melhorias em versões futuras:**

* Capacidade de enviar vários ativos do Frame.io para o Workfront de uma só vez

* Registro de tempo em projetos/tarefas do Workfront no Frame.io

### Os coordenadores de projetos podem atribuir o processo de aprovação formal a documentos vinculados do Frame.io

* Usuários e equipes do Workfront podem ser adicionados a novas aprovações de documentos para documentos conectados ao Frame.io

* <span class="preview">Aprimoramento: quando um usuário/equipe não é compartilhado de um documento habilitado para Frame, ele também perderá o acesso ao ativo no Visualizador Frame.io</span>

**Possíveis melhorias em versões futuras:**

* Enviar vários ativos como uma única revisão

* Atribuição em massa de aprovadores/revisores a documentos do Workfront

### As partes interessadas podem realizar sua análise e aprovação no Frame.io Viewer

* As partes interessadas serão notificadas e poderão exibir o documento conectado ao Quadro no Visualizador Frame.io

* O Visualizador Frame.io pode ser acessado de diferentes locais dentro do Workfront, por exemplo, Lista de documentos, Detalhes do documento, Página inicial do Workfront

* Capacidade de aproveitar os recursos existentes de revisão e comentário fornecidos pelo Visualizador Frame.io que será sincronizado com o Fluxo de atualização do Workfront

* <span class="preview">Capacidade de tomar uma nova decisão de aprovação de documento dentro do Visualizador Frame.io</span>

### No Frame.io, a Equipe de criação será informada sobre a decisão geral tomada no ativo Frame.io conectado

* <span class="preview">Aprimoramento: o status de aprovação geral do documento será exibido no ativo dentro do Frame.io</span>

### Os coordenadores de projetos podem enviar ativos finais para o AEM

* <span class="preview">Aprimoramento: documentos conectados a quadros, incluindo metadados, podem ser enviados ao AEM usando o conector Workfront + AEM Asset CS existente</span>
