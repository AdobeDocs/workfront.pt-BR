---
content-type: reference
product-area: reporting;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: "Exibir: editar permanentemente a largura de uma coluna"
description: Você pode modificar temporariamente a largura das colunas arrastando e soltando suas margens para corresponder à largura desejada. Para obter mais informações, consulte Modificar a largura e a ordem da coluna.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 42633036-8e42-4cec-876c-f20a5ece2478
source-git-commit: 7ee96045e5673c51c3ce348f395226857686a923
workflow-type: tm+mt
source-wordcount: '434'
ht-degree: 0%

---

# Exibir: edite permanentemente a largura de uma coluna

Você pode modificar temporariamente a largura das colunas arrastando e soltando suas margens para corresponder à largura desejada. Para obter mais informações, consulte [Modificar a largura e a ordem da coluna](../../../reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md).

É possível alterar permanentemente a largura de qualquer coluna de qualquer exibição usando o modo de texto na coluna à medida que você edita a exibição.

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront*</td> 
   <td> <p>Qualquer Um</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Solicitação para modificar uma exibição </p>
   <p>Planejar a modificação de um relatório</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a relatórios, painéis e calendários para modificar um relatório</p> <p>Editar acesso a Filtros, Visualizações, Agrupamentos para modificar uma visualização</p> <p><b>Nota</b>

Se você ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td>
</tr>  
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões para um relatório</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir seu plano, tipo de licença ou acesso, entre em contato com o administrador do Workfront.

## Editar permanentemente a largura de uma coluna

>[!IMPORTANT]
>
>Se você modificar manualmente a largura de uma coluna conforme descrito na seção &quot;Modifique temporariamente a largura e a ordem das colunas&quot; no artigo [Modificar a largura e a ordem da coluna](../../../reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md) depois de modificar permanentemente a largura da coluna, ela será preservada de acordo com o redimensionamento manual e a largura da coluna atualizada de acordo com as etapas a seguir será substituída. Você pode visualizar a coluna de acordo com a largura definida nas etapas a seguir depois de limpar o cache ou fazer logon em outro navegador.
>
>Para obter informações adicionais sobre como personalizar a largura das colunas ao usar a interface do Modo de texto, consulte as definições de &quot;largura&quot; e &quot;ampliação&quot; na [Glossário da terminologia do Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

1. Ir para uma lista de objetos.
1. No **Exibir** clique em **Nova visualização**.

1. Clique em **Adicionar coluna** para adicionar uma nova coluna.

   Ou

   Clique no cabeçalho de qualquer coluna existente.

1. Clique em **Alternar para modo de texto**.
1. Passe o mouse sobre a área do modo de texto e clique em **Clique para editar o texto**.
1. Adicione o seguinte código ao modo de texto da coluna:

   ```
   width=200
   usewidths=true
   ```

   Para o **largura** especifique qualquer número (em pixels) que represente a largura desejada para a exibição da coluna na exibição.

1. Clique em **Salvar**, depois **Salvar visualização**.


