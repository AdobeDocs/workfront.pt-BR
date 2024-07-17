---
product-area: projects
navigation-topic: approvals
title: Aprovar trabalho
description: Aprovar trabalho
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: 6e43edbb-14dd-493d-a76b-84be6c3bef82
source-git-commit: 95679dd71ef7e4991853e63573a387f26321159d
workflow-type: tm+mt
source-wordcount: '1134'
ht-degree: 0%

---

# Aprovar trabalho

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;From&nbsp;Courtney: Linked to Training sites/ articles , don't change title and link)</p>
-->

Se você estiver definido como um aprovador, deverá revisar regularmente qual trabalho está aguardando sua aprovação.

Para obter informações sobre como criar processos de aprovação, consulte [Criar um processo de aprovação para itens de trabalho](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

Para obter informações sobre como associar aprovações ao trabalho no Workfront, consulte [Associar um processo de aprovação novo ou existente ao trabalho](../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront*</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Revisar ou superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Visualizar ou ter maior acesso aos objetos associados às aprovações</p> <p>Observação: se você ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Exibir permissões ou mais altas para os objetos associados às aprovações</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso aos objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qual plano, tipo de licença ou acesso você tem, contate o administrador do Workfront.

## Localizar aprovações no Adobe Workfront

Você pode visualizar e gerenciar aprovações em várias áreas do Workfront.

Para obter mais informações sobre como exibir itens que estão aguardando aprovação ou itens que você mesmo enviou para aprovação, consulte [Exibir aprovações](../../review-and-approve-work/manage-approvals/view-approvals.md).

## Aprovar trabalho na área Página inicial

1. Clique no ícone **Página inicial** ![](assets/home-icon-30x29.png) no canto superior esquerdo do Adobe Workfront.

   >[!NOTE]
   >
   >O administrador do Workfront pode fazer as seguintes alterações no ícone Início do ambiente:
   >
   >   
   >* Substitua-a por uma imagem personalizada para ilustrar sua organização. Nesse caso, o ícone será diferente do mostrado neste artigo.
   >* Substituir a página vinculada a ela por uma página diferente. Nesse caso, clique no **Menu Principal** ![](assets/main-menu-icon.png) no canto superior direito da página e clique em **Página Inicial**.

1. Clique no menu suspenso **Filtro**.

   ![](assets/displaying-work-items-filters-nwe-350x401.png)

1. Selecione **Aprovações**.\
   Todos os itens de trabalho que exigem sua aprovação são exibidos. 

   >[!NOTE]
   >
   >As aprovações atribuídas a funções ou grupos de trabalho não são exibidas na Página inicial. As aprovações atribuídas a Equipes são exibidas no agrupamento Solicitação de equipe na Lista de trabalho.

1. (Opcional) Altere a ordem na qual as aprovações são exibidas, conforme descrito na seção &quot;Agrupar e classificar por data, projeto ou prioridade&quot; no artigo [Exibir itens na Lista de Trabalho na área Página Inicial](../../workfront-basics/using-home/using-the-home-area/display-items-in-home-work-list.md).
1. Selecione o item em que deseja tomar uma decisão de aprovação.

   ![](assets/task-approval-home-350x127.png)

1. Clique em uma das opções disponíveis ao tomar uma decisão de aprovação no painel direito. As seguintes opções são exibidas no canto superior direito da página, dependendo do tipo de item que você está aprovando:

   * **Projetos:** Clique em **Aprovar** ou **Rejeitar**.

   * **Tarefas:** Clique em **Aprovar** ou **Rejeitar**.

   * **Problemas:** Clique em **Aprovar** ou **Rejeitar**.

   * **Folhas de horas:** Clique em **Aprovar** ou **Rejeitar**.

   * **Documentos:** Clique em **Aprovar**, **Rejeitar** ou **Alterações**.\
      Considere o seguinte ao visualizar  aprovações:

      * As aprovações de prova são exibidas aqui quando um usuário compartilha uma prova com você, conforme descrito na seção &quot;Compartilhar um link de prova&quot; no artigo [Compartilhar uma prova no Adobe Workfront](../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md).
      * As aprovações de provas são exibidas na área Página inicial somente se o ambiente do Workfront estiver integrado a uma conta do Workfront Proof Premium. Se não conseguir usar provas como discutido aqui, entre em contato com o administrador do Workfront.
      * Você recebe uma notificação no aplicativo, notificando você sobre a aprovação da prova.\
        Para obter mais informações sobre notificações no aplicativo, consulte [Exibir e gerenciar notificações no aplicativo](../../workfront-basics/using-notifications/view-and-manage-in-app-notifications.md).

      * O nome do usuário que solicitou a aprovação é exibido ao lado da imagem em miniatura na área Página inicial, com o seguinte texto:\
        &quot;*O Usuário A* deseja obter sua aprovação em...&quot;

        <!--      
        <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">      
        (NOTE:&nbsp;From&nbsp;Courtney: Is this true?)      
        </MadCap:conditionalText>      
        -->

        Se o nome de usuário não estiver disponível, o seguinte texto será exibido:\
        &quot;Uma nova versão de uma prova está pronta para ser visualizada&quot;
      * Para tomar uma decisão de aprovação na prova, clique em **Ir para Prova**, clique em **Concluir revisão** e em uma das opções disponíveis. As opções disponíveis ao aprovar uma prova são: **Aprovado**, **Aprovado com alterações**, **Alterações necessárias** e **Não relevante**.

      * Depois que uma decisão é tomada sobre a prova, ela permanece na guia Minhas aprovações com o texto &quot;Tomada de decisão&quot; até que você clique no botão **Atualizar** ou até que você atualize a página do navegador.

        Para obter informações sobre como revisar uma prova, consulte [Revisar provas no Adobe Workfront](../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-proofs-in-wf.md).

   * **Acesso:** Selecione o nível de acesso a ser concedido no menu suspenso **Alterar acesso** e clique em **Conceder acesso**. Ou clique em **Ignorar**.

## Aprovar o trabalho diretamente de um projeto, tarefa ou problema

Quando um projeto, tarefa ou problema tem aprovação pendente, você pode aprovar ou rejeitar a aprovação diretamente do projeto, tarefa ou problema. Você também pode exibir detalhes sobre o processo de aprovação.

Para aprovar o trabalho diretamente de um projeto, tarefa ou problema:

1. Vá para o projeto, tarefa ou problema que requer sua aprovação.

   As informações de aprovação referentes ao processo de aprovação atual de um projeto, tarefa ou problema são exibidas no cabeçalho do item.

   ![](assets/current-approval-process-in-project-header-with-stages-nwe-350x92.png)

   As seguintes informações de aprovação estão disponíveis:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Status</td> 
      <td>O status atual do projeto, tarefa ou problema. Este é o status atual do item que está pendente de aprovação. O status é approved após cada estágio do processo de aprovação ser aprovado.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Estágios de aprovação</td> 
      <td>Os estágios do processo de aprovação. <br>O estágio atual com aprovação pendente é exibido como Pendente. Os estágios que já foram aprovados são exibidos como Aprovado ; os estágios que ainda não foram aprovados são exibidos como Não iniciado .</td> 
     </tr> 
    </tbody> 
   </table>

1. Clique em **Aprovar** ou **Rejeitar**, dependendo se você deseja aprovar ou rejeitar o processo de aprovação.\
   O estágio de aprovação que estava pendente de aprovação agora é aprovado, e o processo de aprovação passa para o próximo estágio. O status é aprovado após a aprovação de todos os estágios.

## Aprovar um documento diretamente de um documento 

1. Vá para a área de documentos que contém o documento que requer sua aprovação.
1. Selecione o documento e clique em **Aprovar**, **Alterações** ou **Rejeitar**.\
   ![](assets/approval-approve-document-350x215.png)\
   ![](assets/document-approval-350x199.png)

1. (Opcional) Se uma prova tiver sido gerada para o documento, você poderá aprovar o documento na interface de prova, conforme descrito em [Aprovar um documento a partir de uma prova](#approve-a-document-from-a-proof).

## Aprovar um documento a partir de um email de notificação de aprovação

Dependendo das configurações de notificação, você pode receber emails notificando sobre documentos para os quais outros usuários precisam que você tome uma decisão de aprovação. Ao receber um email contendo um botão **Tomar uma Decisão de Aprovação**, você pode iniciar o processo de aprovação diretamente do email:

1. No email, clique em **Tomar uma decisão de aprovação** para abrir a página Detalhes do documento para a prova.
1. Siga um destes procedimentos para revisar o documento:

   * Visualize os metadados sobre o documento.
   * Se uma prova tiver sido criada para revisar o documento com marcação e comentários, clique em **Abrir prova** ![](assets/open-proof-icon-qs.png) próximo ao canto superior direito e revise a prova.

     <!--   
     <span style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">[Andrzej, does it make sense to leave this here if it's s document approval?&nbsp;Would there never be a proof in that situation?]</span>   
     -->

     Para obter informações sobre como revisar provas, consulte [Revisar provas no Adobe Workfront](../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-proofs-in-wf.md).

1. Clique em uma opção de **Decisão** no canto superior direito para aprovar, aprovar com alterações ou rejeitar o documento.

## Aprovar um documento a partir de uma prova {#approve-a-document-from-a-proof}

Você pode aprovar um documento no visualizador de provas. Para obter mais informações, consulte [Tomar uma decisão sobre uma prova no visualizador de provas](../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md) no artigo [Tomar uma decisão sobre uma prova no visualizador de provas](../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md).
