---
content-type: overview;reference
product-previous: workfront-goals
navigation-topic: goal-management
title: Visão geral do status da meta no Adobe Workfront Goals
description: Os status da meta indicam se uma meta está ativa e registrando progresso no momento, ou se está inativa, rascunhada ou já foi alcançada.
author: Alina
feature: Workfront Goals
exl-id: dc70dfac-2bdd-41ab-b316-0cd20f749423
source-git-commit: 024c612d46848c55529e902a00d481588d261584
workflow-type: tm+mt
source-wordcount: '845'
ht-degree: 4%

---

# Visão geral do status da meta no Adobe Workfront Goals

Sua organização deve ter as seguintes opções para usar a funcionalidade descrita neste artigo:

* Para o novo plano e estrutura de licença:

   * Um plano Ultimate

     Ou

     Uma licença adicional para o Adobe Workfront Goals para os planos Prime ou Select Adobe Workfront. Para obter informações, consulte [plano do Adobe Workfront](https://www.workfront.com/plans).

* Para o plano e a estrutura de licença atuais:

   * A Pro ou superior
   * Uma licença do Adobe Workfront Goals, além de uma licença da Workfront.

Entre em contato com o gerente de conta da Workfront para saber mais sobre uma licença do Workfront Goals.

Os status da meta indicam se uma meta está ativa e registrando progresso no momento, ou se está inativa, rascunhada ou já foi alcançada.

## Consideração ao atualizar status de meta nas Metas do Workfront

* Não é possível atualizar manualmente o status das metas que você criou ou que foram compartilhadas com você. O status das atualizações de metas dependendo das ações que você realizar na meta. Por exemplo, ativar uma meta altera o status Rascunho para Ativo.
* Existem algumas restrições e, às vezes, não é possível alterar o status de uma meta para outro status, de acordo com as seguintes regras:

  | De/ Para | Rascunho | Ativo | Inativo | Fechado |
  |---|---|---|---|---|
  | Rascunho | - | Sim | Não | Não |
  | Ativo | Não | - | Sim | Sim |
  | Inativo | Não | Sim | - | Não |
  | Fechado | Não | Sim | Não | - |

* Abrir uma meta fechada também atualiza o progresso da meta.
* Certas ações que você executa em uma meta também atualizam seu status. Para obter informações sobre como atualizar status de meta, consulte os seguintes artigos:

   * [Criar metas no Adobe Workfront Goals](../../workfront-goals/goal-management/create-goals.md)
   * [Ativar metas no Adobe Workfront Goals](../../workfront-goals/goal-management/activate-goals.md)
   * [Excluir e desativar metas no Adobe Workfront Goals](../../workfront-goals/goal-management/delete-and-deactivate-goals.md)
   * [Fechar e reabrir metas no Adobe Workfront Goals](../../workfront-goals/goal-management/close-and-reopen-goals.md)

## Visão geral dos status das metas no Workfront Goals

Para obter informações sobre como criar metas do Workfront, consulte [Criar metas no Adobe Workfront Goals](../../workfront-goals/goal-management/create-goals.md).

Para obter informações sobre como ativar metas, consulte [Ativar metas no Adobe Workfront Goals](../../workfront-goals/goal-management/activate-goals.md).

As metas podem ter um dos seguintes status nas Metas do Workfront:

* [Rascunho](#draft)
* [Ativo](#active)
* [Inativo](#inactive)
* [Fechado](#closed)

### Rascunho {#draft}

* Este é o status padrão para uma meta recém-criada. Para obter informações sobre como criar metas, consulte [Criar metas no Adobe Workfront Goals](../../workfront-goals/goal-management/create-goals.md).
* O Workfront Goals não registra o progresso em uma meta de rascunho.
* Não é possível atualizar o progresso de uma meta rascunhada.
* Não é possível fechar ou desativar metas rascunhadas porque elas não têm informações sobre o progresso.
* Metas rascunhadas não contribuem para o cálculo do progresso de outras metas, e não são consideradas em gráficos.
* Metas rascunhadas são exibidas nas seguintes áreas das Metas do Workfront:

   * Lista de metas
   * Seção Alinhamento de metas (somente como uma meta alinhada)


>[!IMPORTANT]
>
>Depois de alterar o status de uma meta para qualquer outro status, a meta nunca poderá ser colocada em um status de Rascunho novamente.

### Ativo {#active}

* Você só pode ativar uma meta rascunhada quando a associa a um resultado, uma atividade ou alinha outra meta a ela. Ativar a meta altera seu status para Ativo. Para obter informações sobre como ativar metas, consulte [Ativar metas no Adobe Workfront Goals](../../workfront-goals/goal-management/activate-goals.md).
* As Metas do Workfront registram o progresso em metas ativas.
* As metas ativas contribuem para o cálculo do progresso de outras metas e são consideradas em gráficos.
* As metas ativas são exibidas nas seguintes áreas das Metas do Workfront:

   * Lista de metas
   * Seção Alinhamento de metas
   * O progresso das metas ativas é exibido em gráficos

* Você pode reativar uma meta Fechada ou Inativa.

### Inativo {#inactive}

* Você pode desativar uma meta ativa quando o proprietário parou de trabalhar nela temporariamente ou permanentemente. Você pode mantê-la para obter informações históricas. Isso atualiza o status da meta para Inativo.

  Para obter informações sobre como desativar metas, consulte a seção &quot;Desativar metas&quot; no artigo [Excluir e desativar metas no Adobe Workfront Goals](../../workfront-goals/goal-management/delete-and-deactivate-goals.md).

* Não é possível desativar uma meta de rascunho ou encerrada.
* Você pode reativar uma meta inativa e continuar a trabalhar nela.
* O Workfront Goals não calcula o progresso em metas inativas.
* Não é possível atualizar o progresso de uma meta inativa.
* Metas inativas não contribuem para o cálculo de progresso de outras metas, e elas não são consideradas em gráficos.
* As metas inativas têm um histórico de progresso porque já foram ativas, ao contrário das metas rascunhadas.
* Metas inativas são exibidas nas seguintes áreas do Workfront Goals:

   * Lista de metas
   * Seção Alinhamento de metas (somente como metas alinhadas)

### Fechado {#closed}

* Você pode fechar uma meta quando quiser indicar que a atingiu ou que não está mais trabalhando nela, nem a fará no futuro. Para obter informações sobre o fechamento de metas, consulte [Fechar e reabrir metas no Adobe Workfront Goals](../../workfront-goals/goal-management/close-and-reopen-goals.md).

  >[!TIP]
  >
  >Se você planejar trabalhar posteriormente em uma meta que ainda não foi atingida, recomendamos alterar o status para Inativo em vez de Fechado.

* Não é possível fechar metas que nunca foram ativadas, como metas rascunhadas.
* Você pode reabrir uma meta fechada e continuar trabalhando nela.
* O Workfront Goals para de registrar o progresso em metas fechadas.
* Não é possível atualizar o progresso de uma meta encerrada.
* As metas fechadas são exibidas na seguinte área das Metas do Workfront:

   * Lista de metas
   * Seção Alinhamento de metas (somente como metas alinhadas)
   * Informações de metas fechadas também são consideradas na seção Gráficos.
