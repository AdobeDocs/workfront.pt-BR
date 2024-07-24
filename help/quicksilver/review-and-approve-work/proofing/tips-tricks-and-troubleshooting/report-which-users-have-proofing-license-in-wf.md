---
content-type: tips-tricks-troubleshooting
product-area: documents
navigation-topic: tips-tricks-and-troubleshooting-proofing-within-workfront
title: Listar usuários com uma licença de prova no Adobe Workfront
description: Você pode visualizar quais usuários no Adobe Workfront têm atualmente a opção "O usuário pode gerar provas" ativada em qualquer uma das seguintes maneiras abaixo.
author: Courtney
feature: Digital Content and Documents
exl-id: 4d45ecd9-4348-43a4-9fa7-090b996b4695
source-git-commit: 8af531868249f609113af6d2a8465af01edcbc3f
workflow-type: tm+mt
source-wordcount: '380'
ht-degree: 1%

---

# Listar usuários com uma licença de prova no Adobe Workfront

Você pode visualizar quais usuários no Adobe Workfront têm atualmente a opção &quot;O usuário pode gerar provas&quot; ativada em qualquer uma das seguintes maneiras abaixo.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront*</td> 
   <td> <p>Plano herdado: Select ou Premium</p> <p>Para obter mais informações sobre acesso de revisão de texto com os diferentes planos, consulte <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Acesso à funcionalidade de revisão de texto no Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Plano</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Editar acesso a:</p> 
    <ul> 
     <li> <p>Criar relatórios, painéis e calendários</p> </li> 
     <li> <p>Criar filtros, visualizações e agrupamentos</p> </li> 
    </ul> <p>Observação: se você ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode alterar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qual perfil de plano, função ou permissão de prova você tem, contate o administrador do Workfront ou do Workfront Proof.

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
