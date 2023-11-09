---
title: Aplicar filtros na análise aprimorada
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: Os filtros na área Analítica aprimorada ajudam você a se concentrar em projetos específicos ou tipos específicos de dados.
author: Nolan
feature: Reports and Dashboards
exl-id: 25854c04-d914-4302-a36b-e8134637efe1
source-git-commit: bcafa607da733b89747f6b448dd295d9b906d060
workflow-type: tm+mt
source-wordcount: '1484'
ht-degree: 1%

---

# Aplicar filtros na análise aprimorada

Os filtros na área Analítica aprimorada ajudam você a se concentrar em projetos específicos ou tipos específicos de dados. Os tipos de filtros que você usa podem fornecer informações sobre:

* Projetos que possui
* Exibições específicas de portfólio ou programa
* Indicadores-chave de desempenho para um período específico (semana, trimestre, ano fiscal)

Você pode adicionar e remover filtros conforme necessário, e o Adobe Workfront retém os filtros que você aplica mesmo se você fizer logout.

## Requisitos de acesso

Para concluir essa tarefa, você deve ter o seguinte:

<table style="table-layout:auto"> 
 <caption style="text-align: left;">
  *Para descobrir que plano, tipo de licença ou acesso você tem, entre em contato com o administrador do Workfront.
 </caption> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><a href="https://www.workfront.com/plans" target="_blank">plano do Workfront</a>*</p> </td> 
   <td>Business ou superior</td> 
  </tr> 
  <tr> 
   <td> <p><a href="../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Visão geral das licenças do Adobe Workfront</a>*</p> </td> 
   <td> <p>Revisar ou superior</p> </td> 
  </tr> 
  <tr> 
   <td><b>Nível de acesso*</b> </td> 
   <td> <p>Visualizar acesso aos projetos</p> <p>Você também deve ter acesso de Visualização a Tarefas, Portfolio e Usuários para ver opções específicas de filtro de campo do projeto.</p> <p>Observação: se as restrições forem selecionadas na seção Definir restrições adicionais da caixa de diálogo Editar nível de acesso, talvez você não veja todas as informações nos filtros ou na página Analítica aprimorada depois que o filtro for aplicado. Para obter informações sobre como um administrador do Workfront pode alterar seu nível de acesso, consulte <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td> <p><b>Permissões de objeto</b> </p> </td> 
   <td> <p>Exibir</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Pré-requisitos

Para obter os pré-requisitos para usar o Enhanced Analytics, consulte [Pré-requisitos](../enhanced-analytics/enhanced-analytics-overview.md#prerequi) in [Visão geral da análise aprimorada](../enhanced-analytics/enhanced-analytics-overview.md).

## Alterar o filtro de intervalo de datas {#change-the-date-range-filter}

Por padrão, as visualizações na área Analítica aprimorada mostram dados dos últimos 60 dias e dos próximos 15 dias. Você pode selecionar um novo intervalo de datas e aplicá-lo a todas as visualizações na área Analítica aprimorada. Se você navegar para fora da página, o intervalo de datas padrão será aplicado na próxima vez que navegar de volta.

>[!TIP]
>
>Você também pode usar as teclas do teclado para navegar, abrir e selecionar um intervalo de datas no widget de calendário.\
>Para obter mais informações, consulte [Atalhos de teclado](../enhanced-analytics/enhanced-analytics-overview.md#keyboard) no artigo [Visão geral da análise aprimorada](../enhanced-analytics/enhanced-analytics-overview.md).

Para selecionar um novo intervalo de datas:

1. Clique no ícone Menu principal ![](assets/main-menu-icon-16x12.png)e selecione **Analytics**.
1. No canto superior direito da tela, clique no campo de intervalo de datas para abrir a exibição do calendário.
1. Use as setas acima do calendário para localizar o mês da data inicial e, em seguida, selecione a data inicial.

   ![](assets/filters-select-date-range-350x344.png)

1. Use as setas acima do calendário para localizar o mês da data final e, em seguida, selecione a data final.
1. (Opcional) Para ampliar um intervalo de datas menor, arraste o mouse de uma data específica para outra em uma das visualizações.

   Todas as visualizações na tela são atualizadas para corresponder ao período selecionado, e um filtro de Período é exibido ao lado de qualquer filtro existente. Esse filtro não será retido se você fizer logoff ou navegar fora da área Analítica aprimorada.

   ![](assets/timeframe-filter-350x220.png)

## Adicionar um filtro

Você pode adicionar filtros com base em campos de projeto padrão, campos de formulário personalizado e equipes locais atribuídas a projetos.

>[!TIP]
>
>Você também pode usar as teclas do teclado para navegar até um novo filtro e adicioná-lo.\
>Para obter mais informações, consulte [Atalhos de teclado](../enhanced-analytics/enhanced-analytics-overview.md#keyboard) no artigo [Visão geral da análise aprimorada](../enhanced-analytics/enhanced-analytics-overview.md).

* [Adicionar um filtro de campo de projeto](#add-a-project-field-filter)
* [Adicionar um filtro de campo de projeto](#add-a-project-field-filter)
* [Adicionar um filtro de Equipe](#add-a-team-filter)

### Adicionar um filtro de campo de projeto {#add-a-project-field-filter}

Os filtros de campo de projeto permitem filtrar dados de projetos e tarefas com base nos valores inseridos em campos incluídos em projetos por padrão.

Os seguintes tipos de filtro de campo de projeto estão disponíveis:

| **Projeto** | Exibe dados somente para os projetos selecionados |
|---|---|
| **Programa** | Exibe dados somente para projetos nos programas selecionados |
| **Portfólio** | Exibe dados somente para projetos nos portfólios selecionados |
| **Condição** | Exibe dados somente para projetos que tiveram as condições selecionadas mais recentemente (no destino, em risco ou com problemas) |
| **Status** | Exibe dados somente para projetos que tiveram os status selecionados mais recentemente (concluído, atual, em espera, cancelado, etc.) |
| **Patrocinador** | Exibe dados somente para projetos com o(s) patrocinador(es) selecionado(s) |
| **Proprietário do projeto** | Exibe dados somente para projetos com o(s) proprietário(s) do projeto selecionado(s) |

{style="table-layout:auto"}

Os filtros de formulário personalizados funcionam de forma diferente. Para obter mais informações, consulte [Adicionar um filtro de campo de projeto](#add-a-project-field-filter).

Para adicionar um filtro de campo de projeto:

1. Clique no ícone Menu principal ![](assets/main-menu-icon-16x12.png)e selecione **Analytics**.
1. No canto superior esquerdo da tela, clique em **Adicionar filtro**, em seguida, selecione o tipo de filtro desejado.

   >[!NOTE]
   >
   >Tipos de filtros diferentes exibem dados diferentes. Você pode usar apenas um tipo de filtro em um filtro. Depois de selecionado, um tipo de filtro não está disponível para uso em outro filtro de campo de projeto.

1. Localize os valores para os quais você deseja ver dados inserindo pelo menos 3 caracteres de texto na **Pesquisar** e selecione cada valor que deseja incluir no filtro.

   Para selecionar todos os valores atuais, clique em **Selecionar tudo**.

   ![](assets/select-filter-value-350x251.png)

1. Após selecionar todos os valores desejados, clique em **Aplicar filtro**.\
   A contagem de projetos no canto superior direito da página é atualizada para refletir os filtros aplicados.
1. Repita essas etapas para cada filtro que deseja adicionar.

   Conforme você adiciona filtros, os dados são exibidos nas visualizações abaixo para até 50 projetos.

   >[!TIP]
   >
   >Para ver dados de mais de 50 projetos exibidos por padrão, é possível:
   >
   >   
   >   
   >   * Use as setas no canto inferior esquerdo para exibir os próximos 50 projetos nessa visualização.\
   >     ![](assets/pagination-350x118.png)
   >   
   >   * Use o menu suspenso Classificar por em uma visualização para exibir os projetos em uma ordem diferente.\
   >     ![](assets/sort-by-menu-350x247.png)
   >   
   >   
   >

   Para ajustar o intervalo de datas, consulte [Alterar o filtro de intervalo de datas](#change-the-date-range-filter).

### Adicionar um filtro de Formulário personalizado de projeto

O tipo de filtro Formulário personalizado permite filtrar dados de projetos e tarefas com base nos valores inseridos em campos de Formulário personalizado em projetos. Diferentemente de outros tipos de filtros Analítica aprimorada, é possível adicionar mais de um filtro Formulário personalizado. Cada filtro Formulário personalizado contém valores inseridos somente no campo selecionado em um formulário personalizado específico.

Para adicionar um filtro de Formulário personalizado:

1. Clique no ícone Menu principal ![](assets/main-menu-icon-16x12.png)e selecione **Analytics**.
1. No canto superior esquerdo da tela, clique em **Adicionar filtro** e selecione **Formulário personalizado**.

   ![](assets/select-custom-form-filter-350x271.png)

1. Localize o Formulário personalizado desejado inserindo pelo menos 3 caracteres de texto na **Pesquisar** e selecione o formulário personalizado.
1. Selecione o campo desejado e conclua uma das seguintes ações com base no tipo de campo que você está adicionando ao filtro:

   >[!NOTE]
   >
   >Nem todos os tipos de campo Formulário personalizado podem ser adicionados a um filtro. Atualmente, a Análise aprimorada é compatível apenas com os tipos de campo listados acima.

   * **Caixa de seleção**, **menu suspenso** ou **botão de opção**: selecione cada valor no campo selecionado que deseja incluir no filtro ou clique no **Selecionar tudo** caixa de seleção\
     ![](assets/custom-form-filter-checkbox-350x255.png)

   * **Data**: use as setas para navegar até um mês específico e selecione a data no campo selecionado que deseja incluir no filtro.\
     ![](assets/custom-form-filter-date-350x348.png)

   * **Texto**: insira o texto no campo selecionado que deseja incluir no filtro.\
     ![](assets/custom-form-filter-text-350x90.png)

   * **Número**: insira o número no campo selecionado que deseja incluir no filtro.\
     ![](assets/custom-form-filter-number-350x93.png)

1. Depois de inserir ou selecionar os valores que deseja filtrar, clique em **Aplicar filtro**.

   A contagem de projetos no canto superior direito da página é atualizada para refletir os filtros aplicados.

1. Repita essas etapas para cada filtro que deseja adicionar.

   Conforme você adiciona filtros, os dados são exibidos nas visualizações abaixo para até 50 projetos.

   >[!TIP]
   >
   >Para ver dados de mais de 50 projetos exibidos por padrão, é possível:
   >
   >   
   >   
   >   * Use as setas no canto inferior esquerdo para exibir os próximos 50 projetos nessa visualização.\
   >     ![](assets/pagination-350x118.png)
   >   
   >   * Use o menu suspenso Classificar por em uma visualização para exibir os projetos em uma ordem diferente.\
   >     ![](assets/sort-by-menu-350x247.png)
   >   
   >   
   >

   Para ajustar o intervalo de datas, consulte [Alterar o filtro de intervalo de datas](#change-the-date-range-filter).

### Adicionar um filtro de Equipe {#add-a-team-filter}

1. Clique no ícone Menu principal ![](assets/main-menu-icon-16x12.png)e selecione **Analytics**.
1. No painel esquerdo, clique em **Pessoas**.

   ![](assets/people-area-cropped-qs-350x276.png)

1. No canto superior esquerdo da tela, clique em **Adicionar filtro**, em seguida, selecione a **Equipe** filtro.
1. Localize as equipes cujos dados você deseja ver inserindo pelo menos 3 caracteres de texto na **Pesquisar** e selecione cada equipe que deseja incluir no filtro. Para selecionar todas as equipes, clique em **Selecionar tudo**.

   ![](assets/select-team-value-350x253.png)

   >[!NOTE]
   >
   >Todas as equipes estão incluídas como opções de filtro, independentemente do seu nível de acesso.


1. Após selecionar todas as equipes desejadas, clique em **Aplicar filtro**.

   À medida que você adiciona filtros, os dados são exibidos nas visualizações abaixo.

   Para ajustar o intervalo de datas, consulte [Alterar o filtro de intervalo de datas](#change-the-date-range-filter).

## Remover um filtro

É possível remover um filtro a qualquer momento. Se você remover um filtro, ele não será exibido da próxima vez que você visitar a área de Análise aprimorada.

>[!TIP]
>
>Você também pode usar as teclas do teclado para navegar até um filtro existente e removê-lo.\
>Para obter mais informações, consulte [Atalhos de teclado](../enhanced-analytics/enhanced-analytics-overview.md#keyboard) no artigo [Visão geral da análise aprimorada](../enhanced-analytics/enhanced-analytics-overview.md).

Para remover um filtro:

1. Clique no ícone Menu principal ![](assets/main-menu-icon-16x12.png)e selecione **Analytics**.
1. Se quiser remover um filtro de Trabalho, continue na **Trabalho** área.

   Ou

   Se quiser remover um filtro Pessoas, selecione **Pessoas** no painel esquerdo.

1. Localize o filtro desejado e clique no link **X** para removê-lo.

   ![](assets/remove-filter-350x213.png)

   O filtro não está mais ativo e não é exibido a menos que você o adicione novamente.
