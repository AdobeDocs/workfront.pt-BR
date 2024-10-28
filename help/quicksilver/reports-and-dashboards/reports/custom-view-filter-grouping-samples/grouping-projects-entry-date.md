---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: "Agrupamento: projetos por Data de Entrada"
description: Neste agrupamento de projeto personalizado, você pode exibir projetos agrupados por seus valores de Data de entrada.
author: Nolan
feature: Reports and Dashboards
exl-id: 511faad5-b5bd-4e2d-8daa-3fcde49a502c
source-git-commit: 7b25d3b5fe69f610e245db5ada116ea967f22c7b
workflow-type: tm+mt
source-wordcount: '267'
ht-degree: 0%

---

# Agrupamento: projetos por Data de Entrada

Neste agrupamento de projeto personalizado, você pode exibir projetos agrupados por seus valores de Data de entrada.

Cada agrupamento mostra projetos com uma Data de Entrada dentro de:

* Os últimos 30 dias
* 30 a 60 dias
* 60 dias ou mais

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> 
    <p>Novo:</p>
   <ul><li><p>Colaborador para modificar um filtro </p></li>
   <li><p>Padrão para modificar um relatório</p></li> </ul>

<p>Atual:</p>
   <ul><li><p>Solicitação para modificar um filtro </p></li>
   <li><p>Planejar a modificação de um relatório</p></li> </ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Editar acesso a relatórios, painéis e calendários para modificar um relatório</p> <p>Editar acesso a Filtros, Visualizações, Agrupamentos para modificar um filtro</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões para um relatório</p>  </td> 
  </tr> 
 </tbody> 
</table>

*Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Agrupar projetos por data de entrada

Para aplicar esse agrupamento:

1. Vá para um relatório de projeto existente ou crie um novo relatório de projeto.\
   Para obter mais informações sobre como criar um relatório, consulte o artigo [Criar um relatório personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
1. Clique em **Ações de Relatório** > **Editar**.
1. Na guia **Agrupamento**, clique em **Adicionar agrupamento**.
1. Clique em **Alternar para Modo de Texto**.
1. Remover o texto da área **Agrupar por**.
1. Substitua o texto pelo seguinte código:

   group.0.linkedname=direct
group.0.name=Entrada do projeto
group.0.valueexpression=IF(ABS(DATEDIFF({entryDate},$$TODAY))&lt;=30,&quot;Últimos 30 Dias&quot;,IF(ABS(DATEDIFF({entryDate},$$TODAY))>30&amp;&amp;ABS(DATEDIFF({entryDate},$$TODAY))&lt;=60,&quot;30-60 Dias&quot;,&quot;Mais de 60 dias&quot;)
group.0.valueformat=atDateAsMonthString
textmode=true

1. Clique em **Concluído** > **Salvar agrupamento**.
1. (Opcional) Atualize o nome do agrupamento e clique em **Salvar agrupamento**.
