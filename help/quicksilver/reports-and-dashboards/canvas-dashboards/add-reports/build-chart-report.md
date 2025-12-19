---
product-area: Canvas Dashboards
navigation-topic: report-types
title: Criar um relatório de gráfico em um painel da tela
description: Um relatório de gráfico que visualiza seus dados como um gráfico de barras, colunas, linhas ou de pizza pode ser adicionado a um Painel da Tela de Pintura.
author: Courtney and Jenny
feature: Reports and Dashboards
exl-id: 4262cae8-602f-416d-94b9-409eb9d6241c
source-git-commit: 56af1b6c8e4ae7bb990288d9e6a4326ffd18c2c9
workflow-type: tm+mt
source-wordcount: '1838'
ht-degree: 1%

---

# Criar um relatório de gráfico em um painel da tela

<span class="preview">As informações destacadas nesta página referem-se a funcionalidades que ainda não estão disponíveis. Ele está disponível somente no ambiente de Visualização para todos os clientes.</span>

>[!IMPORTANT]
>
>No momento, o recurso Painéis do Canvas está disponível apenas para usuários que participam da fase beta. Partes do recurso podem não estar completas ou não funcionar conforme o esperado durante essa etapa. Envie seus comentários sobre a experiência seguindo as instruções na seção [Fornecer feedback](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-beta-information.md#provide-feedback) do artigo de visão geral sobre a versão beta dos Painéis da Tela.<br>
>Se você tiver feedback sobre um possível erro ou problema técnico, envie um tíquete ao Suporte da Workfront. Para obter mais informações, consulte [Contate o Suporte ao Cliente](/help/quicksilver/workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md).<br>
>Observe que esse beta não está disponível nos seguintes provedores de nuvem:
>
>* Traga sua própria chave para o Amazon Web Services
>* Azure
>* Google Cloud Platform

Você pode criar e adicionar um relatório de gráfico a um Painel da Tela de Pintura para visualizar seus dados como um gráfico de barras, colunas, linhas ou pizza.

![Relatório de gráfico](assets/chart-report-main.png)

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>Pacote do Adobe Workfront</p></td> 
   <td> 
<p>Qualquer </p> 
   </td> 
<tr> 
 <tr> 
   <td role="rowheader"><p>Licença do Adobe Workfront</p></td> 
   <td> 
<p>Padrão</p> 
<p>Plano</p> 
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
      >É possível exibir um número máximo de 60 séries em um gráfico. Quando esta caixa estiver marcada, todas as séries acima do limite serão consolidadas em um agrupamento **Outro** no gráfico.
1. Escolha o tipo de gráfico que deseja criar:
   * [Gráfico de barras, colunas ou linhas](#bar-column-or-line-chart)
   * [Gráfico de pizza](#pie-chart)

### Gráfico de barras, colunas ou linhas

>[!NOTE]
>
>Pode haver campos adicionais dependendo do tipo de campo selecionado. As opções descritas abaixo são padrão para todos os tipos de campo.


1. No painel esquerdo, clique no ícone **Criar gráfico** ![Criar gráfico](assets/build-chart-icon.png).

1. No menu suspenso **Tipo de gráfico**, selecione **Barra**, **Coluna** ou **Linha**.
1. No segundo menu suspenso, selecione o tipo de barra, coluna ou linha:
   * **Simples**
   * **Várias séries**
   * **Empilhado**

1. Na seção **Eixo inferior (X)**, selecione o **Atualizar campo**, localize e selecione o campo que contém os dados que serão resumidos no gráfico.
1. No menu suspenso **Tipo de agregação**, selecione como os dados são acumulados para produzir a saída do gráfico.
1. <span class="preview">(Opcional) Adicione um rótulo de eixo no espaço fornecido.</span>
1. <span class="preview"> (Opcional) Alternar **Ocultar eixo** em. </span>
1. <span class="preview">(Opcional) Insira um **Valor da linha de referência** para definir um destino ou limite no gráfico.</span>
1. Escolha um **Tipo de linha** no menu suspenso.
1. Selecione o botão **Atualizar campo** na segunda seção, localize e selecione o segundo campo que deseja exibir no gráfico.


### Gráfico de pizza

>[!NOTE]
>
>Pode haver campos adicionais dependendo do tipo de campo selecionado. As opções descritas abaixo são padrão para todos os tipos de campo.


1. No painel esquerdo, clique no ícone **Criar gráfico** ![Criar gráfico](assets/build-chart-icon.png).

1. No menu suspenso **Tipo de gráfico**, selecione **Barra**.
1. Na seção **Métrica**, selecione o **Atualizar campo**, localize e selecione o campo que contém os dados que serão resumidos no gráfico.
1. No menu suspenso **Tipo de agregação**, selecione como os dados são acumulados para produzir a saída do gráfico.
1. Na seção **Segmento**, selecione o **Atualizar campo**, localize e selecione o campo que contém os segmentos que deseja exibir no gráfico de pizza.
1. <span class="preview"> (Opcional) Na seção **Pizza**, alterne **Mostrar rótulos de segmentos** para exibir rótulos de segmentos.</span>
1. <span class="preview"> (Opcional) Ative **Mostrar total** para exibir o total no meio do gráfico. Quando habilitado, há opções adicionais para mostrar um rótulo central e escolher o formato do valor.</span>

>[!NOTE]
>
>Os tipos de agregação são exibidos da seguinte maneira:
>
>* Tipos de agregação de contagem: o valor central exibido é uma contagem de todos os segmentos do gráfico.
>* Sum aggregation types: o valor central exibido é o total agregado do valor numérico ou de moeda.
>* Tipos de agregação média, máxima e mínima: O valor central exibe o valor médio, máximo ou mínimo adequadamente.

1. <span class="preview">(Opcional) Na seção Legenda, alterne **Mostrar legenda** para exibir a legenda do gráfico.</span>

1. <span class="preview"> (Opcional) Escolha uma **Posição da legenda** no menu suspenso.</span>

## Definir configurações adicionais de relatório de gráfico

### Filtros

Siga as etapas abaixo para configurar a seção **Filtro**:

1. No painel esquerdo, clique no ícone **Filtro**![ Filtro](assets/filter-icon.png).
1. Selecione **Editar filtro**.
1. Clique em **Adicionar condição** e especifique o campo pelo qual deseja filtrar e o modificador que define o tipo de condição que o campo deve atender.
1. (Opcional) Clique em **Adicionar grupo de filtros** para adicionar outro conjunto de critérios de filtragem. O operador padrão entre os conjuntos é AND. Clique no operador para alterá-lo para OU.

### Configurações de detalhamento

Siga as etapas abaixo para configurar a seção **Configurações de Coluna de Detalhamento**:

1. No painel esquerdo, clique no ícone **Colunas de Detalhamento** ![Colunas de Detalhamento](assets/drilldown-column.png). Os campos do gráfico aparecem automaticamente como colunas na seção de visualização à direita.

1. (Opcional) Para atualizar qualquer uma das configurações de coluna existentes, selecione a coluna que deseja atualizar na seção **Colunas atuais** e atualize as informações desejadas (por exemplo, rótulo, status vinculado e condições).

1. Clique em **Adicionar coluna** e selecione o campo que deseja exibir como uma coluna na tabela. Repita esse processo para cada coluna que deseja adicionar.

### Configurações do grupo de detalhamento

Siga as etapas abaixo para configurar a seção **Configurações do Grupo de Detalhamento**:

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

      Para obter mais informações sobre curingas, consulte a seção Variáveis de filtro de curingas com base em data no artigo [Editar filtros de relatório em um painel da tela](/help/quicksilver/reports-and-dashboards/canvas-dashboards/manage-reports/edit-report-filters.md).

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

## Considerações ao criar um relatório de gráfico

### Relatórios com dados financeiros

Os usuários com acesso de Visualização ou Edição a Dados financeiros em seu nível de acesso ainda verão os dados financeiros nas visualizações do Painel do Canvas, mesmo se a permissão de Visualização de finanças for removida no nível de tarefa ou projeto.

* Os usuários sem direitos de dados financeiros no nível de acesso não verão dados financeiros nos relatórios.
* Os usuários que veem dados financeiros estão limitados a registros para os quais já têm permissão para visualizar (projetos, tarefas, problemas, etc.). Eles não verão valores financeiros para registros que não podem acessar.
* Os criadores de relatórios devem ter cuidado ao incluir dados financeiros nos painéis e estar cientes de com quem compartilham painéis para evitar acesso não intencional.

Esse é um limite conhecido e pretendemos resolvê-lo o mais rápido possível.

### Utilização do seletor de campos

O menu suspenso **Seções** da seção **Gráfico de compilação** foi criado para restringir as opções em um seletor de campos para facilitar a localização de um objeto ao criar um relatório de tabela. Para iniciar, você selecionaria um objeto de entidade base.

* **Todas as Seções**: todos os tipos de objetos no Workfront Workflow e no Workfront Planning.
* **Objetos Workfront**: objetos de Fluxo de Trabalho Workfront nativos.
* **Tipos de Registro do Planning**: tipos de registro personalizados definidos no Workfront Planning.

![Menu suspenso de seções](assets/sections-dropdown.png)

Depois que o objeto de entidade base for selecionado, o menu suspenso **Seções** será atualizado com as opções de tipo de campo aplicáveis.

* **Todas as Seções**: campos nativos, campos personalizados e objetos relacionados.
* **Todos os campos**: campos nativos e personalizados (exclui relações).
* **Campos Personalizados**: campos definidos pelo cliente em um formulário personalizado ou em um registro do Planning.
* **Campos do Workfront**: somente campos nativos.
* **Relações**: registros conectados.

![Seleção de objetos relatáveis](assets/reportable-objects-selection.png)

### Fazendo referência a objetos filho

Os relacionamentos disponíveis para colunas adicionais, opções de filtro e atributos de agrupamento geralmente são limitados a objetos superiores na hierarquia de objetos do Workfront ou têm uma única seleção no objeto de entidade base do relatório. Há algumas exceções a isso, que incluem:

* Projeto > Tarefas
* Aprovação de documento > Estágios de aprovação de documento
* Estágios de aprovação de documento > Participantes do estágio de aprovação de documento

Ao utilizar qualquer uma das relações pai-filho listadas acima, você verá uma linha na tabela para cada registro filho conectado ao objeto pai.