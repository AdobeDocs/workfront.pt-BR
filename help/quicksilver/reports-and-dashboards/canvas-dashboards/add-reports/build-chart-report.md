---
product-area: Canvas Dashboards
navigation-topic: report-types
title: Criar um relatório de gráfico
description: Um relatório de gráfico que visualiza seus dados como um gráfico de barras, colunas, linhas ou de pizza pode ser adicionado a um Painel da Tela de Pintura.
author: Courtney and Jenny
feature: Reports and Dashboards
exl-id: 4262cae8-602f-416d-94b9-409eb9d6241c
source-git-commit: ba9256255905e139c281099555a6d129fc570984
workflow-type: tm+mt
source-wordcount: '1037'
ht-degree: 0%

---

# Criar um relatório de gráfico

>[!IMPORTANT]
>
>No momento, o recurso Painéis do Canvas está disponível apenas para usuários que participam da fase beta. Para obter mais informações, consulte [informações beta de Painéis do Canvas](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-beta-information.md).

Você pode criar e adicionar um relatório de gráfico a um Painel da Tela de Pintura para visualizar seus dados como um gráfico de barras, colunas, linhas ou pizza.

![Relatório de gráfico](assets/chart-report-main.png)

+++ Expanda para visualizar os requisitos de acesso.

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>plano do Adobe Workfront</p></td> 
   <td> 
<p>Qualquer </p> 
   </td> 
<tr> 
 <tr> 
   <td role="rowheader"><p>Licença do Adobe Workfront</p></td> 
   <td> 
<p>Atual: Plano </p> 
<p>Novo: Padrão</p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Configurações de nível de acesso</p></td> 
   <td><p>Editar acesso a relatórios, painéis e calendários</p>
  </td> 
  </tr>  
</tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).
+++

## Pré-requisitos

Você deve criar um painel antes de criar um relatório de gráfico.

## Criar um relatório de gráfico em um painel da tela

Há muitas opções de configuração disponíveis para criar um relatório de gráfico. Nesta seção, guiaremos você pelo processo geral de criação de um.

{{step1-to-dashboards}}

1. No painel esquerdo, clique em **Painéis do Canvas**.

1. Clique em **Novo Painel** no canto superior direito.

1. Na caixa **Criar painel**, digite o **Nome** e a **Descrição** do painel.

1. Clique em **Criar**.

1. Na caixa **Adicionar relatório**, selecione **Criar relatório**.

1. No lado esquerdo, selecione **Gráfico**.

1. No canto superior direito, clique em **Criar relatório**.

1. (Opcional) Siga as etapas abaixo para configurar a seção **Detalhes**:

   1. Insira um relatório **Nome**.

   1. Insira uma **Descrição** do relatório.

   1. Se desejar, desmarque a caixa **Mostrar séries extras como &quot;Outros&quot;**.

      >[!NOTE]
      >
      >Há um número máximo de séries que podem ser exibidas em um gráfico. Quando esta caixa estiver marcada, todas as séries acima do limite serão consolidadas em um agrupamento **Outro** no gráfico.

1. Siga as etapas abaixo para configurar a seção **Criar gráfico**:

   1. No painel esquerdo, clique no ícone **Criar gráfico** ![Criar gráfico](assets/build-chart-icon.png).

   1. No menu suspenso **Tipo de gráfico**, selecione o tipo de gráfico que deseja criar:

      * **Barra**
      * **Coluna**
      * **Linha**
      * **Pizza**

   1. No menu suspenso **Tipo de coluna**, selecione o tipo de coluna:
      * **Simples**
      * **Várias séries**
      * **Empilhado**

   1. Selecione o botão **Atualizar campo** na primeira seção, localize e selecione o campo que contém os dados que serão resumidos no gráfico.
   1. No menu suspenso **Tipo de agregação**, selecione como os dados são acumulados para produzir a saída do gráfico.

   1. Selecione o botão **Atualizar campo** na segunda seção, localize e selecione o segundo campo que deseja exibir no gráfico.

1. Siga as etapas abaixo para configurar a seção **Filtro**:

   1. No painel esquerdo, clique no ícone **Filtro**![ Filtro](assets/filter-icon.png).
   1. Selecione **Editar filtro**.
   1. Clique em **Adicionar condição** e especifique o campo pelo qual deseja filtrar e o modificador que define o tipo de condição que o campo deve atender.
   1. (Opcional) Clique em **Adicionar grupo de filtros** para adicionar outro conjunto de critérios de filtragem. O operador padrão entre os conjuntos é AND. Clique no operador para alterá-lo para OU.

1. Siga as etapas abaixo para configurar a seção **Configurações de Coluna de Detalhamento**:

   1. No painel esquerdo, clique no ícone **Colunas de Detalhamento** ![Colunas de Detalhamento](assets/drilldown-column.png). Os campos do gráfico aparecem automaticamente como colunas na seção de visualização à direita.

   1. (Opcional) Para atualizar qualquer uma das configurações de coluna existentes, selecione a coluna que deseja atualizar na seção **Colunas atuais** e atualize as informações desejadas (por exemplo, rótulo, status vinculado e condições).

   1. Clique em **Adicionar coluna** e selecione o campo que deseja exibir como uma coluna na tabela. Repita esse processo para cada coluna que deseja adicionar.

1. Siga as etapas abaixo para configurar a seção **Configurações do Grupo de Detalhamento**:

   1. No painel esquerdo, clique no ícone **Configurações de grupo** ![Configurações de grupo](assets/drilldown-group-icon.png).

   1. Clique no botão **Adicionar agrupamento** e selecione o campo que deseja criar como agrupamento.

1. Clique em **Salvar** para criar o relatório e adicioná-lo ao painel.

## Criar um exemplo de relatório de gráfico

Nesta seção, veremos as etapas para criar um gráfico de colunas que mostra as tarefas vencidas pelo proprietário do projeto.


{{step1-to-dashboards}}

1. No painel esquerdo, clique em **Painéis do Canvas**.

1. Clique em **Novo Painel** no canto superior direito.

1. Na caixa **Criar painel**, digite o **Nome** e a **Descrição** do painel.

1. Clique em **Criar**.

1. Na caixa **Adicionar relatório**, selecione **Criar relatório**.

1. No lado esquerdo, selecione **Gráfico**.

1. No canto superior direito, clique em **Criar relatório**.

1. Siga as etapas abaixo para configurar a seção **Detalhes**:

   1. Insira um relatório **Nome** (por exemplo, *Tarefas Vencidas por Proprietário do Projeto*).

   1. Insira uma **Descrição** do relatório.

1. Siga as etapas abaixo para configurar a seção **Criar gráfico**:

   1. No painel esquerdo, clique no ícone **Criar gráfico**.

   1. No menu suspenso **Tipo de gráfico**, selecione **Coluna**.

   1. No menu suspenso **Tipo de coluna**, selecione **Simples**.

   1. Selecione o botão **Atualizar campo** na seção **Eixo inferior (X)**, localize e selecione o campo **Tarefa** > **Projeto** > **Proprietário** > **Nome**.

      ![Atualizar campo](assets/bottom-x-axis.png)

   1. Clique no botão **Selecionar campo** sob a seção **Eixo esquerdo (Y)**, localize e selecione o campo **Tarefa** > **Nome**.

   1. No menu suspenso **Tipo de agregação**, selecione **Contagem**.

      ![Campo de tipo de agregação](assets/left-y-axis.png)

1. Siga as etapas abaixo para configurar a seção **Filtro**:

   1. No painel esquerdo, clique no ícone **Filtro**.

   1. Selecione **Editar filtro**.

   1. Clique em **Adicionar condição**.

   1. Clique na área de condição vazia e selecione **Selecionar campo**.

   1. Selecione o campo **Percentual concluído**.

   1. No menu suspenso **Operadores**, selecione **Menor que** e digite *100* no campo avaliador.

   1. Clique em **Adicionar condição** e em **Escolher campo**.

   1. Selecione o campo **Data de conclusão planejada**.

   1. No menu suspenso **Operadores**, selecione **Menor que**.

   1. Alternar **Definir data relativa** para **EM**.

   1. Insira *$$TODAY* no campo avaliador.

      ![Campo avaliador](assets/add-condition.png)

1. Siga as etapas abaixo para configurar a seção **Configurações de Coluna de Detalhamento**:

   1. No painel esquerdo, clique no ícone **Colunas de Detalhamento** ![Colunas de Detalhamento](assets/drilldown-column.png). Os campos do gráfico aparecem automaticamente como colunas na seção de visualização à direita.

   1. Clique em **Adicionar coluna** e selecione o campo **Atribuído a** > **Nome**.

   1. Clique em **Adicionar coluna** e selecione o campo **Data de Início Planejada**.

   1. Clique em **Adicionar coluna** e selecione o campo **Data de conclusão planejada**.

   1. Clique em **Adicionar coluna** e selecione o campo **Data da Última Atualização**.

   1. (Opcional) Para exibir a hora de atualização, selecione a opção **Data da Última Atualização** no campo **Colunas Atuais** e, em seguida, selecione uma opção de valor de hora no menu suspenso **Formato de data**.

1. Siga as etapas abaixo para configurar a seção **Configurações do Grupo de Detalhamento**:

   1. No painel esquerdo, clique no ícone **Configurações de grupo** ![Configurações de grupo](assets/drilldown-group-icon.png).

   1. Clique no botão **Adicionar agrupamento** e selecione o campo **Projeto** > **Nome**.

1. Clique em **Salvar** para criar o relatório e adicioná-lo ao painel.