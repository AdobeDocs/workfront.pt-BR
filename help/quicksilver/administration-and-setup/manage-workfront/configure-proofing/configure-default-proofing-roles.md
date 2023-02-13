---
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-proofing-functionality
title: Configurar funções de prova padrão
description: Como administrador do Adobe Workfront, você pode configurar as funções de prova padrão para usuários e usuários convidados que acessam provas criadas no Workfront. Qualquer pessoa que adicione usuários a uma prova pode ajustar essas funções para eles.
author: Courtney
feature: System Setup and Administration, Digital Content and Documents
role: Admin
exl-id: d64213bf-f270-404f-a45a-6f94c7b7cb91
source-git-commit: 02191d80ea58f80de2e7be2ff55f43663e415e31
workflow-type: tm+mt
source-wordcount: '508'
ht-degree: 1%

---

# Configurar funções de prova padrão

Como administrador do Adobe Workfront, você pode configurar as funções de prova padrão para usuários e usuários convidados que acessam provas criadas no Workfront. Qualquer pessoa que adicione usuários a uma prova pode ajustar essas funções para eles.

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plano Adobe Workfront*</td> 
   <td>Qualquer Um</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td>Plano</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Você deve ser um administrador do Workfront. Para obter informações sobre administradores do Workfront, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder ao usuário acesso administrativo total</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

## Configurar funções de prova padrão

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront, em seguida, clique em **Configuração** ![](assets/gear-icon-settings.png).

   <!--
   <li In the left panel, click Proofs Proof roles.
   -->

1. Clique em **Revisão e aprovação** próximo à parte inferior da lista exibida à esquerda.
1. No **Funções para destinatários designados de uma prova de documento** selecione a função padrão para usuários e usuários convidados adicionados ao fluxo de trabalho de uma prova.

   Consulte [Direitos associados às funções de revisão de texto](#rights-associated-with-proofing-roles) abaixo para obter uma lista de cada função de prova e os direitos associados a ela.

   >[!NOTE]
   >
   >* Essa configuração se aplica somente aos usuários criados no sistema Workfront após a definição da função; não aos usuários existentes.
   >* A pessoa que adiciona usuários à prova pode ajustar essa função, conforme descrito em [Adicionar usuários a uma prova](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md#add) em [Compartilhar uma prova no Adobe Workfront](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md).


1. No **Funções para não destinatários que abrem uma prova de documento** selecione a função padrão para usuários e usuários convidados que podem acessar uma prova, mas não são adicionados ao fluxo de trabalho da prova.

   Essa situação ocorre quando usuários e convidados têm acesso a um documento para o qual uma prova foi criada: mesmo que não tenham sido adicionados ao workflow da prova, eles poderão abrir a prova.

   **Exemplos:** Estes são exemplos de como você pode usar essa configuração:

   * Você seleciona **Somente leitura** limitar todas as atividades de prova, como adicionar comentários e tomar decisões àqueles que foram convidados a fazê-lo.
   * Você seleciona **Revisor** porque você deseja que qualquer membro da equipe possa adicionar marcações e comentários em uma prova.

1. Clique em **Salvar**.

## Direitos associados às funções de revisão de texto {#rights-associated-with-proofing-roles}

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
   <th> <p><strong>Editar comentários próprios se não houver respostas</strong> </p> </th> 
   <th> <p><strong>Tomar uma decisão</strong> </p> </th> 
   <th> <p><strong>Excluir comentários feitos por outras pessoas</strong> </p> </th> 
   <th>Resolver comentários</th> 
   <th>Aplicar ações aos comentários</th> 
   <th> <p><strong>Editar a prova</strong> </p> </th> 
   <th>Compartilhar a prova com outras pessoas</th> 
   <th>Criar nova versão</th> 
   <th> <p><strong>Exibir solicitações de aprovação na área inicial</strong> </p> </th> 
   <th>Adicionar novos revisores</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p><strong>Somente leitura</strong> </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
   <td> </td> 
   <td>✓</td> 
   <td> <p> </p> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Oliveira</strong> </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
   <td> </td> 
   <td>✓</td> 
   <td> <p> </p> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Aprovador</strong> </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> </td> 
   <td>✓</td> 
   <td> <p> </p> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> <p>✓</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Revisor e Aprovador</strong> </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> </td> 
   <td>✓</td> 
   <td> <p> </p> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> <p>✓</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Autor</strong> </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> <p>✓</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p><strong>Moderador</strong> </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p><strong>✓</strong> </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> <p> </p> </td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> <p>✓</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>Os usuários em novos planos do Workfront podem conceder funções de autor ou moderador a qualquer usuário do sistema. Os usuários em planos herdados podem conceder funções de autor ou moderador a qualquer usuário com uma licença de prova no sistema.
