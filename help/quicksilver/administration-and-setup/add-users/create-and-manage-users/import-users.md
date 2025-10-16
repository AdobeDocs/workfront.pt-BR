---
title: Importar Usuários
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: Você pode importar usuários para o site do Adobe Workfront sincronizando usuários de um serviço de diretório de rede (como o Ative Diretory ou outro diretório LDAP) ou pode importar usuários usando um arquivo de importação de planilha.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 3dd99d01-a32f-4af8-90e3-f8c0e9027651
source-git-commit: f8d04790caefd12c9811ea3ed94e1f892311d031
workflow-type: tm+mt
source-wordcount: '480'
ht-degree: 1%

---

# Importar usuários

<!--

>[!IMPORTANT]
>
>The procedure described on this page applies only to organizations that have not yet been onboarded to the Admin Console. If your organization has been onboarded to the Adobe Admin Console, you must perform this action through the Adobe Admin Console.
>
>For instructions on editing a user's profile in the Adobe Admin Console, see the section "Add users" in the article [Bulk Upload Users](https://helpx.adobe.com/br/enterprise/using/bulk-upload-users.html) or contact your Adobe Admin Console Administrator.
>
>For a list of procedures that differ based on whether your organization has been onboarded to the Adobe Admin Console, see [Platform-based administration differences (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

-->

Você pode importar usuários usando um arquivo de importação de planilha.

Antes de criar um novo usuário, primeiro verifique se você criou todos os objetos que deseja associar ao usuário. Por exemplo, se não tiver criado um agendamento, você não poderá atribuir um agendamento ao novo usuário e o campo usado para associar um agendamento ao novo usuário não aparecerá na tela Novo usuário.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Pacote do Adobe Workfront</td> 
   <td><p>Qualquer</p></td> 
  </tr> 
  <tr> 
   <td>Licença do Adobe Workfront</td> 
   <td><p>Standard</p><p>Plano</p></td> 
  </tr> 
  <tr> 
   <td>Configurações de nível de acesso</td> 
   <td> <p>Você deve ter um dos seguintes:</p> 
    <ul> 
     <li> <p>O nível de acesso Administrador do sistema. </li> 
     <li> <p>A configuração <b>Usuários</b> no seu nível de acesso foi configurada para <b>Editar</b> acesso, com as opções <b>Criar</b> e pelo menos uma das duas opções <b>Administrador de Usuários</b> habilitadas em <b>Ajustar suas configurações</b> <img src="assets/gear-icon-in-access-levels.png">. </p> <p>Dessas duas opções, se <b>Administrador de Usuários (Usuários de Grupo)</b> estiver habilitado, você deverá ser um administrador de grupo de um grupo do qual o usuário seja membro.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Use um arquivo de importação de planilha para importar usuários

{{step-1-to-users}}

1. Clique na seta suspensa **Novo Usuário** e clique em **Importar Usuários**.

1. Na caixa **Importar usuários** que é exibida, baixe o arquivo de amostra e atualize-o para incluir suas informações pessoais de usuário.

   Cada linha inclui os seguintes campos:

   * **Nome**
   * **Sobrenome**
   * **Endereço de email**

     Os endereços de email devem ser exclusivos.

   * **Nível de Acesso**

     Os Níveis de acesso fazem distinção entre maiúsculas e minúsculas.

   * **ID de Logon do SSO**

     Este campo só será incluído se o SSO estiver habilitado no sistema. Você deve adicionar a ID da Federação neste campo para cada usuário. Ao criar um usuário na guia Pessoas, você pode configurar uma senha para o usuário se quiser permitir que os usuários façam logon sem SSO. No entanto, o recurso de importação não permite que você deixe a ID DE LOGON DE SSO em branco.

   * Verifique se não há espaços extras antes ou depois do endereço de email de um usuário.

   Quando terminar de usar uma linha, ela deverá ter esta aparência:

   ![importando-novos-usuários.png](assets/importing-new-users.png)

1. Salve o arquivo em um local na estação de trabalho.
1. Clique em **Escolher arquivo** na caixa **Importar usuários**.

1. Navegue até o arquivo salvo e selecione-o.

<!--
1. (Optional) Select the **Send an invite email to this user** option to send an email invitation to the user, notifying them that a Workfront account has been created and prompting them to set their password.

   Deselect this option if you want to set the password for the user.

-->

1. Clique em **Importar**.

   Você receberá uma mensagem de confirmação na parte superior da tela de que os usuários foram importados com êxito.

>[!NOTE]
>
>Os usuários são criados com status Desativado e Pendente de Aprovação.
> 
>Se um usuário não sair do status Desativado e Aprovação pendente em alguns minutos e uma atualização de tela não remover o selo Aprovação pendente, é possível adicionar o lote de usuários diretamente ao Adobe Admin Console.
>
>Para obter instruções, consulte [Gerenciar vários usuários | Upload em massa de CSV](https://helpx.adobe.com/br/enterprise/using/bulk-upload-users.html) na documentação do Adobe.
