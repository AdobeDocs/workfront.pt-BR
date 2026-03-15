---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Agrupamento: Projetos por Data de Entrada'
description: Neste agrupamento de projeto personalizado, você pode exibir projetos agrupados por seus valores de Data de entrada.
author: Courtney
feature: Reports and Dashboards
exl-id: 511faad5-b5bd-4e2d-8daa-3fcde49a502c
source-git-commit: 6a6d3d47ed5741e3202c44b7240a2e67b687ea95
workflow-type: tm+mt
source-wordcount: '220'
ht-degree: 26%

---

# Agrupamento: projetos por data de entrada

<!--Audited: 10/2024-->

Neste agrupamento de projeto personalizado, você pode exibir projetos agrupados por seus valores de Data de entrada.

Cada agrupamento mostra projetos com uma Data de Entrada dentro de:

* Os últimos 30 dias
* 30-60 dias
* 60 dias ou mais

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacote do Adobe Workfront</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td> 
   <p>Colaborador ou solicitação para modificar um filtro </p>
   <p>Padrão ou Plano para modificar um relatório</p>
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Acesso de edição a relatórios, painéis e calendários para modificar um relatório</p> <p>Editar acesso a filtros, exibições e agrupamentos para modificar um filtro</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões para um relatório</p>  </td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações contidas nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Agrupar projetos por Data de Entrada

Para aplicar este agrupamento:

1. Vá para um relatório de projeto existente ou crie um novo.\
   Para obter mais informações sobre como criar um relatório, consulte o artigo [Criar um relatório personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
1. Clique em **Ações de Relatório** > **Editar**.
1. Na guia **Agrupamento**, clique em **Adicionar agrupamento**.
1. Clique em **Alternar para o Modo de Texto**.
1. Remova o texto na área **Agrupar por**.
1. Substitua o texto pelo seguinte código:


   ```
   group.0.linkedname=direct
   group.0.name=Project Entry
   group.0.valueexpression=IF(ABS(DATEDIFF({entryDate},$$TODAY))<=30,"Last 30 Days",IF(ABS(DATEDIFF({entryDate},$$TODAY))>30&&ABS(DATEDIFF({entryDate},$$TODAY))<=60,"30-60 Days","Older than 60 days"))
   group.0.valueformat=atDateAsMonthString
   textmode=true
   ```

1. Clique em **Concluído** > **Salvar Agrupamento**.
1. (Opcional) Atualize o nome do agrupamento e clique em **Salvar Agrupamento**.
