---
user-type: administrator
product-area: system-administration
navigation-topic: emails-administration
title: Gerenciar convites por email para novos usuários
description: Como administrador do Adobe Workfront, você pode adicionar usuários ao Workfront e notificá-los de que foram adicionados, por meio de convites por email.
author: Lisa, Caroline
feature: System Setup and Administration
role: Admin
exl-id: e13e3479-391f-4aec-b998-e9b6057f256b
source-git-commit: 9bcd792139f8f2f0198da943e5c63a2add32e856
workflow-type: tm+mt
source-wordcount: '947'
ht-degree: 1%

---

# Gerenciar convites por email para novos usuários

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">*** DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

>[!IMPORTANT]
>
>O procedimento descrito nesta página se aplica somente a organizações que ainda não foram integradas ao Admin Console. Se sua organização tiver sido integrada à Adobe Admin Console, você deverá executar essa ação por meio da Adobe Admin Console.
>
>Para obter uma lista de procedimentos diferentes com base no fato de sua organização ter sido integrada à Adobe Admin Console, consulte [Diferenças de administração baseadas em plataforma (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

Como administrador do Adobe Workfront, você pode adicionar usuários ao Workfront e notificá-los de que foram adicionados, por meio de convites por email.

O convite por email permite que novos usuários sigam um link, onde podem escolher uma senha para sua conta do Workfront. Eles podem então terminar de configurar sua conta.

Para garantir a segurança das novas contas, recomendamos que você use convites por email para seus novos usuários, para que eles possam escolher sua própria senha. Como alternativa, você também pode selecionar uma senha para um novo usuário ao criar sua conta. Para obter mais informações sobre como adicionar novos usuários ao Workfront, consulte [Adicionar usuários](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

Você pode configurar os novos emails do usuário para:

* Qualquer novo usuário adicionado ao Workfront
* Usuários adicionados ao Workfront com uma licença Solicitante

Todos os novos usuários veem o mesmo email quando um convite é enviado.

Para obter informações sobre recebimento de convites por email, consulte [Receber convites por email e criar uma senha para o Adobe Workfront](../../../workfront-basics/manage-your-account-and-profile/managing-your-workfront-account/receive-email-invitations.md).

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plano Adobe Workfront</td> 
   <td>Qualquer Um</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença Adobe Workfront</td> 
   <td>Plano</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Administrador do sistema</p> </td> 
  </tr> 
 </tbody> 
</table>

## Gerar convites por email {#generate-email-invitations}

Os convites por email são gerados nos seguintes cenários:

* Ao criar um novo usuário e selecionar a variável **Enviar um email de convite para esta pessoa** no **Novo usuário** formulário. Para obter mais informações sobre como criar novos usuários, consulte [Adicionar usuários](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md).
* Ao importar vários novos usuários, selecione o **Enviar e-mails de convite para essas pessoas** opção. Para obter mais informações sobre como importar vários novos usuários, consulte [Importar usuários](../../../administration-and-setup/add-users/create-and-manage-users/import-users.md).
* Depois que os usuários forem criados, você poderá gerar manualmente os convites para usuários que ainda não registraram sua conta na Workfront e eles não estabeleceram uma senha da Workfront.\
   Os usuários que têm uma conta criada, mas ainda não registraram sua conta, são marcados como **Não registrado** no Workfront.

   >[!NOTE]
   >
   >Se você desmarcar a **Enviar um convite por email para esta pessoa** quando você cria o usuário, o convite por email não pode ser gerado manualmente. O reenvio manual de convites por email só é possível para usuários que receberam o convite original por email quando a conta foi criada. Para obter mais informações sobre como criar novos usuários, consulte [Adicionar usuários](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

Para gerar manualmente convites por email para usuários não registrados existentes:

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront, em seguida, clique em **Usuários** ![](assets/users-icon-in-main-menu.png).
1. Selecione o usuário que mostra a variável **Não registrado** após o nome.

   ![](assets/unreg-user-qs-350x221.png)

1. Clique no ícone Mais ![](assets/more-icon.png), depois clique em **Lembrar o usuário de se registrar**.

   Um convite é enviado por email para o novo usuário com um novo link que ele pode usar para criar sua senha do Workfront.

   >[!NOTE]
   >
   >Se sua organização tiver sido integrada ao Admin Console e você adicionar um usuário por meio do Workfront, não terá a opção de enviar um convite por email para novos usuários.
   >
   >Novos usuários do Adobe são adicionados ao Admin Console e o Admin Console fornece um email convidando-os a concluir o processo de registro. Todos os usuários devem concluir o processo de registro para acessar qualquer sistema de Adobe.
   >
   >Para usuários existentes do Adobe, o usuário pode ou não receber um email sobre a disponibilidade do Workfront. Esta é uma preferência controlada pelo administrador do Adobe para o produto.

## Configurar convites por email {#configure-email-invitations}

Como administrador do Workfront, você pode configurar a mensagem que inclui com os convites por email para novos usuários.

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront, em seguida, clique em **Configuração** ![](assets/gear-icon-settings.png).

1. Na lista à esquerda, clique em **Email** > **Convites**.

1. No **Opções gerais** faça qualquer uma das seguintes modificações:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Desativar links de convite após ... dias</strong> </td> 
      <td> <p>Escolha o período após o qual os convites por email não conterão mais um link válido para o Workfront. A quantidade padrão de dias é 45.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Incluir uma mensagem e/ou termo de serviço</strong> </td> 
      <td> <p>Selecione essa opção se desejar modificar o convite por email de todos os novos usuários adicionados ao Workfront. Isso não inclui usuários com uma licença do Solicitante.</p> 
       <ul> 
        <li><strong>Mensagem</strong>: Se você optar por modificar o convite por email para todos os novos usuários, especifique o texto que deseja incluir nos convites por email como o corpo do email.</li> 
        <li><strong>Termos e condições</strong>: Se você optar por modificar o convite por email para todos os novos usuários, especifique o texto que deseja incluir nos convites por email como os termos e condições.<br></li> 
        <li><strong>Incluir uma mensagem e/ou um termo de serviço para os utilizadores do helpdesk</strong>: Selecione essa opção se quiser modificar o convite por email de todos os novos usuários adicionados ao Workfront que tenham uma licença do Solicitante.</li> 
        <li><strong>Mensagem</strong>: Se você optar por modificar o convite por email para todos os novos usuários com uma licença do Requestor , especifique o texto que deseja incluir em seus convites por email como o corpo do email.</li> 
        <li><strong>Termos e condições</strong>: Se você optar por modificar o convite por email para todos os novos usuários com uma licença do Requestor , especifique o texto que deseja incluir em seus convites por email como os termos e condições.<br></li> 
        <li> <p>No <strong>Pré-visualização do Convite</strong> você pode visualizar seu convite por email. Se você optou por incluir uma mensagem personalizada em seu convite por email, a mensagem personalizada será exibida nessa área.</p> <p> <img src="assets/email-invitation-for-all-users-preview-qs-350x190.png" style="width: 350;height: 190;"> </p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. Clique em **Salvar**.
