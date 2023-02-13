---
content-type: reference
product-area: reporting;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: '"Exibir: relatório de documento com link para uma prova'''
description: '"Exibir: relatório de documento com link para uma prova'''
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: a38c5e86-9789-41ca-a832-2ee5eb0a570b
source-git-commit: 40c7142574c3491b7bdf8799c287db1c3f7e9e8c
workflow-type: tm+mt
source-wordcount: '339'
ht-degree: 0%

---

# Exibir: relatório de documento com link para uma prova

Nesta exibição de documento, você pode inserir um link para uma prova da versão atual do documento.

![](assets/view-document-with-proof-link-350x92.png)

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

## Exibir um relatório de documento com link para uma prova

Para aplicar esta exibição:

1. Vá para uma lista de documentos.
1. No **Exibir** , selecione **Nova exibição**.

1. Clique em **Adicionar coluna**.
1. Clique em **Alternar para o modo de texto**.
1. Passe o mouse sobre a área do modo de texto e clique em **Clique para editar texto**.
1. Remova o texto que você encontrar no **Modo de texto** e substitua-a pelo seguinte código:

   ```
   displayname=Proof Link
   
   shortview=true
   
   textmode=true
   
   valueexpression=CONCAT("https://Your domain.my.workfront.com/document/",{currentVersion}.{ID},"/proof/",{currentVersion}.{proofID},"/view")
   
   valueformat=HTML
   ```

   >[!TIP]
   >
   >Substitua &quot;Seu domínio&quot; pelo domínio real do Workfront. Por exemplo, se o url do Workfront de sua empresa for *Company.my.workfront.com*, seu domínio é &quot;Empresa&quot;.

1. Clique em **Salvar**, em seguida **Salvar exibição**.
1. Digite um nome para a exibição e clique em **Salvar exibição**.
1. (Opcional) Para garantir que você exiba apenas documentos com provas, adicione um filtro fazendo o seguinte:

   1. Clique no botão **Filtro** menu suspenso e, em seguida, clique em **Novo filtro**.
   1. Clique em **Adicionar uma regra de filtro** e comece a digitar Proprietário da Prova e selecione **ID de Proprietário da Prova** quando for exibido na lista.
   1. Selecionar **Não está em Branco** para o modificador de filtro.
   1. Clique em **Salvar filtro**, digite o nome do filtro e, em seguida, clique em **Salvar filtro**.

1. Clique no link na coluna Link de prova para acessar a prova da última versão do documento.
