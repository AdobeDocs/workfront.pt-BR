---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '"Exibir: exibir objetos que não estão incluídos na interface padrão'''
description: É possível exibir em uma exibição objetos que não estão incluídos na interface do modo padrão. Você só pode fazer isso referenciando-os por meio do modo de texto. Você pode determinar quais campos podem ser incluídos em uma exibição de qualquer uma das seguintes maneiras - EDITE-ME.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: c0138730-494b-4443-865a-44f8f00d5342
source-git-commit: 89a6d856f9f87a67b6a2ccfb4282f9f6200b977c
workflow-type: tm+mt
source-wordcount: '498'
ht-degree: 0%

---

# Exibir: exibir objetos que não estão incluídos na interface padrão

É possível exibir em uma exibição objetos que não estão incluídos na interface do modo padrão. Você só pode fazer isso referenciando-os por meio do modo de texto.\
Você pode determinar quais campos podem ser incluídos em uma exibição de uma das seguintes maneiras:

* Use o [API Explorer](https://one.workfront.com/s/api-explorer) para descobrir outros objetos que podem ser referenciados por meio do modo de texto.\
   Nem todos os campos documentados no API Explorer são campos válidos para o modo de texto. Alguns campos só podem ser reportados por meio da API.

* Localize o campo ID do objeto em uma coluna. A maioria dos objetos que têm uma ID de campo também tem uma coluna ou nome de campo correspondente que pode não ser acessível por meio da interface de modo padrão.

   Você pode usar o modo de texto para incluir em uma exibição o nome da coluna ou do campo, em vez da ID, substituindo o `fieldnameID` com o `fieldname:name`.

   Por exemplo, na interface de modo padrão, a variável **ID do proprietário do Portfolio** está disponível para uma visualização de projeto, mas o campo **Nome do proprietário do Portfolio** não é. Você pode usar o modo de texto para exibir a variável **Nome do proprietário do Portfolio** na coluna de uma exibição.

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

## Exemplo: adicionar a coluna Nome do Proprietário do Portfolio a uma exibição de projeto

1. Acesse uma lista de projetos.
1. No **Exibir** , clique em **Nova exibição**.

1. Clique em **Adicionar coluna** em seguida, comece a digitar &quot;ID de proprietário do Portfolio&quot; no **Mostrar nesta coluna** e, em seguida, selecione-o quando for exibido na lista.

1. Clique em **Alternar para o modo de texto**.
1. Passe o mouse sobre a área do modo de texto e clique em **Clique para editar texto**.
1. Substitua o `valuefield` linha (`valuefield=portfolio:ownerID`) com a seguinte linha:

   ```
   valuefield=portfolio:owner:name
   ```

   Ou

   Remova o texto que você encontrar no **Modo de texto** e substitua-a pelo seguinte código:

   ```
   valuefield=portfolio:owner:name
   querysort=portfolio:ownerID
   valueformat=HTML
   displayname=Portfolio Owner Name
   linkedname=portfolio
   ```

   Neste exemplo específico, o relatório classificará o relatório pela ID de proprietário do Portfolio, conforme indicado pela variável `querysort` linha.

   >[!TIP]
   >
   >Para substituir qualquer campo `ID` com o campo `name` usando o modo de texto, sempre substituir `ID` com `:name` no `valuefield` linha.

1. Clique em **Salvar**, em seguida **Salvar exibição**.
