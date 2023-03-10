---
navigation-topic: business-case-and-scorecards
title: Aplicar um cartão de pontuação a um projeto e gerar uma Pontuação de alinhamento
description: Você pode usar um cartão de pontuação para medir como um projeto se alinha aos critérios estabelecidos anteriormente de um portfólio. Um cartão de pontuação geralmente reflete a missão, os valores e os objetivos estratégicos de uma organização.
author: Alina
feature: Work Management
exl-id: 21cf5493-147d-4b8d-8b16-2891eb7e0491
source-git-commit: 921749caf6a61fa4f0efae9357c6e05c581421c5
workflow-type: tm+mt
source-wordcount: '1399'
ht-degree: 0%

---

# Aplicar um cartão de pontuação a um projeto e gerar uma Pontuação de alinhamento

Você pode usar um cartão de pontuação para medir como um projeto se alinha aos critérios estabelecidos anteriormente de um portfólio. Um cartão de pontuação geralmente reflete a missão, os valores e os objetivos estratégicos de uma organização.

Para obter mais informações sobre cartões de pontuação e como criar um, consulte [Criar um cartão de pontuação](../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-scorecard.md).

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront*</td> 
   <td> <p>Business ou superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Plano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a projetos</p> <p>Acesso de visualização ou superior ao Portfolio</p> <p>Observação: se você ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões para um projeto</p> <p>Exibir ou aumentar as permissões de um portfólio </p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir seu plano, tipo de licença ou acesso, entre em contato com o administrador do Workfront.

## Cartões de pontuação do projeto {#project-scorecards}

* [Visão geral dos Scorecards](#scorecards-overview)
* [Cartões de pontuação do projeto](#project-scorecards)

### Visão geral dos Scorecards {#scorecards-overview}

Normalmente, um gerente de projeto conclui as informações do cartão de pontuação para produzir um valor de alinhamento entre 0 e 100 para o projeto. O valor produzido é usado posteriormente quando o gerente de portfólio revisa os projetos no otimizador de portfólio para compará-los.

Para obter mais informações sobre otimização de portfólio, consulte o artigo [Visão geral do Portfolio Otimizer](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md).

### Aplicar um cartão de pontuação a um projeto

Como usuário com uma licença de Plano e permissões Gerenciar para um projeto, você pode anexar um cartão de pontuação ao projeto.

Para obter mais informações sobre permissões de projeto, consulte [Compartilhar um projeto no Adobe Workfront](../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).

Você pode adicionar scorecards a um projeto como parte da criação do business case do projeto.

Para obter mais informações sobre como criar um business case, consulte [Criar um Business Case para um projeto](../../../manage-work/projects/define-a-business-case/create-business-case.md).

O administrador do Adobe Workfront ou o administrador de grupo deve ativar a seção Scorecard na área Business Case dos projetos antes que você possa acessar scorecards do Business Case. Para obter informações sobre como configurar as preferências do projeto e ativar áreas do Business Case, consulte [Configurar preferências de projeto em todo o sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

Para aplicar um cartão de pontuação a um projeto:

1. Vá para um projeto ao qual deseja aplicar um cartão de pontuação.
1. Clique em **Business Case** no painel esquerdo.
1. Localize o **Scorecard** seção do Business Case.\
   Você deve criar um cartão de pontuação antes da variável **Scorecard** é exibida no Business Case.

   Para obter informações sobre como criar um cartão de pontuação, consulte [Criar um cartão de pontuação](../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-scorecard.md).

1. Selecione um scorecard no menu suspenso.

   ![new_scorecard.png](assets/new-scorecard-350x149.png)

1. Especifique uma resposta para todas as perguntas no cartão de pontuação.

   O Workfront aplica uma pontuação a cada pergunta respondida e calcula a pontuação geral do projeto com base na pontuação individual de cada pergunta.

   Para obter mais informações sobre como gerar a pontuação geral de alinhamento do projeto, consulte [Gerar uma pontuação de alinhamento para um projeto](#generate-an-alignment-score-for-a-project).

1. Clique em **Salvar** para salvar o cartão de pontuação e pontuar o projeto.

   O cartão de pontuação agora está associado ao projeto e o projeto é pontuado.

1. (Condicional) Quando ocorrem alterações nos valores das perguntas do scorecard, você deve recalcular o scorecard para refletir os novos valores para a pontuação do projeto. Para recalcular o cartão de pontuação, faça o seguinte:

   1. Vá para uma lista de projetos e selecione todos os projetos na lista.
   1. Clique em **Editar** no topo da lista.
   1. Clique em **Configurações** no painel esquerdo, verifique a **Recalcular Scorecards** no final da área Configurações.
   1. Clique em Salvar. Isso recalcula o valor da pontuação com base nos cartões de pontuação anexados para todos os projetos selecionados.

      >[!NOTE]
      >
      >   <span class="preview">A opção para recalcular cartões de pontuação foi removida do ambiente de Pré-visualização, ao editar projetos em massa. </span>


## Gerar uma pontuação de alinhamento

* [Gerar uma pontuação de alinhamento para um projeto](#generate-an-alignment-score-for-a-project)
* [Gerar uma Pontuação de alinhamento para um portfólio](#generate-an-alignment-score-for-a-portfolio)

### Gerar uma pontuação de alinhamento para um projeto {#generate-an-alignment-score-for-a-project}

A pontuação de alinhamento é o valor produzido após concluir o cartão de pontuação.

Os cartões de pontuação contêm perguntas com opções de resposta que receberam valores numéricos, chamados de pontos de alinhamento. Esses pontos são usados para determinar o alinhamento do projeto com a organização. Os pontos de alinhamento de cada pergunta contêm um número entre 0 e 100.

Quando o cartão de pontuação é concluído, o Workfront calcula a pontuação de alinhamento do projeto como uma porcentagem, usando a seguinte fórmula:

```
Project Alignment Score = The sum of the question points from the scorecard met at a given time/ The sum of the possible points on the scorecard
```

Para obter mais informações, consulte [Criar um cartão de pontuação](../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-scorecard.md).

### Gerar uma Pontuação de alinhamento para um portfólio {#generate-an-alignment-score-for-a-portfolio}

A pontuação de alinhamento do portfólio é uma média das pontuações de alinhamento de todos os projetos no portfólio.

Quando os scorecards dos projetos são concluídos, o Workfront usa esses valores para calcular a pontuação de alinhamento do portfólio como uma porcentagem, usando a seguinte fórmula:

Pontuação de alinhamento de Portfolio = A soma das porcentagens das pontuações de alinhamento do projeto/Número de projetos no portfólio

>[!NOTE]
>
>Se um projeto não tiver um cartão de pontuação associado a ele e, portanto, não tiver uma pontuação de alinhamento, ele será considerado como tendo um alinhamento de 0% no portfólio. O projeto é considerado no número de projetos no portfólio.

## Exibir a Pontuação do Alinhamento

Você pode visualizar a pontuação de alinhamento de um projeto no nível do projeto ou no Otimizador de Portfolio.

* [Exibir a pontuação de alinhamento em um projeto](#View%20the)
* [Exibir as Pontuações de Alinhamento do projeto e do portfólio no Otimizador de Portfolio](#View%20the2)

### Exibir a pontuação de alinhamento em um projeto

Você pode visualizar a pontuação de alinhamento de um projeto no nível do projeto se tiver direitos de Contribute para o projeto.

1. Vá para o projeto cuja Pontuação de alinhamento você deseja exibir.
1. Clique em **Business Case** no painel esquerdo.
1. Vá para a **Resumo de Business Case** no lado direito da tela.

   A Pontuação de alinhamento está localizada no Resumo de business case, no campo **Alinhado** valor.

   ![alignment_score_on_a_project.png](assets/alignment-score-on-a-project.png)

### Exibir as Pontuações de Alinhamento do projeto e do portfólio no Otimizador de Portfolio

Você pode visualizar a pontuação de alinhamento de um projeto ou de um portfólio no Otimizador de Portfolio, se tiver acesso de Gerenciamento ao portfólio.

Para obter mais informações sobre as informações exibidas no Otimizador de Portfolio, consulte [Visão geral do Portfolio Otimizer](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md).

* [Localize a Pontuação de alinhamento do projeto no Otimizador de Portfolio](#locate-the-alignment-score-of-the-project-in-the-portfolio-optimizer)
* [Localize a Pontuação de alinhamento do portfólio no Otimizador de Portfolio](#locate-the-alignment-score-of-the-portfolio-in-the-portfolio-optimizer)

   ![](assets/alignment-score-in-portfolio-optimizer-nwe-350x97.png)

#### Localize a Pontuação de alinhamento do projeto no Otimizador de Portfolio {#locate-the-alignment-score-of-the-project-in-the-portfolio-optimizer}

1. Clique em **Menu principal** ícone ![](assets/main-menu-icon.png), depois **Portfolio**.

1. Clique no nome de um Portfolio.
1. Clique em **Otimização de Portfolio** no painel esquerdo.

   O Otimizador de Portfolio é exibido.

1. A pontuação de alinhamento de um projeto é exibida como uma porcentagem na **Alinhamento** coluna do Otimizador de Portfolio.

   Essa é a pontuação de alinhamento do projeto com base no cartão de pontuação associado ao projeto.

#### Localize a Pontuação de alinhamento do portfólio no Otimizador de Portfolio  {#locate-the-alignment-score-of-the-portfolio-in-the-portfolio-optimizer}

1. Vá para a **Projetos** na barra de Navegação global.
1. Selecione o **Portfolio** guia.
1. Clique no nome de um Portfolio.
1. Selecione o **Otimização de Portfolio** guia.
1. Na parte superior do Otimizador de Portfolio, encontre **Alinhado** , bem como o **Alinhamento** medidor que indica a pontuação de alinhamento do portfólio.

   Essa é a pontuação de alinhamento do portfólio.

   Para obter mais informações sobre como a pontuação de alinhamento de um portfólio é gerada, consulte [Gerar uma Pontuação de alinhamento para um portfólio](#generate-an-alignment-score-for-a-portfolio).

## Visão geral da pontuação do Portfolio Otimizer

Há uma diferença entre a pontuação de alinhamento e a pontuação do otimizador de portfólio de um projeto.

A pontuação de alinhamento de um projeto é calculada com base nos pontos obtidos após concluir o cartão de pontuação. Essa pontuação é então usada para determinar a pontuação de alinhamento do portfólio. A pontuação de alinhamento é exibida como uma porcentagem.

A pontuação de alinhamento de um projeto é exibida na variável **Alinhamento** coluna do Otimizador de Portfolio.

A pontuação do otimizador de portfólio é uma classificação calculada automaticamente no Otimizador de Portfolio pela qual os projetos podem ser priorizados. A pontuação do otimizador de portfólio é exibida como um ícone de indicador acompanhado por um número e exibida na **Pontuação** coluna do Otimizador de Portfolio. Uma pontuação do Otimizador de Portfolio é gerada somente quando todas as seções do Business Case são concluídas, exceto Metas.

Para obter mais informações sobre como criar um Business Case para um projeto, consulte [Criar um Business Case para um projeto](../../../manage-work/projects/define-a-business-case/create-business-case.md).

Para obter mais informações sobre como calcular a pontuação do otimizador de portfólio de um projeto, consulte [Visão geral da pontuação do Portfolio Otimizer](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-score.md).
