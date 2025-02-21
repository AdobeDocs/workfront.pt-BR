---
product-area: documents
navigation-topic: review-proofs-within-workfront
title: Compartilhar uma prova do visualizador de provas
description: É possível compartilhar uma prova no visualizador de provas se o compartilhamento for ativado pelo proprietário ou criador da prova.
author: Courtney
feature: Digital Content and Documents
exl-id: 20bd2d94-1401-4a38-9042-335d0cb32a3d
source-git-commit: 1e67375c12bc473130127887e6cd4fa474c4fb02
workflow-type: tm+mt
source-wordcount: '1511'
ht-degree: 0%

---

# Compartilhar uma prova do visualizador de provas

É possível compartilhar uma prova no visualizador de provas se o compartilhamento for ativado pelo proprietário ou criador da prova.

>[!IMPORTANT]
>
>A configuração Permitir compartilhamento de prova via URL público ou código de inserção deve estar ativada.

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
   <td> <p>Editar acesso a documentos</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso aos objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qual perfil de plano, função ou permissão de prova você tem, contate o administrador do Workfront ou do Workfront Proof.

+++

## Compartilhar o URL

É possível compartilhar uma prova por meio de um URL se o proprietário tiver configurado a prova para compartilhamento. Os proprietários de provas podem atualizar as configurações de compartilhamento a qualquer momento. Para obter mais informações, consulte [Editar configurações de prova](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/edit-proof-settings.md).

1. Se o menu do ícone esquerdo não for exibido, clique no ícone **Menu** no canto superior esquerdo do visualizador de revisões.

   ![Ícone de menu](assets/menu-icon-in-proofing-viewer-350x188.png)

1. No menu de ícones esquerdo do revisor de provas, clique no ícone **Compartilhar**.

   ![Compartilhar_btn_in_viewer.png](assets/share-btn-in-viewer.png)

1. Nas opções **Compartilhar prova** exibidas, verifique se **Obter link compartilhável** está selecionado.

1.  Siga um destes procedimentos:

   * Para copiar o link para a área de transferência, clique em **Copiar link**.

     Agora é possível distribuir o link por meio de uma ferramenta de terceiros, como um bate-papo ou um aplicativo de email.

   * Para enviar o link por email diretamente do Adobe Workfront, faça o seguinte:

      1. No campo **Ou link de email para**, comece a digitar e selecione o nome do seu destinatário. Ou especifique o endereço de email de um usuário externo com o qual deseja compartilhar.

         >[!NOTE]
         >
         >Se você vir um email de alias ao compartilhar uma prova, não crie um novo usuário convidado inserindo o email original se existir um email de alias correspondente.

      1. Selecione entre as seguintes opções:

         <table style="table-layout:auto">
          <col>
          <col>
          <tbody>
           <tr>
            <td role="rowheader">Enviar link público</td>
            <td><p>Inclui um botão na notificação por email que direciona os usuários para a prova no visualizador de provas que eles estão usando e concede acesso de Visualização.</p><p>Se a opção <strong>Assinar prova por meio de URL pública ou código de inserção</strong> estiver desativada para a prova, os usuários poderão entrar com suas credenciais de logon do Workfront para adicionar comentários à prova. Se estiver ativado, qualquer pessoa que forneça seu endereço de email e nome (nenhuma senha é necessária) poderá assinar e adicionar comentários à prova.</p></td>
           </tr>
           <tr>
            <td role="rowheader">Enviar link de download</td>
            <td>Inclui um botão na notificação por email que direciona os usuários para uma página de download, que fornece detalhes do arquivo, nome do arquivo e tamanho do arquivo, com o arquivo exibido em linha. Os usuários podem clicar no link Download na página de download para baixar o arquivo.</td>
           </tr>
           <tr>
            <td role="rowheader">Adicionar mensagem personalizada</td>
            <td>Permite especificar um assunto e um corpo personalizados para a notificação por email.</td>
           </tr>
          </tbody>
         </table>

      1. Clique em **Enviar**.

         Seus recipients recebem uma notificação por email contendo informações sobre a prova e os botões que você optou por incluir.

         ![](assets/proof-share-email-350x87.png)

## Compartilhar o código de inserção

Você pode compartilhar uma prova por meio do código de inserção, se o proprietário da prova a tiver configurado para isso.

Para compartilhar uma prova por meio do código incorporado:

1. Na barra de ferramentas à esquerda do revisor de provas, clique no ícone **Compartilhar**.

   ![Compartilhar_btn_in_viewer_1_.png](assets/share-btn-in-viewer--1-.png)

1. Nas opções **Compartilhar prova** exibidas, clique em **Obter código incorporado** e em **Copiar**.

## Compartilhar uma prova adicionando usuários a ela

É possível adicionar usuários a uma prova ao revisar uma prova se você tiver uma das seguintes permissões:

* Permissões de supervisor ou administrador
* Permissões de gerente e você é o criador ou proprietário da prova
* Permissões de gerente com a função de prova Autor ou Moderador

Se a prova tiver um Fluxo de trabalho automatizado, é possível adicionar o usuário a um estágio individual. Para obter mais informações, consulte [Visão geral do Fluxo de Trabalho Automatizado](../../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md).

Por padrão, os usuários adicionados à prova:

* Receba uma notificação por email com um link para a prova.
* Pode tomar decisões de aprovação na prova a partir da área Página inicial, conforme descrito em [Aprovando trabalho](../../../../review-and-approve-work/manage-approvals/approving-work.md).
* Não é necessário ter a prova ativada para revisá-la.

Quando o Fluxo de trabalho automatizado está ativado e você adiciona um usuário à prova que não tem a prova ativada no Workfront, um novo estágio é criado no Fluxo de trabalho automatizado. O usuário que você está adicionando é automaticamente adicionado a esse novo estágio quando visualiza a prova pela primeira vez. Para obter mais informações, consulte [Visão geral do Fluxo de Trabalho Automatizado](../../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md).

Para compartilhar uma prova com usuários individuais:

1. Na barra de ferramentas à esquerda do revisor de provas, clique no ícone **Compartilhar**.

   ![Compartilhar_btn_in_viewer_2_.png](assets/share-btn-in-viewer--2-.png)

1. Clique em **Adicionar destinatários** na lista à esquerda.
1. Em **Novos recipients de prova**, comece digitando o nome de um usuário com o qual deseja compartilhar a prova e clique no nome quando ele aparecer na lista suspensa.
1. (Opcional) Altere quaisquer opções de revisor à direita do nome da pessoa:

   * **Função de prova**: para obter mais informações, consulte [Gerenciar Funções de Prova no Workfront Proof](../../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md).

   * **Estágio**: (disponível somente se a prova tiver um Fluxo de Trabalho Automatizado). Para obter mais informações, consulte  [Visão geral dos Estágios do Fluxo de Trabalho Automatizado](../../../../review-and-approve-work/proofing/proofing-overview/stages.md).

   * **Alertas por email**: selecione uma das seguintes opções para especificar como a pessoa será notificada sobre a atividade na prova.

     <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
        <td role="rowheader">Todas as atividades</td> 
        <td>O Workfront envia um email para o revisor sempre que há uma atividade na prova, como um novo comentário, resposta ou decisão. <p>Essa é uma ótima opção para a pessoa que está gerenciando o processo de prova, pois permite que ela veja a atividade enquanto ela acontece. </p><p>Os usuários não recebem um alerta por email sobre suas próprias atividades.</p></td> 
       </tr> 
       <tr> 
        <td role="rowheader">Respostas aos meus comentários</td> 
        <td>Um email é enviado ao revisor somente se alguém responder explicitamente ao comentário (isso exclui as próprias respostas nos comentários). Isso significa que se alguém na prova fizer um novo comentário, o revisor não será notificado.<p>Essa configuração é recomendada para os clientes na prova, para que não sejam notificados de nenhum outro comentário na prova e sejam notificados apenas das respostas aos próprios comentários.</p><p>Embora os revisores com essa configuração de alerta por email não sejam notificados sobre outros novos comentários, eles ainda podem exibir todos os comentários na prova no visualizador da prova.</p><p>Para obter informações sobre comentários, consulte <a href="../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/view-proof-comments.md" class="MCXref xref">Exibir e responder aos comentários de prova</a>.</p></td> 
       </tr> 
       <tr> 
        <td role="rowheader">Decisões</td> 
        <td>O Workfront envia um email para o revisor somente quando alguém toma uma decisão.<p>Isso pode ser útil para a pessoa que está gerenciando o processo de aprovação (como um gerente de projeto) e precisa monitorar o progresso na prova e ver quais usuários tomaram sua decisão.</p><p>Você não é notificado sobre sua própria decisão, a menos que selecione uma opção de confirmação por email ao enviar sua decisão.</p></td> 
       </tr> 
       <tr> 
        <td role="rowheader">Decisão final</td> 
        <td>O Workfront envia um email quando o último aprovador na prova toma sua decisão.<p>Esse alerta é usado com frequência pelo designer, que geralmente não precisa participar da discussão de revisão real. Quando a decisão final é tomada, o designer é notificado e pode então tomar medidas em relação a quaisquer alterações necessárias.</p><p>Esse alerta também pode ser útil para um líder de departamento que precise ser notificado somente quando o processo de revisão for concluído.</p></td> 
       </tr> 
       <tr> 
        <td role="rowheader">Resumo por Hora</td> 
        <td>O Workfront envia um email ao revisor a cada hora com um resumo de todos os comentários, respostas e decisões que ocorreram na hora.<p>O email é enviado somente quando a atividade além da sua ocorre na última hora. </p><p>Este alerta é uma boa maneira de ter uma visão geral do projeto.</p><p>Um exemplo de caso de uso para este resumo é um revisor sênior que precisa de uma visão geral do projeto, mas não precisa ser notificado imediatamente de todas as atividades na prova.</p></td> 
       </tr> 
       <tr> 
        <td role="rowheader">Resumo Diário</td> 
        <td>O Workfront envia um email com todos os comentários, respostas e decisões listados somente em dias quando houver atividade além da sua.<p>Este alerta é uma boa maneira de ver um resumo do projeto sem precisar de várias atualizações ao longo do dia.</p><p>Um exemplo de caso de uso para este resumo é um líder de departamento que deseja monitorar o progresso geral do projeto.</p><p>Para obter mais informações, consulte <a href="../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/manage-notifications-for-proof-comments.md" class="MCXref xref">Gerenciar notificações para comentários de prova e decisões</a>.</p></td> 
       </tr> 
       <tr data-mc-conditions=""> 
        <td role="rowheader">Nenhum email</td> 
        <td>O Workfront não envia alertas de email.<br>Isso é útil para uma pessoa que é adicionada a uma prova somente para fins de referência e não precisa ser notificada de nenhuma alteração.<p>O padrão do sistema é Resumo diário (também visto como Não definido). Se você ou seus revisores não fizerem outras alterações, todas as provas terão essa configuração.</p></td> 
       </tr> 
      </tbody> 
     </table>

1. (Opcional) Repita as duas etapas anteriores para adicionar vários usuários à prova. 
1. (Opcional) Defina um **Prazo** para os revisores (disponível somente se a prova não tiver um fluxo de trabalho automatizado).
1. (Opcional) Selecione **Enviar notificação por email a novos destinatários** para que eles saibam que você os adicionou à prova.
1. Quando terminar de adicionar usuários à prova, clique em **Concluído.**
