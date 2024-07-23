---
product-area: documents
navigation-topic: manage-proofs-within-workfront
title: Compartilhar uma prova no Adobe Workfront
description: Você pode compartilhar um documento revisado no Adobe Workfront compartilhando o documento ou adicionando usuários à prova.
author: Courtney
feature: Digital Content and Documents
exl-id: a5438db3-6507-4ebc-a27c-65f02c45783e
source-git-commit: 7477b62cf0e2e61966f8e74cf268217e2ceb67ef
workflow-type: tm+mt
source-wordcount: '1233'
ht-degree: 0%

---

# Compartilhar uma prova no Adobe Workfront

Você pode compartilhar um documento revisado no Adobe Workfront compartilhando o documento ou adicionando usuários à prova.

Se você compartilhar a prova, conforme explicado neste artigo, seu recipient terá o mesmo acesso ao documento e à prova. Além disso, você pode solicitar aprovação para a prova do recipient.

>[!TIP]
>
>Você também pode compartilhar uma prova no visualizador de provas. Para obter instruções, consulte [Compartilhar uma prova do visualizador de provas](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/share-a-proof-in-proofing-viewer.md).

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
   <td role="rowheader">Função de prova</td> 
   <td>Autor ou moderador</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a documentos</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso aos objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qual perfil de plano, função ou permissão de prova você tem, contate o administrador do Workfront ou do Workfront Proof.

+++

## Compartilhar um link de prova

O compartilhamento de um link de prova concede acesso de visualização aos usuários do Workfront. Os usuários podem comentar na prova e assinar notificações por email para a prova usando suas credenciais de logon do Workfront. Os usuários que não fazem provas podem comentar e se inscrever usando um endereço de email e nome de exibição.

>[!IMPORTANT]
>
>A configuração Permitir compartilhamento de prova via URL público ou código de inserção deve estar ativada.

1. Selecione o documento que contém a prova que você deseja compartilhar com os usuários.

   Você pode selecionar apenas um documento. Não é possível compartilhar o link de vários documentos ao mesmo tempo.

1. Clique em **Compartilhar** > **Link de Prova**.
1. Na caixa **Link de prova** que é exibida, siga um destes procedimentos:

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

## Adicionar usuários a uma prova

É possível adicionar qualquer usuário do Workfront à prova se você tiver direitos de Edição na prova. Se a prova tiver vários estágios, adicione o usuário a um estágio individual

>[!WARNING]
>
>Além dos métodos listados neste artigo, é possível adicionar usuários a uma prova marcando-os em um comentário da guia Atualizações de uma prova existente. No entanto, os usuários adicionados a uma prova dessa maneira não receberão uma notificação por email, a menos que sejam marcados novamente depois de serem adicionados ao fluxo de trabalho da prova.
>
>Dessa forma, recomendamos adicionar usuários a uma prova por meio de um dos métodos listados abaixo e não marcando-os em um comentário.
>

>[!NOTE]
>
>Lembre-se do seguinte se estiver usando um plano herdado do Workfront no qual a prova pode ser ativada e desativada para um usuário:
>
>* Seus destinatários não precisam ter a prova ativada para revisar a prova.
>* Quando o Fluxo de trabalho automatizado está ativado e você adiciona um usuário à prova que não tem a prova ativada no Workfront, um novo estágio é criado no Fluxo de trabalho automatizado. O usuário que você está adicionando é automaticamente adicionado a esse novo estágio quando visualiza a prova pela primeira vez. (Para obter mais informações, consulte [Visão geral do Fluxo de Trabalho Automatizado](../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md).)
>

### Adicionar usuários a uma prova existente na guia Documentos

1. Selecione o documento que contém a prova à qual você deseja adicionar usuários.
1. Se a prova não tiver um fluxo de trabalho automatizado (estágios), clique no ícone **Mais** no canto superior direito da seção Estágio 1 e clique em **Compartilhar** no menu suspenso.

   Ou

   Se a prova tiver um Fluxo de Trabalho Automatizado, clique no ícone **Mais** no canto superior direito do estágio em que você deseja adicionar o revisor e, em seguida, clique em **Compartilhar** no menu suspenso.

1. Na caixa **Compartilhar esta versão** exibida, em **Compartilhar**, comece digitando o nome ou endereço de email de um usuário com o qual deseja compartilhar a prova e clique no nome quando ele aparecer na lista suspensa.

1. (Opcional) Repita essa etapa para adicionar vários usuários à prova.
1. (Opcional) Defina um prazo final para os revisores.
1. (Opcional) Verifique se a opção **Notificar pessoas por email** está selecionada se desejar que os revisores saibam que você as adicionou à prova.
1. (Opcional) **Adicione uma mensagem personalizada** ao email.
1. Depois de adicionar todos os revisores, clique em **Compartilhar**.

### Adicionar usuários a uma prova existente do visualizador de provas

Você pode adicionar usuários a uma prova enquanto revisa uma prova no Web Proofing Viewer e no Desktop Proofing Viewer.

Para obter mais informações, consulte [Compartilhar uma prova adicionando usuários a ela](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/share-a-proof-in-proofing-viewer.md#sharing-with-individual-users) no artigo [Compartilhar uma prova do visualizador de provas](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/share-a-proof-in-proofing-viewer.md)

## Relatório sobre aprovações de provas

Você pode criar um relatório que relate as aprovações de provas que foram compartilhadas no Workfront. Esse relatório fornece as seguintes informações de aprovação de prova no sistema:

* Documento enviado para aprovação
* Nome do aprovador
* Versão da prova
* ID da Prova
* Data de criação da prova

Você acessa esta aprovação ao criar um relatório baseado em um objeto, conforme descrito em [Criar um relatório personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

Para obter mais informações sobre o relatório do objeto Aprovações de Provas, consulte a seção [Relatório sobre objetos](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#reporting-on-objects) em [Entender objetos no Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md)

## Aprovar uma prova compartilhada

Quando um usuário adiciona você a uma prova e concede a função Aprovador ou a função Revisor e Aprovador usando o Fluxo de trabalho automatizado, a solicitação de aprovação é exibida na guia Aprovações na área Página inicial ou Meu trabalho. Em seguida, você pode visualizar a prova e tomar uma decisão de aprovação sobre a prova diretamente do Workfront.

Para obter informações sobre como tomar decisões de aprovação da área Meu Trabalho, consulte [Aprovar trabalho da área Página Inicial](../../../review-and-approve-work/manage-approvals/approving-work.md#approving-work-from-the-home-area) ou [Aprovar trabalho](../../../review-and-approve-work/manage-approvals/approving-work.md#approving-work-from-the-my-work-area) em [Aprovar trabalho](../../../review-and-approve-work/manage-approvals/approving-work.md).
