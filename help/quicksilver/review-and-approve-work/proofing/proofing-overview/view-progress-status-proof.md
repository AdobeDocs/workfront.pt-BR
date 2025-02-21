---
product-area: documents
navigation-topic: manage-proofs-within-workfront
title: Visão geral do progresso e do status da prova
description: Você pode visualizar informações sobre como uma prova está avançando pelo processo de revisão e ver um resumo geral do status de decisão da prova na área Documentos.
author: Courtney
feature: Digital Content and Documents
exl-id: 78e81070-ff82-4d82-90a3-6e0cd176b290
source-git-commit: 1e67375c12bc473130127887e6cd4fa474c4fb02
workflow-type: tm+mt
source-wordcount: '376'
ht-degree: 1%

---

# Visão geral do progresso e do status da prova

Você pode visualizar informações sobre como uma prova está avançando pelo processo de revisão e ver um resumo geral do status de decisão da prova na área Documentos.

## Visão geral do progresso da prova

O progresso da prova indica o trabalho feito em uma prova desde o momento em que você envia a prova para os recipients até o momento em que eles tomam uma decisão sobre a prova. Os ícones de progresso S, O, C e D são exibidos ao lado do nome da prova e fornecem informações sobre o progresso da prova.

![Editar andamento existente](assets/proof-edit-existing-progress-350x62.png)

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <td> <p><strong>Ícone de progresso</strong> </p> </td> 
   <td> <p><strong>Descrição</strong> </p> </td> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p> <img src="assets/proof-progress-sent-icon.png" alt=""> </p> <p><strong>Enviado</strong> </p> </td> 
   <td> <p>A prova foi enviada aos destinatários atribuídos.</p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong></strong> </p> <p><strong>Aberto</strong> </p> </td> 
   <td> <p>Todos os recipients atribuídos abrem a página de detalhes da prova ou da prova.</p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong></strong> </p> <p><strong>Comentários feitos</strong> </p> </td> 
   <td> <p>Todos os recipients atribuídos fazem pelo menos um comentário na prova.</p> <p>Se não houver revisores atribuídos à prova, o ícone <strong>C</strong> não aparecerá na barra de progresso.</p> </td> 
  </tr> 
  <tr> 
   <td> <p> <img src="assets/proof-progress-decision-icon.png" alt=""> </p> <p><strong>Decisão tomada</strong> </p> </td> 
   <td> <p>Todos os aprovadores atribuídos tomam uma decisão sobre a prova, Todos os aprovadores atribuídos tomam uma decisão sobre a prova, a menos que o criador da prova especifique que apenas uma decisão é necessária.</p> <p>Se não houver aprovadores (tomadores de decisão) designados para a prova, o ícone <strong>D</strong> não aparecerá na barra de progresso. </p> </td> 
  </tr> 
 </tbody> 
</table>

Os ícones de progresso podem aparecer nas cores a seguir para indicar determinadas informações sobre o progresso da prova:

* **Verde**: Concluído.
* **Branco**: Não concluído.
* **Laranja**: não concluído e o prazo final é de menos de 24 horas.
* **Vermelho**: não concluído e ultrapassado o prazo.

<!--
<h3 data-mc-conditions="QuicksilverOrClassic.Draft mode">Levels of proof progress</h3>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Workfront Proof uses the progress icons to track a proof's progress at each of the following levels:</p>
-->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">For each reviewer, based on that person's activity on the proof.&nbsp;</li>
  -->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">For each stage, based on the progress the reviewer on the stage who is most behind in the proofing process.&nbsp;To learn more about stages, see <a href="../../../review-and-approve-work/proofing/proofing-overview/stages.md" class="MCXref xref">Automated Workflow Stages overview</a>.</li>
  -->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">For the proof, based on the progress of the stage (group of reviewers) who is the most behind in the proofing process.</li>
  -->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">For an example of how Workfront Proof determines progress using the reviewer or stage that is most behind,&nbsp;suppose three reviewers on a proof need to make a&nbsp;decision. If two of them have made their&nbsp;decision&nbsp;but the third has not, the progress bar for the proof does not show&nbsp;the D in green because of the outstanding&nbsp;decision.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">If the Primary Decision Maker setting is selected on a proof and the primary decision maker submits a decision, the D in the proof progress bar turns&nbsp;green for all reviewers because no other decisions are required.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Similarly, if the Only One Decision Required setting is selected on a proof and any reviewer submits a decision, the D in the proof progress bar turns&nbsp;green for all reviewers because no other decisions are required.</p>
-->

## Visão geral do status da prova

O status da prova exibe o status das decisões necessárias para a prova. O status da prova é determinado pelo participante com &quot;pior caso&quot;. Por exemplo, suponha que haja três decisões na prova: duas com o status **Aceitas** e uma com o status **Rejeitadas**. A decisão &quot;pior caso&quot; de **Rejected** ultrapassa as outras decisões e o status geral da prova é mostrado como **Rejected**. 

![Progresso existente de edição de prova](assets/proof-edit-existing-progress-350x62.png)

As opções de status padrão são as seguintes:

* Pendente
* Aprovado
* Aprovado com alterações
* Alterações necessárias
* Não Relevante

Se decisões personalizadas forem configuradas em sua conta, as opções de status refletirão suas configurações de decisão personalizadas.

<!--
<h2 data-mc-conditions="QuicksilverOrClassic.Draft mode">Viewing proof progress and status</h2>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> You can view the progress and status of proofs for individual documents. </p>
-->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="#view-proof-progress-and-status-for-a-document" class="MCXref xref">View proof progress and status&nbsp;for a document</a> </li>
  -->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="#view-proof-approval-information-in-home" class="MCXref xref">View proof approval information&nbsp;in Home</a> </li>
  -->

<!--
<h3 data-mc-conditions="QuicksilverOrClassic.Draft mode" id="view-proof-progress-and-status-for-a-document">View proof progress and status&nbsp;for a document</h3>
-->

<!--
   <li value="1" data-mc-conditions="QuicksilverOrClassic.Draft mode">If a proof has not already been generated for the document in Adobe Workfront, generate it, as described in the articles.</li>
   -->

<!--
   <li value="2" data-mc-conditions="QuicksilverOrClassic.Draft mode">In the Documents area, under the proof's name, click <strong>Proof Details</strong>.</li>
   -->

<!--
   <li value="3" data-mc-conditions="QuicksilverOrClassic.Draft mode">In the <strong>Proofing Details</strong> box that appears, the proof's progress for each stage, then click <strong>Done</strong>.</li>
   -->

<!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Under the proof's name, click <strong>Proofing Workflow</strong>.</p>
   -->

<!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
   <img src="assets/click-proofing-workflow-qs-350x149.png" style="width: 350;height: 149;" data-mc-conditions="QuicksilverOrClassic.Draft mode">
   -->
<!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   These screenshots will need to change with new terminology ("Review Workflow" for this one?)
   </MadCap:conditionalText>
   <br> </p>
   -->

<!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">In the Workflow information that appears, scroll down to see the proof's progress for each stage:</p>
   -->

<!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/scroll-to-see-socd-for-stages-qs-350x152.png" style="width: 350;height: 152;"> </p>
   -->

<!--
<h3 data-mc-conditions="QuicksilverOrClassic.Draft mode" id="view-proof-approval-information-in-home">View proof approval information&nbsp;in Home</h3>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">You can view information about proofs that you have submitted for approval. Proof approval information is displayed in the Home area only while the proof is pending approval.&nbsp;For information about how to view information about proof approvals in the Home area, see&nbsp;<a href="../../../review-and-approve-work/manage-approvals/view-approvals.md" class="MCXref xref">View approvals </a>.</p>
-->
