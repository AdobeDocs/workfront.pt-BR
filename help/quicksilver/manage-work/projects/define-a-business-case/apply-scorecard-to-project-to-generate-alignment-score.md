---
navigation-topic: business-case-and-scorecards
title: Aplicar um cartão de pontuação a um projeto e gerar uma Pontuação de alinhamento
description: Você pode usar um cartão de pontuação para medir como um projeto se alinha aos critérios estabelecidos anteriormente de um portfólio. Um cartão de pontuação geralmente reflete a missão, os valores e os objetivos estratégicos de uma organização.
author: Alina
feature: Work Management
exl-id: 21cf5493-147d-4b8d-8b16-2891eb7e0491
source-git-commit: 14b6b9c4a184131cfdc33b6156c578218ed9119a
workflow-type: tm+mt
source-wordcount: '1208'
ht-degree: 0%

---

# Aplicar um cartão de pontuação a um projeto e gerar uma Pontuação de alinhamento

<!-- Audited: 06/2025 -->

Você pode usar um cartão de pontuação para medir como um projeto se alinha aos critérios estabelecidos anteriormente de um portfólio. Um cartão de pontuação geralmente reflete a missão, os valores e os objetivos estratégicos de uma organização.

Para obter mais informações sobre cartões de pontuação e como criar um, consulte [Criar um cartão de pontuação](../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-scorecard.md).

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront*</td> 
   <td>
   <p>Atual: Prime ou superior</p>
   <p>ou</p>
   <p>Herdados: Business ou superior</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td>
   <p>Atual: Padrão</p>
   <p>ou</p>
   <p>Herdados: plano</p></td>  
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Editar acesso a projetos</p> <p>Visualização ou maior acesso a portfólios</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td><p>Gerenciar permissões para um projeto</p> <p>Exibir ou aumentar as permissões de um portfólio</p> </td> 
  </tr> 
 </tbody> 
</table>

*Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Cartões de pontuação do projeto {#project-scorecards}

* [Visão geral dos scorecards](#scorecards-overview)
* [Aplicar um cartão de pontuação a um projeto](#apply-a-scorecard-to-a-project)

### Visão geral dos Scorecards {#scorecards-overview}

Normalmente, um gerente de projeto conclui as informações do cartão de pontuação para produzir um valor de alinhamento entre 0 e 100 para o projeto. O valor produzido é usado posteriormente quando o gerente de portfólio revisa os projetos no otimizador de portfólio para compará-los.

Para obter mais informações sobre otimização de portfólio, consulte [Visão geral do Portfolio Otimizer](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md).

### Aplicar um cartão de pontuação a um projeto

Como um usuário com uma licença Padrão ou de Plano e permissões de Gerenciamento para um projeto, você pode anexar um cartão de pontuação ao projeto.

Para obter mais informações sobre permissões de projeto, consulte [Compartilhar um projeto no Adobe Workfront](../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).

Você pode adicionar scorecards a um projeto como parte da criação do business case do projeto.

Para obter mais informações sobre a criação de um business case, consulte [Criar um business case para um projeto](../../../manage-work/projects/define-a-business-case/create-business-case.md).

O administrador do Adobe Workfront ou o administrador de grupo deve ativar a seção Scorecard na área Business Case dos projetos antes que você possa acessar scorecards do Business Case. Para obter informações sobre como configurar preferências de projeto e habilitar áreas do Business Case, consulte [Configurar preferências de projeto do sistema inteiro](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

Para aplicar um cartão de pontuação a um projeto:

1. Vá para um projeto ao qual deseja aplicar um cartão de pontuação.
1. Clique em **Business Case** no painel esquerdo.
1. Localize a seção **Scorecard** do Business Case.\
   Você deve criar um scorecard antes que a seção **Scorecard** seja exibida no Business Case.

   Para obter informações sobre como criar um cartão de pontuação, consulte [Criar um cartão de pontuação](../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-scorecard.md).

1. Selecione um scorecard no menu suspenso.

   <!--![New scorecard](assets/new-scorecard.png)-->

1. Insira uma resposta para todas as perguntas no cartão de pontuação.

   O Workfront aplica uma pontuação a cada pergunta respondida e calcula a pontuação geral do projeto com base na pontuação individual de cada pergunta.

   Para obter mais informações sobre como gerar a pontuação de alinhamento geral do projeto, consulte [Gerar uma Pontuação de Alinhamento para um projeto](#generate-an-alignment-score-for-a-project).

1. Clique em **Salvar** para salvar o cartão de pontuação e pontuar o projeto.

   O cartão de pontuação agora está associado ao projeto e o projeto é pontuado.

<!--This functionality was removed when we redesigned bulk editing projects with 23.2: 

1. (Conditional) When changes occur in the values of scorecard questions, you must recalculate the scorecard to reflect the new values for the project score. To recaulate the scorecard, do the following: 

   1. Go to a list of projects and select all projects in the list. 
   1. Click the **Edit** icon at the top of the list. 
   1. Click **Settings** in the left panel, then check the **Recalculate Scorecards** option at the end of the Settings area. 
   1. Click Save. This recalculates the score value based on the scorecards attached for all the selected projects.  

      >[!NOTE]
      >
      >   The option to recalculate scorecards has been removed from the Preview environment, when editing projects in bulk. 

-->

## Gerar uma pontuação de alinhamento

* [Gerar uma Pontuação de Alinhamento para um projeto](#generate-an-alignment-score-for-a-project)
* [Gerar uma Pontuação de alinhamento para um portfólio](#generate-an-alignment-score-for-a-portfolio)

### Gerar uma pontuação de alinhamento para um projeto {#generate-an-alignment-score-for-a-project}

A pontuação de alinhamento é o valor produzido após concluir o cartão de pontuação.

Os cartões de pontuação contêm perguntas com opções de resposta que receberam valores numéricos, chamados de pontos de alinhamento. Esses pontos são usados para determinar o alinhamento do projeto com a organização. Os pontos de alinhamento de cada pergunta contêm um número entre 0 e 100.

Quando o cartão de pontuação é concluído, o Workfront calcula a pontuação de alinhamento do projeto como uma porcentagem, usando a seguinte fórmula:

`Project Alignment Score = The sum of the question points from the scorecard met at a given time / The sum of the possible points on the scorecard`

Para obter mais informações, consulte [Criar um cartão de pontuação](../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-scorecard.md).

### Gerar uma Pontuação de alinhamento para um portfólio {#generate-an-alignment-score-for-a-portfolio}

A pontuação de alinhamento do portfólio é uma média das pontuações de alinhamento de todos os projetos no portfólio.

Quando os scorecards dos projetos são concluídos, o Workfront usa esses valores para calcular a pontuação de alinhamento do portfólio como uma porcentagem, usando a seguinte fórmula:

`Portfolio Alignment Score = The sum of the percentages of the project alignment scores / Number of projects in the portfolio`

>[!NOTE]
>
>Se um projeto não tiver um cartão de pontuação associado a ele e, portanto, não tiver uma pontuação de alinhamento, ele será considerado como tendo um alinhamento de 0% no portfólio. O projeto é considerado no número de projetos no portfólio.

## Exibir a Pontuação do Alinhamento

Você pode visualizar a pontuação de alinhamento de um projeto no nível do projeto ou no Portfolio Otimizer.

* [Exibir a Pontuação de Alinhamento em um projeto](#view-the-alignment-score-on-a-project)
* [Exibir as pontuações de alinhamento do projeto e do portfólio no Portfolio Otimizer](#view-the-alignment-scores-of-the-project-and-of-the-portfolio-in-the-portfolio-optimizer)

### Exibir a pontuação de alinhamento em um projeto

Você pode visualizar a pontuação de alinhamento de um projeto no nível do projeto se tiver direitos de Contribute para o projeto.

1. Vá para o projeto cuja Pontuação de alinhamento você deseja exibir.
1. Clique em **Business Case** no painel esquerdo.
1. Vá para o **Resumo do Business Case** no lado direito da tela.

   A Pontuação de alinhamento está localizada no Resumo de business case, no valor **Aligned**.

   <!--![Alignment score on a project](assets/alignment-score-on-a-project.png)-->

### Exibir as pontuações de alinhamento do projeto e do portfólio no Portfolio Otimizer

Você pode visualizar a pontuação de alinhamento de um projeto ou de um portfólio no Portfolio Otimizer, se tiver acesso de Gerenciamento ao portfólio.

Para obter mais informações sobre as informações exibidas no Portfolio Otimizer, consulte [visão geral do Portfolio Otimizer](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md).

* [Localizar a Pontuação de Alinhamento do projeto no Portfolio Otimizer](#locate-the-alignment-score-of-the-project-in-the-portfolio-optimizer)
* [Localize a Pontuação de alinhamento do portfólio no Portfolio Otimizer](#locate-the-alignment-score-of-the-portfolio-in-the-portfolio-optimizer)

  <!--![Alignment score in Portfolio Optimizer](assets/alignment-score-in-portfolio-optimizer.png)-->

#### Localizar a Pontuação de alinhamento do projeto no Portfolio Otimizer {#locate-the-alignment-score-of-the-project-in-the-portfolio-optimizer}

{{step1-to-portfolios}}

1. Clique no nome de um portfólio.
1. Clique em **Otimização do Portfolio** no painel esquerdo.

   O Portfolio Otimizer é exibido.

   A pontuação de alinhamento de um projeto é exibida como uma porcentagem na coluna **Alinhamento** do Portfolio Otimizer.

   Essa é a pontuação de alinhamento do projeto com base no cartão de pontuação associado ao projeto.

#### Localize a Pontuação de alinhamento do portfólio no Portfolio Otimizer  {#locate-the-alignment-score-of-the-portfolio-in-the-portfolio-optimizer}

{{step1-to-portfolios}}

1. Clique no nome de um portfólio.
1. Clique em **Otimização do Portfolio** no painel esquerdo.
1. Na parte superior do Portfolio Otimizer, encontre o valor **Alinhado**, bem como o medidor **Alinhamento**, que indica a pontuação de alinhamento do portfólio.

   Essa é a pontuação de alinhamento do portfólio.

   Para obter mais informações sobre como a pontuação de alinhamento de um portfólio é gerada, consulte [Gerar uma pontuação de alinhamento para um portfólio](#generate-an-alignment-score-for-a-portfolio).

## Visão geral da pontuação do Portfolio Otimizer

Há uma diferença entre a pontuação de alinhamento e a pontuação do otimizador de portfólio de um projeto.

A pontuação de alinhamento de um projeto é calculada com base nos pontos obtidos após concluir o cartão de pontuação. Essa pontuação é então usada para determinar a pontuação de alinhamento do portfólio. A pontuação de alinhamento é exibida como uma porcentagem.

A pontuação de alinhamento de um projeto é exibida na coluna **Alinhamento** do Portfolio Otimizer.

A pontuação do otimizador de portfólio é uma classificação calculada automaticamente no Portfolio Otimizer pela qual os projetos podem ser priorizados. A pontuação do otimizador de portfólio é exibida como um ícone de indicador acompanhado por um número e exibida na coluna **Score** do Portfolio Otimizer. Uma pontuação do Portfolio Otimizer é gerada somente quando todas as seções do Business Case são concluídas, exceto Metas.

Para obter mais informações sobre como criar um Business Case para um projeto, consulte [Criar um Business Case para um projeto](../../../manage-work/projects/define-a-business-case/create-business-case.md).

Para obter mais informações sobre como calcular a pontuação do otimizador de portfólio de um projeto, consulte [Visão geral da pontuação do Portfolio Otimizer](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-score.md).
