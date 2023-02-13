---
title: Recalcular as finanças do projeto
product-area: projects
navigation-topic: financials
description: As finanças são calculadas em um projeto conforme as alterações ocorrem nas horas registradas para o projeto ou nas taxas usadas para calcular custos e receita.
author: Alina
feature: Work Management
exl-id: 5a90c5a1-8b26-4b6f-b9ec-f446a2e94ff0
source-git-commit: a849ecaf6097dcdc924aaab2867f37bf57d5bc09
workflow-type: tm+mt
source-wordcount: '1590'
ht-degree: 0%

---

# Recalcular as finanças do projeto

As finanças são calculadas em um projeto conforme as alterações ocorrem nas horas registradas para o projeto ou nas taxas usadas para calcular custos e receita.

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plano Adobe Workfront*</td> 
   <td> <p>Qualquer Um</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Plano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a Projetos e Dados Financeiros</p> <p>Observação: Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerencie permissões do projeto com permissões para Gerenciar finanças</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

## Considerações sobre o cálculo das finanças no Adobe Workfront

As finanças são calculadas no Enhanced Analytics das seguintes maneiras:

* Você pode recalcular manualmente os custos e as receitas em um projeto, usando a opção Recalcular Financiamento em um projeto.
* Além disso, algumas ações acionam um recálculo automático.

Quando a taxa de um usuário ou de uma função muda durante a vida de um projeto, o seguinte pode ocorrer:

* Quando a alteração é feita, a taxa atualizada é usada a partir desse ponto, à medida que as horas são registradas e as informações financeiras são calculadas. Alterar a taxa não afeta como as coisas foram calculadas antes da alteração ser feita. Para todas as horas registradas, a taxa antiga é usada para calcular informações financeiras.
* Você pode forçar o Adobe Workfront a usar a nova taxa retroativamente para todas as horas registradas até agora, usando a opção Recalcular Financiamento. Isso força a Workfront a recalcular retroativamente todas as horas inseridas anteriormente, os custos planejados e as receitas de acordo com as novas informações de taxa.

>[!CAUTION]
>
>Antes de recalcular manualmente as finanças de um determinado projeto, convém preservar os dados financeiros que já foram calculados em uma taxa anterior. Recomendamos usar a opção Recalcular financiamento somente quando você tiver certeza de que não está fazendo alterações nas informações existentes ou somente quando essas alterações forem desejadas.

## Preservar dados financeiros para tarefas com horas existentes {#preserve-financial-data-for-tasks-with-existing-hours}

Quando os dados financeiros de um projeto são recalculados, o Workfront recalcula retroativamente todas as horas registradas anteriormente, planejadas, custos reais e receita planejada e real, de acordo com qualquer informação financeira nova ou atualizada.

* [Preservar Receita do Projeto](#preserve-project-revenue)
* [Preservar Custo do Projeto](#preserve-project-cost)

### Preservar Receita do Projeto  {#preserve-project-revenue}

As taxas de receita podem mudar durante a vida útil de um projeto.

Para obter mais informações sobre taxas de faturamento e receita, consulte o artigo [Visão Geral da Faturamento e Receita](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

As taxas de receita podem mudar nos seguintes níveis:

* O nível do sistema (para funções de trabalho)\
   Para obter mais informações sobre como criar funções de cargo com taxas de faturamento no nível do sistema, consulte o artigo [Criar e gerenciar funções de trabalho](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

* O nível do usuário\
   Para obter mais informações sobre como alterar as informações de taxa de faturamento dos usuários, consulte o artigo [Editar o perfil de um usuário](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

* O nível Empresa (para funções de cargo)\
   Para obter mais informações, consulte [Substituir as taxas de faturamento da função de trabalho no nível da empresa](../../../administration-and-setup/set-up-workfront/organizational-setup/override-job-role-billing-rates-company-level.md).

* O nível do Projeto (para funções de cargo)\
   Para obter mais informações sobre a substituição de taxas de função de trabalho no nível do projeto, consulte o artigo [Visão Geral das Taxas de Faturamento da Função do Trabalho e cálculo da Receita em um projeto](../../../manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).

Por exemplo, a taxa de faturamento de um usuário muda de US$ 50 para US$ 75 por hora durante o curso de um projeto e você deseja que todos os dados existentes permaneçam calculados na taxa antiga ($ 50 e hora). No entanto, quando as finanças do projeto forem recalculadas, as tarefas que já têm dados financeiros existentes terão a receita atualizada para refletir a nova taxa de faturamento (de US$ 75 por hora).

* [Preservar Receita do Projeto criando um Registro de Faturamento](#preserve-project-revenue-by-creating-a-billing-record)
* [Preservar receita do projeto usando várias substituições da taxa de faturamento](#preserve-project-revenue-by-using-multiple-billing-rate-overrides)

#### Preservar Receita do Projeto criando um Registro de Faturamento {#preserve-project-revenue-by-creating-a-billing-record}

Quando as taxas de faturamento mudam em qualquer nível mencionado acima, você pode preservar a receita existente que já foi calculada no projeto, evitando o uso da opção Recalcular Financiamento manual ou bloqueando o tempo registrado no projeto e calculado usando a taxa antiga em um registro de faturamento com um status Faturado.

Quando você não recalcula as finanças no projeto ou bloqueia as horas registradas em um registro de faturamento faturado, as horas registradas após as alterações da taxa são calculadas com a nova taxa e as horas registradas antes das alterações da taxa de custo permanecem calculadas com a taxa antiga.

Para obter mais informações sobre como criar registros de faturamento, consulte o artigo [Criar registros de faturamento](../../../manage-work/projects/project-finances/create-billing-records.md).

#### Preservar receita do projeto usando várias substituições da taxa de faturamento {#preserve-project-revenue-by-using-multiple-billing-rate-overrides}

Quando as taxas de faturamento mudam para funções de cargo no nível do projeto, você pode preservar a receita existente que já foi calculada no projeto usando várias substituições de taxas de faturamento que são bloqueadas em um intervalo de tempo especificado.

Para obter mais informações sobre o uso de várias substituições de taxas de faturamento, consulte o artigo [Visão Geral das Taxas de Faturamento da Função do Trabalho e cálculo da Receita em um projeto](../../../manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).

>[!NOTE]
>
>Isso se aplica somente às taxas de faturamento da função de trabalho que são alteradas no nível do projeto.

### Preservar Custo do Projeto {#preserve-project-cost}

As taxas de custo podem mudar nos seguintes níveis:

* Nível do sistema (para funções de trabalho)\
   Para obter mais informações sobre como criar funções de cargo com taxas de custo no nível do sistema, consulte o artigo [Criar e gerenciar funções de trabalho](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

* Nível do usuário\
   Para obter mais informações sobre como alterar as informações da taxa de custo para os usuários, consulte o artigo [Editar o perfil de um usuário](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

Quando as taxas de faturamento mudam em qualquer nível mencionado acima, você pode preservar os custos existentes que já foram calculados no projeto, bloqueando o tempo registrado no projeto e calculado usando a taxa antiga em um registro de faturamento com um status Faturado. Para obter mais informações sobre como criar registros de faturamento, consulte o artigo [Criar registros de faturamento](../../../manage-work/projects/project-finances/create-billing-records.md).

Você também pode evitar o uso da opção manual Recalculate Finance , se não quiser criar um registro de faturamento, conforme descrito na seção [Recalcular manualmente as finanças de um projeto](#manually-recalculate-finances-for-a-project) neste artigo.

Quando você não recalcula as finanças no projeto ou bloqueia as horas registradas em um registro de faturamento faturado, as horas registradas após as alterações da taxa são calculadas com a nova taxa e as horas registradas antes das alterações da taxa de custo permanecem calculadas com a taxa antiga.

## Recalcular manualmente as finanças de um projeto {#manually-recalculate-finances-for-a-project}

Se suas taxas mudarem durante a vida de um projeto e você quiser que seus cálculos de custo e receita reflitam as novas taxas, será necessário recalcular manualmente as finanças do projeto.

>[!NOTE]
>
>Você pode impedir que os valores da receita sejam atualizados para refletir as novas taxas ao recalcular manualmente o financiamento seguindo as etapas da seção [Preservar dados financeiros para tarefas com horas existentes](#preserve-financial-data-for-tasks-with-existing-hours) deste artigo. Os valores de custo são sempre atualizados para refletir as novas taxas quando você recalcula manualmente as finanças em um projeto.

Você pode recalcular as finanças dos projetos no Workfront a partir da página do projeto ou de uma lista de projetos ou relatório.

Você pode recalcular as finanças ao editá-las em massa. Para obter informações, consulte o [Recalcular manualmente as finanças em massa na caixa Editar projetos](#manually-recalculate-finances-in-bulk-in-the-edit-projects-box) neste artigo.

1. Vá para o projeto onde deseja recalcular as finanças e clique no link **Mais** ícone ![](assets/qs-more-icon-on-an-object.png) à direita do nome do projeto

   ![](assets/project-level-more-drop-down-expanded-nwe-350x516.png)

   Ou

   Vá para uma lista de projetos ou relatório, selecione um ou vários projetos e clique no botão **Mais** ícone ![](assets/qs-more-icon-on-an-object.png) na parte superior da lista.

   ![](assets/recalculate-expressions-timeline-finances-drop-down-in-project-list-nwe.png)

   >[!TIP]
   >
   >Dependendo da complexidade de seus projetos, recomendamos não selecionar um grande número de projetos ao recalcular suas finanças em massa para garantir um desempenho ideal. Algumas coisas que podem tornar um projeto muito complexo podem ser várias dependências ou atribuições ou um grande número de campos personalizados.

1. Clique em **Recalcular Finanças**.

   Todos os custos e receitas previstos no projeto são recalculados com quaisquer novas informações.

   Você deve receber uma confirmação na parte superior do navegador de que as finanças do projeto foram recalculadas com êxito.\
   Valores de custo existentes e alguns valores de receita que não foram bloqueados são atualizados para refletir as novas taxas.

## Recalcular manualmente as finanças em massa na caixa Editar projetos {#manually-recalculate-finances-in-bulk-in-the-edit-projects-box}

Você pode recalcular manualmente as finanças de vários projetos editando-os em massa. Isso faz com que a receita dos projetos seja recalculada retroativamente.

>[!IMPORTANT]
>
>Você pode impedir que os valores da receita sejam atualizados para refletir as novas taxas ao recalcular manualmente o financiamento seguindo as etapas da seção [Preservar dados financeiros para tarefas com horas existentes](#preserve-financial-data-for-tasks-with-existing-hours) deste artigo. Os valores de custo são sempre atualizados para refletir as novas taxas quando você recalcula manualmente as finanças em projetos.

Para recalcular manualmente as finanças de vários projetos:

1. Acesse uma lista de projetos.
1. Selecione vários projetos na lista e clique em **Editar**.

   >[!TIP]
   >
   >Dependendo da complexidade de seus projetos, recomendamos não selecionar um grande número de projetos ao editá-los em massa para garantir um desempenho ideal. Algumas coisas que podem tornar um projeto muito complexo podem ser várias dependências ou atribuições ou um grande número de campos personalizados.

1. Clique em **Configurações**, em seguida selecione **Recalcular Custos E Receitas**.

1. Clique em **Salvar alterações**.

## Ações que desencadeiam um recálculo automático das finanças

As seguintes ações acionam o recálculo financeiro dos projetos no Workfront:

* Alterar o status da tarefa
* Mover uma tarefa com horas para outro projeto
* Alterar o status do projeto de Concluído para um status ativo

>[!NOTE]
>
>Quando você altera o status do projeto, somente os valores planejados estão sendo recalculados.

Também é possível recalcular as finanças manualmente na variável **Mais** menu ![](assets/qs-more-menu.png) no nível do projeto, clicando em **Recalcular Finanças**.
