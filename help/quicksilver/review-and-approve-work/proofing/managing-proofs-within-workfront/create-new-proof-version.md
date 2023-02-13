---
product-area: documents
navigation-topic: manage-proofs-within-workfront
title: Criar uma nova versão de uma prova
description: O gerenciamento de feedback em várias versões ou revisões de um trabalho pode ser um grande desafio. A Workfront simplifica esse processo, permitindo que você crie e compare várias versões de uma prova.
author: Courtney
feature: Digital Content and Documents
exl-id: ee0c859e-349b-4e7a-ac80-164740b950f0
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '1721'
ht-degree: 0%

---

# Criar uma nova versão de uma prova

O gerenciamento de feedback em várias versões ou revisões de um trabalho pode ser um grande desafio. A Workfront simplifica esse processo, permitindo que você crie e compare várias versões de uma prova.

Considere as seguintes informações ao criar uma nova versão de uma prova:

* Você pode conceder permissão ao usuário para ver uma versão, mas não outra. Por outro lado, se você compartilhar uma versão posterior com um usuário, ele não poderá ver as versões anteriores, a menos que você volte e conceda explicitamente ao usuário acesso a essas versões anteriores.
* Para criar uma nova versão de uma prova, você deve ter direitos de edição na prova.

   Consulte [Gerenciar funções de prova na Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md) e [Perfis de permissões de prova na Workfront Proof](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md) para obter mais informações sobre quem tem direitos de edição em uma prova.

   Para obter informações sobre o compartilhamento de versões de prova, consulte  [Compartilhar uma prova na Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/share-proof.md).

>[!IMPORTANT]
>
>Se uma prova for criada no Adobe Workfront, qualquer nova versão criada para essa prova também deverá ser criada no Workfront. Não é possível criar uma nova versão de uma prova no Workfront Proof se essa prova foi criada no Workfront.

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
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a documentos</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, função ou Perfil de permissão de prova você possui, entre em contato com o administrador da Workfront ou da Workfront Proof.

## Criar uma nova versão de uma prova no Workfront

Há várias maneiras de carregar uma nova versão de prova no Workfront. As configurações de prova padrão podem ou não ser transferidas da versão anterior, dependendo do método escolhido:

* **Gerar provas automaticamente ao carregar documentos**: As configurações de prova padrão não são carregadas. Se essa configuração estiver ativada no perfil do usuário, as configurações de prova padrão não serão carregadas ao arrastar e soltar uma nova versão.
* **Criar prova > Simples**: As configurações de prova padrão não são carregadas. Se você escolher Simples ao criar uma nova versão de prova, as configurações de prova padrão não serão transferidas da versão anterior.
* **Adicionar novo > Versão > Prova**: As configurações de prova padrão são transferidas da versão anterior.
* **Criar prova > Avançado**: As configurações de prova padrão são transferidas da versão anterior.

   <table>
  <tbody>
  <tr>
  <td>Gerar provas automaticamente ao carregar documentos</td>
  <td>As configurações de prova padrão não são carregadas. Se essa configuração estiver ativada no perfil do usuário, as configurações de prova padrão não serão carregadas ao arrastar e soltar uma nova versão.</td>
  </tr>
  <tr>
  <td>Criar prova &gt; Simples</td>
  <td>As configurações de prova padrão não são carregadas. Se você escolher Simples ao criar uma nova versão de prova, as configurações de prova padrão não serão transferidas da versão anterior.</td>
  </tr>
  <tr>
  <td>Adicionar novo &gt; Versão &gt; Prova</td>
  <td>As configurações de prova padrão são transferidas da versão anterior.</td>
  </tr>
  <tr>
  <td>Criar prova &gt; Avançado</td>
  <td>As configurações de prova padrão são transferidas da versão anterior.</td>
  </tr>
  </tbody>
  </table>




Para criar uma nova versão de uma prova:

1. Abra a lista de documentos que contém a prova.
1. A partir do sistema de arquivos do seu computador, arraste e solte um novo arquivo sobre a prova.

   Ou

   Selecione a linha na qual a prova está listada, clique em **Adicionar novo** > **Versão**, em seguida, clique na opção que deseja usar para adicionar a nova versão da prova.

   ![](assets/add-new-version-350x185.png)

## Criar uma nova versão de uma prova no visualizador de prova (somente Workfront Proof)

Se você estiver usando a Workfront Proof independente, poderá criar uma nova versão de uma prova contendo um único arquivo ou captura da Web. 

>[!NOTE]
>
>Se sua conta estiver em um plano Enterprise e você fizer upload de vários arquivos ou capturas da Web, eles serão combinados automaticamente em uma única nova versão. Consulte [Criar uma prova de várias páginas](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-multi-page-proof.md) para obter mais informações.

Para criar uma nova versão de uma prova no Workfront Proof:

1. Abra a prova.
1. Clique no botão **Versão** menu suspenso no canto superior esquerdo e clique em **+ Nova versão** na caixa exibida.

   No **Nova versão de prova de** na página exibida, é possível visualizar todos os revisores da versão anterior, incluindo suas funções e configurações de notificação por email. É possível editar facilmente as funções e notificações dos revisores existentes ou remover os revisores existentes da nova versão nesta página.

1. Em **Adicionar arquivos**, faça upload de um arquivo como uma nova versão da prova arrastando e soltando do seu computador ou clicando em **navegar** e selecionando o arquivo desejado. Você pode digitar um **Nome da prova** para a versão ou deixe essa caixa em branco para usar o mesmo nome de arquivo com um número de versão adicionado no final.

   Ou

   Capture uma página da Web como uma nova versão da prova digitando um URL.

   >[!NOTE]
   >
   >O recurso de arrastar e soltar está disponível somente em navegadores que suportam totalmente o HTML5. Isso exclui o Internet Explorer 7 a 9 e o Safari.

1. Em **Fluxo de trabalho**, faça qualquer uma das alterações a seguir para especificar os revisores para essa versão da prova.

   Os revisores da versão anterior são substituídos pelos revisores adicionados.

   * Altere o **Proprietário** da versão para outro usuário na sua conta.\
      Para obter informações sobre permissões de proprietário, consulte [Perfis de permissões de prova na Workfront Proof](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md).

   * Usar o **Digite o nome do contato ou endereço de email para adicionar uma caixa de destinatário**, adicionar revisores à versão. Você pode especificar uma **Função de prova** e um **Alertas por email** para cada recipient.

      Para obter informações sobre como adicionar grupos à prova, consulte  [Adicionar grupos a uma prova](../../../workfront-proof/wp-mnguserscontacts/groups/add-groups.md). Para obter informações sobre funções, consulte [Gerenciar funções de prova na Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md).

      >[!NOTE]
      >
      >Se o criador ou o proprietário da prova tiver [O email de prova feita](../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/proof-made-email.md) desabilitados por padrão (em suas configurações pessoais), eles não receberão nenhum email de prova ou Nova prova mesmo se a caixa Notificar pessoas por email estiver marcada na página Nova prova . Para obter informações sobre notificações por email, consulte [Definir configurações de notificação de email no Workfront Proof](../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md). Consulte também [O email de prova feita](../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/proof-made-email.md) e [Novo email de prova](../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/new-proof-email.md).

   * Defina um prazo de prova para a versão.
   * Passe o mouse sobre o nome de um revisor para ver as decisões que ele ou ela tomaram em uma versão anterior.

1. Em **Notificação por e-mail**, execute um dos seguintes procedimentos:

   * Especifique se deseja notificar os revisores sobre a nova versão.\
      Sua seleção será registrada na seção Atividade da página Detalhes da prova . Para obter mais informações, consulte [Gerenciar detalhes de prova na prova do Workfront](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).

   * Adicione um assunto e uma mensagem personalizados.

1. No **Organização** siga um destes procedimentos: 

   * Aplique uma ou mais tags à prova. Para obter mais informações, consulte [Criar e gerenciar tags na Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/create-and-manage-tags.md).\
      Observe que as tags também são herdadas da versão anterior da prova. Se você adicionar uma nova tag à nova versão, as versões anteriores também serão marcadas.

   * Adicione a versão a uma pasta. Consulte [Gerenciar pastas na prova do Workfront](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md) para obter mais informações. A pasta será copiada da versão anterior da prova. Se você selecionar uma pasta diferente, toda a prova (todas as versões) será movida.

   * Os administradores de faturamento e administradores podem tornar o campo de pasta obrigatório em toda a conta na guia Configurações . Consulte para obter mais informações.

1. Em Configurações de prova, faça qualquer uma das alterações abaixo:

   * Exigir logon na prova
   * Exigir assinaturas eletrônicas na prova (somente no Enterprise plan)
   * Bloquear a prova quando todas as decisões forem tomadas
   * Permitir ou bloquear o download do arquivo original
   * Compartilhamento público da prova, incluindo configurações de compartilhamento público
   * Assinatura da prova\
      As seleções feitas nesta seção serão mostradas na página Detalhes da prova (onde alguns campos podem ser editados). Para obter mais informações, consulte [Gerenciar detalhes de prova na prova do Workfront](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).

<!--
<h2 data-mc-conditions="QuicksilverOrClassic.Draft mode">Create a new version of a proof from the proofing viewer</h2>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">To create a new version from the proofing viewer</p>
-->

<!--
<ol data-mc-conditions="QuicksilverOrClassic.Draft mode">
<li value="1">Open the proof.</li>
<li value="2"> <p>Click the <strong>Version</strong> drop-down menu in the upper-left corner, then click <strong>+ New version</strong> in the box that appears.</p> <p>On the <strong>New proof version of</strong> page that appears, you can see all the reviewers from the previous version, including their roles and email notification settings. You can easily edit the roles and notifications of existing reviewers or remove existing reviewers from the new version on this page.</p> </li>
<li value="3"> <p>Under <strong>Add files</strong>, upload a file as a new version of the proof by dragging and dropping from your computer or by clicking <strong>browse</strong> and selecting the file you want. You can type a&nbsp;<strong>Proof name</strong>&nbsp;for the version or leave this box blank to&nbsp;use the same filename with a version number added on the end.</p> <p>Or<br></p> <p>Capture a web page as a new version of the proof by typing a URL</p> <note type="note">
Drag and drop is available only with browsers that fully support HTML5. This excludes Internet Explorer 7 through 9 and Safari.
<br>
</note> </li>
<li value="4"> <p>Under <strong>Workflow</strong>, make any of the following changes to specify the reviewers for this version of the proof.</p> <p>Reviewers from the previous version are replaced by the reviewers you add.</p>
<ul>
<li>Change the <strong>Owner</strong> of the version to another user in your account.<br>For information about owner permissions, see <a href="../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md" class="MCXref xref">Proof Permissions Profiles in Workfront Proof</a>.</li>
<li> <p>Using the <strong>Type contact name or email address to add a recipient box</strong>, add reviewers to the version. You can specify a <strong>Proof role</strong> and an <strong>Email alerts</strong> type for each recipient.</p> <p>For information about adding groups to the proof, see&nbsp;<a href="../../../workfront-proof/wp-mnguserscontacts/groups/add-groups.md" class="MCXref xref">Add Groups to a Proof</a>.&nbsp;For information about roles, see <a href="../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md" class="MCXref xref">Manage Proof Roles in Workfront Proof</a>.</p> <note type="note">
If the creator or owner of&nbsp;&nbsp;the proof has
<a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/proof-made-email.md" class="MCXref xref">The Proof Made email</a> disabled by default (in their personal settings), they won't receive any Proof made or New proof emails even if the Notify people by email box is checked on the New proof page. For information about email notifications, see
<a href="../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md" class="MCXref xref">Configure email notification settings in Workfront Proof</a>.&nbsp;See also
<a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/proof-made-email.md" class="MCXref xref">The Proof Made email</a> and
<a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/new-proof-email.md" class="MCXref xref">New proof email</a>.
<br>
</note> </li>
<li>Set a proof deadline for the version.</li>
<li>Hover over a reviewer's name to see any decisions he or she made on a previous version.</li>
</ul> </li>
<li value="5">Under <strong>Email notification</strong>, do any of the following:
<ul>
<li>Specify whether you want to notify the reviewers of the new version.<br>Your selection will be logged in the Proof activity section on the Proof details page.</li>
<li>Add a custom subject and message.</li>
</ul></li>
<li value="6">Under Proof settings, make any of the changes below:
<ul>
<li>Require login on the proof</li>
<li>Require electronic signatures on the proof (Enterprise plan only)</li>
<li>Lock the proof when all decisions are made</li>
<li>Allow or block download of original file</li>
<li>Public sharing of the proof,&nbsp;including public sharing settings</li>
<li>Subscription to the proof<br>The selections made in this section will be shown in the Proof details page.</li>
</ul></li>
</ol>
-->

## Sobre a mensagem Nova versão

Se houver um assunto/mensagem personalizado incluído na versão anterior da prova, ele será exibido por padrão na página Nova versão . Você pode:

* Edite o assunto e a mensagem.
* Desmarque a caixa Notificar pessoas por email, o que significa que nenhum email será enviado aos revisores para notificá-los de que eles têm uma nova versão para revisão.

   >[!NOTE]
    Isso não é afetado por nenhum assunto/mensagem personalizada padrão salvo em suas configurações pessoais.

Se você tiver um assunto e uma mensagem padrão salvos em suas configurações pessoais, isso afetará a mensagem que é exibida por padrão na página Nova versão :

* Se você optar por notificar seus revisores por email para a versão anterior da prova usando o email padrão (por exemplo, nenhum assunto/mensagem personalizada), o assunto/mensagem personalizada padrão (suas configurações pessoais) será exibido na página Nova versão. É possível editar o assunto e a mensagem personalizados ou desmarcar a caixa Notificar pessoas por email (o que significa que nenhum email será enviado aos revisores para notificá-los de que eles têm uma nova versão para revisão).
* Se você optar por não notificar seus revisores por email para a versão anterior da prova (por exemplo, nenhum email padrão ou personalizado), a página Nova versão não incluirá nenhuma mensagem por padrão. Para notificar seus revisores sobre a nova versão, clique no link Send a Message , que mostrará o assunto/mensagem personalizado padrão (de acordo com suas configurações pessoais). Em seguida, você pode editar o assunto e a mensagem personalizados, se necessário.

Se você não tiver um assunto e mensagem padrão salvos em suas configurações pessoais, o seguinte será exibido na página Nova versão :

* Se você optar por notificar seus revisores por email para a versão anterior da prova usando o email padrão (por exemplo, nenhum assunto/mensagem personalizado), a opção Notificar pessoas por email será selecionada por padrão na página Nova versão . Para adicionar uma mensagem personalizada, clique no link .
* Se você optar por não notificar seus revisores por email para a versão anterior da prova (por exemplo, nenhum email padrão ou personalizado), a página Nova versão não incluirá nenhuma mensagem por padrão. Para notificar seus revisores sobre a nova versão, clique no link Send a Message . É possível adicionar um assunto e uma mensagem personalizados clicando no link Adicionar mensagem personalizada .
