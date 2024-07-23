---
product-area: documents;system-administration;setup
navigation-topic: manage-proofs-within-workfront
title: Definir configurações de acesso e subscrição para uma prova
description: Você pode definir determinadas configurações de acesso e subscrição para provas individuais, como exigir que os usuários façam logon e permitir que os usuários assinem a prova. Você pode definir as configurações de acesso e subscrição para uma prova enquanto a cria ou pode defini-las para uma prova que já existe no Workfront.
author: Courtney
feature: Digital Content and Documents
exl-id: f242887b-d768-4d56-b530-a1ac6294b2d4
source-git-commit: 7477b62cf0e2e61966f8e74cf268217e2ceb67ef
workflow-type: tm+mt
source-wordcount: '960'
ht-degree: 0%

---

# Definir configurações de acesso e subscrição para uma prova

Você pode definir determinadas configurações de acesso e subscrição para provas individuais, como exigir que os usuários façam logon e permitir que os usuários assinem a prova. Você pode definir as configurações de acesso e subscrição para uma prova enquanto a cria ou pode defini-las para uma prova que já existe no Workfront.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront*</td> 
   <td> <p>Plano atual: Pro ou Superior</p> <p>ou</p> <p>Plano herdado: Premium</p> <p>Para obter mais informações sobre acesso de revisão de texto com os diferentes planos, consulte <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Acesso à funcionalidade de revisão de texto no Workfront</a>.</p> </td> 
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
   <td> <p>Editar acesso a documentos</p> <p>Observação: se você ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qual perfil de plano, função ou permissão de prova você tem, contate o administrador do Workfront ou do Workfront Proof.

+++

## Definir configurações de acesso e subscrição ao criar uma prova

Para definir as configurações de acesso e subscrição de uma prova enquanto a cria:

1. Vá para o projeto, tarefa ou problema em que deseja a prova e clique na seção **Documentos**.
1. Clique em **Adicionar novo** na área superior direita.
1. Role até a seção **Configurações de prova** no canto inferior direito da página **Nova prova**.

1. Defina as seguintes configurações:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Permitir compartilhamento de prova via URL pública ou código de inserção</strong> </td> 
      <td>Quando essa opção é selecionada, a prova pode ser compartilhada por meio de um URL público ou código integrado.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Permitir assinatura da prova via URL pública ou código de inserção</strong> </td> 
      <td>Quando essa opção é selecionada, as pessoas que não foram adicionadas explicitamente à prova podem assinar a prova. A pessoa que se inscreve na prova recebe a função e o email definidos nas seguintes configurações:
       <ul>
        <li><p><strong>Função do assinante:</strong> a função de prova padrão que é atribuída a todos os revisores que assinam a prova. </p><p>Importante: se <strong>Permitir Compartilhamento com</strong> estiver definido como algo diferente de <strong>Todos</strong> nas configurações do Workfront Proof, a assinatura funcionará somente para as pessoas da organização. Para obter mais informações, consulte <a href="../../../workfront-proof/wp-work-proofsfiles/manage-your-work/configure-proof-settings.md" class="MCXref xref">Definir Configurações de Prova no Workfront Proof</a>.</p></li>
        <li><strong>Configurações de alerta por email para assinantes:</strong> o alerta por email padrão atribuído a todos os revisores que assinam a prova.</li>
       </ul><p>
        <ul>
         <li><strong>Acesso de prova via link de email necessário para:</strong> Configure se o assinante receberá um email com um link para a prova. Você pode selecionar <strong>Nenhum email</strong> (o link do email não é necessário para acessar a prova), <strong>Somente email de notificação de prova</strong> (o assinante recebe um link para a prova por email sem qualquer verificação) ou <strong>Emails de notificação de validação e prova</strong> (o assinante recebe um link para a prova por email e deve clicar no link para acessar uma prova; a finalidade dessa opção é garantir que a pessoa tenha inserido um endereço de email correto ao qual tem acesso).</li>
        </ul><p>Nota:  Se as provas tiverem o Fluxo de trabalho automatizado anexado, todas as assinaturas gerarão emails de confirmação para os Proprietários da prova, para que eles possam decidir em qual estágio a pessoa deve ser adicionada.<br></p></p></td> 
     </tr> 
    </tbody> 
   </table>

1. Continue criando sua prova.

## Definir configurações de acesso e subscrição para uma prova existente

Para definir as configurações de acesso e subscrição para uma prova que já existe no Workfront:

1. Na área Documentos, selecione o documento que contém a prova para a qual deseja definir configurações e clique em **Detalhes do Documento**.
1. No painel esquerdo, clique em **Configurações do visualizador de provas**.
1. Defina as seguintes configurações:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Permitir compartilhamento de prova via URL pública ou código de inserção</strong><strong>e</strong> </td> 
      <td>Quando essa opção é selecionada, a prova pode ser compartilhada por meio de um URL público ou código integrado.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Permitir assinatura da prova via URL pública ou código de inserção</strong> </td> 
      <td>Quando essa opção é selecionada, as pessoas que não foram adicionadas explicitamente à prova podem assinar a prova. A pessoa que se inscreve na prova recebe a função e o email definidos nas seguintes configurações:
       <ul>
        <li><p><strong>Função do assinante:</strong> a função de prova padrão que é atribuída a todos os revisores que assinam a prova. </p><p>Importante: se <strong>Permitir Compartilhamento com</strong> estiver definido como algo diferente de <strong>Todos</strong> nas configurações do Workfront Proof, a assinatura funcionará somente para as pessoas da organização. Para obter mais informações, consulte <a href="../../../workfront-proof/wp-work-proofsfiles/manage-your-work/configure-proof-settings.md" class="MCXref xref">Definir Configurações de Prova no Workfront Proof</a>.</p></li>
        <li><strong>Configurações de alerta por email para assinantes:</strong> o alerta por email padrão atribuído a todos os revisores que assinam a prova.</li>
       </ul><p>
        <ul>
         <li><strong>Acesso de prova via link de email necessário para:</strong> Configure se o assinante receberá um email com um link para a prova. Você pode selecionar <strong>Nenhum email</strong> (o link do email não é necessário para acessar a prova), <strong>Somente email de notificação de prova</strong> (o assinante recebe um link para a prova por email sem qualquer verificação) ou <strong>Emails de notificação de validação e prova</strong> (o assinante recebe um link para a prova por email e deve clicar no link para acessar uma prova; a finalidade dessa opção é garantir que a pessoa tenha inserido um endereço de email correto ao qual tem acesso).</li>
        </ul><p>Nota:  Se as provas tiverem o Fluxo de trabalho automatizado anexado, todas as assinaturas gerarão emails de confirmação para os Proprietários da prova, para que eles possam decidir em qual estágio a pessoa deve ser adicionada.<br></p></p></td> 
     </tr> 
    </tbody> 
   </table>

1. Clique em **Salvar**.
