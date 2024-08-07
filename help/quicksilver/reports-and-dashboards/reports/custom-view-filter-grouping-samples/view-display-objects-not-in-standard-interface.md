---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: "View: objetos de exibição que não estão incluídos na interface padrão"
description: Você pode exibir em uma view objetos que não estão incluídos na interface de modo padrão. Você pode fazer isso somente referenciando-os pelo modo de texto.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: c0138730-494b-4443-865a-44f8f00d5342
source-git-commit: bcafa607da733b89747f6b448dd295d9b906d060
workflow-type: tm+mt
source-wordcount: '492'
ht-degree: 0%

---

# View: objetos de exibição que não estão incluídos na interface padrão

Você pode exibir em uma view objetos que não estão incluídos na interface de modo padrão. Você pode fazer isso somente referenciando-os pelo modo de texto.\
Você pode determinar quais campos podem ser incluídos em uma view de uma das seguintes maneiras:

* Use o [API Explorer](../../../wf-api/general/api-explorer.md) para descobrir outros objetos que podem ser referenciados pelo modo de texto.\
  Nem todos os campos documentados no API Explorer são campos válidos para o modo de texto. Alguns campos só podem ser relatados por meio da API.

* Localize o campo ID do objeto em uma coluna. A maioria dos objetos que têm uma ID de campo também tem uma coluna ou nome de campo correspondente que pode não ser acessível por meio da interface de modo padrão.

  Você pode usar o modo de texto para incluir em uma exibição o nome da coluna ou do campo, em vez da ID, substituindo o `fieldnameID` pelo `fieldname:name`.

  Por exemplo, na interface de modo padrão, o campo **ID do Proprietário do Portfolio** está disponível para uma exibição de projeto, mas o campo **Nome do Proprietário do Portfolio** não está. Você pode usar o modo texto para exibir o **Nome do Proprietário do Portfolio** na coluna de uma exibição.

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront*</td> 
   <td> <p>Qualquer</p> </td> 
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
   <td> <p>Gerenciar permissões para um relatório</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso aos objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qual plano, tipo de licença ou acesso você tem, contate o administrador do Workfront.

## Exemplo: adicionar a coluna Nome do proprietário do Portfolio a uma visualização do projeto

1. Ir para uma lista de projetos.
1. No menu suspenso **Exibir**, clique em **Nova Exibição**.

1. Clique em **Adicionar coluna** e comece a digitar &quot;ID de proprietário do Portfolio&quot; no campo **Mostrar nesta coluna** e, em seguida, selecione-a quando ela for exibida na lista.

1. Clique em **Alternar para Modo de Texto**.
1. Passe o mouse sobre a área do modo de texto e clique em **Clicar para editar o texto**.
1. Substitua a linha `valuefield` (`valuefield=portfolio:ownerID`) pela seguinte linha:

   ```
   valuefield=portfolio:owner:name
   ```

   Ou

   Remova o texto localizado na caixa **Modo de Texto** e substitua-o pelo seguinte código:

   ```
   valuefield=portfolio:owner:name
   querysort=portfolio:ownerID
   valueformat=HTML
   displayname=Portfolio Owner Name
   linkedname=portfolio
   ```

   Neste exemplo específico, o relatório classificará pelo ID de proprietário do Portfolio, conforme indicado pela linha `querysort`.

   >[!TIP]
   >
   >Para substituir qualquer campo `ID` pelo campo `name` usando o modo texto, sempre substitua `ID` por `:name` na linha `valuefield`.

1. Clique em **Salvar** e depois em **Salvar exibição**.
