---
product-area: documents
navigation-topic: manage-proofs-within-workfront
title: Compartilhar uma prova no Adobe Workfront
description: Você pode compartilhar um documento com prova no Adobe Workfront compartilhando o documento ou adicionando usuários à prova.
author: Courtney
feature: Digital Content and Documents
exl-id: a5438db3-6507-4ebc-a27c-65f02c45783e
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '1137'
ht-degree: 0%

---

# Compartilhar uma prova no Adobe Workfront

Você pode compartilhar um documento com prova no Adobe Workfront compartilhando o documento ou adicionando usuários à prova.

Se você compartilhar a prova, conforme explicado neste artigo, o recipient terá o mesmo acesso ao documento e à prova. Além disso, você pode solicitar aprovação para a prova do recipient.

>[!TIP]
>
>Você também pode compartilhar uma prova no visualizador de prova. Para obter instruções, consulte [Compartilhar uma prova do visualizador de prova](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/share-a-proof-in-proofing-viewer.md).

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
   <td role="rowheader">Função de prova</td> 
   <td>Autor ou moderador</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a documentos</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, função ou Perfil de permissão de prova você possui, entre em contato com o administrador da Workfront ou da Workfront Proof.

## Compartilhar um link de prova

O compartilhamento de um link de prova concede acesso à visualização aos usuários do Workfront. Os usuários podem comentar na prova e assinar notificações por email para a prova usando suas credenciais de logon do Workfront. Usuários sem provas podem comentar e assinar usando um endereço de email e nome de exibição.

>[!IMPORTANT]
>
>A configuração Permitir o compartilhamento de prova por URL público ou código incorporado deve estar ativada.

1. Selecione o documento que contém a prova que você deseja compartilhar com os usuários.

   Você pode selecionar apenas um documento. Não é possível compartilhar o link de vários documentos ao mesmo tempo.

1. Clique em **Compartilhar** > **Link de prova**.
1. No **Link de prova** for exibida, siga um destes procedimentos:

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

## Adicionar usuários a uma prova

Você pode adicionar qualquer usuário do Workfront à prova se tiver direitos de edição na prova. Se a prova tiver vários estágios, você adicionará o usuário a um estágio individual

>[!NOTE]
>
>Lembre-se do seguinte se estiver usando um plano Workfront herdado no qual a prova pode ser ativada e desativada para um usuário:
>
>* Seus recipients não precisam ter a prova ativada para revisar a prova.
>* Quando o Fluxo de trabalho automatizado é ativado e você adiciona um usuário à prova que não tem a prova ativada no Workfront, um novo estágio é criado no Fluxo de trabalho automatizado. O usuário que você está adicionando é adicionado automaticamente a esse novo estágio quando ele exibir a prova pela primeira vez. (Para obter mais informações, consulte [Visão geral do fluxo de trabalho automatizado](../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md).)
>


### Adicionar usuários a uma prova existente na guia Documentos

1. Selecione o documento que contém a prova à qual deseja adicionar usuários.
1. Se a prova não tiver um fluxo de trabalho automatizado (etapas), clique no botão **Mais** ícone no canto superior direito da seção Estágio 1, em seguida, clique em **Compartilhar** no menu suspenso.

   Ou

   Se a prova tiver um fluxo de trabalho automatizado, clique no botão **Mais** ícone no canto superior direito do palco onde deseja adicionar o revisor e clique em **Compartilhar** no menu suspenso.

1. No **Compartilhar esta versão** que aparece, em **Compartilhar**, comece a digitar o nome ou o endereço de email de um usuário com quem você deseja compartilhar a prova e clique no nome quando ele for exibido na lista suspensa.

1. (Opcional) Repita essa etapa para adicionar vários usuários à prova.
1. (Opcional) Defina um prazo para os revisores.
1. (Opcional) Certifique-se de **Notificar pessoas por email** é selecionada se você deseja informar aos revisores que você os adicionou à prova.
1. (Opcional) **Adicionar uma mensagem personalizada** ao email.
1. Depois de adicionar todos os revisores, clique em **Compartilhar**.

### Adicionar usuários a uma prova existente no visualizador de prova

Você pode adicionar usuários a uma prova enquanto revisa uma prova no Visualizador de Verificação de Verificação na Web e no Visualizador de Verificação de Verificação de Verificação Linguística da Área de Trabalho.

Para obter mais informações, consulte [Compartilhar uma prova adicionando usuários a ela](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/share-a-proof-in-proofing-viewer.md#sharing-with-individual-users) no artigo [Compartilhar uma prova do visualizador de prova](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/share-a-proof-in-proofing-viewer.md)

## Relatório de aprovações de prova

Você pode criar um relatório que relata as aprovações de prova que foram compartilhadas com o Workfront. Este relatório fornece as seguintes informações de aprovação de prova no sistema:

* Documento submetido para aprovação
* Nome do aprovador
* Versão de prova
* ID da Prova
* Data de criação da prova

Você acessa essa aprovação ao criar um relatório com base em um objeto, conforme descrito em [Criar um relatório personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

Para obter mais informações sobre o relatório de objeto de Aprovações de Prova , consulte o [Relatório sobre objetos](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#reporting-on-objects) seção em [Entender objetos no Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md)

## Aprovar uma prova compartilhada

Quando um usuário adiciona você a uma prova e concede a função de Aprovador ou o Revisor e Aprovador usando o Fluxo de trabalho automatizado, a solicitação de aprovação é exibida na guia Aprovações em sua Página inicial ou Minha área de trabalho. Em seguida, você pode exibir a prova e tomar uma decisão de aprovação na prova diretamente do Workfront.

Para obter informações sobre como tomar decisões de aprovação na área Meu trabalho , consulte [Aprovar trabalho da área inicial](../../../review-and-approve-work/manage-approvals/approving-work.md#approving-work-from-the-home-area) ou [Aprovar trabalho](../../../review-and-approve-work/manage-approvals/approving-work.md#approving-work-from-the-my-work-area) em [Aprovar trabalho](../../../review-and-approve-work/manage-approvals/approving-work.md).
