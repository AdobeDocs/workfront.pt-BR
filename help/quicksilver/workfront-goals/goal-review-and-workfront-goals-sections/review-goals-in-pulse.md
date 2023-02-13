---
product-previous: workfront-goals
navigation-topic: goal-review-and-sections
title: Analisar metas na seção Publicação de metas da Adobe Workfront
description: Você pode visualizar todas as metas em sua organização, independentemente de quem é o proprietário. Para obter informações sobre como criar metas, consulte Criar metas em Metas da Adobe Workfront.
author: Alina
feature: Workfront Goals
exl-id: 33873797-183d-4efc-9099-26eb907ca799
source-git-commit: 1d221d10e5845e477dff825f853330b9b4df0adf
workflow-type: tm+mt
source-wordcount: '911'
ht-degree: 1%

---

# Analisar metas na seção Publicação de metas da Adobe Workfront

>[!IMPORTANT]
> 
>A funcionalidade descrita neste artigo foi removida do Workfront, a partir da versão 23.1.\
>Este artigo também será removido logo após a versão 23.1, no início de 2023. Nesse momento, recomendamos que você atualize todos os marcadores adequadamente.


Você pode visualizar todas as metas em sua organização, independentemente de quem é o proprietário. Para obter informações sobre como criar metas, consulte [Criar metas nas metas da Adobe Workfront](../../workfront-goals/goal-management/create-goals.md).

Você pode usar a seção Impulso das Metas da Adobe Workfront como uma ferramenta de colaboração, onde pode analisar e participar de um fluxo de atualizações sobre as metas atuais que pertencem a você, suas equipes, grupos ou organizações e garantir que as metas permaneçam atuais. Os grupos de Metas do Workfront apresentam atualizações de progresso, comentários e histórico de edição por meta na seção Publicação .

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as ações descritas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plano Adobe Workfront*</td> 
   <td> <p>Pro ou superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Solicitação ou superior</p> <p>Para obter mais informações, consulte <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Visão geral das licenças do Adobe Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produto</td> 
   <td> <p>Você deve comprar uma licença adicional para a funcionalidade Metas da Adobe Workfront para acessar descrita neste artigo. </p> <p>Para obter mais informações, consulte <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requisitos para usar as metas do Workfront</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Nível de acesso*</td> 
   <td> <p>Visualizar ou aumentar o acesso às metas</p> <p>Nota:  <p>Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode alterar seu nível de acesso, consulte:</p> 
     <ul> 
      <li> <p><a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a> </p> </li> 
      <li> <p><span href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md"><a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md" class="MCXref xref">Conceder acesso às Metas da Adobe Workfront</a></span> </p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> 
    <div> 
     <p>Visualizar ou aumentar permissões em metas</p> 
     <p>Para obter informações sobre como compartilhar metas, consulte <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Compartilhar uma meta na Workfront</a>. </p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

## Pré-requisitos

Você deve ter o seguinte antes de começar:

* Um modelo de layout que inclui a área Metas no Menu principal.

## Gerenciar atualizações de metas e comentários na seção Publicação 

>[!TIP]
>
>Somente as metas que foram verificadas pelo menos uma vez são exibidas na seção Pulse .

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) > **Metas** no canto superior direito da tela.

   Isso abre a área Metas do Workfront .

   Todas as metas são exibidas por padrão.

1. Clique em **Pulso** no painel esquerdo.

   <!--
      <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
      (NOTE: see the numbering in the procedure)
      </MadCap:conditionalText>
      -->

   Uma lista de metas é exibida. A lista contém as seguintes colunas com informações sobre cada meta:

   <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
      <tr> 
         <td role="rowheader">Metas</td> 
         <td>O nome da meta.</td> 
      </tr> 
      <tr> 
         <td role="rowheader">Proprietário</td> 
         <td>O nome do proprietário da meta.</td> 
      </tr> 
      <tr> 
         <td role="rowheader">Período</td> 
         <td>O período para o qual a meta é agendada.</td> 
      </tr> 
      <tr> 
         <td role="rowheader">Progresso</td> 
         <td>O indicador de progresso para a meta que normalmente é um valor de porcentagem.</td> 
      </tr> 
      <tr> 
         <td role="rowheader"> <p>Status (inclui o ícone de alinhamento)</p> <p> <img src="assets/alignment-icon-large.png"> </p> </td> 
         <td> <p>O status da meta, que pode ser um dos seguintes:</p> 
         <ul> 
         <li>Ativo</li> 
         <li>Rascunho</li> 
         <li>Inativo</li> 
         <li>Fechado</li> 
         </ul> <p>O ícone de alinhamento é exibido em metas que estão alinhadas a outras metas. Para obter informações sobre como alinhar metas, consulte <a href="../../workfront-goals/goal-alignment/align-goals-by-connecting-them.md" class="MCXref xref">Alinhar metas ao conectá-las às metas da Adobe Workfront</a>.</p>

   <p>A coluna Status também inclui as atualizações incrementais feitas para cada resultado ou atividade com cada check-in na meta.</p>

   Por exemplo, se a meta tiver uma atividade manual da barra de progresso e você fizer check-in na meta e atualizar a atividade para 50%, a coluna Status exibirá 50% para a atividade dessa meta. Posteriormente, você pode atualizar a mesma atividade para 60%. Nesse caso, uma nova linha é exibida abaixo da mesma meta para a mesma atividade por 10% - porque você acabou de adicionar 10% ao progresso da atividade.
   </td>
   </tr> 
      </tbody> 
      </table>

1. (Opcional) Selecione o tipo de informação que deseja exibir atualizando os filtros no canto superior direito da seção Pulse .

   A Lista de pulsos exibe metas e seu histórico atualizado que correspondem aos critérios do filtro selecionado.

   Para obter mais informações sobre como filtrar metas, consulte [Filtrar informações em metas do Adobe Workfront](../../workfront-goals/goal-management/filter-information-wf-goals.md).

1. Clique na seta apontando para a direita à esquerda do nome da meta para expandir uma meta e exibir informações adicionais sobre as atualizações em cada meta.

   As seguintes informações são exibidas na seção Pulso em cada meta:

   * Nomes e proprietários dos resultados. Para obter informações sobre os resultados, consulte [Adicionar resultados às metas em Metas da Adobe Workfront](../../workfront-goals/results-and-activities/add-results-to-goals.md).
   * Nomes e proprietários da atividade. Para obter informações sobre atividades, consulte [Adicionar atividades às metas em Metas da Adobe Workfront](../../workfront-goals/results-and-activities/add-activities-to-goals.md).
   * Barras de progresso e status de progresso de resultados e atividades. Para obter informações sobre como a Workfront Metas calcula o progresso da meta, consulte [Visão geral do progresso e condição da meta nas Metas da Adobe Workfront](../../workfront-goals/goal-management/calculate-goal-progress.md).

1. Clique em **Adicionar um comentário** para adicionar um comentário para a meta, em seguida, clique em **Post**. O comentário é visível na área Check-in , bem como na guia Atualizações do painel Detalhes da meta . Recomendamos que você use a seção Pulse para comentar as metas que não foram atualizadas em algum momento e solicitar uma atualização ao proprietário da meta.

1. (Opcional) Clique em **Mostrar todas as atualizações** para exibir todas as atualizações de meta. Isso abre a guia Atualizações no painel Detalhes da meta à direita.
1. Clique no nome de uma meta para abrir o **Detalhes da meta** painel à direita e revise mais informações sobre a meta, bem como gerencie-a e seus resultados e atividades. Para obter informações sobre a revisão de metas individuais, consulte [Atualizar metas na seção Detalhes da meta em Metas da Adobe Workfront](../../workfront-goals/goal-management/update-goals-in-goal-details-panel.md).
1. (Opcional e condicional) Clique em **o ícone de alinhamento** ![](assets/align-icon.png) para abrir a meta na seção Alinhamento da meta , se a meta estiver alinhada a outras metas.

1. (Opcional) Expanda a **Metas por página** e selecione uma das seguintes opções para exibir metas adicionais:

   * 20. Esta é a seleção padrão.
   * 50
   * 100


