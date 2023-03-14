---
navigation-topic: business-case-and-scorecards
title: Aplicar um scorecard a um projeto e gerar uma Pontuação de alinhamento
description: Você pode usar um scorecard para medir o grau de alinhamento de um projeto aos critérios estabelecidos anteriormente de um portfólio. Um scorecard geralmente reflete a missão, os valores e os objetivos estratégicos de uma organização.
author: Alina
feature: Work Management
exl-id: 21cf5493-147d-4b8d-8b16-2891eb7e0491
source-git-commit: b2859f3d268bd947fba5bb0280677465b3039d93
workflow-type: tm+mt
source-wordcount: '1420'
ht-degree: 0%

---

# Aplicar um scorecard a um projeto e gerar uma Pontuação de alinhamento

<span class="preview">As informações destacadas nesta página se referem à funcionalidade ainda não disponível no geral. Está disponível somente no ambiente de Visualização.</span>

Você pode usar um scorecard para medir o grau de alinhamento de um projeto aos critérios estabelecidos anteriormente de um portfólio. Um scorecard geralmente reflete a missão, os valores e os objetivos estratégicos de uma organização.

Para obter mais informações sobre scorecards e como criar um, consulte [Criar um scorecard](../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-scorecard.md).

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plano Adobe Workfront*</td> 
   <td> <p>Empresa ou superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Plano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a Projetos</p> <p>Visualizar ou aumentar o acesso ao Portfolio</p> <p>Observação: Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões de um projeto</p> <p>Exibir permissões ou permissões mais altas para um portfólio </p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

## Scorecards de projeto {#project-scorecards}

* [Visão geral dos scorecards](#scorecards-overview)
* [Scorecards de projeto](#project-scorecards)

### Visão geral dos scorecards {#scorecards-overview}

Normalmente, um gerente de projeto conclui as informações do scorecard para produzir um valor de alinhamento entre 0 e 100 para o projeto. O valor produzido é usado posteriormente quando o gerente de portfólio analisa os projetos no otimizador de portfólio para compará-los.

Para obter mais informações sobre otimização de portfólio, consulte o artigo [Visão geral do Portfolio Otimizer](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md).

### Aplicar um scorecard a um projeto

Como usuário com uma licença do Plano e permissões de Gerenciamento para um projeto, você pode anexar um scorecard ao projeto.

Para obter mais informações sobre permissões de projeto, consulte [Compartilhar um projeto no Adobe Workfront](../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).

Você pode adicionar scorecards a um projeto como parte da criação do business case do projeto.

Para obter mais informações sobre a criação de um caso comercial, consulte [Criar um caso de negócios para um projeto](../../../manage-work/projects/define-a-business-case/create-business-case.md).

O administrador do Adobe Workfront ou o administrador do grupo deve ativar a seção Scorecard na área Caso de negócios de seus projetos antes que você possa acessar scorecards do Caso de negócios. Para obter informações sobre como configurar preferências de projeto e ativar áreas do Caso de negócios, consulte [Configurar preferências de projeto em todo o sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

Para aplicar um scorecard a um projeto:

1. Vá para um projeto ao qual deseja aplicar um scorecard.
1. Clique em **Caso de negócios** no painel esquerdo.
1. Encontre a **Scorecard** seção do Caso de negócios.\
   Você deve criar um scorecard antes do **Scorecard** é exibida no Caso de negócios.

   Para obter informações sobre como criar um scorecard, consulte [Criar um scorecard](../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-scorecard.md).

1. Selecione um scorecard no menu suspenso.

   ![new_scorecard.png](assets/new-scorecard-350x149.png)

1. Especifique uma resposta para todas as perguntas no scorecard.

   O Workfront aplica uma pontuação a cada pergunta respondida e calcula a pontuação geral do projeto com base na pontuação individual de cada pergunta.

   Para obter mais informações sobre a geração da pontuação de alinhamento geral do projeto, consulte [Gerar uma pontuação de alinhamento de um projeto](#generate-an-alignment-score-for-a-project).

1. Clique em **Salvar** para salvar o scorecard e pontuar o projeto.

   O scorecard agora está associado ao projeto e o projeto é pontuado.

1. (Condicional) Quando as alterações ocorrem nos valores das perguntas do scorecard, você deve recalcular o scorecard para refletir os novos valores da pontuação do projeto. Para recalcular o scorecard, faça o seguinte:

   1. Acesse uma lista de projetos e selecione todos os projetos na lista.
   1. Clique no botão **Editar** na parte superior da lista.
   1. Clique em **Configurações** no painel esquerdo e, em seguida, verifique o **Recalcular Scorecards** no final da área Configurações .
   1. Clique em Salvar. Isso recalcula o valor da pontuação com base nos scorecards anexados para todos os projetos selecionados.

      >[!NOTE]
      >
      >   <span class="preview">A opção para recalcular os scorecards foi removida do ambiente de Visualização, ao editar projetos em massa. </span>


## Gerar uma pontuação de alinhamento

* [Gerar uma pontuação de alinhamento de um projeto](#generate-an-alignment-score-for-a-project)
* [Gerar uma Pontuação de alinhamento para um portfólio](#generate-an-alignment-score-for-a-portfolio)

### Gerar uma pontuação de alinhamento de um projeto {#generate-an-alignment-score-for-a-project}

A pontuação de alinhamento é o valor produzido após a conclusão do scorecard.

Os scorecards contêm perguntas com opções de resposta que receberam valores numéricos, chamados de pontos de alinhamento. Esses pontos são usados para determinar se o projeto se alinha à organização. Os pontos de alinhamento de cada pergunta contêm um número entre 0 e 100.

Quando o scorecard é concluído, o Workfront calcula a pontuação de alinhamento do projeto como uma porcentagem, usando a seguinte fórmula:

```
Project Alignment Score = The sum of the question points from the scorecard met at a given time/ The sum of the possible points on the scorecard
```

Para obter mais informações, consulte [Criar um scorecard](../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-scorecard.md).

### Gerar uma Pontuação de alinhamento para um portfólio {#generate-an-alignment-score-for-a-portfolio}

A pontuação de alinhamento do portfólio é uma média das pontuações de alinhamento de todos os projetos no portfólio.

Quando os scorecards dos projetos são concluídos, o Workfront usa esses valores para calcular a pontuação de alinhamento do portfólio como uma porcentagem, usando a seguinte fórmula:

Pontuação de alinhamento de Portfolio = A soma das porcentagens das pontuações de alinhamento do projeto/Número de projetos no portfólio

>[!NOTE]
>
>Se um projeto não tiver um scorecard associado a ele e, portanto, não tiver uma pontuação de alinhamento, ele será considerado como tendo um alinhamento de 0% no portfólio. O projeto é levado em conta no número de projetos do portfólio.

## Exibir a pontuação de alinhamento

Você pode visualizar a pontuação de alinhamento de um projeto no nível do projeto ou no Portfolio Otimizer.

* [Exibir a pontuação de alinhamento em um projeto](#View%20the)
* [Exibir as Pontuações de alinhamento do projeto e do portfólio no Portfolio Otimizer](#View%20the2)

### Exibir a pontuação de alinhamento em um projeto

Você pode visualizar a pontuação de alinhamento de um projeto no nível do projeto se tiver direitos de Contribute para o projeto.

1. Vá para o projeto cuja Pontuação de alinhamento você deseja visualizar.
1. Clique em **Caso de negócios** no painel esquerdo.
1. Vá para o **Resumo do caso de negócios** no lado direito da tela.

   A Pontuação de alinhamento está localizada no Resumo do caso comercial, na seção **Alinhado** valor.

   ![alignment_score_on_a_project.png](assets/alignment-score-on-a-project.png)

### Exibir as Pontuações de alinhamento do projeto e do portfólio no Portfolio Otimizer

Você pode exibir a pontuação de alinhamento de um projeto ou de um portfólio no Portfolio Otimizer, se tiver acesso de Gerenciar ao portfólio.

Para obter mais informações sobre as informações exibidas no Portfolio Otimizer, consulte [Visão geral do Portfolio Otimizer](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md).

* [Localize a Pontuação de alinhamento do projeto no Portfolio Otimizer](#locate-the-alignment-score-of-the-project-in-the-portfolio-optimizer)
* [Localize a Pontuação de alinhamento do portfólio no Portfolio Otimizer](#locate-the-alignment-score-of-the-portfolio-in-the-portfolio-optimizer)

   ![](assets/alignment-score-in-portfolio-optimizer-nwe-350x97.png)

#### Localize a Pontuação de alinhamento do projeto no Portfolio Otimizer {#locate-the-alignment-score-of-the-project-in-the-portfolio-optimizer}

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png), em seguida **Portfolio**.

1. Clique no nome de um Portfolio.
1. Clique em **Otimização de Portfolio** no painel esquerdo.

   O Portfolio Otimizer é exibido.

1. A pontuação de alinhamento de um projeto é exibida como uma porcentagem na variável **Alinhamento** coluna do Portfolio Otimizer.

   Esta é a pontuação de alinhamento do projeto com base no scorecard associado ao projeto.

#### Localize a Pontuação de alinhamento do portfólio no Portfolio Otimizer  {#locate-the-alignment-score-of-the-portfolio-in-the-portfolio-optimizer}

1. Vá para o **Projetos** na barra Navegação global.
1. Selecione o **Portfolio** guia .
1. Clique no nome de um Portfolio.
1. Selecione o **Otimização de Portfolio** guia .
1. Na parte superior do Portfolio Otimizer, encontre a variável **Alinhado** , bem como a variável **Alinhamento** medidor que indica a pontuação de alinhamento do portfólio.

   Esta é a pontuação de alinhamento do portfólio.

   Para obter mais informações sobre como a pontuação de alinhamento de um portfólio é gerada, consulte [Gerar uma Pontuação de alinhamento para um portfólio](#generate-an-alignment-score-for-a-portfolio).

## Visão geral da pontuação do Portfolio Otimizer

Há uma diferença entre a pontuação de alinhamento e a pontuação do otimizador de portfólio de um projeto.

A pontuação de alinhamento de um projeto é calculada com base nos pontos obtidos após a conclusão do scorecard. Essa pontuação é então usada para determinar a pontuação de alinhamento do portfólio. A pontuação de alinhamento é exibida como uma porcentagem.

A pontuação de alinhamento de um projeto é exibida na **Alinhamento** coluna do Portfolio Otimizer.

A pontuação do otimizador de portfólio é uma classificação calculada automaticamente no Portfolio Otimizer pela qual os projetos podem ser priorizados. A pontuação do otimizador de portfólio é exibida como um ícone de indicador acompanhado por um número e é exibida no **Pontuação** coluna do Portfolio Otimizer. Uma pontuação Portfolio Otimizer é gerada somente quando todas as seções do Caso de negócios são concluídas, exceto por Metas.

Para obter mais informações sobre como criar um Caso de negócios para um projeto, consulte [Criar um caso de negócios para um projeto](../../../manage-work/projects/define-a-business-case/create-business-case.md).

Para obter mais informações sobre o cálculo da pontuação do otimizador de portfólio de um projeto, consulte [Visão geral da pontuação do Portfolio Otimizer](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-score.md).
