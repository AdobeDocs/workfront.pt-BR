---
product-area: documents
navigation-topic: review-proofs-within-workfront
title: Tomar uma decisão sobre uma prova no visualizador de provas
description: Você pode tomar uma decisão sobre uma prova diretamente no visualizador de provas.
author: Courtney
feature: Digital Content and Documents
exl-id: cf74ac54-b8c1-4404-b35f-2aa94831ecad
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '391'
ht-degree: 3%

---

# Tomar uma decisão sobre uma prova no visualizador de provas

Você pode tomar uma decisão sobre uma prova diretamente no visualizador de provas.

## Requisitos de acesso

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
   <td role="rowheader">Função de prova</td> 
   <td>Aprovador, Revisor e Aprovador, Autor, Moderador</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a documentos</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso aos objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qual perfil de plano, função ou permissão de prova você tem, contate o administrador do Workfront ou do Workfront Proof.

## Tomar uma decisão sobre uma prova no visualizador de provas

1. Vá para o projeto, tarefa ou problema que contém o documento e selecione **Documentos**.
1. Encontre a prova necessária e clique em **Abrir prova**.

1. Clique em **Tomar uma Decisão** na parte superior central do visualizador de revisões.

1. Na caixa **Decisão da prova** exibida, clique em uma das seguintes decisões:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Aprovado</td> 
      <td>A prova está pronta para ir ao próximo estágio do fluxo de trabalho automatizado.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Aprovado com alterações</td> 
      <td>A prova exige algumas alterações, mas você não precisa ver a revisão antes de ela passar para o próximo estágio do Fluxo de trabalho automatizado.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Alterações exigidas</td> 
      <td>A prova exige alterações e você precisa ver outra revisão antes de passar para o próximo estágio do Fluxo de trabalho automatizado.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Não é relevante</td> 
      <td>A prova não é relevante para você e você não precisa tomar uma decisão.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Decisão personalizada</td> 
      <td> <p>Nos planos Select e Premium, o administrador do Workfront ou do Workfront Proof pode renomear, reordenar e ocultar decisões. Para obter mais informações, consulte <a href="../../../../workfront-proof/wp-acct-admin/account-settings/configure-approval-decision-in-wp.md" class="MCXref xref">Configurar opções de decisão de aprovação no Workfront Proof</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Condicional) Se o administrador do Adobe Workfront ou do Workfront Proof tiver adicionado uma seção Motivos, selecione os motivos aplicáveis para sua decisão. Para obter mais informações sobre como os administradores podem configurar motivos de decisão, consulte  [Configurar opções de decisão de aprovação no Workfront Proof](../../../../workfront-proof/wp-acct-admin/account-settings/configure-approval-decision-in-wp.md).
1. (Opcional) Selecione **Enviar-me uma confirmação por email** para receber uma confirmação por email da sua decisão.
1. Clique em **Tomar uma decisão**.

<!--
<h2 data-mc-conditions="QuicksilverOrClassic.Draft mode">Make a decision when the proof is configured with an approval process</h2>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">You can make decisions on a proof when it is configured with an approval process (within Workfront) and&nbsp;a user has sent you a document approval request, as described in <a href="../../../../review-and-approve-work/manage-approvals/request-document-approvals.md" class="MCXref xref">Request document approvals</a>.</p>
-->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="#make-a-workfront-approval-decision-in-a-proof" class="MCXref xref">Make a Workfront approval decision in a proof</a> </li>
  -->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="#change-your-workfront-approval-decision-in-a-proof" class="MCXref xref">Change your Workfront approval decision in a proof</a> </li>
  -->

<!--
<h3 data-mc-conditions="QuicksilverOrClassic.Draft mode" id="make-a-workfront-approval-decision-in-a-proof">Make a Workfront approval decision in a proof</h3>
-->

<!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Open the proof of the document that you want to make a decision on.</p>
   -->

<!--
   <li value="2" data-mc-conditions="QuicksilverOrClassic.Draft mode">In the proofing viewer, select whether you want to <strong>Approve</strong>, require <strong>Changes</strong>, or <strong>Reject</strong> the approval request.</li>
   -->

<!--
<h3 data-mc-conditions="QuicksilverOrClassic.Draft mode" id="change-your-workfront-approval-decision-in-a-proof">Change your Workfront approval decision in a proof</h3>
-->

<!--
<ol data-mc-conditions="QuicksilverOrClassic.Draft mode">
<li value="1">Open the proof of the document where you want to change your Workfront approval decision.</li>
<li value="2"> <p>At the top-center of the proofing viewer, click the decision you made previously.</p> </li>
<li value="3">In the <strong>Proof decision</strong> box that appears, select whether you want to <strong>Approve</strong>, require <strong>Changes</strong>, or <strong>Reject</strong> the approval request.</li>
</ol>
-->
