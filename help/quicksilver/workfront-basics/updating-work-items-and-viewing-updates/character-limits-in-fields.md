---
content-type: reference
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: Limites de caracteres em campos
description: Determinados campos no Adobe Workfront limitam o número de caracteres que podem ser incluídos no campo. O Workfront indexa o conteúdo para que ele possa ser pesquisado posteriormente. Um limite de caracteres é aplicado para garantir o desempenho de alta qualidade do sistema Workfront.
author: Alina
feature: Get Started with Workfront
exl-id: f09dadf4-24f2-46d9-85ae-6081731d917d
TQID: https://experienceleague.adobe.com/5oa9RRT-VOFngI2UJncfwlVYfHXilftl8kpetBBY7-k
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 254
ht-degree: 8%

---

# Limites de caracteres em campos

Determinados campos no Adobe Workfront limitam o número de caracteres que podem ser incluídos no campo. O Workfront indexa o conteúdo para que ele possa ser pesquisado posteriormente. Um limite de caracteres é aplicado para garantir o desempenho de alta qualidade do sistema Workfront.

Quando você se aproxima do limite, um contador é exibido. Quando o limite é excedido, os caracteres em excesso são realçados e não é possível publicar o texto. Exclua os caracteres até que esteja dentro do limite permitido.

O limite de caracteres difere dependendo do campo que você está usando. Os limites mostrados abaixo se aplicam aos idiomas que usam o alfabeto latino (como inglês). O limite pode ser menor para idiomas que contenham caracteres estendidos ou de byte duplo.

Os administradores de grupo ou Workfront não podem modificar os limites de caracteres nos campos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Tipo de campo</strong> </p> </th> 
   <th> <p><strong>Limite de caracteres (</strong><strong>incluindo espaços)</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Campo de texto com formatação em um formulário personalizado</td> 
   <td>15.000</td> 
  </tr> 
  <tr> 
   <td> <p>Atualização de status</p> </td> 
   <td> <p>15.000</p>
   <p> 4.000 ao usar a API</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Atualização</p> </td> 
   <td> <p>15.000</p> 
   <p> 4.000 ao usar a API</p></td> 
  </tr> 
  <tr> 
   <td> <p>Descrição (documentos, tarefas, problemas, portfólios, programas e projetos)</p> </td> 
   <td> <p>4.000</p> </td> 
  </tr> 
  <tr> 
   <td>Campo de descrição em um formulário personalizado</td> 
   <td>4.000</td> 
  </tr> 
  <tr> 
   <td> <p>Parágrafo de dados personalizado ou texto de linha única  </p> </td> 
   <td> <p>2.000</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Campo de descrição na Report Builder</p> </td> 
   <td> <p>512</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Rótulo do menu suspenso</p> </td> 
   <td> <p>255</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Nome do objeto</p> </td> 
   <td> <p>255</p> </td> 
  </tr> 
 </tbody> 
</table>
