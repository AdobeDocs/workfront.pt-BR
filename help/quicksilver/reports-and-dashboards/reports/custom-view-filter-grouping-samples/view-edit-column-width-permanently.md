---
content-type: reference
product-area: reporting;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Exibir: Editar Permanentemente a Largura de uma Coluna'
description: É possível modificar temporariamente a largura das colunas arrastando e soltando suas margens para corresponder à largura desejada. Para obter mais informações, consulte Modificar a largura e a ordem das colunas.
author: Courtney
feature: Reports and Dashboards
exl-id: 42633036-8e42-4cec-876c-f20a5ece2478
source-git-commit: 6a6d3d47ed5741e3202c44b7240a2e67b687ea95
workflow-type: tm+mt
source-wordcount: '381'
ht-degree: 12%

---

# Exibição: editar permanentemente a largura de uma coluna

<!-- Audited: 11/2024 -->

É possível modificar temporariamente a largura das colunas arrastando e soltando suas margens para corresponder à largura desejada. Para obter mais informações, consulte [Modificar largura e ordem da coluna](../../../reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md).

Para alterar permanentemente a largura de qualquer coluna de qualquer exibição, é necessário usar o modo de texto na coluna ao editar a exibição.

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
   <p>Colaborador ou Solicitação de modificação de uma exibição </p>
   <p>Padrão ou Plano para modificar um relatório</p>
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Acesso de edição a relatórios, painéis e calendários para modificar um relatório</p> <p>Acesso de edição a filtros, visualizações, agrupamentos para modificar uma visualização</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões para um relatório</p>  </td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações contidas nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Editar permanentemente a largura de uma coluna

>[!IMPORTANT]
>
>Se você modificar manualmente a largura de uma coluna conforme descrito na seção [Modificar a largura e a ordem das colunas temporariamente](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md#modify-width-and-order-of-columns-temporarily) do artigo [Modificar a largura e a ordem das colunas](../../../reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md) depois de modificar permanentemente a largura da coluna, a largura da coluna será preservada de acordo com seu redimensionamento manual. Nesse caso, a largura da coluna atualizada de acordo com as etapas a seguir será substituída. Você pode exibir a coluna de acordo com a largura definida nas etapas a seguir depois de limpar o cache ou fazer logon em outro navegador.
>
>Para obter informações adicionais sobre como personalizar a largura das colunas ao usar a interface do Modo de Texto, consulte as definições de “largura” e “ampliação” no [Glossário de terminologia do Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

1. Ir para uma lista de objetos.
1. No menu suspenso **Exibição**, clique em **Nova Exibição**.

1. Clique em **Adicionar Coluna** para adicionar uma nova coluna.

   Ou

   Clique no cabeçalho de qualquer coluna existente.

1. Clique em **Alternar para o Modo de Texto**.
1. Clique Em **Editar Modo De Texto**.T
1. Adicione o seguinte código ao modo de texto da coluna:

   ```
   width=200
   usewidths=true
   ```

   Para a linha **largura**, especifique qualquer número (em pixels) que represente a largura desejada para a coluna exibir no modo de exibição.

1. Clique em **Concluído** e depois em **Salvar exibição**.


