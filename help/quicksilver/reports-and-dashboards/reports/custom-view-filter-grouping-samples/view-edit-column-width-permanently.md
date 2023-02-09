---
content-type: reference
product-area: reporting;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: '"Exibir: editar permanentemente a largura de uma coluna'''
description: Você pode modificar temporariamente a largura das colunas, arrastando e soltando as margens para corresponder à largura desejada. Para obter mais informações, consulte Modificar a largura e a ordem da coluna.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 42633036-8e42-4cec-876c-f20a5ece2478
source-git-commit: bb348deb9841320a367695845efe0ca36a9a9d8b
workflow-type: tm+mt
source-wordcount: '389'
ht-degree: 0%

---

# Exibir: editar permanentemente a largura de uma coluna

Você pode modificar temporariamente a largura das colunas, arrastando e soltando as margens para corresponder à largura desejada. Para obter mais informações, consulte [Modificar a largura e a ordem da coluna](../../../reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md).

É possível alterar permanentemente a largura de qualquer coluna de qualquer exibição usando o modo de texto na coluna à medida que você edita a exibição.

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plano Adobe Workfront*</td> 
   <td> <p>Qualquer Um</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Plano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a Relatórios, Painéis, Calendários</p> <p>Editar acesso a filtros, visualizações, agrupamentos</p> <p>Observação: Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões de um relatório</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

## Editar permanentemente a largura de uma coluna

>[!IMPORTANT]
>
>Se você modificar manualmente a largura de uma coluna, conforme descrito na seção &quot;Modificar largura e ordem das colunas temporariamente&quot; no artigo [Modificar a largura e a ordem da coluna](../../../reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md) depois de modificar permanentemente a largura da coluna, a largura da coluna é preservada de acordo com o redimensionamento manual e a largura da coluna atualizada de acordo com as etapas a seguir é substituída. Você pode exibir a coluna de acordo com a largura definida nas etapas a seguir após limpar o cache ou fazer logon em outro navegador.

1. Vá para uma lista de objetos.
1. No **Exibir** , clique em **Nova exibição**.

1. Clique em **Adicionar coluna** para adicionar uma nova coluna.

   Ou

   Clique no cabeçalho da coluna de qualquer coluna existente.

1. Clique em **Alternar para o modo de texto**.
1. Passe o mouse sobre a área do modo de texto e clique em **Clique para editar texto**.
1. Adicione o seguinte código ao modo de texto da coluna:

   ```
   width=200
   usewidths=true
   ```

   Para o **largura** , especifique qualquer número (em pixels) que represente a largura com a qual você deseja que a coluna seja exibida na exibição.

1. Clique em **Salvar**, em seguida **Salvar exibição**.
