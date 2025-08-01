---
product-area: Canvas Dashboards
navigation-topic: report-types
title: Criar um relatório de KPI em um painel da tela
description: Um relatório de KPI que exibe de forma destacada um único KPI agregado pode ser adicionado a um Painel da tela.
author: Courtney and Jenny
feature: Reports and Dashboards
exl-id: e1c68ac3-112e-4f9e-b644-f44bb0778b92
source-git-commit: 8b9676c7ef4efcad1294a9aa786aa6fe52d26cc0
workflow-type: tm+mt
source-wordcount: '587'
ht-degree: 0%

---

# Criar um relatório de KPI em um painel da tela

>[!IMPORTANT]
>
>No momento, o recurso Painéis do Canvas está disponível apenas para usuários que participam da fase beta. Para obter mais informações, consulte [informações beta de Painéis do Canvas](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-beta-information.md).

É possível criar e adicionar um relatório de KPI a um Painel da tela que representa visualmente seus dados principais do indicador de desempenho como um número, que você pode usar para ver como seus projetos e equipes estão se saindo.

![Exemplo de relatório de KPI](assets/kpi-example-main.png)

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

Você deve criar um painel antes de criar um relatório de KPI.

## Criar um relatório de KPI em um painel da tela

Há muitas opções de configuração disponíveis para criar um relatório de KPI. Nesta seção, guiaremos você pelo processo geral de criação de um.

{{step1-to-dashboards}}

1. No painel esquerdo, clique em **Painéis do Canvas**.

1. Clique em **Novo Painel** no canto superior direito.

1. Na caixa **Criar painel**, digite o **Nome** e a **Descrição** do painel.

1. Clique em **Criar**.

1. Na caixa **Adicionar relatório**, selecione **Criar relatório**.

1. No lado esquerdo, selecione **KPI**.

1. No canto superior direito, clique em **Criar relatório**.

1. Siga as etapas abaixo para configurar a seção **Detalhes**:

   1. Insira um relatório **Nome**.
   1. Insira uma **Descrição** do relatório.

      >[!NOTE]
      >
      >A descrição será usada como uma legenda abaixo do valor do KPI. Se você não inserir uma descrição, uma legenda será gerada para você com base no agregador e no tipo de agregação selecionados nas etapas a seguir.

1. Siga as etapas abaixo para configurar a seção **Criar KPI**:

   1. No painel esquerdo, clique no ícone **Criar KPI** ![Criar KPI](assets/build-kpi-icon.png).

   1. Clique em **Selecionar campo** e especifique o campo que deseja adicionar ao relatório.

   1. No menu suspenso **Tipo de agregação**, selecione como os dados são acumulados para produzir a saída de KPI. As opções nesse campo variam de acordo com o tipo de campo selecionado na etapa anterior.

1. Siga as etapas abaixo para configurar a seção **Filtro**:

   1. No painel esquerdo, clique no ícone **Filtro** ![Filtro](assets/filter-icon.png).

   1. Selecione **Editar filtro**.

   1. Clique em **Adicionar condição** e especifique o campo pelo qual deseja filtrar e o modificador que define o tipo de condição que o campo deve atender.

   1. (Opcional) Clique em **Adicionar grupo de filtros** para adicionar outro conjunto de critérios de filtragem. O operador padrão entre os conjuntos é AND. Clique no operador para alterá-lo para OU.

1. Siga as etapas abaixo para configurar a seção **Configurações de Coluna de Detalhamento**:

   1. No painel esquerdo, clique no ícone **Colunas de Detalhamento** ![Colunas de Detalhamento](assets/drilldown-column.png). Os campos do gráfico aparecem automaticamente como colunas na seção de visualização à direita.

   1. (Opcional) Para atualizar qualquer uma das configurações de coluna existentes, selecione a coluna que deseja atualizar na seção **Colunas atuais** e atualize as informações desejadas (por exemplo, rótulo, status vinculado e regras de formatação).

   1. Clique em **Adicionar coluna** e selecione o campo que deseja exibir como uma coluna na tabela. Repita esse processo para cada coluna que deseja adicionar.

1. Siga as etapas abaixo para configurar a seção **Configurações do Grupo de Detalhamento**:

   1. No painel esquerdo, clique no ícone do **Grupo de configurações** ![Grupo de detalhamento](assets/drilldown-group-icon.png).

   1. Clique no botão **Adicionar agrupamento** e selecione o campo que deseja criar como agrupamento.

1. Clique em **Salvar** para criar o relatório e adicioná-lo ao painel.


