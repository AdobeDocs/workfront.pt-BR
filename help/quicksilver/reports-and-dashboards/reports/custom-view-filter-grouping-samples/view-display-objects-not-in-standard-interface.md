---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Exibir: Exibir Objetos que Não Estão Incluídos na Interface Padrão'
description: É possível exibir em uma exibição objetos que não estão incluídos na interface de modo padrão. Você só pode fazer isso fazendo referência a eles por meio do modo de texto.
author: Courtney
feature: Reports and Dashboards
exl-id: c0138730-494b-4443-865a-44f8f00d5342
source-git-commit: 6a6d3d47ed5741e3202c44b7240a2e67b687ea95
workflow-type: tm+mt
source-wordcount: '437'
ht-degree: 9%

---

# Exibir: objetos de exibição que não estão incluídos na interface padrão

Você pode exibir em uma view objetos que não estão incluídos na interface de modo padrão. Você pode fazer isso somente referenciando-os pelo modo de texto.\
É possível determinar quais campos podem ser incluídos em uma view de uma das seguintes maneiras:

* Use o [API Explorer](../../../wf-api/general/api-explorer.md) para descobrir outros objetos que podem ser referenciados por meio do modo de texto.\
  Nem todos os campos documentados no API Explorer são campos válidos para o modo de texto. Alguns campos podem ser relatados somente por meio da API.

* Localize o campo ID do objeto em uma coluna. A maioria dos objetos que tem um ID de campo também tem uma coluna ou nome de campo correspondente, que pode não ser acessível pela interface de modo padrão.

  Você pode usar o modo de texto para incluir em uma exibição o nome da coluna ou do campo em vez da ID, substituindo a `fieldnameID` pela `fieldname:name`.

  Por exemplo, na interface de modo padrão, o campo **ID do proprietário do Portfolio** está disponível para uma exibição de projeto, mas o campo **Nome do proprietário do Portfolio** não está. Você pode usar o modo de texto para exibir o **Nome do Proprietário do Portfolio** na coluna de um modo de exibição.

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

## Exemplo: adicionar a coluna Nome do proprietário do Portfolio a uma visualização do projeto

1. Ir para uma lista de projetos.
1. No menu suspenso **Exibição**, clique em **Nova Exibição**.

1. Clique em **Adicionar coluna** e comece a digitar “ID de proprietário do Portfolio&quot; no campo **Mostrar nesta coluna** e selecione-a quando for exibida na lista.

1. Clique em **Alternar para o Modo de Texto** e depois em **Editar Modo de Texto**.
1. Substitua a linha `valuefield` (`valuefield=portfolio:ownerID`) pela seguinte linha:

   `valuefield=portfolio:owner:name`

   Ou

   Remova o texto encontrado na caixa **Editar Modo de Texto** e substitua-o pelo seguinte código:

   ```
   valuefield=portfolio:owner:name
   querysort=portfolio:ownerID
   valueformat=HTML
   displayname=Portfolio Owner Name
   linkedname=portfolio
   ```

   Neste exemplo específico, o relatório classificará o relatório pelo ID do Proprietário do Portfolio, conforme indicado pela linha `querysort`.

   >[!TIP]
   >
   >Para substituir qualquer campo `ID` pelo campo `name` usando o modo texto, sempre substitua `ID` por `:name` na linha `valuefield`.

1. Clique em **Concluído** e depois em **Salvar exibição**.
