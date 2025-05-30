---
user-type: administrator
product-area: system-administration
navigation-topic: emails-administration
title: Gerenciar convites por email para novos usuários
description: Como administrador do Adobe Workfront, você pode adicionar usuários ao Workfront e notificá-los de que foram adicionados, usando convites por email.
author: Courtney
feature: System Setup and Administration
role: Admin
exl-id: e13e3479-391f-4aec-b998-e9b6057f256b
source-git-commit: dccbd5a036e1b148bc8f3e41fac3a67babe6dc9a
workflow-type: tm+mt
source-wordcount: '936'
ht-degree: 0%

---

# Gerenciar convites por email para novos usuários

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">*** DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

>[!IMPORTANT]
>
>O procedimento descrito nesta página se aplica apenas a organizações que ainda não foram integradas à Admin Console. Se sua organização tiver sido integrada à Adobe Admin Console, você deverá executar essa ação por meio da Adobe Admin Console.
>
>Para obter uma lista de procedimentos que diferem dependendo de sua organização ter sido integrada à Adobe Admin Console, consulte [Diferenças de administração baseadas em plataforma (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

Como administrador do Adobe Workfront, você pode adicionar usuários ao Workfront e notificá-los de que foram adicionados, usando convites por email.

O convite por email permite que novos usuários sigam um link para que possam escolher uma senha para sua conta do Workfront. Depois disso, ele poderá concluir a configuração da conta.

Para garantir a segurança das novas contas, recomendamos que você use convites por email para seus novos usuários, para que eles possam escolher sua própria senha. Como alternativa, você também pode selecionar uma senha para um novo usuário ao criar sua conta. Para obter mais informações sobre como adicionar novos usuários ao Workfront, consulte [Adicionar usuários](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

Você pode configurar os novos emails de usuário para:

* Qualquer novo usuário adicionado ao Workfront
* Usuários adicionados ao Workfront com uma licença de Solicitante

Todos os novos usuários veem o mesmo email quando um convite por email é enviado.

Para obter informações sobre como receber convites por email, consulte [Receber convites por email e criar uma senha para o Adobe Workfront](../../../workfront-basics/manage-your-account-and-profile/managing-your-workfront-account/receive-email-invitations.md).

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront</td> 
   <td>Qualquer</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td>Plano</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Administrador do sistema</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## Reenviar convites por email para usuários não registrados existentes

Convites por email são gerados nos seguintes cenários:

* Ao criar um novo usuário e selecionar o **Enviar um email de convite para essa pessoa** no formulário **Novo Usuário**. Para obter mais informações sobre como criar novos usuários, consulte [Adicionar usuários](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md).
* Ao importar vários usuários novos e selecionar a opção **Enviar emails de convite para essas pessoas**. Para obter mais informações sobre como importar vários usuários novos, consulte [Importar usuários](../../../administration-and-setup/add-users/create-and-manage-users/import-users.md).
* Após a criação dos usuários, é possível gerar manualmente os convites para usuários que ainda não registraram sua conta na Workfront e que não estabeleceram uma senha do Workfront.\
  Os usuários que têm uma conta criada, mas ainda não registraram sua conta, são marcados como **Não Registrados** no Workfront.

  >[!NOTE]
  >
  >Se você desmarcar a caixa **Enviar um convite por email para esta pessoa** ao criar o usuário, o convite por email não poderá ser gerado manualmente. O reenvio manual dos convites por email só é possível para usuários que receberam o convite original por email quando sua conta foi criada. Para obter mais informações sobre como criar novos usuários, consulte [Adicionar usuários](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

Para reenviar convites por email manualmente para usuários não registrados existentes:

{{step-1-to-users}}

1. Selecione o usuário que mostra o rótulo **Não registrado** depois de seu nome.

   ![Não registrado](assets/unreg-user-qs-350x221.png)

1. Clique no ícone Mais ![ícone Mais](assets/more-icon.png) e em **Lembrar usuário de se registrar**.

   Um convite é enviado por email para o novo usuário com um novo link que ele pode usar para criar sua senha do Workfront.

   >[!NOTE]
   >
   >Se sua organização tiver sido integrada à Admin Console e você adicionar um usuário por meio do Workfront, não será possível enviar um convite por email para novos usuários.
   >
   >Novos usuários do Adobe são adicionados à Admin Console, e a Admin Console fornece um email convidando-os a concluir o processo de registro. Todos os usuários devem concluir o processo de registro para acessar qualquer sistema da Adobe.
   >
   >Para usuários existentes do Adobe, o usuário pode ou não receber um email sobre a disponibilidade do Workfront. Esta é uma preferência controlada pelo administrador do Adobe para o produto.

## Configurar convites por email {#configure-email-invitations}

Como administrador do Workfront, você pode configurar a mensagem que inclui com os convites por email para novos usuários.

{{step-1-to-setup}}

1. Na lista à esquerda, clique em **Email** > **Convites**.

1. Na seção **Opções Gerais**, faça qualquer uma das seguintes modificações:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Desativar links de convite após ... dias</strong> </td> 
      <td> <p>Escolha o período após o qual os convites por email não contêm mais um link válido para o Workfront. O valor padrão de dias é 45.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Incluir uma mensagem e/ou termo de serviço</strong> </td> 
      <td> <p>Selecione essa opção se quiser modificar o convite por email para todos os novos usuários adicionados ao Workfront. Isso não inclui usuários com uma licença de Solicitante.</p> 
       <ul> 
        <li><strong>Mensagem</strong>: se você optar por modificar o convite por email para todos os novos usuários, especifique o texto que deseja incluir nos convites por email como corpo do email.</li> 
        <li><strong>Termos e Condições</strong>: se você optar por modificar o convite por email para todos os novos usuários, especifique o texto que deseja incluir nos convites por email como os termos e condições.<br></li> 
        <li><strong>Incluir uma mensagem e/ou termo de serviço para usuários do helpdesk</strong>: selecione essa opção se desejar modificar o convite por email para todos os novos usuários adicionados ao Workfront que tenham uma licença de Solicitante.</li> 
        <li><strong>Mensagem</strong>: se você optar por modificar o convite por email para todos os novos usuários com uma licença de Solicitante, especifique o texto que deseja incluir nos convites por email como corpo do email.</li> 
        <li><strong>Termos e Condições</strong>: se você optar por modificar o convite por email para todos os novos usuários com uma licença de Solicitante, especifique o texto que deseja incluir nos convites por email como os termos e condições.<br></li> 
        <li> <p>Na seção <strong>Visualização do Convite</strong>, você pode ver uma visualização do seu convite por email. Se você optou por incluir uma mensagem personalizada no convite por email, a mensagem personalizada será exibida nesta área.</p> <p> <img src="assets/email-invitation-for-all-users-preview-qs-350x190.png" style="width: 350;height: 190;"> </p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. Clique em **Salvar**.
