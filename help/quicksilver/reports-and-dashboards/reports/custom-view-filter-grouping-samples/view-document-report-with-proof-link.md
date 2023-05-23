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
ht-degree: 0%

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

## Exibir um relatório de documento com link para uma prova

Para aplicar esta exibição:

1. Ir para uma lista de documentos.
1. No **Exibir** selecione **Nova visualização**.

1. Clique em **Adicionar coluna**.
1. Clique em **Alternar para modo de texto**.
1. Passe o mouse sobre a área do modo de texto e clique em **Clique para editar o texto**.
1. Remova o texto localizado na **Modo de texto** e substitua-o pelo seguinte código:

   ```
   displayname=Proof Link
   
   shortview=true
   
   textmode=true
   
   valueexpression=CONCAT("https://Your domain.my.workfront.com/document/",{currentVersion}.{ID},"/proof/",{currentVersion}.{proofID},"/view")
   
   valueformat=HTML
   ```

   >[!TIP]
   >
   >Substitua &quot;Seu domínio&quot; pelo domínio real do Workfront. Por exemplo, se o URL do Workfront da sua empresa for *Company.my.workfront.com*, seu domínio é &quot;Empresa&quot;.

1. Clique em **Salvar**, depois **Salvar visualização**.
1. Digite um nome para a exibição e clique em **Salvar visualização**.
1. (Opcional) Para garantir que você exiba apenas documentos com provas, adicione um filtro fazendo o seguinte:

   1. Clique em **Filtro** e, em seguida, clique em **Novo Filtro**.
   1. Clique em **Adicionar uma regra de filtro** e comece digitando Proprietário da prova, em seguida, selecione **ID do proprietário da prova** quando ele é exibido na lista.
   1. Selecionar **Não está em branco** para o modificador de filtro.
   1. Clique em **Salvar Filtro**, digite o nome do filtro e clique em **Salvar Filtro**.

1. Clique no link na coluna Link de prova para acessar a prova da última versão do documento.
