---
content-type: overview
navigation-topic: business-case-and-scorecards
title: Visão geral das áreas do caso comercial
description: Este artigo descreve as áreas do Caso de negócios de um projeto.
author: Alina
feature: Work Management
exl-id: 0646e4f0-e8fb-48f2-b533-358229543081
source-git-commit: a849ecaf6097dcdc924aaab2867f37bf57d5bc09
workflow-type: tm+mt
source-wordcount: '1604'
ht-degree: 2%

---

# Visão geral das áreas do caso comercial

Este artigo descreve as áreas do Caso de negócios de um projeto.

Para obter informações sobre como criar um Caso de Negócios para um projeto, consulte [Criar um caso de negócios para um projeto](../../../manage-work/projects/define-a-business-case/create-business-case.md).

O administrador do Adobe Workfront ou o administrador do grupo deve habilitar todas as seções no Caso comercial antes que elas estejam visíveis no projeto, exceto na seção Informações do projeto . A seção Informações do projeto é ativada por padrão.

Para obter mais informações sobre como habilitar as áreas do Caso de negócios, consulte a seção &quot;Casos de negócios&quot; em  [Configurar preferências de projeto em todo o sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

Estas são as áreas no Caso de negócios de um projeto:

* Informações do Projeto
* Metas
* Despesas
* Estimativa de Recurso
* Riscos
* Scorecard
* Formulários personalizados
* Resumo de Business Case

## Informações do Projeto

O **Informações do projeto** A área do Caso de negócios não pode ser configurada pelo administrador do Workfront. Todos os projetos têm uma área Informações do projeto no Caso de negócios. 

A seção Informações do projeto do Caso de negócios inclui as informações básicas de um projeto, antes que o projeto realmente tenha iniciado.

Considere editar os seguintes campos:

* **Descrição**: Especifique uma descrição para o seu projeto.
* **Proprietário do projeto**

   Por padrão, o usuário que está criando o projeto também é o Proprietário do projeto. É possível editar esse campo e indicar outro usuário ativo como proprietário do projeto.

* **Patrocinador do projeto**

   Considere adicionar outra pessoa que não o Proprietário do projeto como Patrocinador do projeto. O patrocinador recebe a aprovação do Caso de negócios. 

* **Portfolio**: Especifique um Portfolio para o projeto. Você deve criar o Portfolio e colocá-lo no status de **Ativo** antes que esteja disponível, selecione neste menu suspenso.

   Para obter mais informações sobre portfólios, consulte [Visão geral do Portfolio no Adobe Workfront](../../../manage-work/portfolios/portfolios-overview/portfolio-overview.md).

   Para obter mais informações sobre como criar Portfolio, consulte [Criar um portfólio](../../../manage-work/portfolios/create-and-manage-portfolios/create-portfolios.md).

* **Benefício planejado**: Estime qual será o benefício monetário planejado para sua organização quando este projeto for concluído. Pode ser qualquer quantidade de moeda e deve ser um valor positivo. Por exemplo, US$ 10.000.
* **Status**: Por padrão, o Status de uma solicitação de projeto é definido como **Ideia**.

   Se você alterar o Status para algo diferente de Ideia ou Planejamento, a variável **Enviar** O botão desaparece da área Resumo do caso de negócios e não é mais possível enviar o Caso de negócios para aprovação. 

* **Data de início fixa**: Especifique uma data em que deseja que o projeto seja iniciado.
* **Data final fixa**: Especifique uma data em que deseja que o projeto termine.

   >[!NOTE]
   >
   >A Data inicial e final fixa no Caso de negócios não afeta as Datas inicial e de conclusão planejadas do projeto. Elas representam as datas solicitadas pelo criador do projeto para quando o projeto idealmente se desenvolveria. Em vez disso, as Datas de Início Planejado e de Conclusão Planejada do projeto mostram a linha do tempo planejada para o projeto, que se baseia nas tarefas do projeto.

## Metas

Os objetivos definem os objetivos do projeto. Essa área é ativada por padrão no Caso de negócios, mas o administrador do Workfront pode optar por não exibi-la. Este campo exibe as metas em ordem de prioridade.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: below snippet: NWE only, not classic)</p>
-->

>[!TIP]
Você pode criar metas estratégicas para sua organização que não estejam conectadas ao Caso de negócios individual de um projeto. Você deve ter acesso às Metas da Adobe Workfront para poder criar metas estratégicas. Em seguida, você pode conectá-los a projetos fora de seus Casos de negócios. Para obter informações sobre como criar metas usando metas do Workfront, consulte [Visão geral das Metas da Adobe Workfront](../../../workfront-goals/goal-management/wf-goals-overview.md).

A definição das metas é opcional para o projeto receber uma Pontuação no Portfolio Otimizer. Esta seção é a única seção opcional no Caso de negócios. Todas as outras seções do Caso de negócios devem ser concluídas antes que o projeto seja classificado no Portfolio Otimizer. Você pode indicar um nível de prioridade para uma meta enquanto cria a meta.

Para obter mais informações sobre metas, consulte  [Criar metas de caso de negócios](../../../manage-work/projects/define-a-business-case/create-business-case-goals.md).

## Despesas

As despesas representam os custos não laborais que podem ser incorridos durante a vida de um projeto. Essa área é ativada por padrão no Caso de negócios, mas o administrador do Workfront pode optar por não exibi-la. 

Qualquer despesa que você informar no Caso de Negócios também será informada na guia Despesas do projeto, como Despesas Planejadas.

As despesas afetam os seguintes campos no projeto:

* Custo Orçado
* Valor líquido

Para obter mais informações sobre os Custos Orçados e Valores Líquidos, consulte [Visão geral dos campos financeiros do Caso de negócios](../../../manage-work/projects/define-a-business-case/business-case-finances.md).

Para obter mais informações sobre despesas, consulte  [Gerenciar despesas do projeto](../../../manage-work/projects/project-finances/manage-project-expenses.md) .

O administrador do Workfront pode configurar Tipos de Despesa personalizados.

Para obter mais informações sobre como criar Tipos de Despesa personalizados, consulte [Criar tipos de despesas personalizadas](../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-custom-expense-types.md). 

## Estimativa de Recurso

Você pode executar as seguintes ações na área Orçamento de Recursos do Caso de Negócios:

* Associar Grupos de Recursos ao projeto.
* Faça o orçamento de seus recursos no nível do projeto.

As horas orçadas para os recursos do projeto são exibidas na área Orçamento de Recursos do Caso de Negócios, gerando o Custo de Mão-de-Obra Orçado do projeto. Essa área do Caso de negócios é ativada por padrão.

Para obter mais informações sobre como orçar recursos para o projeto no Caso de Negócios, consulte [Recursos orçamentários no Caso de Negócios](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md).

![](assets/business-case-sp-selected-with-choose-button-350x121.png)

Considere o seguinte ao exibir a seção Orçamento de Recursos do Caso de Negócios:

* Você pode orçar informações de recursos aqui usando as seguintes ferramentas:

   * O Planejador de recursos

      Para obter mais informações, consulte [Recursos de orçamento no Caso de negócios usando o Planejador de recursos](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case-use-resource-planner.md).

   * O Planejador de Cenário , se sua empresa adquiriu uma licença adicional para o Planejador de Cenário do Adobe

      Para obter mais informações, consulte [Recursos de orçamento no Caso de negócios usando o Planejador de cenário](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case-use-scenario-planner.md).

      O Planejador de cenário está disponível somente na nova experiência do Adobe Workfront e requer uma licença adicional. Para obter informações sobre o Planejador de Cenário do Workfront, consulte [A visão geral do Planejador de cenário](../../../scenario-planner/scenario-planner-overview.md).

* As informações exibidas aqui também são exibidas no Planejador de Recursos no nível do sistema ou no Planejador de Cenários. 

   <!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: the "or" stays in&nbsp;NWE&nbsp;only)<br></p>
  -->

* Depois de orçar seus recursos, o Custo da Mão-de-Obra Orçada do projeto é exibido na área de Orçamento de Recursos se as funções estiverem associadas às taxas de Custo por Hora. O Custo da Mão-de-Obra Orçada é exibido na moeda do projeto.

   >[!IMPORTANT]
   O Custo da Mão-de-Obra Orçada é o custo associado às funções no projeto, e não aos usuários. A soma de todos os Custos de Mão-de-Obra Orçados para os usuários pode ou não ser igual ao Custo de Mão-de-Obra Orçada da função de cargo associada aos usuários. 

   Para obter mais informações sobre o Custo da Mão de obra Orçada, consulte [Visão geral dos campos financeiros do Caso de negócios](../../../manage-work/projects/define-a-business-case/business-case-finances.md).

   Para obter mais informações sobre como criar funções de cargo e associar as taxas de Custo por Hora a elas, consulte [Criar e gerenciar funções de trabalho](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

## Riscos

Os riscos são fatores que podem impedir que um projeto termine a tempo ou no orçamento. A definição desses fatores é importante para o Portfolio Manager ou o Project Sponsor tomar uma decisão instruída sobre a aprovação do projeto. Essa área é ativada por padrão no Caso de negócios, mas o administrador do Workfront pode optar por não exibi-la.

Você pode associar um custo potencial aos riscos que está definindo caso ocorra. O custo dos riscos de um projeto afeta o valor líquido do projeto. 

Para obter mais informações sobre o Valor Líquido do projeto, consulte [Visão geral dos campos financeiros do Caso de negócios](../../../manage-work/projects/define-a-business-case/business-case-finances.md).

Para obter mais informações sobre como criar riscos, consulte  [Criar e editar riscos em projetos](../../../manage-work/projects/define-a-business-case/create-edit-risks-on-projects.md).

O administrador do Workfront pode configurar Tipos de risco personalizados.

Para obter mais informações sobre a criação e edição de Tipos de Risco personalizados, consulte [Editar e criar tipos de risco](../../../administration-and-setup/set-up-workfront/configure-system-defaults/edit-create-risk-types.md).

## Scorecard

Os scorecards avaliam o Alinhamento do projeto. Essa área é ativada por padrão no Caso de negócios, mas o administrador do Workfront pode optar por não exibi-la.

Para obter mais informações sobre como aplicar um scorecard a um projeto e gerar uma pontuação de alinhamento, consulte [Aplicar um scorecard a um projeto e gerar uma Pontuação de alinhamento](../../../manage-work/projects/define-a-business-case/apply-scorecard-to-project-to-generate-alignment-score.md).

Para aplicar um scorecard, o administrador do Workfront deve criar um. O **Scorecard** A área do Caso de negócios não é exibida, a menos que um scorecard seja criado.

Para obter mais informações sobre como criar um scorecard, consulte  [Criar um scorecard](../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-scorecard.md).

## Formulários personalizados

Você pode anexar Forms personalizado a um projeto, ao definir um Caso de negócios. Essa área não é habilitada por padrão no Caso de negócios. O administrador do Workfront deve habilitá-lo para exibi-lo no Caso de negócios.

Para obter mais informações sobre como habilitar as áreas do Caso de negócios, consulte [Configurar preferências de projeto em todo o sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

Para aplicar um formulário personalizado, o administrador do Workfront deve primeiro criar um formulário personalizado.

Para obter mais informações sobre como criar um formulário personalizado, consulte [Criar ou editar um formulário personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md) .

Você pode usar formulários personalizados para coletar informações adicionais que não são exibidas nos outros campos do Caso de negócios.

Para obter mais informações sobre como aplicar um formulário personalizado, consulte [Anexar um formulário personalizado a um caso de negócios](../../../manage-work/projects/define-a-business-case/attach-custom-form-to-business-case.md).

## Resumo de Business Case

* [Visão Geral do Resumo do Caso Comercial](#overview-of-the-business-case-summary)
* [Exportar o caso comercial](#export-the-business-case)

### Visão Geral do Resumo do Caso Comercial {#overview-of-the-business-case-summary}

Você pode ver um resumo das finanças do projeto principal e se um projeto está alinhado ou não a um Scorecard no painel Resumo do caso de negócios , no canto superior direito do Caso de negócios .

Não é possível editar o Resumo do Caso Comercial. Esta é apenas uma visualização rápida do estado do projeto, pois está relacionada aos campos financeiros e ao Scorecard. \
 

Os seguintes campos são exibidos no Resumo do Caso de Negócios:

* O Valor Líquido do Projeto
* O Custo Orçado do Projeto
* O Custo do Risco Potencial
* O benefício planejado
* A pontuação de alinhamento

Para obter mais informações sobre esses campos, consulte [Visão geral dos campos financeiros do Caso de negócios](../../../manage-work/projects/define-a-business-case/business-case-finances.md).

### Exportar o caso comercial {#export-the-business-case}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: made this into a standalone article, linked in the first paragraph of this section)</p>
-->

Você pode exportar o Business Case para um arquivo PDF, caso precise imprimi-lo ou anexá-lo a um email em um formato mais condensado. 

Para obter mais informações, consulte [Exportar o Caso de Negócios de um projeto](../../../manage-work/projects/define-a-business-case/export-business-case.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>To export a Business Case:</p>
<ol>
<li value="1">Go to the <strong>Business Case</strong> area of a project. </li>
<li value="2"> <p>In the<strong>Business Case Summary</strong> area, click <strong>Export</strong>.<br>A PDF file is downloaded to your computer. The file contains all areas of the Business Case in an easy to read format.</p> <p> <img src="assets/bc-summary-exported-350x160.png" alt="BC_Summary_exported.png" style="width: 350;height: 160;"> </p> </li>
<li value="3">(Optional) You can attach the PDF file to an email, or print it.&nbsp;</li>
</ol>
</div>
-->

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>You can export the Business Case to a PDF file, in case you need to print it or attach it to an email in a more condensed format.&nbsp; The file contains all areas of the Business Case in an easy to read format.</p>
<p>For information about how to export the Business Case, see <a href="../../../manage-work/projects/define-a-business-case/export-business-case.md" class="MCXref xref">Export the Business Case of a project </a></p> <!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: drafted and will replace the info above, when the standalone arrticle is live >> Becky!)</p>
-->
</div>
--&gt;
