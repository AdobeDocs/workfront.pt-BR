---
product-area: documents
navigation-topic: approvals
title: Gerenciar aprovações agrupadas
description: Você pode adicionar ou remover participantes e ativos em uma aprovação agrupada sem interromper o fluxo de trabalho do restante do grupo.
author: Courtney
feature: Work Management, Digital Content and Documents
source-git-commit: 8250a95bec88df91e3422c8da7c05ac802b3cb22
workflow-type: tm+mt
source-wordcount: '957'
ht-degree: 4%
---

# Gerenciar aprovações agrupadas

{{highlighted-preview-article-level}}

Uma aprovação agrupada agrupa vários ativos em um único fluxo de trabalho de aprovação, de modo que todos os ativos passam pelos mesmos estágios juntos, em vez de exigir uma aprovação separada por ativo. Você pode adicionar ou remover participantes e ativos em uma aprovação agrupada ativa sem recriar o fluxo de trabalho.

As aprovações agrupadas oferecem suporte ao modo Básico e Avançado, vários estágios e caminhos paralelos da mesma forma que as aprovações de ativo único. Para obter mais informações, consulte [Criar um fluxo de trabalho de aprovação de documento](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md).

>[!IMPORTANT]
>
>O conteúdo deste artigo se refere à funcionalidade atualizada de aprovação de documentos, disponível somente para contas específicas. Para obter informações sobre processos de aprovação padrão, consulte os artigos listados em [Aprovações de trabalho](/help/quicksilver/review-and-approve-work/manage-approvals/manage-approvals.md).

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo.

<table style="table-layout:auto">
 <col>
 <col>
 <tbody>
  <tr>
   <td role="rowheader">Pacote do Adobe Workfront</td>
   <td> <p>Qualquer pacote de fluxo de trabalho para gerenciar aprovações usando o Adobe Cloud Storage</p> </td>
  </tr>
  <tr>
   <td role="rowheader">Licença do Adobe Workfront</td>
   <td>
   <p>Colaborador ou posterior</p>
   <p>Revisar ou superior</p>
   <p>Se você estiver usando a integração Frame.io, é necessário ter uma licença Standard para criar workflows de aprovação.</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader">Configurações de nível de acesso</td>
   <td> <p>Visualize ou tenha acesso superior a projetos, tarefas, problemas, modelos, portfólios, programas, relatórios, painéis, calendários e documentos</p></td>
  </tr>
  <tr>
   <td role="rowheader">Permissões de objeto</td>
   <td> <p>Gerenciar acesso ao objeto associado à solicitação ou aprovação</p></td>
  </tr>
 </tbody>
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Adicionar participantes a uma aprovação agrupada ativa

Você pode adicionar aprovadores ou revisores a uma aprovação agrupada enquanto um estágio estiver ativo, sem interromper as aprovações que já estão em andamento.

Para adicionar participantes a uma aprovação agrupada ativa:

1. Vá para o projeto, tarefa ou problema que contém a aprovação agrupada e selecione **Documentos** no painel esquerdo.

1. Clique em qualquer documento do grupo e, em seguida, clique no ícone **Aprovações**, no lado direito da página.

   ![Adicionar aprovadores no resumo do documento](assets/approvals-icon-new.png)

1. Clique em **Editar workflow**.

1. Digite o usuário, a equipe ou o email no campo **Adicionar nomes ou emails** do estágio ativo.

1. Para cada pessoa que você adicionar, escolha se ela é um aprovador ou revisor.

1. Clique em **Salvar**.

   Os novos participantes veem cada aprovação aberta no grupo em sua fila. Eles não veem as decisões que foram tomadas antes de serem adicionados, portanto, ainda precisam concluir todas as aprovações abertas no momento.

## Remover participantes de uma aprovação agrupada ativa

Você pode remover aprovadores ou revisores de uma aprovação agrupada enquanto um estágio estiver ativo. Os participantes removidos param imediatamente de ver as aprovações do grupo em sua fila, mas as decisões que já tomaram são mantidas e não são redefinidas.

Para remover participantes de uma aprovação agrupada ativa:

1. Vá para o projeto, tarefa ou problema que contém a aprovação agrupada e selecione **Documentos** no painel esquerdo.

1. Clique em qualquer documento do grupo e, em seguida, clique no ícone **Aprovações**, no lado direito da página.

1. Clique em **Editar workflow**.

1. Localize o participante que você deseja remover do estágio ativo e clique no ícone **Remover** ao lado do nome.

1. Clique em **Salvar**.

   O status de aprovação dos participantes restantes é reavaliado para contabilizar a alteração.

## Adicionar ativos a uma aprovação agrupada

Você pode adicionar ativos a uma aprovação agrupada até que seu primeiro estágio seja bloqueado. Depois que o primeiro estágio é bloqueado, não é mais possível adicionar ativos, pois os participantes desse estágio não teriam a chance de analisá-los.

Para adicionar um ativo a uma aprovação agrupada:

1. Vá para o projeto, tarefa ou problema que contém a aprovação agrupada e selecione **Documentos** no painel esquerdo.

1. Clique em qualquer documento do grupo e, em seguida, clique no ícone **Aprovações**, no lado direito da página.

1. Clique em **Editar fluxo de trabalho** e na guia **Documentos**.

1. Selecione o ativo ou os ativos que deseja adicionar ao grupo.

1. Clique em **Salvar**.

   Todos os participantes do grupo são notificados de que um ativo adicional foi adicionado para que analisem.

## Remover ativos de uma aprovação agrupada

É possível remover um ativo de uma aprovação agrupada em qualquer ponto do fluxo de trabalho. O ativo removido se torna sua própria aprovação independente e mantém todas as decisões, comentários e histórico existentes sem reiniciar. Como o ativo já carrega uma decisão de aprovação, você não pode adicioná-lo novamente a uma aprovação agrupada posteriormente.

Para remover um ativo de uma aprovação agrupada:

1. Vá para o projeto, tarefa ou problema que contém a aprovação agrupada e selecione **Documentos** no painel esquerdo.

1. Clique no documento que você deseja remover e no ícone **Aprovações**, no lado direito da página.

1. Clique em **Editar fluxo de trabalho** e na guia **Documentos**. O documento selecionado está fixado no topo da lista e já está marcado.

1. Desmarque a seleção do documento que deseja remover do grupo.

1. Clique em **Salvar**.

   O status de aprovação do ativo permanece visível e inalterado a partir do momento em que foi removido. A visualização de aprovação agrupada é atualizada para refletir os ativos restantes no grupo.

## Resolver uma decisão do tipo &quot;Precisa de trabalho&quot; em uma aprovação agrupada de vários estágios

Em uma aprovação agrupada de vários estágios, todos os ativos em um estágio devem chegar a uma decisão antes que o grupo possa avançar para o próximo estágio. Se um ativo estiver marcado como **Precisa de trabalho**, ele não poderá avançar com o restante do grupo e, portanto, deverá ser removido do grupo para que o estágio avance.

Para resolver uma decisão &quot;Precisa de trabalho&quot;:

1. Remova o ativo marcado como **Precisa do trabalho** do grupo. Para obter mais informações, consulte [Remover ativos de uma aprovação agrupada](#remove-assets-from-a-grouped-approval). O ativo removido se torna sua própria aprovação independente e mantém suas decisões, comentários e histórico existentes.

1. Depois que o ativo for atualizado, solicite aprovação novamente, como um único ativo ou como parte de um novo grupo. Como o ativo já carrega uma decisão de aprovação, você não pode adicioná-lo de volta ao grupo original.

   Para obter mais informações, consulte [Criar um fluxo de trabalho de aprovação de documento](create-a-document-approval.md) e [Criar uma aprovação agrupada](create-a-grouped-approval.md).
