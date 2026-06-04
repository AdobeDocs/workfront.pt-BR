---
title: Visão geral dos limites do projeto
content-type: overview
product-area: projects
navigation-topic: manage-projects
description: O Adobe Workfront tem limites para quantos objetos podem ser associados a um projeto. Existem limites de projeto para melhorar o desempenho do produto e a sua experiência com o Workfront.
author: Alina
feature: Work Management
exl-id: 60576107-89f1-4328-89e2-5b1e5e243fd9
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/t6tfn132hAQe--u8g73CAFAfrJTf2qFi7yOhm4flP58
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
subfeature_v2:
  - id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: bce87dde-a4ab-44c9-8a18-ad66e4ddb377
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 458
ht-degree: 1%

---

# Visão geral dos limites do projeto

O Adobe Workfront tem limites para quantos objetos podem ser associados a um projeto. Existem limites de projeto para melhorar o desempenho do produto e a sua experiência com o Workfront.

Os seguintes objetos associados a projetos têm os seguintes limites:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><p>Tarefas</p></td> 
   <td>  <p>O número máximo de tarefas por projeto é 5.000. Uma mensagem de aviso é exibida quando o número de tarefas se aproximar desse máximo. Quando o máximo é atingido, uma mensagem de erro é exibida e tarefas adicionais não podem ser adicionadas ao projeto.</p> <p>Para evitar atingir esse máximo, mova as tarefas fechadas para outro projeto designado para tarefas fechadas. Os relatórios sobre esses projetos podem precisar ser ajustados.</p>

<b>IMPORTANTE</b>

Para projetos em que as tarefas têm muitas dependências, pode ocorrer uma degradação do desempenho no cálculo da linha do tempo ou ao trabalhar no projeto.

Por esse motivo, recomendamos que o número de tarefas em projetos com dependências complexas seja muito menor do que o máximo permitido de 5.000 tarefas.

Alguns exemplos de dependências de tarefas que podem influenciar ou impedir o recálculo da linha do tempo do projeto são:

<ul><li>Número de filhos</li>
   <li>Vários níveis de recuo da tarefa</li>
   <li>Número de predecessores</li>
   <li>Várias atribuições</li>
   </ul>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Problemas</p></td> 
   <td>  <p>O número máximo de problemas por projeto é 10.000. Uma mensagem de aviso é exibida quando o número de problemas se aproximar desse máximo. Quando o máximo é atingido, uma mensagem de erro é exibida e problemas adicionais não podem ser adicionados ao projeto.</p> <p>Para evitar atingir esse máximo, mova os problemas que estão fechados para outro projeto designado para problemas fechados. Os relatórios sobre esses projetos podem precisar ser ajustados.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Duração</p></td> 
   <td> <p>A duração máxima de um projeto deve ser de 15 anos para que o Workfront calcule automaticamente sua linha do tempo. Uma mensagem de aviso é exibida quando a duração do projeto se aproximar do máximo. Quando o máximo for atingido, uma mensagem de aviso será exibida e os cálculos automáticos da linha do tempo não ocorrerão mais.</p> <p>Os cálculos automáticos de cronograma serão retomados assim que a duração de um projeto for reduzida para menos de 15 anos, ajustando as datas das tarefas no projeto.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Cálculos de linha do tempo</p></td> 
   <td>A Workfront não executa cálculos automáticos de cronograma para projetos que não foram atualizados em 6 meses e não retomarão até que uma atualização seja feita.<p>Para projetos que não são atualizados há três meses, o Workfront realiza cálculos de cronograma semanalmente em vez de à noite.</p><p>Para obter informações sobre como calcular a linha de tempo do projeto, consulte <a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref">Recalcular linhas de tempo do projeto</a>. </p></td> 
  </tr> 
    <tr> 
   <td role="rowheader"><p>Converter objetos </p></td> 
   <td>O Workfront tem um limite de processamento de 5 minutos ao converter objetos. Se o objeto tiver um grande número de documentos anexados a ele, poderá falhar ao converter dentro do limite de 5 minutos. Talvez seja necessário remover alguns documentos e tentar novamente.</td> 
  </tr> 
 </tbody> 
</table>

<!--
 Notes from the table: 
     <p>For tasks limits: (This is NOT TRUE , but the PMs always wanted this to stay the way it is because they don't want customers creating projects bigger than this.)</p>
    <p>For issue limits: (this is true only for some clusters; according to Anna A., some clusters are set to a million.)</p>
    -->
