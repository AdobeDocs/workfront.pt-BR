---
content-type: tips-tricks-troubleshooting
product-area: documents
navigation-topic: tips-tricks-and-troubleshooting-proofing-within-workfront
title: Listar usuários com licença de revisão no Adobe Workfront
description: Você pode visualizar quais usuários no Adobe Workfront têm atualmente a opção "O usuário pode gerar provas" ativada em qualquer uma das seguintes maneiras abaixo.
author: Courtney
feature: Digital Content and Documents
exl-id: 4d45ecd9-4348-43a4-9fa7-090b996b4695
TQID: https://experienceleague.adobe.com/9P5Bp9TrJ1ECSwpK7C4AW4rQlTQOBH4U7-CPYl92RKU
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: c1579802-ddd4-4214-8a91-97b2066abe11id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 312
ht-degree: 20%

---

# Listar usuários com licença de revisão no Adobe Workfront

Você pode visualizar quais usuários no Adobe Workfront têm atualmente a opção &quot;O usuário pode gerar provas&quot; ativada em qualquer uma das seguintes maneiras abaixo.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo.

Você deve ter o seguinte acesso para realizar as etapas descritas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacote do Adobe Workfront</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> 
   <p>Padrão</p> 
   <p>Plano</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Editar acesso a:</p> 
    <ul> 
     <li> <p>Criar relatórios, painéis e calendários</p> </li> 
     <li> <p>Criar filtros, visualizações e agrupamentos</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Criar um relatório de usuário

É possível criar um relatório de usuário para exibir quais usuários podem gerar provas:

1. Navegue até a área **Relatórios**.
1. Clique no menu suspenso **Novo Relatório** e em **Relatório de Usuário**.

1. Na guia **Filtros**, clique em **Adicionar uma Regra de Filtro**.

1. No campo disponível, expanda **Usuário** e clique em **Tem licença de comprovação**.

1. Selecione **Igual** > **Verdadeiro**.

   ![report_prooflicenses.png](assets/report-prooflicenses-350x135.png)

1. Clique em **Salvar+Fechar**.

   O relatório exibe todos os usuários do Workfront que têm uma licença de prova atribuída a eles.

## Atualizar a exibição Pessoas

Você pode adicionar uma nova coluna na visualização Pessoas para ver quais usuários podem gerar provas:

1. Vá para a área **Pessoas**.
1. Clique na guia **Pessoas**.
1. No menu suspenso **Exibir**, siga um destes procedimentos:

   * Para adicionar essas informações a um modo de exibição existente, selecione o modo de exibição que deseja personalizar e clique em **Personalizar Modo de Exibição**.
   * Para adicionar estas informações a um novo modo de exibição, clique em **Novo Modo de Exibição**.

1. Clique em **Adicionar coluna**.
1. No campo disponível, expanda **Usuário** e clique em **Tem licença de comprovação**.

1. Clique em **Concluído** e em **Salvar exibição** ou **Salvar como nova exibição**.

   A exibição mostra **True** ou **False**, dependendo se o usuário tem uma licença de prova atribuída a ele.
