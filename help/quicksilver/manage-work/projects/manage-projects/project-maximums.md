---
title: Visão geral dos limites do projeto
content-type: overview
product-area: projects
navigation-topic: manage-projects
description: O Adobe Workfront tem limites para quantos objetos podem ser associados a um projeto. Os limites do projeto estão em vigor para melhorar o desempenho do produto e sua experiência com o Workfront.
author: Alina
feature: Work Management
exl-id: 60576107-89f1-4328-89e2-5b1e5e243fd9
source-git-commit: 11c4028038fe3d410ee0d4f238d2138435d9a3fa
workflow-type: tm+mt
source-wordcount: '327'
ht-degree: 0%

---

# Visão geral dos limites do projeto

O Adobe Workfront tem limites para quantos objetos podem ser associados a um projeto. Os limites do projeto estão em vigor para melhorar o desempenho do produto e sua experiência com o Workfront.

Os seguintes objetos associados aos projetos têm os seguintes limites:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><p>Tarefas</p></td> 
   <td>  <p>O número máximo de tarefas por projeto é de 5.000. Uma mensagem de aviso é exibida quando o número de tarefas se aproxima desse máximo. Quando o máximo é atingido, uma mensagem de erro é exibida e tarefas adicionais não podem ser adicionadas ao projeto.</p> <p>Para evitar atingir esse máximo, mova as tarefas que são fechadas para outro projeto designado para tarefas fechadas. Talvez seja necessário adaptar os relatórios sobre estes projetos.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Problemas</p></td> 
   <td>  <p>O número máximo de problemas por projeto é de 10.000. Uma mensagem de aviso é exibida quando o número de problemas se aproxima desse máximo. Quando o máximo é atingido, uma mensagem de erro é exibida e problemas adicionais não podem ser adicionados ao projeto.</p> <p>Para evitar atingir esse máximo, mova os problemas que são fechados para outro projeto designado para problemas fechados. Talvez seja necessário adaptar os relatórios sobre estes projetos.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Durações</p></td> 
   <td> <p>A duração máxima de um projeto deve ser de 15 anos para que o Workfront calcule automaticamente sua linha do tempo. Uma mensagem de aviso é exibida quando a duração do projeto se aproxima do máximo. Quando o máximo é atingido, uma mensagem de aviso é exibida e os cálculos automáticos de linha do tempo não ocorrem mais.</p> <p>Os cálculos automáticos da linha do tempo serão retomados assim que a duração de um projeto for reduzida para menos de 15 anos, ajustando as datas das tarefas no projeto.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Cálculos de linha do tempo</p></td> 
   <td>A Workfront não executa cálculos automáticos de linha do tempo para projetos que não foram atualizados em 6 meses e não serão retomados até que uma atualização seja feita.<p>Para projetos que não foram atualizados em 3 meses, o Workfront realiza cálculos de linha do tempo semanalmente em vez de durante a noite.</p><p>Para obter informações sobre o cálculo da linha do tempo do projeto, consulte <a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref">Recalcular linhas do tempo do projeto</a>. </p></td> 
  </tr> 
 </tbody> 
</table>

<!-- Notes from the table: 
     <p>For tasks limits: (This is NOT TRUE , but the PMs always wanted this to stay the way it is because they don't want customers creating projects bigger than this.)</p>
    <p>For issue limits: (this is true only for some clusters; according to Anna A., some clusters are set to a million.)</p>
    -->