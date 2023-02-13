---
title: Importar usuários
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: Você pode importar usuários para o site do Adobe Workfront sincronizando usuários de um serviço de diretório de rede (como o Ative Diretory ou outro diretório LDAP) ou pode importar usuários usando um arquivo de importação de planilha.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 3dd99d01-a32f-4af8-90e3-f8c0e9027651
source-git-commit: 2cbdd0cb065dee01ad128d782334a55233c13156
workflow-type: tm+mt
source-wordcount: '599'
ht-degree: 2%

---

# Importar usuários

>[!IMPORTANT]
>
>O procedimento descrito nesta página se aplica somente a organizações que ainda não foram integradas ao Admin Console. Se sua organização tiver sido integrada à Adobe Admin Console, você deverá executar essa ação por meio da Adobe Admin Console.
>
>Para obter instruções sobre como editar o perfil de um usuário no Adobe Admin Console, consulte a seção &quot;Adicionar usuários&quot; no artigo [Usuários de upload em massa](https://helpx.adobe.com/enterprise/using/bulk-upload-users.html) ou entre em contato com o administrador do Adobe Admin Console.
>
>Para obter uma lista de procedimentos diferentes com base no fato de sua organização ter sido integrada à Adobe Admin Console, consulte [Diferenças de administração baseadas em plataforma (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

É possível importar usuários usando um arquivo de importação de planilha.

Antes de criar um novo usuário, primeiro verifique se você criou todos os objetos que deseja associar ao usuário. Por exemplo, se você não tiver criado uma programação, não poderá atribuir uma programação ao novo usuário e o campo usado para associar uma programação ao novo usuário não aparecerá na tela Novo usuário.

## Requisitos de acesso

Você deve ter o seguinte para executar as etapas neste artigo:

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
   <td> <p>Você deve ter uma das seguintes opções:</p> 
    <ul> 
     <li> <p>O nível de acesso do Administrador do sistema. Para obter mais informações, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder ao usuário acesso administrativo total</a>. </p> </li> 
     <li> <p><b>Usuários</b> na configuração do seu nível de acesso configurado como <b>Editar</b> acesso, com <b>Criar</b> e pelo menos um dos dois <b>Administrador do usuário</b> opções ativadas em <b>Ajustar as configurações</b> <img src="assets/gear-icon-in-access-levels.png">. </p> <p>Dessas duas opções, se Usuário <b>Administrador (usuários do grupo)</b> estiver habilitado, você deve ser um administrador de grupo de um grupo no qual o usuário é membro.</p> <p>Para obter mais informações sobre o <b>Usuários</b> configurar em um nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Conceder acesso aos usuários</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Usar um arquivo de importação de planilha para importar usuários

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront, em seguida, clique em **Usuários** ![](assets/users-icon-in-main-menu.png).

1. Clique no botão **Novo usuário** seta suspensa e, em seguida, clique em **Importar usuários**.

1. No **Importar usuários** for exibida, baixe o arquivo de amostra e atualize o arquivo de amostra para incluir as informações pessoais de seu próprio usuário.

   Cada linha inclui os seguintes campos:

   * **Nome**
   * **Sobrenome**
   * **Endereço de email**

      Os endereços de email devem ser exclusivos.

   * **Nível de acesso**

      Níveis de Acesso fazem distinção entre maiúsculas e minúsculas.

   * **ID de Login de SSO**

      Este campo é incluído somente se o SSO estiver ativado em seu sistema. Você deve adicionar a ID de Federação neste campo para cada usuário. Ao criar um usuário na guia Pessoas, você pode configurar uma senha para o usuário se quiser permitir que os usuários façam logon sem SSO. No entanto, o recurso de importação não permite que você deixe a ID de LOGON do SSO em branco.

   * Certifique-se de que não existam espaços adicionais antes ou depois do endereço de email de um usuário.

   Quando terminar de usar uma linha, ela terá a seguinte aparência:

   ![import-new-users.png](assets/importing-new-users.png)

1. Salve o arquivo em um local na estação de trabalho.
1. Clique em **Escolher arquivo** no **Importar usuários** caixa.

1. Navegue até o arquivo salvo e o selecione.
1. (Opcional) Selecione o **Enviar um email de convite para este usuário** para enviar um convite por email ao usuário, notificando-o de que uma conta do Workfront foi criada e solicitando que ele defina sua senha.

   Desmarque essa opção se desejar definir a senha do usuário.

1. Clique em **Importar**.

   Você recebe uma mensagem de confirmação na parte superior da tela de que o usuário foi importado com êxito.
