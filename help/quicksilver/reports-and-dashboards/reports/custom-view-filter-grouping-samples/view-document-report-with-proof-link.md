---
content-type: reference
product-area: reporting;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Exibir: Relatório de documento com link para uma prova'
description: 'Exibição: relatório do documento com link para uma prova'
author: Courtney
feature: Reports and Dashboards
exl-id: a38c5e86-9789-41ca-a832-2ee5eb0a570b
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/bRL7x0qjHQrwg-HfxtJcazG9GK0WifSsl13VL1K5hGs
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 306
ht-degree: 20%

---

# Exibição: relatório do documento com link para uma prova

<!--Audited: 11/2024-->

Nesta visualização de documento, você pode inserir um link para uma prova da versão atual do documento.

![Exibir documento com link de prova](assets/view-document-with-proof-link-350x92.png)

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
   <p>Colaborador ou Solicitação para modificar um filtro </p>
   <p>Padrão ou Plano para modificar um relatório</p>
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

Para obter mais detalhes sobre as informações contidas nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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
