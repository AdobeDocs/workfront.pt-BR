---
content-type: reference
product-area: reporting;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: "Exibir: relatório de documento com link para uma prova"
description: "Exibir: relatório de documento com link para uma prova"
author: Nolan
feature: Reports and Dashboards
exl-id: a38c5e86-9789-41ca-a832-2ee5eb0a570b
source-git-commit: 6405c01c8b1d842a4175f9caa18a7ed31316a3a1
workflow-type: tm+mt
source-wordcount: '313'
ht-degree: 1%

---

# Exibir: relatório de documento com link para uma prova

<!--Audited: 11/2024-->

Nesta visualização de documento, você pode inserir um link para uma prova da versão atual do documento.

![](assets/view-document-with-proof-link-350x92.png)

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

## Exibir um relatório de documento com link para uma prova

Para aplicar esta exibição:

1. Ir para uma lista de documentos.
1. No menu suspenso **Exibir**, selecione **Nova Exibição**.
1. Clique em **Adicionar coluna**.
1. Clique em **Alternar para Modo de Texto** e em **Editar Modo de Texto**.
1. Remova o texto localizado na caixa **Editar Modo de Texto** e substitua-o pelo seguinte código:

   ```
   displayname=Proof Link
   shortview=true
   textmode=true
   valueexpression=CONCAT("https://Your domain.my.workfront.com/document/",{currentVersion}.{ID},"/proof/",{currentVersion}.{proofID},"/view")
   valueformat=HTML
   ```

   >[!TIP]
   >
   >Substitua &quot;Seu domínio&quot; pelo domínio real do Workfront. Por exemplo, se a URL do Workfront da sua empresa for *Company.my.workfront.com*, seu domínio será &quot;Empresa&quot;.

1. Clique em **Concluído** e depois em **Salvar exibição**.
1. (Opcional) Atualize o nome da exibição e clique em **Salvar exibição**.
1. (Opcional) Para garantir que você exiba apenas documentos com provas, adicione um filtro fazendo o seguinte:

   1. Clique no menu suspenso **Filtro** e em **Novo Filtro**.
   1. Clique em **Adicionar uma regra de filtro** e comece a digitar &quot;Proprietário da prova&quot; e selecione **ID do proprietário da prova** quando ele for exibido na lista.
   1. Selecione **Não está em branco** para o modificador de filtro.
   1. Clique em **Salvar filtro**.
   1. (Opcional) Atualize o nome do filtro e clique em **Salvar filtro**.

1. Clique no link na coluna Link de prova para acessar a prova da última versão do documento.
