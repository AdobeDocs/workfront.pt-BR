---
product-area: documents;system-administration;setup
navigation-topic: manage-proofs-within-workfront
title: Definir configurações de acesso e assinatura para uma prova
description: Você pode definir determinadas configurações de acesso e assinatura para provas individuais, como exigir que os usuários façam logon e permitir que os usuários assinem a prova. Você pode configurar as configurações de acesso e de assinatura para uma prova durante a criação ou pode configurá-las para uma prova que já existe no Workfront.
author: Courtney
feature: Digital Content and Documents
exl-id: f242887b-d768-4d56-b530-a1ac6294b2d4
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '949'
ht-degree: 3%

---

# Definir configurações de acesso e assinatura para uma prova

Você pode definir determinadas configurações de acesso e assinatura para provas individuais, como exigir que os usuários façam logon e permitir que os usuários assinem a prova. Você pode configurar as configurações de acesso e de assinatura para uma prova durante a criação ou pode configurá-las para uma prova que já existe no Workfront.

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plano Adobe Workfront*</td> 
   <td> <p>Plano atual: Pro ou superior</p> <p>ou</p> <p>Plano herdado: Premium</p> <p>Para obter mais informações sobre como revisar o acesso com os diferentes planos, consulte <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Acesso à funcionalidade de prova no Workfront</a>.</p> </td> 
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
   <td> <p>Editar acesso a documentos</p> <p>Observação: Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, função ou Perfil de permissão de prova você possui, entre em contato com o administrador da Workfront ou da Workfront Proof.

## Definir as configurações de acesso e assinatura ao criar uma prova

Para configurar as configurações de acesso e subscrição de uma prova durante a criação:

1. Vá para o projeto, tarefa ou problema onde deseja obter a prova e clique no botão **Documentos** seção.
1. Clique em **Adicionar novo** na área superior direita.
1. Role para **Configurações de prova** no canto inferior direito do **Nova prova** página.

1. Configure as seguintes configurações:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Permitir o compartilhamento da prova por meio de URL público ou código de inserção</strong> </td> 
      <td>Quando essa opção é selecionada, a prova pode ser compartilhada por meio de um URL público ou código incorporado.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Permitir assinatura da prova por meio de URL público ou código de inserção</strong> </td> 
      <td>Quando essa opção é selecionada, as pessoas que não foram adicionadas explicitamente à prova podem assinar a prova. A pessoa que assinar a prova recebe a função e o email definidos nas seguintes configurações:
       <ul>
        <li><p><strong>Função do assinante:</strong> A função de prova padrão atribuída a todos os revisores que assinam a prova. </p><p>Importante: If <strong>Permitir compartilhamento com</strong> está definida como qualquer outro que não seja <strong>Todos</strong> nas configurações da Workfront Proof, a assinatura funciona somente para pessoas na organização. Para obter mais informações, consulte <a href="../../../workfront-proof/wp-work-proofsfiles/manage-your-work/configure-proof-settings.md" class="MCXref xref">Definir configurações de prova na Workfront Proof</a>.</p></li>
        <li><strong>Configurações de alerta de email para assinantes:</strong> O alerta por email padrão atribuído a todos os revisores que assinam a prova.</li>
       </ul><p>
        <ul>
         <li><strong>Prova de acesso via link de email necessária para:</strong> Configure se o assinante recebe um email com um link para a prova. Você pode selecionar <strong>Nenhum email</strong> (o link do email não é necessário para acessar a prova), <strong>Somente email de notificação de prova</strong> (o assinante recebe um link para a prova por email sem qualquer verificação) ou <strong>Emails de notificação de validação e prova</strong> (o assinante recebe um link para a prova por email e deve clicar no link para acessar uma prova, a finalidade dessa opção é garantir que a pessoa tenha inserido um endereço de email correto ao qual tem acesso).</li>
        </ul><p>Observação:  Se as provas tiverem o Fluxo de trabalho automatizado anexado, todas as assinaturas gerarão emails de confirmação para os Proprietários de prova, para que possam decidir em qual estágio a pessoa deve ser adicionada.<br></p></p></td> 
     </tr> 
    </tbody> 
   </table>

1. Continue criando sua prova.

## Definir configurações de acesso e assinatura para uma prova existente

Para configurar as configurações de acesso e de assinatura para uma prova que já existe no Workfront:

1. Na área Documents , selecione o documento que contém a prova para a qual você deseja definir as configurações e clique em **Detalhes do documento**.
1. No painel esquerdo, clique em **Configurações do visualizador de prova**.
1. Configure as seguintes configurações:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Permitir compartilhamento de prova via URL público ou código incorporado</strong><strong>e</strong> </td> 
      <td>Quando essa opção é selecionada, a prova pode ser compartilhada por meio de um URL público ou código incorporado.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Permitir assinatura da prova por meio de URL público ou código de inserção</strong> </td> 
      <td>Quando essa opção é selecionada, as pessoas que não foram adicionadas explicitamente à prova podem assinar a prova. A pessoa que assinar a prova recebe a função e o email definidos nas seguintes configurações:
       <ul>
        <li><p><strong>Função do assinante:</strong> A função de prova padrão atribuída a todos os revisores que assinam a prova. </p><p>Importante: If <strong>Permitir compartilhamento com</strong> está definida como qualquer outro que não seja <strong>Todos</strong> nas configurações da Workfront Proof, a assinatura funciona somente para pessoas na organização. Para obter mais informações, consulte <a href="../../../workfront-proof/wp-work-proofsfiles/manage-your-work/configure-proof-settings.md" class="MCXref xref">Definir configurações de prova na Workfront Proof</a>.</p></li>
        <li><strong>Configurações de alerta de email para assinantes:</strong> O alerta por email padrão atribuído a todos os revisores que assinam a prova.</li>
       </ul><p>
        <ul>
         <li><strong>Prova de acesso via link de email necessária para:</strong> Configure se o assinante recebe um email com um link para a prova. Você pode selecionar <strong>Nenhum email</strong> (o link do email não é necessário para acessar a prova), <strong>Somente email de notificação de prova</strong> (o assinante recebe um link para a prova por email sem qualquer verificação) ou <strong>Emails de notificação de validação e prova</strong> (o assinante recebe um link para a prova por email e deve clicar no link para acessar uma prova, a finalidade dessa opção é garantir que a pessoa tenha inserido um endereço de email correto ao qual tem acesso).</li>
        </ul><p>Observação:  Se as provas tiverem o Fluxo de trabalho automatizado anexado, todas as assinaturas gerarão emails de confirmação para os Proprietários de prova, para que possam decidir em qual estágio a pessoa deve ser adicionada.<br></p></p></td> 
     </tr> 
    </tbody> 
   </table>

1. Clique em **Salvar**.
