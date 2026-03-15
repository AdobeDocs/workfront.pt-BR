---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Agrupamento: Organizar os Resultados da Lista por um Valor Calculado Comum a Todos os Objetos no Agrupamento'
description: Convém exibir as tarefas agrupadas por Porcentagem Concluída em intervalos de 0-25, 26-50, 51-75, 75-99 e 100. Para fazer isso, você pode criar um agrupamento usando o modo de texto.
author: Courtney
feature: Reports and Dashboards
exl-id: 93b743ce-7e54-4a96-933b-912e2107a84f
source-git-commit: 6a6d3d47ed5741e3202c44b7240a2e67b687ea95
workflow-type: tm+mt
source-wordcount: '247'
ht-degree: 22%

---

# Agrupamento: organizar os resultados da lista por um valor calculado comum a todos os objetos no agrupamento

<!--Audited: 10/2024-->

Convém exibir as tarefas agrupadas por Porcentagem Concluída em intervalos de 0-25, 26-50, 51-75, 75-99 e 100. Para fazer isso, você pode criar um agrupamento usando o modo de texto.

![Agrupando por valor calculado](assets/grouping-calculated-value-column-to-all-objects.png)

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

## Organizar os resultados da lista por um valor calculado comum a todos os objetos no agrupamento

Para aplicar este agrupamento a uma lista de tarefas:

1. Ir para uma lista de tarefas.
1. No menu suspenso **Agrupamento** selecione **Novo Agrupamento**.

1. Clique em **Alternar para o Modo de Texto**.
1. No espaço disponível, adicione o seguinte código:

   ```
   textmode=true
   group.0.valueexpression=IF({percentComplete}>=0&&{percentComplete}<=25,'0-25%',IF({percentComplete}>25&&{percentComplete}<=50,'26-50%',IF({percentComplete}>50&&{percentComplete}<=75,'51-75%',IF({percentComplete}>75&&{percentComplete}<=100,'76-100%',''))))
   group.0.linkedname=direct
   group.0.valueformat=doubleAsString
   group.0.namekey=percentComplete
   ```

1. Clique em **Concluído** e depois em **Salvar Agrupamento**.
1. (Opcional) Atualize o nome do agrupamento e clique em **Salvar Agrupamento**.
