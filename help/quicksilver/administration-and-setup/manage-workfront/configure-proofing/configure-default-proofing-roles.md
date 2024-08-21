---
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-proofing-functionality
title: Configurar Funções de Revisão Padrão
description: Como administrador do Adobe Workfront, você pode configurar as funções de prova padrão para usuários e usuários convidados que acessam provas criadas no Workfront. Qualquer pessoa que adicionar usuários a uma prova poderá ajustar essas funções para ela.
author: Courtney
feature: System Setup and Administration, Digital Content and Documents
role: Admin
exl-id: d64213bf-f270-404f-a45a-6f94c7b7cb91
source-git-commit: ab774e937a15aaa04704e872579df880a9b80aaf
workflow-type: tm+mt
source-wordcount: '550'
ht-degree: 2%

---

# Configurar funções de revisão padrão

Como administrador do Adobe Workfront, você pode configurar as funções de prova padrão para usuários e usuários convidados que acessam provas criadas no Workfront. Qualquer pessoa que adicionar usuários a uma prova poderá ajustar essas funções para ela.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront*</td> 
   <td>Qualquer</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td>Plano</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Você deve ser um administrador do Workfront. Para obter informações sobre administradores do Workfront, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder a um usuário acesso administrativo total</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qual plano, tipo de licença ou acesso você tem, contate o administrador do Workfront.

+++

## Configurar funções de revisão padrão

{{step-1-to-setup}}

<!--
   <li In the left panel, click Proofs Proof roles.
   -->

1. Clique em **Revisar e aprovar** próximo à parte inferior da lista exibida à esquerda.
1. Na seção **Funções para destinatários designados de uma prova de documento**, selecione a função padrão para usuários e usuários convidados adicionados ao fluxo de trabalho de uma prova.

   Consulte [Direitos associados a funções de revisão](#rights-associated-with-proofing-roles) abaixo para obter uma lista de cada função de revisão e os direitos associados a ela.

   >[!NOTE]
   >
   >* Essa configuração se aplica somente aos usuários que são criados no sistema Workfront depois que a função é definida; não aos usuários existentes.
   >* A pessoa adicionando usuários à prova pode ajustar esta função, conforme descrito em [Adicionar usuários a uma prova](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md#add) em [Compartilhar uma prova no Adobe Workfront](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md).

1. Na seção **Funções para usuários que não são destinatários e que abrem uma prova de documento**, selecione a função padrão para usuários e usuários convidados que podem acessar uma prova, mas não são adicionados ao fluxo de trabalho da prova.

   Essa situação ocorre quando usuários e convidados têm acesso a um documento para o qual uma prova foi criada: mesmo que não tenham sido adicionados ao fluxo de trabalho da prova, eles podem abrir a prova.

   **Exemplos:** Estes são exemplos de como você pode usar esta configuração:

   * Você seleciona **Somente leitura** para limitar todas as atividades de prova, como adicionar comentários e tomar decisões para aqueles que foram solicitados a fazê-lo.
   * Você seleciona **Revisor** porque deseja que qualquer membro da equipe possa adicionar marcações e comentários em uma prova.

1. Clique em **Salvar**.

## Direitos associados a funções de prova {#rights-associated-with-proofing-roles}

A tabela a seguir mostra cada função e os direitos associados a ela:

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p> </p> </th> 
   <th> <p><strong>Exibir uma prova</strong> </p> </th> 
   <th> <p><strong>Adicionar marcações</strong> </p> </th> 
   <th> <p><strong>Adicionar comentários</strong> </p> </th> 
   <th> <p><strong>Editar comentários se não houver respostas</strong> </p> </th> 
   <th> <p><strong>Tomar uma decisão</strong> </p> </th> 
   <th> <p><strong>Excluir comentários feitos por outros</strong> </p> </th> 
   <th>Resolver comentários</th> 
   <th>Aplicar ações a comentários</th> 
   <th> <p><strong>Editar a prova</strong> </p> </th> 
   <th>Compartilhar a prova com outras pessoas</th> 
   <th>Criar nova versão</th> 
   <th> <p><strong>Exibir solicitações de aprovação na área Página inicial</strong> </p> </th> 
   <th>Adicionar novos revisores</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p><strong>Somente Leitura</strong> </p> </td> 
   <td> <p>✓ µ</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
   <td> </td> 
   <td>✓ µ</td> 
   <td> <p> </p> </td> 
   <td>✓ µ</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Oliveira</strong> </p> </td> 
   <td> <p>✓ µ</p> </td> 
   <td> <p>✓ µ</p> </td> 
   <td> <p>✓ µ</p> </td> 
   <td> <p>✓ µ</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
   <td> </td> 
   <td>✓ µ</td> 
   <td> <p> </p> </td> 
   <td>✓ µ</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Aprovador</strong> </p> </td> 
   <td> <p>✓ µ</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
   <td> <p>✓ µ</p> </td> 
   <td> <p> </p> </td> 
   <td> </td> 
   <td>✓ µ</td> 
   <td> <p> </p> </td> 
   <td>✓ µ</td> 
   <td> </td> 
   <td> <p>✓ µ</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Revisor e Aprovador</strong> </p> </td> 
   <td> <p>✓ µ</p> </td> 
   <td> <p>✓ µ</p> </td> 
   <td> <p>✓ µ</p> </td> 
   <td> <p>✓ µ</p> </td> 
   <td> <p>✓ µ</p> </td> 
   <td> <p> </p> </td> 
   <td> </td> 
   <td>✓ µ</td> 
   <td> <p> </p> </td> 
   <td>✓ µ</td> 
   <td> </td> 
   <td> <p>✓ µ</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Autor</strong> </p> </td> 
   <td> <p>✓ µ</p> </td> 
   <td> <p>✓ µ</p> </td> 
   <td> <p>✓ µ</p> </td> 
   <td> <p>✓ µ</p> </td> 
   <td> <p>✓ µ</p> </td> 
   <td> <p> </p> </td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td> <p>✓ µ</p> </td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td> </td> 
   <td>✓ µ</td> 
  </tr> 
  <tr> 
   <td> <p><strong>Moderador</strong> </p> </td> 
   <td> <p>✓ µ</p> </td> 
   <td> <p>✓ µ</p> </td> 
   <td> <p>✓ <strong></strong> </p> </td> 
   <td> <p>✓ µ</p> </td> 
   <td> <p>✓ µ</p> </td> 
   <td> <p>✓ µ</p> <p> </p> </td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td> <p>✓ µ</p> </td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>Os usuários nos novos planos do Workfront podem conceder funções de autor ou moderador a qualquer usuário no sistema. Os usuários em planos herdados podem conceder funções de autor ou moderador a qualquer usuário com uma licença de prova no sistema.
