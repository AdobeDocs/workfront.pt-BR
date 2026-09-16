---
product-area: Canvas Dashboards
navigation-topic: report-types
title: Agrupar dados de relatório em um painel da tela
description: Organize os resultados do relatório em grupos. O agrupamento funciona de forma diferente dependendo do tipo de relatório.
author: Courtney
feature: Reports and Dashboards
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
    internal-label: Reporting
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: 375d62fc12af075c2224f979d3ef87cdffdf03ea
workflow-type: tm+mt
source-wordcount: '484'
ht-degree: 13%
---
# Agrupar dados de relatório em um painel da tela

>[!IMPORTANT]
>
>No momento, o recurso Painéis do Canvas está disponível apenas para usuários que participam da fase beta. Partes do recurso podem não estar completas ou não funcionar conforme o esperado durante essa etapa. Envie seus comentários sobre a experiência seguindo as instruções na seção [Fornecer feedback](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-beta-information.md#provide-feedback) do artigo de visão geral sobre a versão beta dos Painéis da Tela.<br>
>Se você tiver feedback sobre um possível erro ou problema técnico, envie um tíquete ao Suporte da Workfront. Para obter mais informações, consulte [Falar com o suporte ao cliente](/help/quicksilver/workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md).<br>
>Observe que esse beta não está disponível nos seguintes provedores de nuvem:
>
>* Traga sua própria chave para o Amazon Web Services
>* Azure
>* Google Cloud Platform

O agrupamento organiza os resultados do relatório para que registros relacionados apareçam juntos. Como o agrupamento funciona depende do tipo de relatório, portanto, este artigo tem uma seção separada para cada um.

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
        <tr> 
   <td role="rowheader"><p>Permissões de objeto</p></td> 
   <td><p>Gerenciar permissões do painel</p>
  </td> 
  </tr>
</tbody> 
</table>

Para obter mais detalhes sobre as informações contidas nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).
+++

## Pré-requisitos

Você deve ter um relatório em um painel ou estar criando um antes de poder agrupar seus dados. Para obter mais informações, consulte [Criar um Painel da Tela](/help/quicksilver/reports-and-dashboards/canvas-dashboards/create-dashboards/create-dashboards.md).

## Agrupar linhas em um relatório de tabela

Em um relatório de tabela, o agrupamento organiza as linhas do próprio relatório.

1. Na caixa de diálogo **Configurar**, clique no ícone **Configurações de Grupo** no painel esquerdo.

1. Clique em **Adicionar agrupamento** e selecione o campo pelo qual deseja agrupar. O agrupamento aparece na visualização à direita.

1. (Opcional) Repita para adicionar mais agrupamentos.

## Configurar agrupamentos de detalhamento em relatórios de gráfico e KPI

No gráfico e nos relatórios de KPI, você não agrupa a visualização principal. Em vez disso, você configura como a tabela de detalhamento é agrupada quando um visualizador faz o detalhamento em um valor.

1. Na caixa de diálogo **Configurar**, clique no ícone **Configurações do Grupo de Detalhamento** no painel esquerdo.

1. Clique em **Adicionar agrupamento** e selecione o campo pelo qual deseja agrupar a tabela de detalhamento.

## Configurar segmentos em um relatório de tabela dinâmica

Os relatórios de tabela dinâmica não usam agrupamentos. Em vez disso, você define até dois segmentos, que são as categorias pelas quais as métricas da tabela dinâmica são agrupadas e totalizadas.

1. Na caixa de diálogo **Configurar**, clique no ícone **Segmentos** no painel esquerdo.

1. Clique em **Adicionar segmento** e selecione o campo desejado. O segmento aparece como uma coluna na visualização.

1. (Opcional) Repita para adicionar um segundo segmento. É possível adicionar no máximo dois segmentos.

## Visualizar dados agrupados em um painel

Os visualizadores de relatórios podem expandir, recolher e classificar dados agrupados. Para obter mais informações, consulte [Exibir relatórios com dados agrupados](/help/quicksilver/reports-and-dashboards/canvas-dashboards/use-canvas-dashboards.md#view-reports-with-grouped-data) em [Usar Painéis da Tela](/help/quicksilver/reports-and-dashboards/canvas-dashboards/use-canvas-dashboards.md).
