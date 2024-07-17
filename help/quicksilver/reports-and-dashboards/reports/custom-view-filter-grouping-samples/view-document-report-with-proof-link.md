---
content-type: reference
product-area: reporting;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: "Exibir: relatório de documento com link para uma prova"
description: "Exibir: relatório de documento com link para uma prova"
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: a38c5e86-9789-41ca-a832-2ee5eb0a570b
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '356'
ht-degree: 1%

---

# Exibir: relatório de documento com link para uma prova

Nesta visualização de documento, você pode inserir um link para uma prova da versão atual do documento.

![](assets/view-document-with-proof-link-350x92.png)

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

## Exibir um relatório de documento com link para uma prova

Para aplicar esta exibição:

1. Ir para uma lista de documentos.
1. No menu suspenso **Exibir**, selecione **Nova Exibição**.

1. Clique em **Adicionar coluna**.
1. Clique em **Alternar para Modo de Texto**.
1. Passe o mouse sobre a área do modo de texto e clique em **Clicar para editar o texto**.
1. Remova o texto localizado na caixa **Modo de Texto** e substitua-o pelo seguinte código:

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

1. Clique em **Salvar** e depois em **Salvar exibição**.
1. Digite um nome para o modo de exibição e clique em **Salvar Modo de Exibição**.
1. (Opcional) Para garantir que você exiba apenas documentos com provas, adicione um filtro fazendo o seguinte:

   1. Clique no menu suspenso **Filtro** e em **Novo Filtro**.
   1. Clique em **Adicionar uma regra de filtro**, comece a digitar o Proprietário da prova e selecione **ID do Proprietário da prova** quando ele for exibido na lista.
   1. Selecione **Não está em branco** para o modificador de filtro.
   1. Clique em **Salvar filtro**, digite o nome do filtro e clique em **Salvar filtro**.

1. Clique no link na coluna Link de prova para acessar a prova da última versão do documento.
