---
user-type: administrator
product-area: system-administration
navigation-topic: organization-setup
title: Gerenciar Associações da Empresa
description: Na área [!UICONTROL Empresas] da Configuração, você pode adicionar e remover os membros de uma empresa. Você também pode editar os perfis de usuário, lembrá-los de se registrar no sistema  [!DNL Workfront], deactivate them in [!DNL Workfront], and remove them from the [!DNL Workfront] .
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: f0efd985-76e3-435e-bf19-87008f6a5e9d
source-git-commit: 705fc990f2d90ff2102233fc68947fdbe1eb6946
workflow-type: tm+mt
source-wordcount: '879'
ht-degree: 1%

---

# Gerenciar associações de empresa

Na área [!UICONTROL Empresas] em [!UICONTROL Configuração], você pode adicionar e remover os membros de uma empresa. Você também pode editar os perfis de usuário, lembrá-los de se registrar no [!DNL Workfront], desativá-los no [!DNL Workfront] e removê-los do sistema [!DNL Workfront].

Para obter informações sobre como criar uma nova empresa, consulte [Criar e editar empresas](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto">
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Workfront] plano</p> </td> 
   <td><p>Atual: [!UICONTROL Team] ou superior</p>
   <p>Ou</p>
   <p>Novo: Qualquer um</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Adobe Workfront] licença</p> </td> 
   <td><p>Atual: [!UICONTROL Plano]</p>
   <p>Ou</p>
   <p>Novo: [!UICONTROL Padrão]</p>
   </td> 
  </tr>
  <tr data-mc-conditions=""> 
   <td role="rowheader"><strong>Configurações de nível de acesso</strong> </td> 
   <td> <p>Uma das seguintes opções:</p> 
    <ul> 
     <li> <p>O nível de acesso do [!UICONTROL System Administrator], que permite editar qualquer empresa no sistema.</p> </li> 
     <li> <p>Acesso administrativo para gerenciar empresas, que permite editar qualquer empresa no sistema.</p> </li> 
    </ul> <p><b>NOTA</b>:  
     <ul> 
      <li> <p>Você também pode gerenciar empresas associadas a qualquer grupo ao qual esteja atribuído como administrador de grupo.</p> </li> 
      <li> <p>Para adicionar e remover usuários do sistema [!DNL Workfront], você deve ter um dos seguintes:</p> 
       <ul> 
        <li> <p>O nível de acesso do [!UICONTROL System Administrator].</p> </li> 
        <li> <p>Em seu nível de acesso, [!UICONTROL Editar] deve ser selecionado para a configuração [!UICONTROL Usuários]. Além disso, para a configuração [!UICONTROL Usuários], em [!UICONTROL Ajustar suas configurações] <img src="assets/gear-icon-in-access-levels.png"> , a opção [!UICONTROL Criar] e pelo menos uma das duas opções [!UICONTROL Administrador de Usuário] devem estar habilitadas. </p> <p> <img src="assets/access-req-users.png"> </p> <p>Se você estiver usando a opção [!UICONTROL Administrador de Usuários (Usuários de Grupo)], deverá ser um administrador de grupo de um grupo do qual o usuário seja membro.</p> </li> 
       </ul>
       </li> 
     </ul> </p> </td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Gerenciar associações de empresa

{{step-1-to-setup}}

1. Clique em **[!UICONTROL Empresas]**.
1. Clique no nome da empresa.
1. Clique em **[!UICONTROL Membros da empresa]** no painel esquerdo.
1. Siga um destes procedimentos:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Adicionar um membro</td> 
      <td> <p>Clique em <b>[!UICONTROL Adicionar membro]</b> e selecione uma destas opções no menu suspenso que exibe:</p> 
       <ul> 
        <li> <p><b>[!UICONTROL Novo usuário]</b>: adicionar um usuário que ainda não foi adicionado a [!DNL Workfront].</p> <p>Para obter informações sobre como adicionar usuários a [!DNL Workfront], consulte <a href="../../../administration-and-setup/add-users/create-and-manage-users/add-users.md" class="MCXref xref">Adicionar usuários</a> e <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Editar perfil de usuário</a>.</p> </li> 
        <li> <p><b>[!DNL Existing user]</b>: adiciona um usuário já existente, existente no sistema, que você tem acesso para editar.</p> <p><b>IMPORTANTE</b>: se o usuário já for membro de outra empresa, a nova atribuição substituirá a antiga. O usuário perde acesso aos itens compartilhados com a empresa anterior e obtém acesso aos itens compartilhados com esta empresa.</p> </li> 
        <li> <p><b>[!UICONTROL Importar Usuários]</b>: importe um usuário carregando um arquivo de importação de planilha. Para obter mais informações, consulte <a href="../../../administration-and-setup/add-users/create-and-manage-users/import-users.md" class="MCXref xref">Importar usuários</a>.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Editar membros</td> 
      <td> 
       <ol> 
        <li value="1"> <p>Selecione pelo menos um usuário e clique no ícone [!UICONTROL Editar] <img src="assets/edit-icon.png"> na barra de ferramentas.</p> </li> 
        <li value="2"> <p>Configure as opções na caixa <b>[!UICONTROL Editar Usuário]</b> que é exibida.</p> <p>Para obter informações sobre essas opções, consulte <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Editar perfil de usuário</a>.</p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Copiar membro</td> 
      <td> <p>Você pode criar um membro da empresa copiando um existente. </p> <p><b>NOTA</b>:  <p>Quando você cria um usuário dessa maneira, todas as informações são copiadas do usuário original para o usuário recém-criado, exceto para o seguinte:</p> 
        <ul> 
         <li>As informações na seção [!UICONTROL Informações Pessoais].</li> 
         <li>[!UICONTROL Quando eu fizer logon, mostrar]: a guia de aterrissagem padrão do nível de acesso está selecionada nesta caixa.</li> 
         <li>[!UICONTROL Relatórios Diretos]</li> 
        </ul> </p> 
       <ol> 
        <li value="1"> <p>Selecione o usuário e clique no ícone [!UICONTROL Copiar] <img src="assets/copy-icon.png">. </p> </li> 
        <li value="2"> <p>Na caixa <b>[!UICONTROL Novo Usuário]</b> que é exibida, edite os campos disponíveis para o novo usuário.</p> <p>Para obter informações sobre todos os campos associados a um usuário, consulte <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Editar perfil de usuário</a>.</p> </li> 
        <li value="3"> <p>Clique em <strong>[!UICONTROL Adicionar Este Usuário]</strong>.</p> <p>Ou</p> <p>Clique em <strong>[!UICONTROL Adicionar Usuário de Pessoa e Iniciar Outro]</strong> para salvar o novo usuário e adicionar outro.</p> </li> 
       </ol> <p>Isso cria uma nova conta em [!DNL Workfront] para o usuário.</p> <p>Se você selecionou a opção para enviar um convite ao usuário, ele deve receber um email onde possa seguir um link para criar sua senha do [!DNL Workfront].</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Remover usuários</td> 
      <td> 
       <div> 
        <p>Selecione pelo menos um usuário, clique em <b>[!UICONTROL Remover usuários]</b> e selecione uma das seguintes opções no menu suspenso exibido:</p> 
        <ul> 
         <li> <p><b>[!UICONTROL Remover da empresa]</b>: remove o(s) usuário(s) da empresa.</p> </li> 
         <li> <p><b>[!UICONTROL Excluir]</b>: exclui o(s) usuário(s) do sistema [!DNL Workfront].</p> <p><b>IMPORTANTE</b>: excluir um usuário do sistema também exclui as informações associadas ao usuário que você talvez queira manter. Recomendamos desativar os usuários em vez de excluí-los. Para obter mais informações, consulte <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">Desativar ou reativar um usuário</a>.</p> </li> 
        </ul> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Enviar um comentário aos usuários e às suas áreas [!UICONTROL Atualizações]</td> 
      <td> 
       <ol> 
        <li value="1"> <p>Selecione pelo menos um usuário e clique em <b>Enviar atualização para o usuário</b> na barra de ferramentas.</p> </li> 
        <li value="2"> <p>Digite o comentário que deseja enviar aos usuários e à área [!UICONTROL Atualizações] de seus perfis de usuário.</p>
         <p>Para obter mais informações, consulte <a href="/help/quicksilver/people-teams-and-groups/work-directly-with-others/send-direct-messages-to-other-users.md">Enviar mensagens diretas a outros usuários</a>.</p></li> 
       </ol>
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Exportar a lista de membros da empresa</td> 
      <td> <p>Clique no ícone [!UICONTROL Exportar] <img src="assets/export.png"> na barra de ferramentas e selecione o formato desejado para o arquivo exportado.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Desativar membros no sistema</td> 
      <td> <p>Selecione pelo menos um usuário, clique no ícone [!UICONTROL Mais] <img src="assets/more-icon.png"> na barra de ferramentas e selecione <b>[!UICONTROL Desativar]</b>.</p> <p>Para obter mais informações, consulte <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">Desativar ou reativar um usuário</a>.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Lembrar um usuário de se registrar no sistema</td> 
      <td> <p> Na coluna <b>[!UICONTROL Name]</b>, <b>[!UICONTROL Unregistered]</b> é exibido próximo ao nome de cada usuário não registrado. Para lembrar esses usuários de se registrarem no sistema, selecione-os, clique no ícone [!UICONTROL Mais] <img src="assets/more-icon.png"> na barra de ferramentas e selecione <b>[!UICONTROL Lembrar usuário a registrar]</b>.</p> </td> 
     </tr> 
    </tbody> 
   </table>
