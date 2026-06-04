---
content-type: reference
product-area: reporting;projects;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Agrupamento: Patrocinador do Projeto para Horas'
description: Este agrupamento de horas organiza as horas pelo patrocinador do projeto onde as horas são registradas. A interface padrão do Report Builder para agrupamentos de horas não fornece um mapeamento para o campo Patrocinador do projeto. Você deve usar a interface Text Mode para acessar esse campo.
author: Courtney
feature: Reports and Dashboards
exl-id: 6b35b0ef-18b7-4121-ae39-d7957d76c04b
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/p-6tFGEEz8nXUaech59Lvw-2ZOml5v0xvK24mRhJ1iQ
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 235
ht-degree: 20%

---

# Agrupamento: patrocinador do projeto em horas

<!--Audited: 10/2024-->

Este agrupamento de horas organiza as horas pelo patrocinador do projeto onde as horas são registradas. A interface padrão do Report Builder para agrupamentos de horas não fornece um mapeamento para o campo Patrocinador do projeto. Você deve usar a interface Text Mode para acessar esse campo.

![hora_relatório_agrupado_por_patrocinador.png](assets/hour-report-grouped-by-sponsor-350x39.png)

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
   <p>Colaborador ou Solicitação para modificar um filtro </p>
   <p>Padrão ou Plano para modificar um relatório</p>
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

Para obter mais detalhes sobre as informações contidas nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Agrupar por Patrocinador do Projeto para horas

Para aplicar esse agrupamento:

1. Ir para uma lista de horas.
1. No menu suspenso **Agrupamento**, selecione **Novo agrupamento**.

1. Clique em **Alternar para Modo de Texto**.
1. Remova o texto na área que é exibida e substitua-o pelo seguinte código:

```
   group.0.linkedname=project:sponsor:name
   group.0.name=
   group.0.valuefield=project:sponsor:name
   group.0.valueformat=HTML
   textmode=true
```

1. Clique em **Concluído**.
1. Atualize o nome do agrupamento e clique em **Salvar agrupamento**.
