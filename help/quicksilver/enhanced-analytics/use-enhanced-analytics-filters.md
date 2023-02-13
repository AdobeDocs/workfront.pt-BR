---
title: Aplicar filtros no Enhanced Analytics
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: Os filtros na área Análise aprimorada ajudam você a se concentrar em projetos específicos ou tipos específicos de dados. Os tipos de filtros que você usa podem fornecer informações - EDITE-ME.
author: Nolan
feature: Reports and Dashboards
exl-id: 25854c04-d914-4302-a36b-e8134637efe1
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '1501'
ht-degree: 0%

---

# Aplicar filtros no Enhanced Analytics

Os filtros na área Análise aprimorada ajudam você a se concentrar em projetos específicos ou tipos específicos de dados. Os tipos de filtros que você usa podem fornecer informações sobre:

* Projetos que você possui
* Exibições específicas de portfólio ou programa
* Principais indicadores de desempenho para um período específico (semana, trimestre, ano fiscal)

Você pode adicionar e remover filtros conforme necessário e o Adobe Workfront retém os filtros que você aplica mesmo que você desconecte.

## Requisitos de acesso

Para concluir essa tarefa, você deve ter o seguinte:

<table style="table-layout:auto"> 
 <caption style="text-align: left;">
  *Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.
 </caption> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><a href="https://www.workfront.com/plans" target="_blank">Plano Workfront</a>*</p> </td> 
   <td>Empresa ou superior</td> 
  </tr> 
  <tr> 
   <td> <p><a href="../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Visão geral das licenças do Adobe Workfront</a>*</p> </td> 
   <td> <p>Revisar ou superior</p> </td> 
  </tr> 
  <tr> 
   <td><b>Nível de acesso*</b> </td> 
   <td> <p>Visualizar o acesso a Projetos</p> <p>Você também deve ter acesso de Exibição a Tarefas, Portfolio e Usuários para ver opções específicas de filtro de campo do projeto.</p> <p>Observação: Se as restrições forem selecionadas na seção Definir restrições adicionais da caixa de diálogo Editar nível de acesso , talvez você não veja todas as informações nos filtros ou na página Análise aprimorada depois que o filtro é aplicado. Para obter informações sobre como um administrador do Workfront pode alterar seu nível de acesso, consulte <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td> <p><b>Permissões de objeto</b> </p> </td> 
   <td> <p>Exibir</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Pré-requisitos

Para obter os pré-requisitos para usar o Enhanced Analytics, consulte [Pré-requisitos](../enhanced-analytics/enhanced-analytics-overview.md#prerequi) em [Visão geral da análise aprimorada](../enhanced-analytics/enhanced-analytics-overview.md).

## Alterar o filtro de intervalo de datas {#change-the-date-range-filter}

Por padrão, as visualizações na área de Análise aprimorada mostram dados dos últimos 60 dias e dos próximos 15 dias. Você pode selecionar um novo intervalo de datas e aplicá-lo a todas as visualizações na área Análise aprimorada . Se você sair da página, o intervalo de datas padrão será aplicado na próxima vez que você voltar.

>[!TIP]
>
>Você também pode usar as teclas do teclado para navegar, abrir e selecionar um intervalo de datas no widget de calendário.\
>Para obter mais informações, consulte o [Atalhos de teclado](../enhanced-analytics/enhanced-analytics-overview.md#keyboard) no artigo [Visão geral da análise aprimorada](../enhanced-analytics/enhanced-analytics-overview.md).

Para selecionar um novo intervalo de datas:

1. Clique no ícone do Menu principal ![](assets/main-menu-icon-16x12.png), em seguida selecione **Analytics**.
1. No canto superior direito da tela, clique no campo de intervalo de datas para abrir a visualização do calendário.
1. Use as setas acima do calendário para localizar o mês da data de início e selecione a data de início.

   ![](assets/filters-select-date-range-350x344.png)

1. Use as setas acima do calendário para localizar o mês da data final e selecione a data final.
1. (Opcional) Para ampliar um intervalo de datas menor, arraste o mouse de uma data específica para outra em uma das visualizações.

   Todas as visualizações na tela são atualizadas para corresponder ao período selecionado e um filtro de Cronograma é exibido ao lado de qualquer filtro existente. Esse filtro não será retido se você sair ou sair da área de análise aprimorada.

   ![](assets/timeframe-filter-350x220.png)

## Adicionar um filtro

Você pode adicionar filtros com base em campos de projeto padrão, campos de Formulário personalizado e equipes iniciais atribuídas a projetos.

>[!TIP]
>
>Você também pode usar as teclas do teclado para navegar e adicionar um novo filtro.\
>Para obter mais informações, consulte o [Atalhos de teclado](../enhanced-analytics/enhanced-analytics-overview.md#keyboard) no artigo [Visão geral da análise aprimorada](../enhanced-analytics/enhanced-analytics-overview.md).

* [Adicionar um filtro de campo de projeto](#add-a-project-field-filter)
* [Adicionar um filtro de campo de projeto](#add-a-project-field-filter)
* [Adicionar um filtro de Equipe](#add-a-team-filter)

### Adicionar um filtro de campo de projeto {#add-a-project-field-filter}

Os filtros de campo do projeto permitem filtrar dados para projetos e tarefas com base nos valores inseridos nos campos incluídos nos projetos por padrão.

Os seguintes tipos de filtro de campo de projeto estão disponíveis:

| **Projeto** | Exibe dados somente para o(s) projeto(s) selecionado(s) |
|---|---|
| **Programa** | Exibe dados somente para projetos no(s) programa(s) selecionado(s) |
| **Portfólio** | Exibe dados somente para projetos no(s) portfólio(s) selecionado(s) |
| **Condição** | Exibe dados apenas para projetos que tiveram as condições selecionadas mais recentemente (no destino, em risco ou em problemas) |
| **Status** | Exibe dados apenas para projetos que tiveram os status selecionados mais recentemente (concluído, atual, suspenso, cancelado, etc.) |
| **Patrocinador** | Exibe dados somente para projetos com o(s) patrocinador(es) selecionado(s) |
| **Proprietário do projeto** | Exibe dados apenas para projetos com o(s) proprietário(s) do projeto selecionado(s) |

{style=&quot;table-layout:auto&quot;}

Os filtros de Formulário personalizado funcionam de forma diferente. Para obter mais informações, consulte [Adicionar um filtro de campo de projeto](#add-a-project-field-filter).

Para adicionar um filtro de campo de projeto:

1. Clique no ícone do Menu principal ![](assets/main-menu-icon-16x12.png), em seguida selecione **Analytics**.
1. No canto superior esquerdo da tela, clique em **Adicionar filtro**, em seguida, selecione o tipo de filtro desejado.

   >[!NOTE]
   >
   >Tipos de filtro diferentes exibem dados diferentes. Você pode usar apenas um tipo de filtro em um filtro. Depois de selecionado, um tipo de filtro não está disponível para uso em outro filtro de campo de projeto.

1. Localize os valores para os quais deseja ver dados inserindo pelo menos 3 caracteres de texto na **Pesquisar** selecione cada valor que deseja incluir no filtro.

   Para selecionar todos os valores atuais, clique em **Selecionar tudo**.

   ![](assets/select-filter-value-350x251.png)

1. Depois de selecionar todos os valores desejados, clique em **Aplicar filtro**.\
   A contagem do projeto no canto superior direito das atualizações de página para refletir os filtros aplicados.
1. Repita essas etapas para cada filtro que deseja adicionar.

   À medida que você adiciona filtros, os dados são exibidos nas visualizações abaixo para até 50 projetos.

   >[!TIP]
   >
   >Para visualizar dados de mais de 50 projetos exibidos por padrão, é possível:
   >
   >   
   >   
   >   * Use as setas no canto inferior esquerdo para exibir os próximos 50 projetos nessa visualização.\
      >     ![](assets/pagination-350x118.png)
   >   
   >   * Use o menu suspenso Classificar por em uma visualização para visualizar os projetos em uma ordem diferente.\
      >     ![](assets/sort-by-menu-350x247.png)


   Para ajustar o intervalo de datas, consulte [Alterar o filtro de intervalo de datas](#change-the-date-range-filter).

### Adicionar um filtro de Formulário personalizado de projeto

O tipo de filtro Formulário personalizado permite filtrar dados de projetos e tarefas com base nos valores inseridos nos campos Formulário personalizado em projetos. Ao contrário de outros tipos de filtros de Análise avançada, é possível adicionar mais de um filtro de Formulário personalizado. Cada filtro de Formulário personalizado contém valores inseridos somente no campo selecionado em um formulário personalizado específico.

Para adicionar um filtro de Formulário personalizado:

1. Clique no ícone do Menu principal ![](assets/main-menu-icon-16x12.png), em seguida selecione **Analytics**.
1. No canto superior esquerdo da tela, clique em **Adicionar filtro**, em seguida selecione **Formulário personalizado**.

   ![](assets/select-custom-form-filter-350x271.png)

1. Localize o Formulário personalizado desejado inserindo pelo menos 3 caracteres de texto no **Pesquisar** e selecione o formulário personalizado.
1. Selecione o campo desejado e conclua uma das seguintes ações com base no tipo de campo que você está adicionando ao filtro:

   >[!NOTE]
   >
   >Nem todos os tipos de campos de Formulário personalizado podem ser adicionados a um filtro. Atualmente, o Enhanced Analytics suporta apenas os tipos de campo listados acima.

   * **Caixa de seleção**, **lista suspensa** ou **botão de opção**: Selecione cada valor no campo selecionado que deseja incluir no filtro ou clique no botão **Selecionar tudo** caixa de seleção.\
      ![](assets/custom-form-filter-checkbox-350x255.png)

   * **Data**: Use as setas para navegar até um mês específico e selecione a data no campo selecionado que deseja incluir no filtro.\
      ![](assets/custom-form-filter-date-350x348.png)

   * **Texto**: Insira o texto no campo selecionado que você deseja incluir no filtro.\
      ![](assets/custom-form-filter-text-350x90.png)

   * **Número**: Insira o número no campo selecionado que você deseja incluir no filtro.\
      ![](assets/custom-form-filter-number-350x93.png)

1. Depois de inserir ou selecionar os valores para os quais deseja filtrar, clique em **Aplicar filtro**.

   A contagem do projeto no canto superior direito das atualizações de página para refletir os filtros aplicados.

1. Repita essas etapas para cada filtro que deseja adicionar.

   À medida que você adiciona filtros, os dados são exibidos nas visualizações abaixo para até 50 projetos.

   >[!TIP]
   >
   >Para visualizar dados de mais de 50 projetos exibidos por padrão, é possível:
   >
   >   
   >   
   >   * Use as setas no canto inferior esquerdo para exibir os próximos 50 projetos nessa visualização.\
      >     ![](assets/pagination-350x118.png)
   >   
   >   * Use o menu suspenso Classificar por em uma visualização para visualizar os projetos em uma ordem diferente.\
      >     ![](assets/sort-by-menu-350x247.png)


   Para ajustar o intervalo de datas, consulte [Alterar o filtro de intervalo de datas](#change-the-date-range-filter).

### Adicionar um filtro de Equipe {#add-a-team-filter}

1. Clique no ícone do Menu principal ![](assets/main-menu-icon-16x12.png), em seguida selecione **Analytics**.
1. No painel esquerdo, clique em **Pessoas**.

   ![](assets/people-area-cropped-qs-350x276.png)

1. No canto superior esquerdo da tela, clique em **Adicionar filtro**, em seguida, selecione o **Equipe** filtro.
1. Localize as equipes para as quais deseja visualizar dados inserindo pelo menos 3 caracteres de texto na **Pesquisar** selecione cada equipe que deseja incluir no filtro. Para selecionar todas as equipes, clique em **Selecionar tudo**.

   ![](assets/select-team-value-350x253.png)

   >[!NOTE]
   >
   >Todas as equipes são incluídas como opções de filtro, independentemente do nível de acesso.


1. Depois de selecionar todas as equipes desejadas, clique em **Aplicar filtro**.

   À medida que você adiciona filtros, os dados são exibidos nas visualizações abaixo.

   Para ajustar o intervalo de datas, consulte [Alterar o filtro de intervalo de datas](#change-the-date-range-filter).

## Remover um filtro

Você pode remover um filtro a qualquer momento. Se você remover um filtro, ele não será exibido na próxima vez que você visitar a área Análise aprimorada .

>[!TIP]
>
>Você também pode usar as teclas do teclado para navegar até um filtro existente e removê-lo.\
>Para obter mais informações, consulte o [Atalhos de teclado](../enhanced-analytics/enhanced-analytics-overview.md#keyboard) no artigo [Visão geral da análise aprimorada](../enhanced-analytics/enhanced-analytics-overview.md).

Para remover um filtro:

1. Clique no ícone do Menu principal ![](assets/main-menu-icon-16x12.png), em seguida selecione **Analytics**.
1. Se quiser remover um filtro de Trabalho, mantenha a função **Trabalho** área.

   Ou

   Se deseja remover um filtro de Pessoas, selecione **Pessoas** no painel esquerdo.

1. Localize o filtro desejado e clique no botão **X** para removê-lo.

   ![](assets/remove-filter-350x213.png)

   O filtro não está mais ativo e não é exibido, a menos que você o adicione novamente.
