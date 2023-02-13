---
product-area: projects
navigation-topic: approvals
title: Aprovar trabalho
description: Aprovar trabalho
author: Courtney
feature: Work Management
exl-id: 6e43edbb-14dd-493d-a76b-84be6c3bef82
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '1134'
ht-degree: 0%

---

# Aprovar trabalho

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;From&nbsp;Courtney: Linked to Training sites/ articles , don't change title and link)</p>
-->

Se você estiver definido como um aprovador, deverá revisar regularmente qual trabalho está aguardando sua aprovação.

Para obter informações sobre a criação de processos de aprovação, consulte [Criar um processo de aprovação para itens de trabalho](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

Para obter informações sobre como associar aprovações ao trabalho no Workfront, consulte [Associar um processo de aprovação novo ou existente ao trabalho](../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plano Adobe Workfront*</td> 
   <td> <p>Qualquer Um</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Revisar ou superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Exibir ou obter acesso mais alto aos objetos associados às aprovações</p> <p>Observação: Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Visualizar permissões ou permissões superiores para os objetos associados às aprovações</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

## Localizar aprovações no Adobe Workfront

Você pode visualizar e gerenciar aprovações em várias áreas do Workfront.

Para obter mais informações sobre como visualizar itens que aguardam aprovações ou itens que você mesmo tenha enviado para aprovação, consulte [Exibir aprovações](../../review-and-approve-work/manage-approvals/view-approvals.md).

## Aprovar trabalho da área inicial

1. Clique no botão **Início** ícone ![](assets/home-icon-30x29.png) no canto superior esquerdo do Adobe Workfront.

   >[!NOTE]
   >
   >O administrador do Workfront pode fazer as seguintes alterações no ícone Início no seu ambiente:
   >
   >   
   >* Substitua por uma imagem personalizada para ilustrar sua organização. Nesse caso, o ícone terá uma aparência diferente da mostrada neste artigo.
   >* Substitua a página vinculada a ela por uma página diferente. Nesse caso, clique no botão **Menu principal** ![](assets/main-menu-icon.png) no canto superior direito da página, em seguida, clique em **Início**.


1. Clique no botão **Filtro** menu suspenso.

   ![](assets/displaying-work-items-filters-nwe-350x401.png)

1. Selecionar **Aprovações**.\
   Todos os itens de trabalho que exigem sua aprovação são exibidos. 

   >[!NOTE]
   >
   >Aprovações atribuídas a Atribuições de Trabalho ou Grupos não são exibidas na Página Inicial. Aprovações atribuídas a equipes são exibidas no agrupamento Solicitação de equipe na Lista de trabalho.

1. (Opcional) Altere a ordem em que as aprovações são exibidas, conforme descrito na seção &quot;Agrupar e classificar por data, projeto ou prioridade&quot; no artigo [Exibir itens na Lista de Trabalho na área Início](../../workfront-basics/using-home/using-the-home-area/display-items-in-home-work-list.md).
1. Selecione o item para o qual deseja tomar uma decisão de aprovação.

   ![](assets/task-approval-home-350x127.png)

1. Clique em uma das opções disponíveis ao tomar uma decisão de aprovação no painel direito. As seguintes opções são exibidas no canto superior direito da página, dependendo do tipo de item que você está aprovando:

   * **Projetos:** Clique em **Aprovar** ou **Rejeitar**.

   * **Tarefas:** Clique em **Aprovar** ou **Rejeitar** .

   * **Problemas:** Clique em **Aprovar** ou **Rejeitar** .

   * **Folhas de horas:** Clique em **Aprovar** ou **Rejeitar** .

   * **Documentos:** Clique em **Aprovar**, **Rejeitar** ou **Alterações**.\
       Considere o seguinte ao exibir aprovações:

      * As aprovações de prova são exibidas aqui quando um usuário compartilha uma prova com você, conforme descrito na seção &quot;Compartilhar um link de prova&quot; no artigo [Compartilhar uma prova no Adobe Workfront](../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md).
      * As aprovações de prova são exibidas na área inicial somente se o ambiente do Workfront estiver integrado a uma conta do Workfront Proof Premium . Se não puder usar a prova, conforme discutido aqui, entre em contato com o administrador do Workfront.
      * Você recebe uma notificação no aplicativo, notificando-o da aprovação de prova.\
         Para obter mais informações sobre notificações no aplicativo, consulte [Exibir e gerenciar notificações no aplicativo](../../workfront-basics/using-notifications/view-and-manage-in-app-notifications.md).

      * O nome do usuário que solicitou a aprovação é exibido ao lado da imagem em miniatura na área Início, com o seguinte texto:\
         &quot;*Usuário A* gostaria de sua aprovação em...&quot;

         <!--      
        <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">      
        (NOTE:&nbsp;From&nbsp;Courtney: Is this true?)      
        </MadCap:conditionalText>      
        -->

         Se o nome de usuário não estiver disponível, o seguinte texto será exibido:\
         &quot;Uma nova versão de uma prova está pronta para exibição&quot;
      * Para tomar uma decisão de aprovação na prova, clique em **Ir para prova**, clique em **Concluir revisão**, em seguida, clique em uma das opções disponíveis. As opções disponíveis ao aprovar uma prova são: **Aprovado**, **Aprovado com alterações**, **Alterações necessárias** e **Não relevante**.

      * Depois que uma decisão é tomada na prova, a prova permanece na guia Minhas aprovações com o texto &quot;Decisão tomada&quot; até que você clique na guia **Atualizar** ou até atualizar a página do navegador.

         Para obter informações sobre como revisar uma prova, consulte [Revisar provas no Adobe Workfront](../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-proofs-in-wf.md).
   * **Acesso:** Selecione o nível de acesso a conceder na **Alterar acesso** menu suspenso e, em seguida, clique em **Conceder acesso**. Ou, clique em **Ignorar**.


## Aprovar o trabalho diretamente de um projeto, tarefa ou problema

Quando um projeto, tarefa ou problema está pendente de aprovação, você pode aprovar ou rejeitar a aprovação diretamente do projeto, tarefa ou problema. Você também pode visualizar detalhes sobre o processo de aprovação.

Para aprovar o trabalho diretamente de um projeto, tarefa ou problema:

1. Vá para o projeto, tarefa ou problema que requer sua aprovação.

   Informações de aprovação sobre o processo de aprovação atual de um projeto, tarefa ou problema são exibidas no cabeçalho do item.

   ![](assets/current-approval-process-in-project-header-with-stages-nwe-350x92.png)

   As seguintes informações de aprovação estão disponíveis:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Status</td> 
      <td>O status atual do projeto, da tarefa ou do problema. Este é o status atual do item que está pendente da aprovação. O status é aprovado após cada etapa do processo de aprovação ser aprovada.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Etapas de aprovação</td> 
      <td>As etapas do processo de aprovação. <br>O estágio atual que está pendente de aprovação é exibido como Pendente . Os estágios já aprovados são exibidos como Aprovado ; os estágios que ainda não foram aprovados são exibidos como Não iniciado .</td> 
     </tr> 
    </tbody> 
   </table>

1. Clique em **Aprovar** ou **Rejeitar**, dependendo de se deseja aprovar ou rejeitar o processo de aprovação.\
   A fase de aprovação que estava pendente de aprovação agora é aprovada e o processo de aprovação avança para a próxima etapa. O status é aprovado após todas as etapas terem sido aprovadas.

## Aprovar um documento diretamente de um documento 

1. Vá para a área de documentos que contém o documento que requer sua aprovação.
1. Selecione o documento e clique em **Aprovar**, **Alterações** ou **Rejeitar**.\
   ![](assets/approval-approve-document-350x215.png)\
   ![](assets/document-approval-350x199.png)

1. (Opcional) Se uma prova tiver sido gerada para o documento, você poderá aprovar o documento na interface de revisão de texto, conforme descrito em [Aprovar um documento de uma prova](#approve-a-document-from-a-proof).

## Aprovar um documento de um email de notificação de aprovação

Dependendo das configurações de notificação, você pode receber emails notificando sobre documentos para os quais outros usuários precisam que você tome uma decisão de aprovação. Ao receber um email contendo um **Tornar decisão de aprovação** , é possível iniciar o processo de aprovação diretamente do email:

1. No email, clique em **Tornar decisão de aprovação** para abrir a página Detalhes do documento para a prova .
1. Siga qualquer um destes procedimentos para revisar o documento:

   * Exibir os metadados sobre o documento.
   * Se tiver sido criada uma prova para revisar o documento com marcação e comentários, clique em **Abrir prova** ![](assets/open-proof-icon-qs.png) próximo ao canto superior direito e revise a prova.

      <!--   
     <span style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">[Andrzej, does it make sense to leave this here if it's s document approval?&nbsp;Would there never be a proof in that situation?]</span>   
     -->

      Para obter informações sobre como revisar provas, consulte [Revisar provas no Adobe Workfront](../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-proofs-in-wf.md).

1. Clique em um **Decisão** no canto superior direito para aprovar, aprovar com alterações ou rejeitar o documento.

## Aprovar um documento de uma prova {#approve-a-document-from-a-proof}

Você pode aprovar um documento no visualizador de prova. Para obter mais informações, consulte [Tome uma decisão em uma prova no visualizador de prova](../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md) no artigo [Tome uma decisão em uma prova no visualizador de prova](../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md).
