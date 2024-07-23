---
product-area: documents
navigation-topic: manage-proofs-within-workfront
title: Exibir estágios do fluxo de trabalho automatizado em uma prova
description: Você pode acompanhar convenientemente o progresso de uma prova configurada com um fluxo de trabalho automatizado. É possível visualizar, modificar, adicionar, iniciar e bloquear o trabalho já feito em estágios na prova.
author: Courtney
feature: Digital Content and Documents
exl-id: 71df1445-c64c-4de2-a9b8-23bd47898b6d
source-git-commit: f252e3562b8ea73486d407138251b3d15d4b9f3a
workflow-type: tm+mt
source-wordcount: '537'
ht-degree: 0%

---

# Exibir estágios do fluxo de trabalho automatizado em uma prova

Você pode acompanhar convenientemente o progresso de uma prova configurada com um fluxo de trabalho automatizado. É possível visualizar, modificar, adicionar, iniciar e bloquear o trabalho já feito em estágios na prova.

Para obter informações sobre como adicionar estágios e usuários a uma prova com um Fluxo de Trabalho Automatizado, consulte [Adicionar estágios e usuários a um Fluxo de Trabalho Automatizado em uma prova](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/add-stages-users-to-automated-workflow-proof.md).

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront*</td> 
   <td> <p>Plano atual: Pro ou Superior</p> <p>ou</p> <p>Plano herdado: Select ou Premium</p> <p>Para obter mais informações sobre acesso de revisão de texto com os diferentes planos, consulte <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Acesso à funcionalidade de revisão de texto no Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Plano atual: Trabalho ou Plano</p> <p>Plano herdado: Qualquer um (Você deve ter a prova ativada para o usuário)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Perfil de Permissões de Prova </td> 
   <td>Gerente ou superior</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a documentos</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso aos objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qual perfil de plano, função ou permissão de prova você tem, contate o administrador do Workfront ou do Workfront Proof.

+++

## Exibir o diagrama de Fluxo de Trabalho Automatizado

1. Em uma lista de documentos que contém o documento, passe o mouse sobre a linha que contém o documento e clique em **Fluxo de Trabalho de Revisão**.

   O diagrama do Fluxo de trabalho automatizado é exibido logo abaixo do título do Fluxo de trabalho.

   As etapas do diagrama são marcadas da seguinte maneira:

   ![dot.png](assets/dot.png) estágio ativo

   Estágio inativo ![gray_dot.png](assets/grey-dot.png)\
   ![sbw-key-icon.png](assets/sbw-key-icon.png)  Estágio privado

   ![sbw-padlock-icon.png](assets/sbw-padlock-icon.png)  Estágio bloqueado

   As linhas entre os estágios retratam as dependências entre os estágios. As linhas que levam aos estágios inativos são pontilhadas até que o estágio seja ativado.

   Você pode passar o mouse sobre um estágio no diagrama para exibir seu progresso. Se o estágio não estiver ativo e você tiver direitos de edição nele, poderá clicar no botão Ativar estágio ![](assets/activate-stage-btn.png) para iniciar o estágio. Se o estágio estiver ativo e você tiver direitos de edição nele, é possível bloqueá-lo. ![](assets/lock-stage-btn.png) Para obter mais informações sobre a Barra de progresso (S, O, C, D) , consulte  [Exibir o progresso e o status de uma prova no Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/view-progress-and-status-of-proof.md).

## Exibir um estágio

1. Em uma lista de documentos que contém o documento, passe o mouse sobre a linha que contém o documento e clique em **Fluxo de Trabalho de Revisão**.
1. No diagrama, clique no estágio que deseja exibir.

   ![](assets/view-stage-diagram-350x204.png)

1. Para expandir os detalhes de um estágio, clique na seta lateral abaixo do nome.

   ![](assets/stage-details-caret-350x167.png)

## Exibir todos os estágios

Para exibir todos os estágios em um fluxo de trabalho automatizado:

1. Clique no botão Alterar Exibição na parte superior da página ![](assets/change-view-btn.png) e em **Exibir todos os estágios**.

   Todos os estágios do fluxo de trabalho automatizado estão listados na seção, no entanto, os detalhes estão ocultos.

1. Para expandir os detalhes de um estágio, clique na seta lateral abaixo do nome.

## Exibir todos os estágios em detalhes

Para exibir todos os estágios do Fluxo de trabalho automatizado com os detalhes expandidos:

1. Clique no botão Alterar Exibição na parte superior da página ![](assets/change-view-btn.png) e clique em **Exibir todos os estágios em detalhes**.
1. Para exibir os detalhes de um estágio, clique na seta para baixo abaixo do nome.
