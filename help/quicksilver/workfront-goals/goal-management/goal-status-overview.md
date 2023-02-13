---
content-type: overview;reference
product-previous: workfront-goals
navigation-topic: goal-management
title: Visão geral do status da meta em Metas da Adobe Workfront
description: Os status da meta indicam se uma meta está ativa e atualmente registrando o progresso, ou se está inativa, redigida ou já alcançada.
author: Alina
feature: Workfront Goals
exl-id: dc70dfac-2bdd-41ab-b316-0cd20f749423
source-git-commit: 1d221d10e5845e477dff825f853330b9b4df0adf
workflow-type: tm+mt
source-wordcount: '825'
ht-degree: 4%

---

# Visão geral do status da meta em Metas da Adobe Workfront

<!--drafted for P&P new model: the note at the top will need to be replaced with this:    
    
Your organization must have the following to use the functionality described in this article:    
    
* For the legacy plan and license structure:     
    
  * A Pro or higher [Adobe Workfront plan](https://www.workfront.com/plans).     
  * An Adobe Workfront Goals license in addition to a Workfront license.    
    
* For the current plan and license structure:    
    
  * An Ultimate plan     
        
    Or    
        
    An additional license for Adobe Workfront Goals for the Prime or Select Adobe Workfront plans. <is there a link we can add here for the plans and what they contain?!>    
    
Contact your Workfront account manager to learn about a Workfront Goals license.    
    
For additional information about access to Workfront Goals, see [Requirements to use Workfront Goals](../workfront-goals/goal-management/access-needed-for-wf-goals.md).    
-->

>[!NOTE]
>
>Sua organização deve ter o seguinte para usar a funcionalidade descrita neste artigo:
>
>* Um Pro ou superior [Plano Adobe Workfront](https://www.workfront.com/plans).
>* Uma licença do Adobe Workfront Metas além de uma licença da Workfront.
>
>Entre em contato com o gerente de conta da Workfront para saber mais sobre uma licença do Workfront Metas.

Para obter informações adicionais sobre o acesso às Metas da Workfront, consulte [Requisitos para usar as metas do Workfront](../../workfront-goals/goal-management/access-needed-for-wf-goals.md).


Os status da meta indicam se uma meta está ativa e atualmente registrando o progresso, ou se está inativa, redigida ou já alcançada.

## Consideração ao atualizar os status da meta nas Metas da Workfront

* Não é possível atualizar manualmente o status das metas que você criou ou que foram compartilhadas com você. O status das metas é atualizado dependendo das ações que você executa na meta. Por exemplo, ativar uma meta altera o status Rascunho para Ativo.
* Algumas restrições existem e, às vezes, não é possível alterar o status de uma meta para outro status, de acordo com as seguintes regras:

   | De/ Para | Rascunho | Ativo | Inativo | Fechado |
   |---|---|---|---|---|
   | Rascunho | - | Sim | não | não |
   | Ativo | não | - | Sim | Sim |
   | Inativo | não | Sim | - | não |
   | Fechado | não | Sim | não | - |

* Abrir uma meta fechada também atualiza o progresso da meta.
* Determinadas ações que você executa em uma meta também atualizam seu status. Para obter informações sobre como atualizar status de meta, consulte os seguintes artigos:

   * [Criar metas nas metas da Adobe Workfront](../../workfront-goals/goal-management/create-goals.md)
   * [Ativar metas nas metas da Adobe Workfront](../../workfront-goals/goal-management/activate-goals.md)
   * [Excluir e desativar metas em metas do Adobe Workfront](../../workfront-goals/goal-management/delete-and-deactivate-goals.md)
   * [Fechar e reabrir metas em Metas da Adobe Workfront](../../workfront-goals/goal-management/close-and-reopen-goals.md)

## Visão geral dos status da meta nas Metas da Workfront

Para obter informações sobre como criar metas do Workfront, consulte [Criar metas nas metas da Adobe Workfront](../../workfront-goals/goal-management/create-goals.md).

Para obter informações sobre como ativar metas, consulte [Ativar metas nas metas da Adobe Workfront](../../workfront-goals/goal-management/activate-goals.md).

As metas podem ter um dos seguintes status nas Metas da Workfront:

* [Rascunho](#draft)
* [Ativo](#active)
* [Inativo](#inactive)
* [Fechado](#closed)

### Rascunho {#draft}

* Este é o status padrão de uma meta recém-criada. Para obter informações sobre como criar metas, consulte [Criar metas nas metas da Adobe Workfront](../../workfront-goals/goal-management/create-goals.md).
* As Metas Workfront não registram o progresso em um objetivo elaborado.
* Não é possível atualizar o progresso de uma meta elaborada.
* Não é possível fechar ou desativar metas elaboradas porque elas não têm informações de progresso.
* Os objetivos desenhados não contribuem para o cálculo do progresso de outros objetivos e não são considerados nos gráficos.
* As metas projetadas são exibidas nas seguintes áreas das Metas do Workfront:

   * Lista de metas
   * Seção Alinhamento da meta (somente como uma meta alinhada)


>[!IMPORTANT]
>
>Após alterar o status de uma meta para qualquer outro status, a meta nunca poderá ser colocada em um status Rascunho novamente.

### Ativo {#active}

* Você pode ativar uma meta elaborada somente quando associá-la a um resultado, uma atividade ou alinhar outra meta a ela. Ativar a meta altera seu status para Ativa. Para obter informações sobre como ativar metas, consulte [Ativar metas nas metas da Adobe Workfront](../../workfront-goals/goal-management/activate-goals.md).
* As Metas do Workfront registram o progresso em metas ativas.
* As metas ativas contribuem para o cálculo do progresso de outras metas, e são consideradas em gráficos.
* As metas ativas são exibidas nas seguintes áreas das Metas do Workfront:

   * Lista de metas
   * Seção Alinhamento da meta
   * O progresso das metas ativas é exibido em gráficos

* Você pode reativar uma meta Fechada ou Inativa.

### Inativo {#inactive}

* Você pode desativar uma meta ativa quando o proprietário parou de trabalhar nela temporária ou permanentemente. Você pode mantê-lo para obter informações históricas. Isso atualiza o status da meta para Inativa.

   Para obter informações sobre como desativar metas, consulte a seção &quot;Desativar metas&quot; no artigo [Excluir e desativar metas em metas do Adobe Workfront](../../workfront-goals/goal-management/delete-and-deactivate-goals.md).

* Não é possível desativar uma meta elaborada ou fechada.
* Você pode reativar uma meta inativa e continuar trabalhando nela.
* As Metas da Workfront não calculam o progresso em metas inativas.
* Não é possível atualizar o progresso de uma meta inativa.
* As metas inativas não contribuem para o cálculo do progresso de outras metas e não são consideradas nos gráficos.
* Os objetivos inativos têm um histórico de progresso porque antes eram ativos, ao contrário dos objetivos elaborados.
* As metas inativas são exibidas nas seguintes áreas das Metas da Workfront:

   * Lista de metas
   * Seção Alinhamento da meta (somente como metas alinhadas)

### Fechado {#closed}

* Você pode fechar uma meta quando quiser indicar que a atingiu ou que não está mais trabalhando nela, nem fará isso no futuro. Para obter informações sobre metas de fechamento, consulte [Fechar e reabrir metas em Metas da Adobe Workfront](../../workfront-goals/goal-management/close-and-reopen-goals.md).

   >[!TIP]
   >
   >Se você planeja trabalhar posteriormente em uma meta que ainda não foi atingida, recomendamos que você altere o status para Inativo em vez de Fechado.

* Não se pode fechar objetivos que nunca foram ativados, como objetivos elaborados.
* Você pode reabrir uma meta fechada e continuar trabalhando nela.
* As Metas da Workfront param de registrar o progresso em metas fechadas.
* Não é possível atualizar o progresso de uma meta fechada.
* As metas fechadas são exibidas na seguinte área das Metas do Workfront:

   * Lista de metas
   * Seção Alinhamento da meta (somente como metas alinhadas)
   * As informações de objetivos fechados também são consideradas na seção Gráficos .
