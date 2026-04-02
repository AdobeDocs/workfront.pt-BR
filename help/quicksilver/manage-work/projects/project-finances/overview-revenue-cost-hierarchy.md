---
content-type: overview
product-area: projects
navigation-topic: financials
title: Visão Geral da Receita e da Hierarquia de Custo
description: Este artigo descreve o processo passo a passo para determinar as taxas de custo e faturamento apropriadas para funções de trabalho e usuários para o tipo de receita por hora e tipo de custo Usuário e Função.
author: Lisa
feature: Work Management
source-git-commit: dfc6344303f33a9c3c89837b759235612e54904e
workflow-type: tm+mt
source-wordcount: '3519'
ht-degree: 0%

---

# Visão geral da hierarquia de receita e custo

{{highlighted-preview-article-level}}

{{ultimate-package}}

Para fornecer cálculos financeiros precisos, o Workfront usa as taxas de faturamento apropriadas ao calcular a receita de uma tarefa ou projeto. As funções de trabalho e as taxas de usuário devem ser bem definidas em todos os níveis para obter cálculos financeiros precisos.

As seções neste artigo descrevem o processo passo a passo para determinar as taxas de faturamento e custo apropriadas para funções de trabalho e usuários para o tipo de receita e tipo de custo Usuário e Função por hora.

Para obter mais informações sobre taxas de cobrança, tipos de receita e como a receita é calculada, consulte [Visão geral de cobrança e receita](/help/quicksilver/manage-work/projects/project-finances/billing-and-revenue-overview.md).

## Visão geral das datas efetivas

Como alternativa, os administradores do Workfront podem definir datas de efetivação que determinem quando as taxas de faturamento, as taxas de custo e outros atributos financeiros entrarão em vigor no sistema. Por exemplo, uma função de trabalho ou usuário pode ter uma taxa de cobrança padrão de US$ 50. Com as datas de efetivação aplicadas, essa taxa de US$ 50 poderia expirar em 31 de março, e uma nova taxa de US$ 55 começaria automaticamente em 1º de abril.

Para cálculos de receita planejada, as taxas de faturamento são baseadas na data das horas planejadas. As horas planejadas são distribuídas uniformemente pela duração da tarefa. Usando o exemplo anterior, as horas planejadas para 31 de março ou antes usam a taxa de US$ 50 e as horas planejadas para 1º de abril ou depois usam a taxa de US$ 55.

Para cálculos de receita real, as taxas de faturamento se baseiam na data das horas reportadas. Usando o exemplo anterior, as horas registradas em 31 de março ou antes usam a taxa de US$ 50 e as horas registradas em 1º de abril ou depois usam a taxa de US$ 55.

>[!NOTE]
>
>As atribuições de tarefa não estão definidas com datas de efetivação. Em vez disso, as atribuições extraem as taxas aplicáveis do sistema, seja de um cartão de taxa, perfil de usuário ou sobreposição no nível da atribuição. As datas de efetivação garantem que a taxa correta seja aplicada com base no tempo do trabalho, mas não definem diretamente as atribuições.

## Visão geral da função de trabalho para faturamento

Uma **função de trabalho para cobrança** está definida para um usuário no nível de atribuição ou no nível de projeto. Ela se aplica somente a usuários e não pode ser usada em outras funções de trabalho. Por exemplo, a função de trabalho principal de um usuário é Designer, mas em uma tarefa ou projeto ele está agindo como um Designer sênior e a taxa deve refletir isso.

Uma função de trabalho no nível da atribuição para faturamento é apenas para essa atribuição específica e não é aplicada automaticamente às outras atribuições do usuário. Uma função de trabalho no nível do projeto para faturamento se aplica a todas as atribuições do usuário nesse projeto. Você pode sobrepô-la no nível de atribuição individual, se necessário.

Quando uma função de trabalho para faturamento é aplicada no nível da atribuição do usuário ou do projeto, a taxa anexada à função de trabalho para faturamento pode ser usada em vez das taxas do usuário ou da função de trabalho nos cálculos de receita. A função de trabalho para faturamento só está disponível quando o tipo de receita Usuário e Função por hora é usado.

>[!NOTE]
>
>Embora um usuário possa agir com uma função diferente para fins de faturamento, os cálculos de custo continuam a usar sua função de trabalho principal. A função de trabalho para faturamento afeta apenas os cálculos de faturamento.

Para obter mais informações, consulte [Configurar uma função de trabalho para cobrança](/help/quicksilver/manage-work/projects/project-finances/set-up-job-role-for-billing.md).

## Visão geral das taxas preservadas

O sinalizador **Preservar informações de taxas de cobrança do projeto** em um projeto controla se o sistema usa as informações de cobrança para atribuições no momento em que o cartão de taxa é finalizado ou se permite modificações com base em alterações durante o curso do projeto. Quaisquer alterações na função de trabalho, salário, cartão de taxa ou outras informações relacionadas ao faturamento do usuário não afetarão as taxas de faturamento das atribuições. As taxas são preservadas de acordo com o cartão de taxa final, no momento em que o sinalizador de projeto é ativado. Essas propriedades de atribuição (como função do cargo e salário) ainda são atualizadas, garantindo que o custo real da atribuição seja preciso.

Quando o sinalizador estiver ativado, o sistema bloqueará as taxas de cobrança de data efetiva (definidas no cartão de taxa finalizado anexado ao projeto) para a duração do projeto.

O sinalizador pode ser ativado em um projeto quando o trabalho foi iniciado e as atribuições e horas já existem. Nesse momento:

* A taxa final do cartão de taxa aprovada torna-se a origem das taxas de faturamento para todas as atribuições do projeto.
* Todas as atribuições passadas, atuais e futuras são recalculadas usando as taxas finais aprovadas.
* Os valores real e planejado são recalculados.

>[!NOTE]
>
>Quando o sinalizador estiver ativado para preservar as taxas de faturamento, ele não poderá ser desativado, a menos que o projeto não tenha atribuições e horas. Isto garante que todos os relatórios financeiros reflitam as taxas contratuais verdadeiras.
>Quando o sinalizador está desativado, o sistema permite que as taxas de cobrança sejam recalculadas ou ajustadas dinamicamente. Qualquer atualização na função, salário ou taxa de faturamento do usuário é refletida imediatamente na taxa de faturamento da atribuição.

Para obter mais informações, consulte [Editar projetos](/help/quicksilver/manage-work/projects/manage-projects/edit-projects.md) e [Gerenciar cartões de taxa](/help/quicksilver/administration-and-setup/manage-enterprise-operations/manage-rate-cards.md).

## Receita planejada - Usuário e função por hora

Quando o tipo de receita na tarefa é Usuário e Função por hora, o Workfront usa as hierarquias de taxa de função de usuário e de cargo para determinar a taxa de faturamento para a receita planejada.

Esta imagem mostra o fluxo da hierarquia de receita planejada:

![Receita planejada para o tipo de receita por hora de usuário e função](assets/planned-revenue-chart.png)

Quando um usuário é atribuído à tarefa, o Workfront pesquisa de acordo com essa hierarquia:

1. Primeiro, o sistema procura uma taxa preservada na atribuição para o usuário.

   Uma taxa preservada ainda segue a hierarquia, mas a taxa é congelada quando o projeto é preservado. Para obter mais informações, consulte [Visão geral das taxas preservadas](#overview-of-preserved-rates).

1. Em seguida, o sistema procura a taxa de faturamento em um cartão de taxa, para a função de trabalho principal ou a função de trabalho para faturamento do usuário atribuído à tarefa. Se existir uma taxa e ela estiver bloqueada, essa taxa será usada no cálculo da receita.

   Se existir uma taxa no cartão de taxa e ela estiver desbloqueada, o sistema não usará essa taxa e pesquisará a próxima taxa na hierarquia.

1. Em seguida, o sistema procura a taxa de substituição no nível da atribuição para o usuário. Essa é uma taxa adicionada manualmente vinculada à atribuição específica e substitui todas as outras taxas para o usuário nessa atribuição (exceto uma taxa bloqueada de cartão de taxa). Se uma taxa for encontrada, ela será usada no cálculo da receita.
1. Em seguida, o sistema procura uma função de trabalho para faturamento no nível de atribuição da tarefa.

   A função de trabalho para faturamento é apenas para uma atribuição específica e se aplica à atribuição em vez da taxa de função de trabalho principal do usuário. Por exemplo, a função de trabalho principal de um usuário é Designer, mas em uma tarefa ele está agindo como um Designer sênior com uma taxa de cobrança mais alta.

   A Workfront procura a função de trabalho para a taxa de cobrança:

   * Primeiro, o sistema procura a taxa de faturamento da função de trabalho para faturamento a partir da atribuição (Designer Sênior no exemplo), levando em conta as datas de efetivação. Você verá isso na área Taxas > Faturamento do projeto, em um agrupamento **Rate Source: Overrides > Resource Type: Job Role**. Essa é uma taxa de substituição no projeto.
   * Em seguida, o sistema procura a função de trabalho para a taxa de faturamento em um cartão de taxa, levando em conta as datas de efetivação. Você verá isso na área Taxas > Faturamento do projeto, em um agrupamento **Rate Source: Attached Rate Card > Tipo de recurso: função de trabalho**.
   * Se a taxa da função de trabalho para faturamento não estiver no projeto ou no cartão de taxa, o sistema procurará a taxa da função de trabalho no nível do sistema (Designer Sênior no exemplo), levando em conta as datas de efetivação.
   * Se uma função de trabalho para faturamento for atribuída, e nenhuma das taxas das etapas anteriores for encontrada, a taxa de faturamento será 0.

     >[!NOTE]
     >
     >Quando uma função de trabalho para faturamento é atribuída, mas a taxa de faturamento é 0, isso é um indicador para revisitar a configuração da taxa. Uma taxa de 0 significa que nenhuma taxa para essa função de trabalho (Designer sênior no exemplo) foi configurada no Workfront. Você deve adicionar taxas à função de trabalho ou excluir a função de trabalho para faturamento da atribuição.
     >
     >Como as tarefas herdam taxas de função de trabalho do projeto quando essas taxas estão disponíveis no nível do projeto, quaisquer taxas de uma pesquisa da função de trabalho para faturamento no projeto já teriam sido localizadas quando o Workfront pesquisou a função de trabalho para faturamento no nível de atribuição da tarefa. A pesquisa no nível do projeto para uma função de trabalho para faturamento ainda permanece na hierarquia de pesquisa.

1. Se uma função de trabalho para faturamento não estava disponível no nível de atribuição de tarefa, o sistema procura a taxa de faturamento no projeto para o usuário específico atribuído à tarefa, levando em conta as datas de efetivação. Você verá isso na área Taxas > Faturamento do projeto, em um agrupamento **Rate Source: Overrides > Resource Type: User**. Essa é uma taxa de substituição no projeto.
1. Em seguida, o sistema procura a taxa de cobrança no nível do sistema no perfil do usuário, levando em conta as datas de efetivação.
1. Em seguida, o sistema procura a taxa de faturamento da função de trabalho principal do usuário (Designer no exemplo).

   * Primeiro, o sistema procura a taxa de faturamento no projeto, para a função de trabalho principal do usuário, levando em conta as datas de efetivação. Você verá isso na área Taxas > Faturamento do projeto, em um agrupamento **Rate Source: Overrides > Resource Type: Job Role**. Essa é uma taxa de substituição no projeto.
   * Em seguida, o sistema procura a taxa de função de trabalho em uma tabela de taxas, levando em conta as datas de efetivação. Você verá isso na área Taxas > Faturamento do projeto, em um agrupamento **Rate Source: Attached Rate Card > Tipo de recurso: função de trabalho**.
   * Em seguida, o sistema procura a taxa de funções de trabalho no nível do sistema, levando em conta as datas de efetivação.

1. Se nenhuma dessas taxas for encontrada, a taxa de cobrança será 0.

Quando um usuário não está atribuído à tarefa, o Workfront pesquisa as taxas de função de trabalho de acordo com esta hierarquia:

1. Primeiro, o sistema procura uma taxa preservada na atribuição da função de trabalho.
1. O sistema procura a taxa de cobrança em um cartão de taxa, para a função de trabalho atribuída à tarefa. Se existir uma taxa e ela estiver bloqueada, essa taxa será usada no cálculo da receita.

   Se existir uma taxa no cartão de taxa e ela estiver desbloqueada, o sistema não usará essa taxa e pesquisará a próxima taxa na hierarquia.

1. Em seguida, o sistema procura a taxa de substituição de tarefa de atribuição para a função de trabalho. Essa é uma taxa adicionada manualmente para a função de trabalho na atribuição específica e substitui todas as outras taxas para a função de trabalho nessa tarefa. Se uma taxa for encontrada, ela será usada no cálculo da receita.
1. Em seguida, o sistema procura a taxa de faturamento da função de trabalho atribuída à tarefa.

   * Primeiro, o sistema procura a taxa de faturamento no projeto para a função de trabalho, levando em conta as datas de efetivação. Você verá isso na área Taxas > Faturamento do projeto, em um agrupamento **Rate Source: Overrides > Resource Type: Job Role**. Essa é uma taxa de substituição no projeto.
   * Em seguida, o sistema procura a taxa de função de trabalho em uma tabela de taxas, levando em conta as datas de efetivação. Você verá isso na área Taxas > Faturamento do projeto, em um agrupamento **Rate Source: Attached Rate Card > Tipo de recurso: função de trabalho**.
   * Em seguida, o sistema procura a taxa de funções de trabalho no nível do sistema, levando em conta as datas de efetivação.

1. Se nenhuma dessas taxas for encontrada, a taxa de cobrança será 0.

## Receita real - Usuário e função por hora

Quando o tipo de receita na tarefa é Usuário e Função por hora, o Workfront usa duas hierarquias para determinar a taxa de faturamento da receita real. A taxa de cobrança é baseada nas horas de logon do usuário em uma tarefa.

O &quot;usuário&quot; nas hierarquias é a pessoa atribuída à tarefa. O &quot;proprietário&quot; é a pessoa cujo tempo é registrado na tarefa, mesmo que não esteja atribuído à tarefa. Por exemplo, Michael é atribuído a uma tarefa, mas Joanna conclui o trabalho porque Michael estava doente. O gerente pode registrar o tempo na tarefa e definir o proprietário das horas reportadas como Joanna. Os valores de receita Planejada são baseados na atribuição e na taxa de Michael na hierarquia, mas os valores de receita Real são baseados na taxa de Joanna.

Esta imagem mostra o fluxo da hierarquia de receita real:

![Receita atual do tipo de custo por hora de usuário e função](assets/actual-revenue-chart.png)

### Quando o proprietário das horas reportadas e o usuário atribuído na tarefa são os mesmos

O Workfront pesquisa primeiro uma taxa de faturamento por atribuição do usuário. Se um usuário não estiver atribuído à tarefa, ele procurará uma taxa de faturamento pela atribuição de função de trabalho.

A hierarquia deste cenário é igual à hierarquia de receita planejada. Consulte [Receita planejada - Usuário e Função por hora](#planned-revenue--user-and-role-hourly) para este fluxo de trabalho.

### Quando o proprietário das horas reportadas não for o usuário atribuído na tarefa

O Workfront pesquisa nas propriedades do usuário do proprietário de acordo com esta hierarquia:

1. Primeiro, o sistema procura uma taxa preservada na atribuição para o proprietário.
1. Em seguida, o sistema procura a taxa de cobrança em um cartão de taxa, para a função de trabalho principal do proprietário. Se existir uma taxa e ela estiver bloqueada, essa taxa será usada no cálculo da receita.

   Se existir uma taxa no cartão de taxa e ela estiver desbloqueada, o sistema não usará essa taxa e pesquisará a próxima taxa na hierarquia.

1. Em seguida, o sistema procura a taxa de faturamento no projeto, para o proprietário, levando em conta as datas de efetivação. Você verá isso na área Taxas > Faturamento do projeto, em uma Source de Taxa: Sobreposições > Tipo de Recurso: Agrupamento de usuários. Essa é uma taxa de substituição no projeto.
1. Em seguida, o sistema procura uma função de trabalho para faturamento no nível do projeto.

   A função de trabalho para faturamento é somente para um projeto específico e se aplica ao projeto em vez da taxa de função de trabalho principal do proprietário. Por exemplo, a função de trabalho principal do proprietário é Designer, mas em um projeto ele está agindo como um Designer Sênior com uma taxa de cobrança mais alta.

   A Workfront procura a função de trabalho para a taxa de cobrança:

   * Primeiro, o sistema procura a função de trabalho para taxa de faturamento em um cartão de taxa, levando em conta as datas de efetivação. Você verá isso na área Taxas > Faturamento do projeto, em um agrupamento **Rate Source: Attached Rate Card > Tipo de recurso: função de trabalho**.
   * Se a taxa da função de trabalho para faturamento não estiver no cartão de taxa, o sistema procurará a taxa da função de trabalho no nível do sistema (Designer Sênior no exemplo), levando em conta as datas de efetivação.
   * Se uma função de trabalho para faturamento for atribuída, e nenhuma das taxas das etapas anteriores for encontrada, a taxa de faturamento será 0.

     >[!NOTE]
     >
     >Quando uma função de trabalho para faturamento é atribuída, mas a taxa de faturamento é 0, isso é um indicador para revisitar a configuração da taxa. Uma taxa de 0 significa que nenhuma taxa para essa função de trabalho (Designer sênior no exemplo) foi configurada no Workfront. Você deve adicionar taxas à função de trabalho ou excluir a função de trabalho para faturamento do projeto.

1. Em seguida, o sistema procura a taxa de faturamento no nível do sistema no perfil de usuário do proprietário, levando em conta as datas de efetivação.
1. Em seguida, o sistema procura a taxa de faturamento da função de trabalho principal do proprietário (Designer no exemplo).

   * Primeiro, o sistema procura a taxa de faturamento no projeto, para a função de trabalho principal do proprietário, levando em conta as datas de efetivação. Você verá isso na área Taxas > Faturamento do projeto, em um agrupamento **Rate Source: Overrides > Resource Type: Job Role**. Essa é uma taxa de substituição no projeto.
   * Em seguida, o sistema procura a taxa de função de trabalho em uma tabela de taxas, levando em conta as datas de efetivação. Você verá isso na área Taxas > Faturamento do projeto, em um agrupamento **Rate Source: Attached Rate Card > Tipo de recurso: função de trabalho**.
   * Em seguida, o sistema procura a taxa de funções de trabalho no nível do sistema, levando em conta as datas de efetivação.

1. Se nenhuma dessas taxas for encontrada, a taxa de cobrança será 0.

## Custo planejado - Usuário e Função por hora

Quando o tipo de custo na tarefa é Usuário e Função por hora, o Workfront usa as hierarquias de taxa de usuário e função de trabalho para determinar a taxa para o custo planejado.

Esta imagem mostra o fluxo da hierarquia de custos planejada:

![Custo Planejado para o tipo de custo por hora Usuário e Função](assets/planned-cost-chart.png)

Quando um usuário é atribuído à tarefa, o Workfront pesquisa de acordo com essa hierarquia:

1. O sistema procura a taxa de substituição de tarefa de atribuição para o usuário. Essa é uma taxa adicionada manualmente para o usuário na atribuição específica e substitui todas as outras taxas para o usuário nessa tarefa. Se uma taxa for encontrada, ela será usada no cálculo de custos.
1. Em seguida, o sistema procura a taxa de custo no projeto, para o usuário específico atribuído à tarefa, levando em conta as datas de efetivação. Você verá isso na área Taxas > Custo do projeto, em um agrupamento **Taxa Source: Substituições > Tipo de recurso: Usuário**. Essa é uma taxa de substituição no projeto.
1. Em seguida, o sistema procura a taxa de custo no nível do sistema no perfil do usuário, considerando as datas de efetivação.
1. Em seguida, o sistema procura a taxa de custo da função de trabalho principal do usuário com a combinação de atributos atribuída, com base na pontuação do atributo.
1. Se nenhuma dessas taxas for encontrada, a taxa de custo será 0.

Quando um usuário não está atribuído à tarefa, o Workfront pesquisa as taxas de custo da função de trabalho de acordo com esta hierarquia:

1. O sistema procura a taxa de substituição de tarefa de atribuição para a função de trabalho. Essa é uma taxa adicionada manualmente para a função de trabalho na atribuição específica e substitui todas as outras taxas para a função de trabalho nessa tarefa. Se uma taxa for encontrada, ela será usada no cálculo de custos.
1. Em seguida, o sistema procura a taxa de custo da função de trabalho no nível do sistema com a combinação de atributos atribuída, com base na pontuação do atributo, considerando as datas de efetivação.
1. Se nenhuma dessas taxas for encontrada, a taxa de custo será 0.

## Custo real - Usuário e Função por hora

Quando o tipo de custo na tarefa é Usuário e Função por hora, o Workfront usa duas hierarquias para determinar a taxa de faturamento para o custo real. A taxa de cobrança é baseada nas horas de logon do usuário em uma tarefa.

O &quot;usuário&quot; nas hierarquias é a pessoa atribuída à tarefa. O &quot;proprietário&quot; é a pessoa cujo tempo é registrado na tarefa, mesmo que não esteja atribuído à tarefa. Por exemplo, Michael é atribuído a uma tarefa, mas Joanna conclui o trabalho porque Michael estava doente. O gerente pode registrar o tempo na tarefa e definir o proprietário das horas reportadas como Joanna. Os valores de receita Planejada são baseados na atribuição e na taxa de Michael na hierarquia, mas os valores de receita Real são baseados na taxa de Joanna.

Esta imagem mostra o fluxo da hierarquia de custo real:

![Custo Efetivo do tipo de custo por Hora do Usuário e da Função](assets/actual-cost-chart.png)

### Quando o proprietário das horas reportadas e o usuário atribuído na tarefa são os mesmos

O Workfront pesquisa primeiro uma taxa de custo por atribuição do usuário. Se um usuário não estiver atribuído à tarefa, ele procurará uma taxa de custo pela atribuição da função de trabalho.

A hierarquia para este cenário é a mesma que a hierarquia de custo planejado. Consulte [Custo planejado - Usuário e Função por hora](#planned-cost--user-and-role-hourly) para este fluxo de trabalho.

### Quando o proprietário das horas reportadas não for o usuário atribuído na tarefa

O Workfront pesquisa nas propriedades do usuário do proprietário de acordo com esta hierarquia:

1. O sistema procura a taxa de custo no projeto, para o proprietário, levando em conta as datas efetivas. Você verá isso na área Taxas > Custo do projeto, em um agrupamento **Taxa Source: Substituições > Tipo de recurso: Usuário**. Essa é uma taxa de substituição no projeto.
1. Em seguida, o sistema procura a taxa de custo no nível do sistema no perfil de usuário do proprietário, levando em conta as datas de efetivação.
1. Em seguida, o sistema procura a taxa de custo da função de trabalho principal do proprietário (Designer no exemplo).

   * Primeiro, o sistema procura a taxa de custo no projeto, para a função de trabalho principal do proprietário, considerando as datas de efetivação. Você verá isso na área Taxas > Custo do projeto, em um agrupamento **Taxa Source: Substituições > Tipo de recurso: Função de trabalho**. Essa é uma taxa de substituição no projeto.
   * Em seguida, o sistema procura a taxa de função de trabalho em uma tabela de taxas, levando em conta as datas de efetivação. Você verá isso na área Taxas > Custo do projeto, em um agrupamento **Rate Source: Attached Rate Card > Tipo de Recurso: Função de Trabalho**.
   * Em seguida, o sistema procura a taxa de funções de trabalho no nível do sistema, levando em conta as datas de efetivação.

1. Se nenhuma dessas taxas for encontrada, a taxa de cobrança será 0.

