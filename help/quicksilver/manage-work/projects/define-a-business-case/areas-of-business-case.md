---
content-type: overview
navigation-topic: business-case-and-scorecards
title: Visão geral das áreas do business case
description: Este artigo descreve as áreas do Business Case de um projeto.
author: Alina
feature: Work Management
exl-id: 0646e4f0-e8fb-48f2-b533-358229543081
source-git-commit: b38c98ec79617a78c76510bcb109da2ff83247af
workflow-type: tm+mt
source-wordcount: '1557'
ht-degree: 1%

---

# Visão geral das áreas de business case

<!-- Audited: 4/2025 -->

Este artigo descreve as áreas do Business Case de um projeto.

Para obter informações sobre como criar um Business Case para um projeto, consulte [Criar um Business Case para um projeto](../../../manage-work/projects/define-a-business-case/create-business-case.md).

O administrador do Adobe Workfront ou do grupo deve ativar todas as seções no Business Case antes que elas fiquem visíveis no projeto, exceto na seção Informações do projeto. A seção Informações do projeto é ativada por padrão.

Para obter mais informações sobre como habilitar as áreas do Business Case, consulte a seção Business Cases no artigo [Configurar preferências de projeto de todo o sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

Estas são as áreas no Business Case de um projeto:

* Informações do Projeto
* Metas
* Despesas
* Estimativa de Recurso
* Riscos
* Scorecard
* Formulários personalizados
* Resumo de Business Case

## Informações do Projeto

A seção Informações do projeto do Business Case inclui as informações básicas de um projeto antes que ele tenha sido realmente iniciado.

Todos os projetos têm uma área Informações do projeto no Business Case com campos predefinidos, o que significa que os administradores do Workfront não podem configurar quais campos aparecem nesta área.

Considere editar os seguintes campos:

* **Descrição**: adicione uma descrição para o projeto.

* **Proprietário do Projeto**: por padrão, o usuário que cria o projeto também é o Proprietário do Projeto. Edite esse campo para selecionar outro usuário ativo como o proprietário do projeto.

* **Patrocinador do Projeto**: selecione um usuário ativo que será o Patrocinador do Projeto. O patrocinador recebe a aprovação do Business Case.

* **Portfolio**: selecione uma Portfolio para o projeto. Você deve criar a Portfolio e colocá-la no status Ative (Ativo) antes que ela esteja disponível para seleção nesse menu suspenso.

  Para obter mais informações sobre portfólios, consulte [visão geral do Portfolio no Adobe Workfront](../../../manage-work/portfolios/portfolios-overview/portfolio-overview.md).

  Para obter mais informações sobre como criar Portfólios, consulte [Criar um portfólio](../../../manage-work/portfolios/create-and-manage-portfolios/create-portfolios.md).

* **Benefício Planejado**: estima qual será o benefício monetário planejado para sua organização quando este projeto for concluído. Pode ser qualquer valor em moeda e deve ser um valor positivo (por exemplo, US$ 10.000).

* **Status**: por padrão, o Status de uma solicitação de projeto é definido como Ideia. Se você alterar o Status para algo diferente de Ideia ou Planejamento, o botão Enviar desaparecerá da área Resumo de Business Case e você não poderá mais enviar o Business Case para aprovação.

* **Data de Início Fixa**: especifique uma data em que deseja que o projeto tenha início.

* **Data de Término Fixa**: especifique uma data quando desejar que o projeto termine.

  >[!NOTE]
  >
  >As Datas de Início e Término Fixas no Business Case não afetam as Datas de Início e Término Planejadas do projeto. Representam as datas solicitadas pelo criador do projeto para quando o projeto seria desenvolvido de preferência. Em vez disso, as Datas de início planejadas e de conclusão planejada do projeto mostram a linha do tempo planejada para o projeto, que se baseia nas tarefas do projeto.

## Metas

Metas definem os objetivos do projeto. Essa área é ativada por padrão no Business Case, mas o administrador do Workfront pode optar por não exibi-la. Este campo exibe as metas em ordem de prioridade.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: below snippet: NWE only, not classic)</p>
-->

>[!TIP]
>
>Você pode criar metas estratégicas para sua organização que não estejam conectadas ao Business Case individual de um projeto. Você deve ter acesso às Metas do Adobe Workfront para criar metas estratégicas. Você pode conectá-los a projetos fora do Business Case. Para obter informações sobre como criar metas usando as Metas do Workfront, consulte [Visão geral das Metas do Adobe Workfront](../../../workfront-goals/goal-management/wf-goals-overview.md).

A definição das metas é opcional para que o projeto receba uma Pontuação no Portfolio Otimizer. Esta seção é a única seção opcional no Business Case. Todas as outras seções do Business Case devem ser concluídas antes que o projeto seja pontuado no Portfolio Otimizer. É possível indicar um nível de prioridade para uma meta ao criá-la.

Para obter mais informações, consulte [Criar metas do Business Case](../../../manage-work/projects/define-a-business-case/create-business-case-goals.md).

## Despesas

As despesas representam os custos não mão de obra que podem ser incorridos durante a vida útil de um projeto. Essa área é ativada por padrão no Business Case, mas o administrador do Workfront pode optar por não exibi-la.

Quaisquer despesas informadas no Business Case também são inseridas como Despesas Planejadas na guia Despesas do projeto.

As despesas afetam os seguintes campos no projeto:

* Custo Orçado
* Valor líquido

O administrador do Workfront pode configurar Tipos de Despesas personalizados.

Para obter mais informações sobre os Custos Orçados e Valores Líquidos, consulte [Visão geral dos campos financeiros do Business Case](../../../manage-work/projects/define-a-business-case/business-case-finances.md).

Para obter mais informações sobre despesas, consulte [Gerenciar despesas do projeto](../../../manage-work/projects/project-finances/manage-project-expenses.md).

Para obter mais informações sobre como criar Tipos de Despesas personalizados, consulte [Criar tipos de despesas personalizados](../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-custom-expense-types.md).

## Estimativa de Recurso

Você pode executar as seguintes ações na área Orçamento de Recursos do Business Case:

* Associar Conjuntos de Recursos ao projeto.
* Estime seus recursos no nível do projeto.

As horas orçadas para os recursos do projeto são exibidas na área Orçamento de Recursos do Business Case, gerando o Custo de Mão de obra Orçado do projeto. Essa área é ativada por padrão.

Para obter mais informações sobre recursos de orçamento para o projeto no Business Case, consulte [Recursos de orçamento no Business Case](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md).

![Orçamento de recursos do Business Case](assets/business-case-sp-selected-with-choose-button-350x121.png)

Considere o seguinte ao exibir a seção Orçamento de Recursos do Business Case:

* É possível orçar informações de recursos aqui usando as seguintes ferramentas:

   * O Planejador de Recursos

     Para obter informações, consulte [Recursos de orçamento no Business Case usando o Planejador de Recursos](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case-use-resource-planner.md).

   * O Planejador de cenários

     Para obter mais informações, consulte [Recursos de orçamento no Business Case usando o Planejador de Cenários](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case-use-scenario-planner.md).

     O Planejador de cenários está disponível somente na nova experiência do Adobe Workfront e requer uma licença adicional. Para obter informações sobre o Planejador de cenários do Workfront, consulte [A visão geral do Planejador de cenários](../../../scenario-planner/scenario-planner-overview.md).

* As informações exibidas aqui também são exibidas no Planejador de recursos ou no Planejador de cenários no nível do sistema.

  <!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: the "or" stays in&nbsp;NWE&nbsp;only)<br></p>
  -->

* Depois de fazer o orçamento de seus recursos, o Custo de Mão de Obra Orçado do projeto será exibido na área Orçamento de Recursos se as funções estiverem associadas às taxas de Custo por Hora. O Custo do Trabalho Orçado é exibido na moeda do projeto.

  >[!IMPORTANT]
  >
  >O Custo do Trabalho Orçado é o custo associado às funções no projeto, e não aos usuários. A soma de todos os Custos de Trabalho Orçados para os usuários pode ou não ser igual ao Custo de Trabalho Orçado da função de trabalho associada aos usuários.

  Para obter mais informações sobre o Custo do Trabalho Orçado, consulte [Visão geral dos campos financeiros do Business Case](../../../manage-work/projects/define-a-business-case/business-case-finances.md).

  Para obter mais informações sobre como criar funções de trabalho e associar taxas de Custo por Hora a elas, consulte [Criar e gerenciar funções de trabalho](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

## Riscos

Os riscos são fatores que podem impedir que um projeto seja concluído no prazo ou dentro do orçamento. A definição desses fatores é importante para que o Gerente do Portfolio ou o Patrocinador do Projeto tome uma decisão bem fundamentada sobre a aprovação do projeto. Essa área é ativada por padrão no Business Case, mas o administrador do Workfront pode optar por não exibi-la.

Você pode associar um custo potencial aos riscos que estiver definindo, caso eles ocorram. O custo dos riscos afeta o valor líquido do projeto.

O administrador do Workfront pode configurar Tipos de risco personalizados.

Para obter mais informações sobre o Valor Líquido do projeto, consulte [Visão geral dos campos financeiros do Business Case](../../../manage-work/projects/define-a-business-case/business-case-finances.md).

Para obter mais informações sobre como criar riscos, consulte [Criar e editar riscos em projetos](../../../manage-work/projects/define-a-business-case/create-edit-risks-on-projects.md).

Para obter mais informações sobre como criar e editar Tipos de Risco personalizados, consulte [Editar e criar tipos de risco](../../../administration-and-setup/set-up-workfront/configure-system-defaults/edit-create-risk-types.md).

## Scorecard

Os scorecards medem o Alinhamento do projeto. Essa área é ativada por padrão no Business Case, mas o administrador do Workfront pode optar por não exibi-la.

Para aplicar um cartão de pontuação, o administrador do Workfront deve primeiro criar um. A área Scorecard do Business Case não será exibida a menos que um scorecard seja criado.

Para obter mais informações sobre como aplicar um cartão de pontuação a um projeto e gerar uma pontuação de alinhamento, consulte [Aplicar um cartão de pontuação a um projeto e gerar uma Pontuação de Alinhamento](../../../manage-work/projects/define-a-business-case/apply-scorecard-to-project-to-generate-alignment-score.md).

Para obter mais informações sobre como criar um cartão de pontuação, consulte [Criar um cartão de pontuação](../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-scorecard.md).

## Formulários personalizados

Você pode anexar um Forms personalizado a um projeto ao definir um Business Case. Essa área não é ativada por padrão no Business Case e o administrador do Workfront deve ativá-la para exibi-la no Business Case.

Para aplicar um formulário personalizado, o administrador do Workfront deve primeiro criar um.

Você pode usar formulários personalizados para coletar informações adicionais que não são exibidas em outros campos do Business Case.

Para obter mais informações sobre como habilitar as áreas do Business Case, consulte [Configurar preferências de projeto do sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

Para obter mais informações sobre como criar um formulário personalizado, consulte [Criar um formulário personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

Para obter mais informações sobre como aplicar um formulário personalizado, consulte [Anexar um formulário personalizado a um Business Case](../../../manage-work/projects/define-a-business-case/attach-custom-form-to-business-case.md).

## Resumo de Business Case

* [Visão Geral do Resumo de Business Case](#overview-of-the-business-case-summary)
* [Exportar o Business Case](#export-the-business-case)

### Visão Geral do Resumo de Business Case {#overview-of-the-business-case-summary}

Você pode ver um resumo das principais finanças do projeto e se um projeto está alinhado ou não a um Scorecard no painel Resumo do Business Case, que está localizado no canto superior direito do Business Case.

O Resumo de business case é apenas uma visualização rápida do estado do projeto, pois se relaciona aos campos financeiros e ao Scorecard, e não pode ser editado.

Os seguintes campos são exibidos no Resumo de Business case:

* O Valor Líquido do Projeto
* O Custo Orçado do Projeto
* O custo do risco potencial
* O benefício planejado
* A Pontuação do Alinhamento

Para obter mais informações sobre esses campos, consulte [Visão geral dos campos financeiros do Business Case](../../../manage-work/projects/define-a-business-case/business-case-finances.md).

### Exportar o Business Case {#export-the-business-case}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: made this into a standalone article, linked in the first paragraph of this section)</p>
-->

Você pode exportar o Business Case para um arquivo PDF se precisar imprimi-lo ou anexá-lo a um email em um formato mais condensado.

Para obter informações, consulte [Exportar o Business Case de um projeto](../../../manage-work/projects/define-a-business-case/export-business-case.md).

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

