---
content-type: tips-tricks-troubleshooting
product-area: documents
navigation-topic: tips-tricks-and-troubleshooting-proofing-within-workfront
title: Listar usuários com uma licença de prova no Adobe Workfront
description: 'Você pode visualizar quais usuários no Adobe Workfront têm atualmente a opção "O usuário pode gerar provas" ativada de uma das seguintes maneiras:'
author: Courtney
feature: Digital Content and Documents
exl-id: 4d45ecd9-4348-43a4-9fa7-090b996b4695
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '370'
ht-degree: 0%

---

# Listar usuários com uma licença de prova no Adobe Workfront

Você pode visualizar quais usuários no Adobe Workfront têm atualmente a opção &quot;O usuário pode gerar provas&quot; ativada de uma das seguintes maneiras:

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plano Adobe Workfront*</td> 
   <td> <p>Plano herdado: Selecionar ou Premium</p> <p>Para obter mais informações sobre como revisar o acesso com os diferentes planos, consulte <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Acesso à funcionalidade de prova no Workfront</a>.</p> </td> 
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
    </ul> <p>Observação: Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode alterar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, função ou Perfil de permissão de prova você possui, entre em contato com o administrador da Workfront ou da Workfront Proof.

## Criar um relatório de usuário

Você pode criar um relatório de usuário para exibir quais usuários podem gerar provas:

1. Navegar para **Relatório** área.
1. Clique no botão **Novo relatório** menu suspenso e, em seguida, clique em **Relatório do usuário**.

1. No **Filtros** clique em **Adicionar uma regra de filtro**.

1. No campo disponível, expanda **Usuário**, depois clique em **Possui licença de prova**.

1. Selecionar **Igual** > **Verdadeiro**.

   ![report_prooflicense.png](assets/report-prooflicenses-350x135.png)

1. Clique em **Salvar+Fechar**.

   O relatório exibe todos os usuários no Workfront que têm uma licença de revisão atribuída a eles.

## Atualizar a exibição de Pessoas

É possível adicionar uma nova coluna na exibição Pessoas para exibir quais usuários podem gerar provas:

1. Vá para o **Pessoas** área.
1. Clique no botão **Pessoas** guia .
1. No **Exibir** no menu suspenso , siga um destes procedimentos:

   * Para adicionar essas informações a uma exibição existente, selecione a exibição que deseja personalizar e clique em **Personalizar exibição**.
   * Para adicionar essas informações a uma nova exibição, clique em **Nova exibição**.

1. Clique em **Adicionar coluna**.
1. No campo disponível, expanda **Usuário**, depois clique em **Possui licença de prova**.

1. Clique em **Concluído**, depois clique em **Salvar exibição** ou **Salvar como nova exibição**.

   A exibição é exibida **Verdadeiro** ou **Falso** dependendo se o usuário tem uma licença de prova atribuída a ele.
