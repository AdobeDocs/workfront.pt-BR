---
user-type: administrator
product-area: system-administration
navigation-topic: organization-setup
title: Gerenciar associações de empresas
description: No [!UICONTROL Empresas] em Configurar, é possível adicionar e remover membros de uma empresa. Também é possível editar os perfis de usuário, lembrá-los de se registrar no [!DNL Workfront], deactivate them in [!DNL Workfront], and remove them from the [!DNL Workfront] sistema.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: f0efd985-76e3-435e-bf19-87008f6a5e9d
source-git-commit: b6f6964bb80f172849434c669df2b0ecd735a590
workflow-type: tm+mt
source-wordcount: '910'
ht-degree: 1%

---

# Gerenciar associações de empresas

No [!UICONTROL Empresas] área em [!UICONTROL Configuração], é possível adicionar e remover membros de uma empresa. Também é possível editar os perfis de usuário, lembrá-los de se registrar no [!DNL Workfront], desative-os em [!DNL Workfront]e remova-as do [!DNL Workfront] sistema.

Para obter informações sobre como criar uma nova empresa, consulte [Criar e editar empresas](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

## Requisitos de acesso

Você deve ter o seguinte para gerenciar empresas no [!DNL Workfront]:

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Workfront] plano*</p> </td> 
   <td>[!UICONTROL Team] ou superior</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Adobe Workfront] licença*</p> </td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"><strong>Configurações de nível de acesso*</strong> </td> 
   <td> <p>Um dos seguintes:</p> 
    <ul> 
     <li> <p>O nível de acesso do [!UICONTROL System Administrator], que permite a edição de qualquer empresa no sistema. Para obter mais informações, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder ao usuário acesso administrativo total</a>. </p> </li> 
     <li> <p>Acesso administrativo para gerenciar empresas, o que permite editar qualquer empresa no sistema. Para obter mais informações, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Conceder aos usuários acesso administrativo a determinadas áreas</a>.</p> </li> 
    </ul> <p><b>Nota</b>:  
     <ul> 
      <li> <p>Também é possível gerenciar empresas associadas a qualquer grupo, onde você está atribuído como administrador de grupo.</p> </li> 
      <li> <p>Para adicionar e remover usuários do [!DNL Workfront] , você deve ter um dos seguintes itens:</p> 
       <ul> 
        <li> <p>O nível de acesso do [!UICONTROL System Administrator]. Para obter mais informações, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder ao usuário acesso administrativo total</a>. </p> </li> 
        <li> <p>No nível de acesso, [!UICONTROL Editar] deve ser selecionado para a configuração [!UICONTROL Usuários]. Além disso, para a configuração [!UICONTROL Usuários], em [!UICONTROL Otimizar suas configurações] <img src="assets/gear-icon-in-access-levels.png"> , a opção [!UICONTROL Criar] e pelo menos uma das duas opções do [!UICONTROL User Admin] devem estar habilitadas. </p> <p> <img src="assets/access-req-users.png"> </p> <p>Se estiver usando a opção [!UICONTROL Administrador de usuário (Usuários de grupo)], você deve ser um administrador de grupo de um grupo no qual o usuário é membro.</p> </li> 
       </ul> <p>Para obter informações sobre a configuração Usuários em um nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Conceder acesso aos usuários</a>.</p> </li> 
     </ul> </p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir que plano, tipo de licença ou configurações de nível de acesso você possui, entre em contato com seu [!DNL Workfront] administrador.

## Gerenciar associações de empresas

1. Clique no botão **[!UICONTROL Menu principal]** ícone ![](assets/main-menu-icon.png) no canto superior direito de [!DNL Adobe Workfront], depois clique em **[!UICONTROL Configuração]** ![](assets/gear-icon-settings.png).

1. Clique em **[!UICONTROL Empresas]**.
1. Clique no nome da empresa.
1. Com o **[!UICONTROL Membros da Empresa]** seção selecionada no painel esquerdo, execute um dos seguintes procedimentos:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Adicionar um membro</td> 
      <td> <p>Clique em <b>[!UICONTROL Adicionar membro]</b>, selecione uma dessas opções no menu suspenso que é exibido:</p> 
       <ul> 
        <li> <p><b>[!UICONTROL Novo usuário]</b>: Adicionar um usuário que ainda não foi adicionado a [!DNL Workfront].</p> <p>Para obter informações sobre como adicionar usuários a [!DNL Workfront], consulte <a href="../../../administration-and-setup/add-users/create-and-manage-users/add-users.md" class="MCXref xref">Adicionar usuários</a> e <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Editar o perfil de um usuário</a>.</p> </li> 
        <li> <p><b>[!DNL Existing user]</b>: Adicione um usuário já existente no sistema que você tenha acesso para editar.</p> <p><b>IMPORTANTE</b>: Se o usuário já for membro de outra empresa, a nova atribuição substituirá a antiga. O usuário perde o acesso aos itens compartilhados com a empresa anterior e obtém acesso aos itens compartilhados com essa empresa.</p> </li> 
        <li> <p><b>[!UICONTROL Importar usuários]</b>: Importe um usuário carregando um arquivo de importação de planilha. Para obter mais informações, consulte <a href="../../../administration-and-setup/add-users/create-and-manage-users/import-users.md" class="MCXref xref">Importar usuários</a>.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Editar membros</td> 
      <td> 
       <ol> 
        <li value="1"> <p>Selecione pelo menos um usuário e clique no ícone [!UICONTROL Editar] <img src="assets/edit-icon.png"> na barra de ferramentas.</p> </li> 
        <li value="2"> <p>Configure as opções na <b>[!UICONTROL Editar usuário]</b> que é exibida.</p> <p>Para obter informações sobre essas opções, consulte <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Editar o perfil de um usuário</a>.</p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Copiar membro</td> 
      <td> <p>Você pode criar um membro da empresa copiando um membro existente. </p> <p><b>Nota</b>:  <p>Ao criar um usuário dessa forma, todas as informações são copiadas do usuário original para o usuário recém-criado, exceto para o seguinte:</p> 
        <ul> 
         <li>As informações na seção [!UICONTROL Informações pessoais].</li> 
         <li>[!UICONTROL Ao fazer logon, mostrar]: A guia de aterrissagem padrão para o nível de acesso é selecionada nesta caixa.</li> 
         <li>[!UICONTROL Relatórios diretos]</li> 
        </ul> </p> 
       <ol> 
        <li value="1"> <p>Selecione o usuário e clique no ícone [!UICONTROL Copiar] <img src="assets/copy-icon.png">. </p> </li> 
        <li value="2"> <p>No <b>[!UICONTROL Novo usuário]</b> for exibida, edite os campos disponíveis para o novo usuário.</p> <p>Para obter informações sobre todos os campos associados a um usuário, consulte <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Editar o perfil de um usuário</a>.</p> </li> 
        <li value="3"> <p>Clique em <strong>[!UICONTROL Adicionar este usuário]</strong>.</p> <p>Ou</p> <p>Clique em <strong>[!UICONTROL Adicionar usuário de pessoa e iniciar outra]</strong> para salvar o novo usuário e adicionar outro.</p> </li> 
       </ol> <p>Isso cria uma nova conta no [!DNL Workfront] para o usuário.</p> <p>Se você selecionou a opção de enviar um convite para o usuário, ele deverá receber um email onde poderá seguir um link para criar [!DNL Workfront] senha.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Remover usuários</td> 
      <td> 
       <div> 
        <p>Selecione pelo menos um usuário e clique em <b>[!UICONTROL Remover usuários]</b>, selecione uma das seguintes opções no menu suspenso que é exibido:</p> 
        <ul> 
         <li> <p><b>[!UICONTROL Remover da empresa]</b>: Remove o usuário ou usuários da empresa.</p> </li> 
         <li> <p><b>[!UICONTROL Excluir]</b>: Exclui o usuário ou usuários do [!DNL Workfront] sistema.</p> <p><b>IMPORTANTE</b>: A exclusão de um usuário do sistema também exclui as informações associadas ao usuário que você deseja manter. Recomendamos desativar usuários em vez de excluí-los. Para obter mais informações, consulte <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">Desativar ou reativar um usuário</a>.</p> </li> 
        </ul> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Envie um comentário para os usuários e suas áreas de [!UICONTROL Atualizações]</td> 
      <td> 
       <ol> 
        <li value="1"> <p>Selecione pelo menos um usuário e clique no ícone [!UICONTROL Comentário] <img src="assets/comment-icon.png"> na barra de ferramentas.</p> </li> 
        <li value="2"> <p>Digite o comentário que deseja enviar aos usuários e à área [!UICONTROL Atualizações] dos perfis de usuário.</p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Exportar a lista de membros da empresa</td> 
      <td> <p>Clique no ícone [!UICONTROL Exportar] <img src="assets/export.png"> na barra de ferramentas, selecione o formato desejado para o arquivo exportado.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Desativar membros no sistema</td> 
      <td> <p>Selecione pelo menos um usuário, clique no ícone [!UICONTROL Mais] <img src="assets/more-icon.png"> na barra de ferramentas, selecione <b>[!UICONTROL Desativar]</b>.</p> <p>Para obter mais informações, consulte <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">Desativar ou reativar um usuário</a>.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Lembrar um usuário de se registrar no sistema</td> 
      <td> <p> No <b>[!UICONTROL Name]</b> coluna, <b>[!UICONTROL Não Registrado]</b> é exibido ao lado do nome de cada usuário não registrado. Para lembrar esses usuários de se registrarem no sistema, selecione os usuários, clique no ícone [!UICONTROL Mais] <img src="assets/more-icon.png"> na barra de ferramentas, selecione <b>[!UICONTROL Lembrar usuário de se registrar]</b>.</p> </td> 
     </tr> 
    </tbody> 
   </table>
