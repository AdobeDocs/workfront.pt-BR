---
product-area: documents
navigation-topic: manage-proofs-within-workfront
title: Criar uma nova versão de uma prova
description: Gerenciar feedback em várias versões ou revisões de um trabalho pode ser um enorme desafio. O Workfront simplifica esse processo permitindo criar e comparar várias versões de uma prova.
author: Courtney
feature: Digital Content and Documents
exl-id: ee0c859e-349b-4e7a-ac80-164740b950f0
source-git-commit: daa46f0e2a5f656d048260d4a714ed02f01cdbbf
workflow-type: tm+mt
source-wordcount: '1521'
ht-degree: 0%

---

# Criar uma nova versão de uma prova

<!-- Audited: 4/2025 -->

Gerenciar feedback em várias versões ou revisões de um trabalho pode ser um desafio. O Adobe Workfront simplifica esse processo permitindo criar e comparar várias versões de uma prova.

Considere as seguintes informações ao criar uma nova versão de uma prova:

* É possível conceder permissão a um usuário para ver uma versão, mas não outra. Por outro lado, se você compartilhar uma versão posterior com um usuário, ele não poderá ver as versões anteriores, a menos que você retorne e conceda a ele acesso a essas versões anteriores.
* Você deve ter direitos de Edição na prova para criar uma nova versão.

  Para obter mais informações, consulte [Gerenciar funções de prova no Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md) e [Perfis de permissões de prova no Workfront Proof](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md).

  Para obter informações sobre o compartilhamento de versões de prova, consulte  [Compartilhar uma prova no Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/share-proof.md).

>[!IMPORTANT]
>
>Se uma prova for criada no Adobe Workfront, quaisquer novas versões dessa prova também deverão ser criadas no Workfront. Não é possível criar uma nova versão de uma prova no Workfront Proof se essa prova foi criada no Workfront.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront</td> 
   <td> <p>Atual: Pro ou superior</p> <p>ou</p> <p>Herdados: Select ou Premium</p> <p>Para obter mais informações sobre acesso de revisão de texto com os diferentes planos, consulte <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Acesso à funcionalidade de revisão de texto no Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td> <p>Atual: Padrão</p> 
   <p>Ou</p>
   <p>Herdados: Trabalho ou Plano (é necessário ter a prova ativada para o usuário)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Perfil de Permissões de Prova </td> 
   <td>Gerente ou superior</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Editar acesso a documentos</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso aos objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Criar uma nova versão de prova no Workfront

Há várias maneiras de fazer upload de uma nova versão de prova no Workfront. As configurações de prova padrão podem ou não ser transferidas da versão anterior, dependendo do método selecionado:

* **Gerar provas automaticamente ao carregar documentos**: se esta configuração estiver habilitada no perfil do usuário, as configurações de prova padrão não serão transferidas quando você arrastar e soltar uma nova versão.
* **Criar prova > Simples**: se você selecionar essa opção, as configurações de prova padrão não serão transferidas da versão anterior.
* **Adicionar nova > Versão > Prova**: se você selecionar essa opção, as configurações de prova padrão serão transferidas da versão anterior.
* **Criar prova > Avançado**: se você selecionar essa opção, as configurações de prova padrão serão transferidas da versão anterior.

Para criar uma nova versão de uma prova:

1. Abra a lista de documentos que contém a prova.
1. No sistema de arquivos do seu computador, arraste e solte um novo arquivo sobre a prova.

   Ou

   Selecione a linha na qual a prova está listada, clique em **Adicionar nova** > **Versão** e clique na opção que deseja usar para adicionar a nova versão da prova.

   ![Adicionar nova versão](assets/add-new-proof-version.png)

## Criar uma nova versão de prova no visualizador de provas (somente Workfront Proof)

Se estiver usando o Workfront Proof independente, você poderá criar uma nova versão de uma prova contendo um único arquivo ou captura da Web. 

>[!NOTE]
>
>Se sua conta estiver em um plano Enterprise e você fizer upload de vários arquivos ou capturas da Web, eles serão combinados automaticamente em uma única versão nova. Consulte [Criar uma prova de várias páginas](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-multi-page-proof.md) para obter mais informações.

Para criar uma nova versão de uma prova no Workfront Proof:

1. Abra a prova.
1. No canto superior esquerdo, clique no menu suspenso **Versão** e em **+ Nova versão** na caixa exibida. A nova página de versão de prova é aberta.

   ![Adicionar nova versão](assets/new-version-button.png)

1. Na seção **Adicionar arquivos**, faça upload de um arquivo como a nova versão de prova arrastando-o e soltando-o do seu computador ou clicando em **procurar** e selecionando um arquivo.

   Ou

   Capture uma página da Web como uma nova versão da prova inserindo um URL.

   >[!NOTE]
   >
   >Arrastar e soltar está disponível somente em navegadores com suporte total para HTML5. Isso exclui o Internet Explorer 7 a 9 e o Safari.

1. (Opcional) Selecione o título da prova e insira um novo **Nome da prova** para a versão.

1. Na seção **Fluxo de trabalho**, faça qualquer uma das seguintes alterações para adicionar revisores para esta versão de prova (isso substituirá os revisores da versão anterior):

   * (Opcional) Altere o **Proprietário** da versão para outro usuário em sua conta.

     Para obter informações, consulte [Perfis de permissões de prova no Workfront Proof](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md).

   * (Opcional) Usando a caixa **Digite o nome do contato ou endereço de email para adicionar um destinatário**, adicione revisores à versão. Em seguida, você pode selecionar um tipo de **Função de prova** e **Alertas de email** para cada destinatário.

     Para obter informações, consulte [Adicionar grupos a uma prova](../../../workfront-proof/wp-mnguserscontacts/groups/add-groups.md) e [Gerenciar funções de prova no Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md).

     >[!NOTE]
     >
     >Se o criador ou proprietário da prova tiver o email de prova desativado por padrão em suas configurações pessoais, ele não receberá nenhum email de prova feito ou novo, mesmo se a caixa **Notificar recipients sobre esta prova** estiver marcada na página Nova prova. Para obter informações, consulte [Definir configurações de notificação por email no Workfront Proof](../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md), [O email de prova](../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/proof-made-email.md) e [Novo email de prova](../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/new-proof-email.md).

   * (Opcional) Defina um prazo de prova.

   * (Opcional e Condicional) Selecione um novo tomador de decisão principal no menu suspenso **Transferir direitos de decisão principais para**.

   * (Opcional) Selecione a caixa **Requer apenas uma decisão para este estágio** para remover a opção para definir um usuário como o novo tomador de decisão principal.

1. Na seção **Notificação por email**, selecione uma das seguintes configurações:

   * (Opcional) **Notificar recipients sobre esta prova**: selecione esta opção para notificar os revisores sobre a nova versão. Sua seleção será registrada na seção **Atividade** da página **Detalhes da prova**. Para obter mais informações, consulte [Gerenciar detalhes da prova no Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).

   * (Condicional e Opcional) **Adicionar assunto e mensagem personalizados**: selecione essa opção para adicionar uma linha de assunto e uma mensagem personalizadas à notificação por email.

1. Na seção **Organização**, selecione uma das seguintes configurações:

   * Aplique uma ou mais tags à prova. Para obter mais informações, consulte [Criar e Gerenciar Marcas no Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/create-and-manage-tags.md).

   * Adicionar a versão a uma pasta. A pasta será copiada da versão anterior da prova. Se você selecionar uma pasta diferente, a prova inteira, que inclui todas as versões, será movida. Para obter mais informações, consulte [Gerenciar pastas no Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md).

   * Administradores e administradores de cobrança podem tornar o campo de pasta obrigatório em toda a conta na guia **Configurações**.

1. Na seção **Configurações de prova**, selecione uma das seguintes configurações:

   * Exigir que um usuário faça logon para visualizar a prova.
   * Exigir assinaturas eletrônicas na prova (somente plano Enterprise).
   * Bloqueie a prova quando todas as decisões forem tomadas.
   * Permitir o download do arquivo original.
   * Permitir compartilhamento público da prova.
   * Permitir assinatura da prova.

     As seleções feitas nesta seção serão mostradas na página **Detalhes da prova** (onde alguns campos podem ser editados). Para obter mais informações, consulte [Gerenciar detalhes da prova no Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).

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

Se houver um assunto/mensagem personalizado incluído na versão anterior da prova, ele será exibido por padrão na página Nova versão. Você pode:

* Editar o assunto e a mensagem.
* Desmarque a caixa Notificar pessoas por email, o que significa que nenhum email será enviado aos revisores para notificá-los de que eles têm uma nova versão para revisar.

  >[!NOTE]
  >
  >Isso não é afetado por nenhum assunto/mensagem padrão personalizado salvo em suas configurações pessoais.

Se você tiver um assunto e uma mensagem padrão salvos nas suas configurações pessoais, isso determinará qual mensagem é mostrada por padrão na página Nova versão:

* Se você notificou seus revisores sobre a versão de prova anterior usando o email padrão (por exemplo, nenhum assunto/mensagem personalizados), seu assunto/mensagem personalizado padrão (suas configurações pessoais) será exibido na página Nova versão. É possível editar o assunto personalizado e a mensagem ou desmarcar a caixa de email Notificar pessoas por, o que significa que nenhum email será enviado aos revisores para notificá-los de que eles têm uma nova versão para revisar.
* Se você não tiver notificado os revisores sobre a versão de prova anterior (por exemplo, nenhum email padrão ou personalizado), a página Nova versão não incluirá uma mensagem por padrão. Para notificar seus revisores sobre a nova versão, clique no link Send a Message, que mostrará o assunto/mensagem personalizado padrão (de acordo com suas configurações pessoais). Em seguida, você pode editar o assunto e a mensagem personalizados, conforme necessário.

Se você não tiver um assunto e uma mensagem padrão salvos nas suas configurações pessoais, os itens a seguir serão exibidos na página Nova versão:

* Se você notificar seus revisores sobre a versão de prova anterior usando o email padrão (por exemplo, sem assunto/mensagem personalizada), a opção Notificar pessoas por email será selecionada por padrão na página Nova versão. Para adicionar uma mensagem personalizada, clique no link.
* Se você não tiver notificado os revisores sobre a versão de prova anterior (por exemplo, nenhum email padrão ou personalizado), a página Nova versão não incluirá nenhuma mensagem por padrão. Para notificar seus revisores sobre a nova versão, clique no link Send a Message. Você pode adicionar um assunto e uma mensagem personalizados clicando no link Adicionar mensagem personalizada.
