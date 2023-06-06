---
product-area: user-management;setup
navigation-topic: configure-your-user-profile
title: Definir minhas configurações
description: Seu [!DNL Adobe Workfront] o perfil contém informações sobre você (por exemplo, seu nome, endereço de email, endereço, número de telefone, cargo etc). Ele também contém informações sobre suas interações com o [!DNL Workfront] e outros usuários em sua empresa.
author: Nolan
feature: Get Started with Workfront
exl-id: 0199bf74-0611-48f0-9c05-da6afac85033
source-git-commit: 1079f85651ec691280e2cccefaa6e48e0b9d89f8
workflow-type: tm+mt
source-wordcount: '3228'
ht-degree: 1%

---

# Definir minhas configurações

<!--
<p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Edit the job role FTE percentage allocation blurbs when more functionality is released: now, it says that the % is that of the user's schedule, but it will be either the user's schedule or the system schedule.</p>
-->

Seu [!DNL Adobe Workfront] o perfil contém informações sobre você (por exemplo, seu nome, endereço de email, endereço, número de telefone, cargo etc). Ele também contém informações sobre suas interações com o [!DNL Workfront] e outros usuários na empresa (por exemplo, as configurações de notificações, as guias que deseja exibir no [!DNL Workfront]ou suas funções de trabalho, gerente e associações de grupo e equipe).

A maioria dessas informações já foi definida pelo [!DNL Workfront] administrador quando seu [!DNL Workfront] conta foi criada.

Dependendo do seu nível de acesso no [!DNL Workfront], é possível editar algumas dessas informações configurando o [!UICONTROL Minhas configurações] área.

## Como os níveis de acesso afetam a edição do [!UICONTROL Minhas configurações] área

Dependendo do nível de acesso, é possível ou não editar seções no [!UICONTROL Minhas configurações] área.

Alguns campos contidos em seções editáveis não podem ser editados, dependendo de outras configurações que podem ou não ser definidas no seu nível de acesso. Para obter mais informações sobre o acesso adicional necessário para editar alguns dos campos encontrados em [!UICONTROL Minhas configurações], consulte as seções em [Configuração do [!UICONTROL Minhas configurações] área](#configuring-the-my-settings-area).

Para descobrir o nível de acesso que você tem, entre em contato com o [!DNL Workfront] administrador.

A grade a seguir mostra quais seções na [!UICONTROL Minhas configurações] são visíveis ou editáveis, dependendo do seu nível de acesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Áreas de [!UICONTROL Minhas Configurações]</strong> </th> 
   <th><strong>Visível ou editável</strong> </th> 
   <th><strong>[!UICONTROL Administrador do Sistema]</strong> </th> 
   <th><strong>[!UICONTROL Planner]</strong> </th> 
   <th><strong>[!UICONTROL Worker]</strong> </th> 
   <th><strong>[!UICONTROL Revisor]</strong> </th> 
   <th><strong>[!UICONTROL Solicitante]</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td rowspan="2">[!UICONTROL Informações Pessoais]</td> 
   <td> <p>Visível</p> </td> 
   <td> <p>✔</p> </td> 
   <td> ✔</td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td> ✔</td> 
  </tr> 
  <tr> 
   <td> <p>Editável</p> </td> 
   <td> <p>✔</p> </td> 
   <td> ✔</td> 
   <td> ✔</td> 
   <td>✔ </td> 
   <td>✔ </td> 
  </tr> 
  <tr> 
   <td rowspan="2">[!UICONTROL Preferências]</td> 
   <td> <p>Visível</p> </td> 
   <td> <p>✔</p> </td> 
   <td> ✔</td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ </td> 
  </tr> 
  <tr> 
   <td> <p>Editável</p> </td> 
   <td> <p>✔</p> </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ </td> 
  </tr> 
  <tr> 
   <td rowspan="2">[!UICONTROL Notificações]</td> 
   <td> <p>Visível</p> </td> 
   <td> <p>✔</p> </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td> ✔</td> 
   <td>✔ </td> 
  </tr> 
  <tr> 
   <td> <p>Editável</p> </td> 
   <td> <p>✔</p> </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td> ✔</td> 
   <td> ✔</td> 
  </tr> 
  <tr> 
   <td rowspan="2">[!UICONTROL Acesso]</td> 
   <td>Visível</td> 
   <td> ✔</td> 
   <td>✔ </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Editável</td> 
   <td> ✔</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td rowspan="2">[!UICONTROL Organização]</td> 
   <td>Visível</td> 
   <td>✔</td> 
   <td>✔ </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Editável</td> 
   <td>✔</td> 
   <td>✔ </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td rowspan="2">[!UICONTROL Planejamento de Recursos]</td> 
   <td>Visível</td> 
   <td>✔</td> 
   <td>✔ </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Editável</td> 
   <td>✔</td> 
   <td>✔ </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td rowspan="2">[!UICONTROL Forms Personalizado]</td> 
   <td>Visível</td> 
   <td>✔</td> 
   <td>✔ </td> 
   <td>✔</td> 
   <td>✔ </td> 
   <td>✔ </td> 
  </tr> 
  <tr> 
   <td>Editável</td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td rowspan="2">[!UICONTROL Comentário]</td> 
   <td>Visível</td> 
   <td>✔</td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ </td> 
  </tr> 
  <tr> 
   <td>Editável</td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ </td> 
  </tr> 
 </tbody> 
</table>

## Configuração do [!UICONTROL Minhas configurações] área

1. Clique em **[!UICONTROL Menu principal]** ícone ![](assets/main-menu-icon.png) no canto superior direito de [!DNL Adobe Workfront]e, em seguida, clique no nome de usuário ao lado da imagem do perfil.

1. Clique em **[!UICONTROL Mais]** menu ![](assets/more-icon.png)e, em seguida, clique em **[!UICONTROL Editar]**.

1. Dependendo do seu nível de acesso, você pode atualizar as seguintes seções:

   * [Informações pessoais](#personal-info)
   * [Preferências](#preferences)
   * [Notificações](#notifications)
   * [Acesso](#access)
   * [Organização](#organization)
   * [Planejamento de recursos](#resource-planning)
   * [Formulário personalizado](#custom-form)
   * [Comentário](#comment)

1. Clique em **[!UICONTROL Salvar]**.

### [!UICONTROL Informações pessoais]

Esta seção inclui as seguintes subseções:

* [Informações básicas](#basic-info)
* [Informações do trabalho](#job-info)
* [Informações de contato](#contact-info)

#### [!UICONTROL Informações básicas]

Essas informações já devem ser configuradas pelo [!DNL Workfront] administrador. Todos os campos desta subseção são obrigatórios.

É possível alterar qualquer um dos itens a seguir nesta subseção:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL Nome]</strong></td> 
   <td>Atualize seu nome. Este campo é obrigatório.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL Sobrenome]</strong></td> 
   <td>Atualize seu sobrenome. Este campo é obrigatório.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL Endereço de email]</strong></td> 
   <td> Atualize seu endereço de email. Este campo é obrigatório. Lembre-se de que seu endereço de email também é seu nome de usuário para [!DNL Workfront].</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL Redefinir senha]</strong></td> 
   <td>Redefina sua senha nesta seção. Para obter mais informações sobre como redefinir a senha, consulte <a href="../../../workfront-basics/manage-your-account-and-profile/managing-your-workfront-account/reset-your-password.md" class="MCXref xref">Redefinir sua senha</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>(Condicional) &lt;sso configuration=""&gt; [!UICONTROL Nome de Usuário]</strong></td> 
   <td> Se o seu [!DNL Workfront] o administrador habilitou uma integração de SSO com [!DNL Workfront], seu Nome de usuário SSO será exibido nesse campo. O tipo de configuração de SSO habilitada para o [!DNL Workfront] instância está visível neste campo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>(Condicional) [!UICONTROL Permitir Somente &lt;sso configuration=""&gt; Autenticação]</strong></td> 
   <td> <p> Se o seu [!DNL Workfront] o administrador habilitou uma integração de SSO com [!DNL Workfront] e tiver atualizado usuários para SSO, esse campo será selecionado por padrão. O tipo de configuração de SSO habilitada para o [!DNL Workfront] instância está visível neste campo.</p> <p>Quando este campo é selecionado, você precisa fazer logon no [!DNL Workfront] com suas credenciais de SSO. Ao desmarcá-la, você poderá fazer logon no [!DNL Workfront] com o seu [!DNL Workfront] credenciais.</p> <p>Para obter mais informações sobre a configuração [!DNL Workfront] com uma solução SSO, consulte <a href="../../../administration-and-setup/add-users/single-sign-on/single-sign-on.md" class="MCXref xref">Logon único [!DNL Adobe Workfront]</a>. Para obter mais informações sobre a atualização de usuários para SSO, consulte <a href="../../../administration-and-setup/add-users/single-sign-on/update-users-sso.md" class="MCXref xref">Atualizar usuários para logon único</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Informações do trabalho]

É possível alterar qualquer um dos itens a seguir nesta subseção:

<table style="table-layout:auto">
    <tr>
        <td><strong>[!UICONTROL Título]</strong></td>
        <td>Especifique seu título. Isso não é o mesmo que sua função de trabalho. Seu título não faz parte do agendamento de recursos, enquanto sua função de trabalho é. Seu título é exibido no campo [!DNL Workfront] interface em todos os lugares em que seu nome e seu avatar são exibidos. É visível para todos que têm acesso para ver o usuário.</td>
    </tr>
    <tr>
        <td><strong>[!UICONTROL Fale Comigo Sobre]</strong></td>
        <td>Especifique seus interesses profissionais neste campo.</td>
    </tr>
</table>

#### [!UICONTROL Informações de contato]

É possível alterar qualquer um dos itens a seguir nesta subseção:

<table style="table-layout:auto">
    <tr>
        <td><strong>[!UICONTROL Número de Telefone]</strong></td>
        <td> </td>
    </tr>
    <tr>
        <td><strong>[!UICONTROL Extensão]</strong></td>
        <td> </td>
    </tr>
    <tr>
        <td><strong>[!UICONTROL Número de Celular]</strong></td>
        <td> </td>
    </tr>
    <tr>
        <td><strong>[!UICONTROL Endereço]</strong></td>
        <td> </td>
    </tr>
    <tr>
        <td><strong>[!UICONTROL Cidade]</strong></td>
        <td> </td>
    </tr>
    <tr>
        <td><strong>[!UICONTROL Estado]</strong></td>
        <td> </td>
    </tr>
    <tr>
        <td><strong>[!UICONTROL CEP]</strong></td>
        <td> </td>
    </tr>
    <tr>
        <td><strong>[!UICONTROL País]</strong></td>
        <td> </td>
    </tr>
    <tr>
        <td><strong>[!UICONTROL Imagem de Perfil]</strong></td>
        <td>Sua imagem do perfil se torna seu avatar e fica visível em todo o [!DNL Workfront] sistema, onde quer que seu nome seja exibido.</td>
    </tr>
</table>

### [!UICONTROL Preferências]

Especifique o que deseja exibir no [!DNL Workfront] nesta seção.

>[!NOTE]
>
>Usuários com um [!UICONTROL Solicitante] licença não têm outros itens do painel esquerdo disponíveis para serem adicionados [!UICONTROL Menu principal], fora do [!UICONTROL Solicitações] área. Como um [!DNL Workfront] administrador, você pode atribuir usuários com uma licença de Solicitante a um modelo de layout que inclua todas as outras áreas na [!UICONTROL Menu principal]. Depois disso, é possível selecionar as áreas a serem exibidas nas [!UICONTROL Menu principal] editando o perfil do usuário.

É possível alterar qualquer um dos itens a seguir nesta subseção:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody>
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL Fuso Horário]</strong> </td> 
   <td><p>Especifique seu fuso horário. Isso controla o tempo mostrado nas mensagens de email de saída.</p>
       <p>O fuso horário também afeta o que é exibido em um relatório de calendário PTO.</p></td>
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL Local de email]</strong> </td> 
   <td>Especifique seu idioma preferido aqui. Controla o idioma, a data e o formato do número usados nas mensagens de email de saída.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL Mostrar porcentagem concluída no status de atualização]</strong> </td> 
   <td>Marque esta caixa de seleção para exibir uma barra de porcentagem no campo [!UICONTROL atualizar status] de tarefas, de modo que você possa atualizar a porcentagem concluída de uma tarefa enquanto está inserindo uma atualização de tarefa.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL Enviar trabalho atribuído a mim mesmo para minha guia Trabalhando em]</strong> </td> 
   <td>Selecione este campo para exibir o trabalho que você está atribuindo a si mesmo diretamente na guia [!UICONTROL Trabalhando Em] em vez da guia [!UICONTROL Solicitações de Trabalho].</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>(Condicional) Gera provas automaticamente ao carregar documentos</strong></td> 
   <td>Selecione este campo para começar a gerar uma prova imediatamente após o documento ser carregado no [!DNL Workfront]. Esse campo está desativado por padrão e só pode ser atualizado por um administrador do Workfront.<br>Esse campo só estará disponível se sua empresa tiver adquirido o componente Workfront Proof para o Workfront e se você estiver habilitado como usuário de prova. Para obter mais informações sobre o Workfront Proof, consulte <a href="../../../review-and-approve-work/proofing/managing-proofs-within-workfront/manage-proofs-in-wf.md" class="MCXref xref">Gerenciar provas no Adobe Workfront</a>.
   <p><b>Nota:</b> Documentos carregados para uma solicitação não geram automaticamente uma prova. </p></td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Notificações]

Especifique de quais notificações você deseja receber [!DNL Workfront]. Para obter mais informações sobre como configurar notificações, consulte [Ativar ou desativar suas próprias notificações de eventos](../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

### [!UICONTROL Acesso]

Seu acesso e outros componentes associados a ele são configurados pelo [!DNL Workfront] administrador, quando sua conta estiver configurada.

Somente um [!DNL Workfront] o administrador pode visualizar e editar todos os campos desta seção.

É possível alterar qualquer um dos itens a seguir nesta subseção:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL Está Ativo]</strong> </td> 
   <td>Este campo está visível somente para um usuário que também é [!DNL Workfront] e deverá ser verificado por padrão. Isso significa que o usuário está ativo e pode fazer logon no [!DNL Workfront]</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL Nível de Acesso]</strong> </td> 
   <td>Este campo é visível para usuários com um nível de acesso [!UICONTROL Plan] ou [!UICONTROL Workfront administrator], e só pode ser editado para [!DNL Workfront] administradores. Se você é um [!DNL Workfront] administrador, tenha cuidado para não alterar seu nível de acesso para algo inferior ao modificar esse campo. </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL Modelo de Layout]</strong> </td> 
   <td>Este campo está visível para usuários com um [!UICONTROL Plano] ou [!UICONTROL [!DNL Workfront] administrador], e só pode ser editado para [!UICONTROL [!DNL Workfront] administradores] ou usuários com uma licença do [!UICONTROL Plan] que também tenham acesso de usuário administrativo. Selecione um modelo de layout aqui para atualizar a aparência e o campo da interface do Workfront. Para obter mais informações sobre a configuração de usuários com acesso de usuário administrativo, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md#access-to-edit" class="MCXref xref">Configurar o acesso dos usuários para editar usuários usando um nível de acesso personalizado</a> in <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Conceder acesso aos usuários</a>.<br>Para obter mais informações sobre modelos de layout e como eles afetam sua interface, consulte <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">Criar e gerenciar modelos de layout</a></td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader"><strong>Log in as</strong> </td> 
    <td> <p><strong>Add access</strong> for a Workfront administrator or group administrator (associated with a group you are in) to log in as you. Select an <strong>Access expiration date</strong> for the login. </p> <p>You can repeat this to grant login access to multiple administrators.</p> <p>The settings you choose in this section are visible only to you.
       <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
        <span class="PinkDraftNote">Add a note about this being only for the Enterprise package if they decide to do it that way. Functionality that may come in a later sprint: If you want to be notified when the administrator logs in as you, select Receive an email when this user logs in.</span> 
       </MadCap:conditionalText>
      </p> </td> 
   </tr>
  --> 
  <tr> 
   <td role="rowheader"><strong>(Condicional) [!UICONTROL Usuário pode gerar provas (... de ... licenças de prova restantes)]</strong></td> 
   <td>Este campo só estará disponível se sua empresa usar um antigo [!DNL Workfront] e adquiriu o [!DNL Workfront Proof] componente. Quando essa opção estiver selecionada, você será ativado como um usuário de prova. Ele também exibe o número de licenças de prova usadas em seu sistema do número total de licenças de prova adquiridas. Este campo fica visível e pode ser editado somente para usuários que também [!DNL Workfront] administradores. Para obter mais informações sobre as opções do plano para prova no [!DNL Workfront], consulte <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md">Acesso à funcionalidade de prova no [!DNL Workfront]</a>.</td>
  </tr> 
  <tr> 
   <td role="rowheader"><strong>(Condicional) [!UICONTROL Perfil de Permissão]</strong></td> 
   <td> <p>Este campo exibe o nível de acesso que você tem no [!DNL Workfront Proof]. Ela só estará disponível se:</p> 
    <ul> 
     <li>Sua empresa usa um antigo [!DNL Workfront] e adquiriu o [!DNL Workfront Proof] ou você tem uma licença de [!UICONTROL Trabalho] ou [!UICONTROL Plano] em um [!DNL Workfront] plano.</li> 
     <li>Você está ativado como um usuário de prova.</li> 
    </ul> <p>[!DNL Workfront] os administradores podem editar o campo para todos os usuários, exceto eles próprios, para que todos os usuários vejam o campo como somente visualização em seus próprios perfis. Para obter mais informações sobre o perfil de permissões, consulte <a href="../../../review-and-approve-work/proofing/proofing-overview/permission-profiles.md" class="MCXref xref">Visão geral do perfil de permissão de prova</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Organização]

Normalmente, essas informações são configuradas pelo seu [!DNL Workfront] administrador, quando eles criarem seus [!DNL Workfront] conta. Você também pode atualizar informações sobre sua organização ou estrutura de organização nesta seção. Somente usuários com um [!UICONTROL Plano] ou [!UICONTROL Administrador do sistema] o nível de acesso pode editar esta seção. 

É possível alterar qualquer um dos itens a seguir nesta subseção:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL Empresa]</strong></td> 
   <td>Selecione o nome da empresa à qual você pertence na lista suspensa.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>(Condicional) [!UICONTROL Relata A]</strong></td> 
   <td>Depois de selecionar um <strong>[!UICONTROL Empresa]</strong> para o seu perfil, você também pode especificar o nome do seu gerente neste campo. Você só pode especificar um nome aqui e recomendamos que especifique o nome do seu gerente imediato. Comece digitando o nome e clique para selecioná-lo quando ele for exibido na lista.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>(Condicional) [!UICONTROL Relatórios Diretos]</strong></td> 
   <td>Depois de selecionar um <strong>[!UICONTROL Empresa]</strong> para seu perfil, você também pode especificar o nome dos subordinados diretos neste campo. Você pode especificar quantos subordinados diretos forem necessários aqui. Comece digitando seus nomes e clique em para selecioná-los quando eles aparecerem na lista.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL Equipe Inicial]</strong> </td> 
   <td> <p>Selecione um <strong>[!UICONTROL Equipe Inicial]</strong> no menu suspenso. Este campo é visível para usuários com um nível de acesso [!UICONTROL Plano] ou [!UICONTROL Administrador do Sistema] e só pode ser editado para [!DNL Workfront] administradores ou usuários com uma licença do [!UICONTROL Plan] que também tenham acesso de usuário administrativo. Para obter mais informações sobre a configuração de usuários com acesso de usuário administrativo, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md#access-to-edit" class="MCXref xref">Configurar o acesso dos usuários para editar usuários usando um nível de acesso personalizado</a> in <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Conceder acesso aos usuários</a>.<br></p> <p>Seu <strong>Equipe interna</strong> podem afetar a aparência da [!DNL Workfront] se algum modelo de layout estiver associado à equipe. </p> <p> <br>Para obter mais informações sobre equipes, consulte <a href="../../../people-teams-and-groups/create-and-manage-teams/teams-overview.md" class="MCXref xref">Visão geral das equipes</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL Outras Equipes]</strong> </td> 
   <td> <p>Você pode pertencer a mais de uma equipe. Especifique as equipes adicionais às quais você pertence neste campo começando a digitar o nome de uma equipe e, em seguida, clique para selecioná-la quando ela for exibida na lista. Pertencer a muitas equipes pode gerar confusão sobre o trabalho atribuído às equipes. Para obter mais informações sobre equipes, consulte <a href="../../../people-teams-and-groups/create-and-manage-teams/teams-overview.md" class="MCXref xref">Visão geral das equipes</a>.</p> <p>Este campo é visível para usuários com uma licença de [!UICONTROL Plano] ou [!UICONTROL Administrador do Sistema] e só pode ser editado para [!DNL Workfront] administradores ou usuários com uma licença do [!UICONTROL Plan] que também tenham acesso de usuário administrativo. Para obter mais informações sobre a configuração de usuários com acesso de usuário administrativo, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md#access-to-edit" class="MCXref xref">Configurar o acesso dos usuários para editar usuários usando um nível de acesso personalizado</a> in <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Conceder acesso aos usuários</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL Grupo Padrão]</strong> </td> 
   <td> <p>Selecione um <strong>[!UICONTROL Grupo Padrão]</strong> no menu suspenso.</p> <p>Observação: este campo é obrigatório. Você não pode ter um usuário não associado a um grupo.<br></p> <p>Este campo é visível para usuários com um nível de [!UICONTROL Plano] ou [!UICONTROL Administrador do Sistema]. Para obter mais informações sobre quem pode editar a <strong>[!UICONTROL Grupo Padrão]</strong> , consulte o <a href="../../../administration-and-setup/add-users/create-and-manage-users/add-users.md#prerequisites" class="MCXref xref">Adicionar usuários</a> seção em <a href="../../../administration-and-setup/add-users/create-and-manage-users/add-users.md" class="MCXref xref">Adicionar usuários</a>.Seu <strong>[!UICONTROL Grupo Padrão]</strong> é o grupo padrão para todos os projetos e o padrão <strong>[!UICONTROL Grupo Padrão]</strong> para todos os novos usuários que você criar. Todos os formulários personalizados que você criar serão compartilhados com a <strong>[!UICONTROL Grupo Padrão]</strong> por padrão.</p> <p>Para obter mais informações sobre grupos, consulte <a href="../../../administration-and-setup/manage-groups/groups-overview/groups.md" class="MCXref xref">Visão geral dos grupos</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL Outros Grupos]</strong> </td> 
   <td> <p>Você pode pertencer a vários grupos. Especifique os grupos adicionais aos quais você pertence neste campo, começando a digitar o nome de um grupo. Clique para selecioná-la quando ela for exibida na lista. Este campo é visível para usuários com um nível de acesso de [!UICONTROL Plano] ou [!UICONTROL Administrador do Sistema]. Para obter mais informações sobre quem pode editar a <strong>[!UICONTROL Outros Grupos]</strong> , consulte a seção "Outros grupos" em <a href="../../../administration-and-setup/add-users/create-and-manage-users/add-users.md" class="MCXref xref">Adicionar usuários</a>.</p> <p>Para obter mais informações sobre grupos, consulte <a href="../../../administration-and-setup/manage-groups/groups-overview/groups.md" class="MCXref xref">Visão geral dos grupos</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Planejamento de recursos]

As informações de planejamento de recursos afetam a linha do tempo das atribuições de trabalho, o tempo registrado, o custo e a receita dos projetos em que você está. Normalmente, essa área é atualizada pela variável [!DNL Workfront] administrador, um gerente de projeto ou de recursos, ou pelo seu gerente direto.

Use qualquer um dos seguintes itens nesta seção:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL Desativação de Agendamento]</strong></td> 
   <td>Marque essa caixa se desejar agendar a desativação da conta após um período. No <p><strong>[!UICONTROL Data de Desativação Agendada]</strong> for exibida, especifique a data após a qual sua conta será desativada. Para obter informações sobre como desativar usuários, consulte <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md#scheduling-users-for-deactivation" class="MCXref xref">Programar usuários para desativação</a> in <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">Desativar ou reativar um usuário</a>. </p><p>É possível editar os campos de desativação da sua conta se você tiver uma licença de plano ou se for o [!DNL Workfront] administrador. </p></td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL Função Primária]</strong></td> 
   <td> <p>Essa é a principal função que você pode desempenhar no Workfront. Todas as tarefas e problemas aos quais você está atribuído também estão atribuídos a esta função de trabalho, por padrão. As funções de trabalho são essenciais no gerenciamento de recursos. Para obter mais informações sobre funções, consulte <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Criar e gerenciar funções de trabalho</a>.</p> <p>Você pode atualizar este campo somente se tiver uma licença do [!UICONTROL Plan] com acesso de usuário administrativo ou se for um [!DNL Workfront] administrador. Para obter mais informações sobre a configuração de usuários com acesso de usuário administrativo, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md#access-to-edit" class="MCXref xref">Configurar o acesso dos usuários para editar usuários usando um nível de acesso personalizado</a> in <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Conceder acesso aos usuários</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>(Condicional) Se você selecionou uma [!UICONTROL Função Primária], o campo [!UICONTROL Porcentagem de Disponibilidade FTE] será exibido.</strong></td> 
   <td>Especifique que porcentagem do seu tempo agendado está alocada para esta função de trabalho. O valor padrão da [!UICONTROL Porcentagem de Disponibilidade FTE] para a Função Primária é 100%</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL Outras Funções]</strong> </td> 
   <td> <p>Você pode ter várias funções de trabalho no [!DNL Workfront]. As funções de trabalho são essenciais no gerenciamento de recursos. Para obter mais informações sobre funções, consulte <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Criar e gerenciar funções de trabalho</a>.</p> <p>Você pode atualizar este campo somente se tiver uma licença do [!UICONTROL Plan] com acesso de usuário administrativo ou se for um [!DNL Workfront] administrador. Para obter mais informações sobre a configuração de usuários com acesso de usuário administrativo, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md#access-to-edit" class="MCXref xref">Configurar o acesso dos usuários para editar usuários usando um nível de acesso personalizado</a> in <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Conceder acesso aos usuários</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>(Condicional) Se você selecionou uma ou várias Outras funções, o campo [!UICONTROL Porcentagem de disponibilidade de FTE] é exibido para cada função.</strong></td> 
   <td> <p>Especifique que porcentagem do seu tempo agendado está alocada para cada função de trabalho. O valor padrão da [!UICONTROL Porcentagem de Disponibilidade FTE] para [!UICONTROL Outras Funções] é 0%.</p> <p> <img src="assets/user-settings-roles-and-dte-boxes-rp-story--1--350x224.png" alt="user_settings_roles_and_date_boxes_rp_story_1_.png" style="width: 350;height: 224;"> </p> <p>Nota:  
     <ul> 
      <li>Se [!UICONTROL Outras Funções] tiverem 0% de Disponibilidade FTE, elas não serão exibidas no [!UICONTROL Resource Planner], a menos que os usuários sejam atribuídos a tarefas nessas funções.</li> 
      <li> <p>A soma de todos <strong>[!UICONTROL Porcentagens de Disponibilidade de FTE]</strong> para todas as funções, deve ser igual a 100%. Cada [!UICONTROL Porcentagem de Disponibilidade FTE] calcula as [!UICONTROL Horas Disponíveis] para cada função por usuário no [!UICONTROL Resource Planner]. </p> <p>As [!UICONTROL Horas Disponíveis] para cada função por usuário dependem do tempo disponível para o usuário. O tempo disponível para o usuário é calculado por [!DNL Workfront] dependendo do método selecionado pelo [!DNL Workfront] administrador para calcular o FTE nas [!UICONTROL Preferências de Gerenciamento de Recursos]. Para obter mais informações sobre como calcular a disponibilidade do usuário, consulte <a href="../../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">Visão geral do cálculo de horas e FTE para usuários e funções no Planejador de recursos</a>. Para obter mais informações sobre a configuração das preferências do Gerenciamento de recursos, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md" class="MCXref xref">Configurar preferências de gerenciamento de recursos</a>.</p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Agendar</strong></td> 
   <td> <p>Somente [!DNL Workfront] administradores ou usuários com uma licença do [!UICONTROL Plan] que também tenham acesso administrativo a folhas de horas e horas podem atualizar este campo. Para obter mais informações sobre acesso administrativo a folhas de horas e horas, consulte a seção "Folhas de horas e horas" em <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Conceder aos usuários acesso administrativo a determinadas áreas</a>.</p> <p>Selecione a folha de horas correta para você no menu suspenso. Isso garante que suas folhas de horas sejam geradas automaticamente, de acordo com as especificações definidas pelo [!DNL Workfront] administrador. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL Tipo de Hora Padrão]</strong> </td> 
   <td>Selecione o tipo de hora padrão. Esse é o tipo de hora que o sistema usa por padrão sempre que você faz logon no Workfront.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL Tipos de Horas Disponíveis]</strong> </td> 
   <td>Selecione os tipos de horas que devem estar disponíveis para você selecionar, ao registrar o tempo. Os tipos de hora nesse menu suspenso são disponibilizados pelo seu [!DNL Workfront] administrador.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL Pool de Recursos]</strong> </td> 
   <td>Selecione um conjunto de recursos ao qual você pertence. Este campo é somente para fins informativos e de emissão de relatórios e não afeta a programação ou o planejamento de recursos.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL FTE]</strong> </td> 
   <td> <p>O número especificado aqui é levado em conta para calcular sua disponibilidade com base no Agendamento Padrão apenas quando as [!UICONTROL Resource Management Preferences] no nível do sistema são definidas como <strong>[!UICONTROL A Agenda Padrão]</strong>.</p> <p>Por exemplo, se o valor de FTE for 0,5 e a [!UICONTROL Default Schedule] for 40 horas, você estará disponível para trabalhar 20 horas por semana.</p> <p>Se as [!UICONTROL Preferências de Gerenciamento de Recursos] no nível do sistema estiverem definidas como <strong>[!UICONTROL A Agenda do Usuário]</strong>, o valor especificado aqui será ignorado e você estará disponível para trabalhar de acordo com o especificado em seu cronograma. Nesse caso, o FTE do [!UICONTROL Resource Planner] é calculado pela seguinte fórmula: </p> <p><code style="font-style: normal;">[!UICONTROL User Available FTE] = [!UICONTROL Hours from the Schedule of the User/ Default Schedule Hours]</code> </p> <p>Para obter mais informações sobre o cálculo do FTE do usuário, consulte <a href="../../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">Visão geral do cálculo de horas e FTE para usuários e funções no Planejador de recursos</a>.</p> <p>Para obter mais informações sobre a criação de agendamentos em [!DNL Workfront], consulte <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Criar um agendamento</a>.</p> <p>Para obter mais informações sobre a configuração de Preferências de Gerenciamento de Recursos, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md" class="MCXref xref">Configurar preferências de gerenciamento de recursos</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL Custo por Hora]</strong> </td> 
   <td>Especifique a quantidade de custo por hora para o usuário. Para obter mais informações sobre o rastreamento de custos no [!DNL Workfront], consulte <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Rastrear custos</a>. Não é possível atualizar essas informações, a menos que você tenha acesso aos dados financeiros do seu nível de acesso ou se for um [!DNL Workfront] administrador. Para obter mais informações sobre acesso financeiro, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md" class="MCXref xref">Conceder acesso a dados financeiros</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL Cobrança por Hora]</strong> </td> 
   <td>Especifique o valor do faturamento por hora para o usuário. Para obter mais informações sobre o rastreamento de faturamento e receita, consulte <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">Visão geral de faturamento e receita</a>. Não é possível atualizar essas informações a menos que você tenha acesso aos dados financeiros do seu nível de acesso ou se for um [!DNL Workfront] administrador. Para obter mais informações sobre acesso financeiro, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md" class="MCXref xref">Conceder acesso a dados financeiros</a>.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Formulário personalizado]

Você pode associar um formulário personalizado ao seu perfil de usuário. Isso permite armazenar informações adicionais para o usuário que, de outra forma, não poderão ser armazenadas na [!DNL Workfront] campos nativos descritos acima.\
Você deve ter um dos seguintes direitos de acesso ou permissões para anexar um formulário personalizado ao seu usuário:

* Você é um [!DNL Workfront] administrador.
* Você é um [!UICONTROL Plano] e o formulário personalizado de usuário é compartilhado com um de seus grupos.

Todos os usuários podem ver formulários personalizados que foram associados a seus usuários.

Seu [!DNL Workfront] o administrador precisa configurar formulários personalizados para o objeto de usuário para que você possa anexar um formulário personalizado ao seu perfil de usuário. Para obter mais informações sobre como criar formulários personalizados, consulte [Criar ou editar um formulário personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

### [!UICONTROL Comentário]

Você pode registrar um comentário no perfil do usuário armazenado no [!UICONTROL Atualizações] do usuário.

Você pode clicar no link [!UICONTROL pessoas] ícone para incluir outros na atualização.

Você pode clicar no link [!UICONTROL bloquear] ícone para tornar esta atualização privada para usuários que estão na mesma empresa que você.
