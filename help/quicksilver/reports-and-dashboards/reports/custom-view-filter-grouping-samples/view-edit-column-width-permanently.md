---
content-type: reference
product-area: reporting;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: "Visualização: editar permanentemente a largura de uma coluna"
description: Você pode modificar temporariamente a largura das colunas arrastando e soltando suas margens para corresponder à largura desejada. Para obter mais informações, consulte Modificar a largura e a ordem da coluna.
author: Nolan
feature: Reports and Dashboards
exl-id: 42633036-8e42-4cec-876c-f20a5ece2478
source-git-commit: 71c0bf664af66bec7122651c1b62dd1c28022565
workflow-type: tm+mt
source-wordcount: '403'
ht-degree: 0%

---

# Exibir: edite permanentemente a largura de uma coluna

<!-- Audited: 11/2024 -->

Você pode modificar temporariamente a largura das colunas arrastando e soltando suas margens para corresponder à largura desejada. Para obter mais informações, consulte [Modificar largura e ordem da coluna](../../../reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md).

Para alterar permanentemente a largura de qualquer coluna de qualquer exibição, você deve usar o modo de texto na coluna à medida que edita a exibição.

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
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td> <p>Novo:<ul><li>Colaborador para modificar uma visualização</li><li>Padrão para modificar um relatório</li></ul></p><p>Ou</p>Atual:<ul><li>Solicitação para modificar uma exibição</li><li>Planejar a modificação de um relatório</li></ul></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Editar acesso a relatórios, painéis e calendários para modificar um relatório</p> <p>Editar acesso a Filtros, Visualizações, Agrupamentos para modificar uma visualização</p> </td> 
  </tr>  
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões para um relatório</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Editar permanentemente a largura de uma coluna

>[!IMPORTANT]
>
>Se você modificar manualmente a largura de uma coluna conforme descrito na seção [Modificar temporariamente a largura e a ordem das colunas](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md#modify-width-and-order-of-columns-temporarily) no artigo [Modificar a largura e a ordem da coluna](../../../reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md) após modificar permanentemente a largura da coluna, ela será preservada de acordo com o redimensionamento manual. Nesse caso, a largura da coluna atualizada de acordo com as etapas a seguir é substituída. Você pode visualizar a coluna de acordo com a largura definida nas etapas a seguir depois de limpar o cache ou fazer logon em outro navegador.
>
>Para obter informações adicionais sobre como personalizar a largura das colunas ao usar a interface do Modo de Texto, consulte as definições de &quot;largura&quot; e &quot;ampliação&quot; no [Glossário da terminologia do Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

1. Ir para uma lista de objetos.
1. No menu suspenso **Exibir**, clique em **Nova Exibição**.

1. Clique em **Adicionar coluna** para adicionar uma nova coluna.

   Ou

   Clique no cabeçalho de qualquer coluna existente.

1. Clique em **Alternar para Modo de Texto**.
1. Clique Em **Editar Modo De Texto**.T
1. Adicione o seguinte código ao modo de texto da coluna:

   ```
   width=200
   usewidths=true
   ```

   Para a linha **largura**, especifique qualquer número (em pixels) que represente a largura desejada para a exibição da coluna no modo de exibição.

1. Clique em **Concluído** e depois em **Salvar exibição**.


