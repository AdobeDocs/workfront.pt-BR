---
product-area: documents
navigation-topic: review-proofs-within-workfront
title: Gerenciar notificações para comentários e decisões de prova
description: Ao trabalhar em uma prova, seja um usuário do Adobe Workfront ou um colaborador externo, você pode especificar quais notificações por email deseja receber sobre comentários e decisões tomadas na prova. Para obter mais informações, consulte Notificações para comentários de prova e visão geral de decisões.
author: Courtney
feature: Digital Content and Documents
exl-id: c38e005c-8984-4e99-9527-94a0a6b1071d
source-git-commit: c79d030ff2d05487e5f7e3457bf98df591822a80
workflow-type: tm+mt
source-wordcount: '800'
ht-degree: 2%

---

# Gerenciar notificações para comentários e decisões de prova

<!-- Audited: 4/2025 -->

Ao trabalhar em uma prova, seja um usuário do Adobe Workfront ou um colaborador externo, você pode especificar quais notificações por email deseja receber sobre comentários e decisões tomadas na prova. Para obter mais informações, consulte [Notificações para obter a visão geral de comentários de prova e decisões](../../../review-and-approve-work/proofing/proofing-overview/notifications-proof-comments-decisions.md).

>[!NOTE]
>
>Essas notificações são diferentes dos alertas de email que você pode receber sobre o fluxo de uma prova entre os revisores, bem como das configurações de alerta por email que podem ser definidas no Workfront.

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

## Gerenciar notificações para comentários e decisões de prova

1. Abra a prova para a qual deseja configurar notificações.
1. Se a barra de ferramentas esquerda não for exibida, clique no ícone **Menu** no canto superior esquerdo do Visualizador de Provas da Web.

   ![Ícone_Menu_in_Proofing_Viewer.png](assets/menu-icon-in-proofing-viewer-350x228.png)

1. Na barra de ferramentas esquerda, clique no ícone **Configurações** ![Ícone_Configurações.png](assets/settings-icon.png).

1. Na seção **Enviar notificações por email sobre**, selecione a configuração de notificação para esta prova.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Todas as atividades</td> 
      <td>Um email é enviado ao revisor sempre que há uma atividade na prova, como um novo comentário, resposta ou decisão.<br><p>Essa configuração é recomendada para a pessoa que gerencia o processo de prova, pois permite que ela veja a atividade quando ela ocorrer. Os usuários não recebem um alerta por email sobre suas próprias atividades (por exemplo, comentários, respostas ou decisões tomadas).</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Respostas aos meus comentários</td> 
      <td>Um email é enviado ao revisor somente se alguém responder diretamente ao comentário (excluindo as respostas em seus próprios comentários).<p>Essa configuração é recomendada para os clientes para que sejam notificados apenas das respostas aos seus próprios comentários e não de quaisquer outros comentários feitos na prova, embora ainda possam exibir todos os comentários no visualizador de provas.</p>
      <p>Para obter informações, consulte <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/view-proof-comments.md" class="MCXref xref">Exibir e responder aos comentários de prova</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Decisões</td> 
      <td>Um email é enviado ao revisor somente quando alguém toma uma decisão.<br><p>Esse alerta por email pode ser útil para a pessoa que está gerenciando o processo de aprovação, pois permite que a pessoa que gerencia o processo de aprovação monitore o progresso na prova e veja quais usuários tomaram sua decisão.<br></p><p>Você não é notificado sobre sua própria decisão, a menos que selecione uma opção de confirmação por email ao enviar sua decisão.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Decisão final</td> 
      <td>Um email é enviado quando a decisão final é tomada sobre a prova.<br><p>Esse alerta é usado com frequência pelo designer porque ele não precisa participar da discussão de revisão real. Quando a decisão final é tomada, o designer é notificado e pode então tomar medidas em relação a quaisquer alterações necessárias.<br></p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Resumo por hora</td> 
      <td>Um email é enviado ao revisor a cada hora com um resumo de todos os comentários, respostas e decisões que ocorreram na última hora.<br><p>O email é enviado somente quando a atividade além da sua ocorre na última hora. Se não houver atividade de outros usuários, nenhum email será enviado.<br></p><p>Este alerta é uma boa maneira de ter uma visão geral do projeto à medida que ele avança.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Resumo diário</td> 
      <td>(Configuração padrão): um email é enviado todos os dias com todos os comentários, respostas e decisões listados. Isso é enviado somente em dias quando há atividade além da sua.<br><p>Este alerta é uma boa maneira de ver um resumo do projeto sem precisar de várias atualizações ao longo do dia.<br></p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Nenhum email</td> 
      <td>Nenhum alerta de email é enviado.<br><p>Essa configuração é útil para uma pessoa que é adicionada a uma prova somente para fins de referência e não precisa ser notificada de qualquer alteração.</p><p>Nota: <p>Essa opção desativa apenas alertas de email sobre comentários e decisões de prova; não desativa os alertas de email que você pode receber sobre o fluxo de uma prova, como o email Nova prova ou Prova atrasada. Para obter mais informações, consulte os seguintes artigos: </p>
        <ul>
         <li><a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/new-proof-email.md" class="MCXref xref">Novo email de prova</a></li>
         <li><a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/new-version-email.md" class="MCXref xref">O email da nova versão</a></li>
         <li><a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/late-proof-email.md" class="MCXref xref">Email de prova tardia</a></li>
         <li><a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/proof-made-email.md" class="MCXref xref">O email de prova</a></li>
        </ul></p></td> 
     </tr> 
    </tbody> 
   </table>
