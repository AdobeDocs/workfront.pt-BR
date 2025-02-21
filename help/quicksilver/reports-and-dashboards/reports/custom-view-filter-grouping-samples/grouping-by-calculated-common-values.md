---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Agrupamento: Organizar os Resultados da Lista por um Valor Calculado Comum a Todos os Objetos no Agrupamento'
description: Talvez você queira exibir suas tarefas agrupadas por Percentual concluído nas faixas de 0 a 25, 26 a 50, 51 a 75, 75 a 99 e 100. Para fazer isso, é possível criar um agrupamento usando o modo de texto.
author: Nolan
feature: Reports and Dashboards
exl-id: 93b743ce-7e54-4a96-933b-912e2107a84f
source-git-commit: 70bda5a7186abfa7e8cbd26e25a4c58583a322b4
workflow-type: tm+mt
source-wordcount: '261'
ht-degree: 0%

---

# Agrupamento: organize os resultados da lista por um valor calculado comum a todos os objetos no agrupamento

<!--Audited: 10/2024-->

Talvez você queira exibir suas tarefas agrupadas por Percentual concluído nas faixas de 0 a 25, 26 a 50, 51 a 75, 75 a 99 e 100. Para fazer isso, é possível criar um agrupamento usando o modo de texto.

![Agrupamento por valor calculado](assets/grouping-calculated-value-column-to-all-objects.png)

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

## Organiza os resultados da lista por um valor calculado comum a todos os objetos no agrupamento

Para aplicar esse agrupamento a uma lista de tarefas:

1. Ir para uma lista de tarefas.
1. No menu suspenso **Agrupamento** selecione **Novo Agrupamento**.

1. Clique em **Alternar para Modo de Texto**.
1. No espaço disponível, adicione o seguinte código:

   ```
   textmode=true
   group.0.valueexpression=IF({percentComplete}>=0&&{percentComplete}<=25,'0-25%',IF({percentComplete}>25&&{percentComplete}<=50,'26-50%',IF({percentComplete}>50&&{percentComplete}<=75,'51-75%',IF({percentComplete}>75&&{percentComplete}<=100,'76-100%',''))))
   group.0.linkedname=direct
   group.0.valueformat=doubleAsString
   group.0.namekey=percentComplete
   ```

1. Clique em **Concluído** e em **Salvar agrupamento**.
1. (Opcional) Atualize o nome do agrupamento e clique em **Salvar agrupamento**.
