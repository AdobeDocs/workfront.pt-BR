---
product-area: documents
navigation-topic: manage-proofs-within-workfront
title: Exibir estágios do fluxo de trabalho automatizado em uma prova
description: Você pode acompanhar o progresso de uma prova configurada com um Fluxo de trabalho automatizado. Você pode exibir, modificar, adicionar, iniciar e bloquear o trabalho já feito em etapas na prova.
author: Courtney
feature: Digital Content and Documents
exl-id: 71df1445-c64c-4de2-a9b8-23bd47898b6d
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '527'
ht-degree: 0%

---

# Exibir estágios do fluxo de trabalho automatizado em uma prova

Você pode acompanhar o progresso de uma prova configurada com um Fluxo de trabalho automatizado. Você pode exibir, modificar, adicionar, iniciar e bloquear o trabalho já feito em etapas na prova.

Para obter informações sobre como adicionar estágios e usuários a uma prova com um Fluxo de trabalho automatizado, consulte [Adicionar estágios e usuários a um Fluxo de trabalho automatizado em uma prova](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/add-stages-users-to-automated-workflow-proof.md).

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plano Adobe Workfront*</td> 
   <td> <p>Plano atual: Pro ou superior</p> <p>ou</p> <p>Plano herdado: Selecionar ou Premium</p> <p>Para obter mais informações sobre como revisar o acesso com os diferentes planos, consulte <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Acesso à funcionalidade de prova no Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Plano atual: Trabalho ou Plano</p> <p>Plano herdado: Qualquer (É necessário ter a prova ativada para o usuário)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Perfil de Permissões de Prova </td> 
   <td>Gerente ou superior</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a documentos</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, função ou Perfil de permissão de prova você possui, entre em contato com o administrador da Workfront ou da Workfront Proof.

## Visualizar o diagrama de Fluxo de trabalho automatizado

1. Em uma lista de documentos que contém o documento, passe o mouse sobre a linha que contém o documento e clique em **Fluxo de trabalho de prova**.

   O diagrama do Fluxo de trabalho automatizado é exibido logo abaixo do título do Fluxo de trabalho.

   As etapas no diagrama são marcadas da seguinte maneira:

   ![dot.png](assets/dot.png) Fase ativa

   ![gray_dot.png](assets/grey-dot.png) Estágio inativo\
   ![sbw-key-icon.png](assets/sbw-key-icon.png)  Fase privada

   ![sbw-padlock-icon.png](assets/sbw-padlock-icon.png)  Estágio bloqueado

   As linhas entre os estágios mostram as dependências entre os estágios. As linhas que levam a estágios inativos são pontilhadas até que o estágio seja ativado.

   Você pode passar o mouse sobre um estágio no diagrama para exibir seu progresso. Se o estágio não estiver ativo e você tiver direitos de edição no palco, clique no botão Ativar palco ![](assets/activate-stage-btn.png) para iniciar o estágio. Se o palco estiver ativo e você tiver direitos de edição no palco, poderá bloqueá-lo. ![](assets/lock-stage-btn.png) Para obter mais informações sobre a Barra de progresso (S, O, C, D) , consulte  [Visualizar o progresso e o status de uma prova na prova do Workfront](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/view-progress-and-status-of-proof.md).

## Exibir um estágio

1. Em uma lista de documentos que contém o documento, passe o mouse sobre a linha que contém o documento e clique em **Fluxo de trabalho de prova**.
1. No diagrama, clique no estágio que deseja visualizar.

   ![](assets/view-stage-diagram-350x204.png)

1. Para expandir os detalhes de um palco, clique na seta para os lados abaixo de seu nome.

   ![](assets/stage-details-caret-350x167.png)

## Exibir todos os estágios

Para exibir todos os estágios em um Fluxo de trabalho automatizado:

1. Clique no botão Alterar exibição na parte superior da página ![](assets/change-view-btn.png), depois clique em **Exibir todos os estágios**.

   Todos os estágios do Fluxo de trabalho automatizado são listados na seção , no entanto, os detalhes são ocultos.

1. Para expandir os detalhes de um palco, clique na seta para os lados abaixo de seu nome.

## Exibir todos os estágios detalhadamente

Para exibir todos os estágios do Fluxo de trabalho automatizado com seus detalhes expandidos:

1. Clique no botão Alterar exibição na parte superior da página ![](assets/change-view-btn.png), depois clique em **Exibir todos os estágios detalhadamente**.
1. Para exibir os detalhes de um palco, clique na seta para baixo sob seu nome.
