---
product-area: documents
navigation-topic: review-proofs-within-workfront
title: Compartilhar uma prova do visualizador de prova
description: Você pode compartilhar uma prova no visualizador de prova se o compartilhamento estiver habilitado pelo proprietário ou criador da prova.
author: Courtney
feature: Digital Content and Documents
exl-id: 20bd2d94-1401-4a38-9042-335d0cb32a3d
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '1512'
ht-degree: 0%

---

# Compartilhar uma prova do visualizador de prova

Você pode compartilhar uma prova no visualizador de prova se o compartilhamento estiver habilitado pelo proprietário ou criador da prova.

>[!IMPORTANT]
>
>A configuração Permitir o compartilhamento de prova por URL público ou código incorporado deve estar ativada.

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
   <td> <p>Editar acesso a documentos</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, função ou Perfil de permissão de prova você possui, entre em contato com o administrador da Workfront ou da Workfront Proof.

## Compartilhar o URL

Você pode compartilhar uma prova por meio de um URL se o proprietário tiver configurado a prova para compartilhamento. Os proprietários de prova podem atualizar as configurações de compartilhamento a qualquer momento. Para obter mais informações, consulte [Editar configurações de prova](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/edit-proof-settings.md).

1. Se o menu do ícone à esquerda não for exibido, clique no botão **Menu** ícone no canto superior esquerdo do visualizador de prova.

   ![](assets/menu-icon-in-proofing-viewer-350x188.png)

1. No menu do ícone à esquerda do visualizador de prova, clique no botão **Compartilhar** ícone .

   ![Share_btn_in_viewer.png](assets/share-btn-in-viewer.png)

1. No **Compartilhar prova** opções exibidas, verifique se **Obter link compartilhável** está selecionada.

1.  Siga um destes procedimentos:

   * Para copiar o link para a área de transferência, clique em **Copiar link**.

      Agora é possível distribuir o link por meio de uma ferramenta de terceiros, como um chat ou um aplicativo de email.

   * Para enviar o link por email diretamente do Adobe Workfront, faça o seguinte:

      1. No **Ou link de email para** , comece a digitar e selecione o nome do recipient. Ou especifique o endereço de email de um usuário externo com o qual você deseja compartilhar.

         >[!NOTE]
         >
         >Se você vir um email de alias ao compartilhar uma prova, não crie um novo usuário convidado inserindo o email original se um email de alias correspondente existir.

      1. Selecione dentre as seguintes opções:

         <table style="table-layout:auto">
          <col>
          <col>
          <tbody>
           <tr>
            <td role="rowheader">Enviar link público</td>
            <td><p>Inclui um botão na notificação por email que direciona os usuários para a prova no visualizador de prova que estão usando e concede acesso à Exibição.</p><p>If <strong>Assinar prova via URL público ou código incorporado</strong> estiver desativado para a prova, os usuários poderão fazer logon com suas credenciais de logon da Workfront para adicionar comentários à prova. Se estiver ativada, qualquer pessoa que forneça seu endereço de email e nome (sem senha necessária) poderá assinar e adicionar comentários à prova.</p></td>
           </tr>
           <tr>
            <td role="rowheader">Enviar link de download</td>
            <td>Inclui um botão na notificação por email que direciona os usuários para uma página de download, que fornece detalhes do arquivo, nome do arquivo e tamanho do arquivo, com o arquivo exibido em linha. Os usuários podem clicar no link Download da página de download para baixar o arquivo.</td>
           </tr>
           <tr>
            <td role="rowheader">Adicionar mensagem personalizada</td>
            <td>Permite especificar um assunto e corpo personalizados para a notificação por email.</td>
           </tr>
          </tbody>
         </table>

      1. Clique em **Enviar**.

         Seus recipients recebem uma notificação por email contendo informações sobre a prova e os botões que você escolheu incluir.

         ![](assets/proof-share-email-350x87.png)

## Compartilhar o código incorporado

Você pode compartilhar uma prova por meio do código incorporado se o proprietário da prova a tiver configurado para isso.

Para compartilhar uma prova por meio do código incorporado:

1. Na barra de ferramentas à esquerda do visualizador de prova, clique no botão **Compartilhar** ícone .

   ![Share_btn_in_viewer__1_.png](assets/share-btn-in-viewer--1-.png)

1. No **Compartilhar prova** opções exibidas, clique em **Obter código incorporado**, depois clique em **Copiar**.

## Compartilhar uma prova adicionando usuários a ela

É possível adicionar usuários a uma prova ao revisar uma prova se você tiver uma das seguintes permissões:

* Permissões de supervisor ou administrador
* Permissões do gerente e você é o criador ou proprietário da prova
* Permissões de gerente com a função de prova Autor ou Moderador

Se a prova tiver um Fluxo de trabalho automatizado, você poderá adicionar o usuário a um estágio individual. Para obter mais informações, consulte [Visão geral do fluxo de trabalho automatizado](../../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md).

Por padrão, os usuários adicionados à prova:

* Receba uma notificação por email com um link para a prova.
* Pode tomar decisões de aprovação na prova da Página inicial ou da Minha área de trabalho, conforme descrito em [Aprovar trabalho](../../../../review-and-approve-work/manage-approvals/approving-work.md).
* Não é necessário ativar a prova para revisar a prova.

Quando o Fluxo de trabalho automatizado é ativado e você adiciona um usuário à prova que não tem a prova ativada no Workfront, um novo estágio é criado no Fluxo de trabalho automatizado. O usuário que você está adicionando é adicionado automaticamente a esse novo estágio quando ele exibir a prova pela primeira vez. Para obter mais informações, consulte [Visão geral do fluxo de trabalho automatizado](../../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md).

Para compartilhar uma prova com usuários individuais:

1. Na barra de ferramentas à esquerda do visualizador de prova, clique no botão **Compartilhar** ícone .

   ![Share_btn_in_viewer__2_.png](assets/share-btn-in-viewer--2-.png)

1. Clique em **Adicionar recipients** na lista à esquerda.
1. Em **Novos destinatários de prova**, comece digitando o nome de um usuário com o qual você deseja compartilhar a prova e clique no nome quando ele for exibido na lista suspensa.
1. (Opcional) Altere quaisquer opções do revisor à direita do nome da pessoa:

   * **Função de prova**: Para obter mais informações, consulte [Gerenciar funções de prova na Workfront Proof](../../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md).

   * **Fase**: (Disponível somente se a prova tiver um fluxo de trabalho automatizado). Para obter mais informações, consulte  [Visão geral das etapas do fluxo de trabalho automatizado](../../../../review-and-approve-work/proofing/proofing-overview/stages.md).

   * **Alertas por email**: selecione uma das opções a seguir para especificar como a pessoa será notificada sobre a atividade na prova.

      <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
        <td role="rowheader">Todas as atividades</td> 
        <td>O Workfront envia um email para o revisor sempre que houver uma atividade na prova, como um novo comentário, resposta ou decisão. <p>Essa é uma ótima opção para a pessoa que está gerenciando o processo de verificação porque permite que ela veja a atividade como ela acontece. </p><p>Os usuários não recebem um alerta por email sobre sua própria atividade.</p></td> 
       </tr> 
       <tr> 
        <td role="rowheader">Respostas aos meus comentários</td> 
        <td>Um email é enviado ao revisor somente se alguém responder explicitamente ao comentário (isso exclui suas próprias respostas em seus próprios comentários). Isso significa que se alguém na prova fizer um novo comentário, o revisor não será notificado.<p>Essa configuração é recomendada para seus clientes na prova, de modo que eles não sejam notificados sobre nenhum outro comentário na prova e sejam notificados apenas das respostas aos próprios comentários.</p><p>Embora os revisores com essa configuração de alerta de email não sejam notificados sobre outros novos comentários, eles ainda podem exibir todos os comentários na prova no visualizador de prova.</p><p>Para obter informações sobre comentários, consulte <a href="../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/view-proof-comments.md" class="MCXref xref">Exibir e responder comentários de prova</a>.</p></td> 
       </tr> 
       <tr> 
        <td role="rowheader">Decisões</td> 
        <td>O Workfront envia um email para o revisor somente quando alguém toma uma decisão.<p>Isso pode ser útil para a pessoa que gerencia o processo de aprovação (como um gerente de projeto) e precisa monitorar o progresso na prova e ver quais usuários tomaram sua decisão.</p><p>Você não será notificado de sua própria decisão, a menos que selecione uma opção de confirmação por email ao enviar sua decisão.</p></td> 
       </tr> 
       <tr> 
        <td role="rowheader">Decisão final</td> 
        <td>O Workfront envia um email quando o último aprovador na prova tomou a decisão.<p>Esse alerta é frequentemente usado pelo designer, que geralmente não precisa participar da discussão da revisão real. Quando a decisão final é tomada, o criador é notificado e pode tomar medidas relativamente às alterações necessárias.</p><p>Esse alerta também pode ser útil para um líder de departamento que precisa ser notificado somente quando o processo de revisão for concluído.</p></td> 
       </tr> 
       <tr> 
        <td role="rowheader">Resumo por hora</td> 
        <td>O Workfront envia um email para o revisor a cada hora com um resumo de todos os comentários, respostas e decisões que ocorreram na hora.<p>O email é enviado somente quando uma atividade além da sua ocorrer na última hora. </p><p>Esse alerta é uma boa maneira de ver uma visão geral do projeto.</p><p>Um exemplo de uso desse resumo é um revisor sênior que precisa de uma visão geral do projeto, mas não precisa ser notificado imediatamente de todas as atividades na prova.</p></td> 
       </tr> 
       <tr> 
        <td role="rowheader">Resumo diário</td> 
        <td>O Workfront envia um email com todos os comentários, respostas e decisões listados somente em dias em que há atividade além da sua.<p>Esse alerta é uma boa maneira de ver um resumo do projeto sem ficar sobrecarregado com várias atualizações ao longo do dia.</p><p>Um exemplo de uso deste resumo é um líder de departamento que deseja monitorar o progresso geral do projeto.</p><p>Para obter mais informações, consulte <a href="../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/manage-notifications-for-proof-comments.md" class="MCXref xref">Gerenciar notificações para comentários e decisões de prova</a>.</p></td> 
       </tr> 
       <tr data-mc-conditions=""> 
        <td role="rowheader">Nenhum email</td> 
        <td>A Workfront não envia alertas de email.<br>Isso é útil para uma pessoa que é adicionada a uma prova somente para fins de referência e não precisa ser notificada de quaisquer alterações.<p>O padrão do sistema é o Resumo diário (também visto como Não definido). Se você ou seus revisores não fizerem outras alterações, todas as provas terão essa configuração.</p></td> 
       </tr> 
      </tbody> 
     </table>

1. (Opcional) Repita as duas etapas anteriores para adicionar vários usuários à prova. 
1. (Opcional) Defina um **Prazo** para os revisores (disponível somente se a prova não tiver um fluxo de trabalho automatizado).
1. (Opcional) Selecione **Enviar notificação por email para novos recipients** para informá-los que você os adicionou à prova.
1. Quando terminar de adicionar usuários à prova, clique em **Feito.**
