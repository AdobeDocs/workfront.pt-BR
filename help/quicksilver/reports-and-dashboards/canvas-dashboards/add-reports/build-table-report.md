---
product-area: Canvas Dashboards
navigation-topic: report-types
title: Criar um relatório de tabela em um painel da tela
description: É possível adicionar um relatório de tabela a um Painel da tela para visualizar seus dados em formato de tabela.
author: Courtney and Jenny
feature: Reports and Dashboards
exl-id: a7aa8614-6e80-4fc1-88ff-d952d87ddcbc
source-git-commit: 8b9676c7ef4efcad1294a9aa786aa6fe52d26cc0
workflow-type: tm+mt
source-wordcount: '444'
ht-degree: 0%

---

# Criar um relatório de tabela em um painel da tela

>[!IMPORTANT]
>
>No momento, o recurso Painéis do Canvas está disponível apenas para usuários que participam da fase beta. Para obter mais informações, consulte [informações beta de Painéis do Canvas](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-beta-information.md).

É possível adicionar um relatório de tabela a um Painel da tela para visualizar seus dados em formato de tabela.

![Exemplo de relatório de tabela](assets/table-example-main.png)

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

Você deve criar um painel antes de criar um relatório de tabela.

## Criar um relatório de tabela em um painel da tela

Há muitas opções de configuração disponíveis para criar um relatório de tabela. Nesta seção, guiaremos você pelo processo geral de criação de um.

{{step1-to-dashboards}}

1. No painel esquerdo, clique em **Painéis do Canvas**.

1. Clique em **Novo Painel** no canto superior direito.

1. Na caixa **Criar painel**, digite o **Nome** e a **Descrição** do painel.

1. Clique em **Criar**.

1. Na caixa **Adicionar relatório**, selecione **Criar relatório**.

1. No lado esquerdo, selecione **Tabela**.

1. No canto superior direito, clique em **Criar relatório**.

1. (Opcional) Siga as etapas abaixo para configurar a seção **Detalhes**:

   1. Insira um relatório **Nome**.

   1. Insira uma **Descrição** do relatório.

1. Siga as etapas abaixo para configurar a seção **Tabela de compilação**:

   1. No painel esquerdo, clique no ícone **Colunas da tabela** ![Criar tabela](assets/drilldown-column.png).

   1. Clique em **Adicionar coluna** e selecione o campo que deseja exibir como uma coluna na tabela. A coluna é exibida na seção de visualização à direita.

   1. Repita a etapa acima para cada coluna que deseja adicionar.

1. Siga as etapas abaixo para configurar a seção **Filtro**:

   1. No painel esquerdo, clique no ícone **Filtro** ![Filtro](assets/filter-icon.png).

   1. Selecione **Editar filtro**.

   1. Clique em **Adicionar condição** e especifique o campo pelo qual deseja filtrar e o modificador que define o tipo de condição que o campo deve atender. A coluna é exibida na seção de visualização à direita.

1. (Opcional) Clique em **Adicionar grupo de filtros** para adicionar outro conjunto de critérios de filtragem. O operador padrão entre os conjuntos é AND. Clique no operador para alterá-lo para OU.

1. Siga as etapas abaixo para configurar a seção **Configurações do Grupo de Detalhamento**:

   1. No painel esquerdo, clique no ícone **Configurações de grupo** ![Configurações de grupo](assets/drilldown-group-icon.png).

   1. Clique no botão **Adicionar agrupamento** e selecione o campo que deseja criar como agrupamento. A coluna de agrupamento aparece na seção de visualização à direita.

1. Clique em **Salvar** para criar o relatório e adicioná-lo ao painel.