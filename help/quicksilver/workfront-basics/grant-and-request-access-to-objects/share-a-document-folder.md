---
product-area: projects
navigation-topic: grant-and-request-access-to-objects
title: Compartilhar uma pasta de documentos
description: Você pode compartilhar uma pasta e seu conteúdo na área Documentos.
author: Alina
feature: Get Started with Workfront
exl-id: c0d318a8-b1cf-4522-b478-acf092687658
source-git-commit: 4ae96f67b15838403ffce32317d871d6904d6d95
workflow-type: tm+mt
source-wordcount: '854'
ht-degree: 0%

---

# Compartilhar uma pasta de documentos

Você pode compartilhar uma pasta e seu conteúdo na área Documentos.

>[!NOTE]
>
>* A pasta deve estar nos cinco níveis superiores de uma hierarquia de pastas em um objeto. Cada pasta no sexto nível ou abaixo herda suas configurações de compartilhamento da pasta diretamente acima dela.
>
>  Para obter informações sobre como adicionar subpastas para criar uma hierarquia de pastas, consulte a seção [Criar pastas e subpastas](../../documents/organizing-documents/create-documents-folder.md#creating-folders) no artigo [Criar pastas de documentos](../../documents/organizing-documents/create-documents-folder.md).
>
>* As pastas inteligentes não podem ser compartilhadas.
>* Se você configurar opções de compartilhamento para uma pasta de documentos em um modelo e alguém criar um projeto a partir desse modelo, suas configurações de compartilhamento não serão transferidas para a pasta de documentos no novo projeto.
>* Se você configurar opções de compartilhamento para uma pasta de documentos em um item de trabalho e, em seguida, copiar o item de trabalho, suas configurações de compartilhamento não serão transferidas para a pasta de documentos no novo item de trabalho.
>

## Requisitos de acesso

<!--drafted for P&P
(I am putting Contributor and higher here because this is what I found in testing. Normally, Review equals Light but I found out that Contributor can also have manage rights to documents and can share them.)

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Contributor or higher</p> 
   Or
   <p>Legacy license: Review or higher</p>
      </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>View access to Documents</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View access to an object</p> <p>For information on requesting additional access, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->
+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacote do Adobe Workfront</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td> <p>Leve ou superior</p> 
   <p>Revisar ou superior</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Visualizar acesso a documentos</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Visualizar o acesso a um objeto</p>  </td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Compartilhar uma pasta

1. Clique no ícone **do** Menu principal![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront e em **Documentos**.

   Ou

   Com um objeto do Workfront aberto, clique em **Documentos** no painel esquerdo.

1. Selecione a pasta e clique no ícone Compartilhar ![](assets/share-icon.png) na barra de ferramentas.

   A pasta deve estar nos cinco níveis superiores de uma hierarquia de pastas em um objeto e não pode ser uma pasta inteligente.

1. Na caixa exibida, em **Conceder acesso à pasta**, comece digitando o nome do usuário, da equipe, da função de trabalho, do grupo ou da empresa com a qual deseja compartilhar a pasta e pressione **Enter** quando o nome for exibido.
1. Para ajustar o acesso do usuário, equipe, função de trabalho, grupo ou empresa que você acabou de adicionar, clique no menu suspenso à direita do nome e configure uma das seguintes opções disponíveis e qualquer uma de suas configurações avançadas:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Visualizar o projeto</td> 
      <td> <p>Capacidade de visualizar a pasta e seu conteúdo.</p> <p>Clique em <strong>Configurações Avançadas</strong> para especificar se deseja permitir o seguinte:</p> 
       <ul> 
        <li><strong>Download</strong>: capacidade de baixar a pasta e seu conteúdo como um arquivo ZIP</li> 
        <li> <p><strong>Compartilhar</strong>: capacidade de compartilhar a pasta com outras pessoas no sistema</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Gerenciar o projeto</td> 
      <td> <p>Capacidade de exibir e editar a pasta e seu conteúdo</p> <p>Clique em <strong>Configurações Avançadas</strong> para especificar se você deseja permitir que os usuários façam o seguinte:</p> 
       <ul> 
        <li><strong>Excluir</strong>: excluir a pasta e seu conteúdo do sistema</li> 
        <li><b>Baixar</b>: baixe a pasta e seu conteúdo como um arquivo ZIP</li> 
        <li><strong>Compartilhar</strong>: compartilhar a pasta e seu conteúdo com outros usuários no sistema</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Opcional) Repita as etapas 3 a 4 para adicionar outros nomes à lista e configurar suas opções.
1. (Opcional) Se quiser que todos no sistema possam ver a pasta e seu conteúdo, clique no ícone de engrenagem ![](assets/gear-icon-settings-with-dn-arrow.jpg) no canto superior direito da caixa de compartilhamento e clique em **Tornar isso visível em todo o sistema.**

   Se mudar de ideia, clique em **Remover acesso a todo o sistema** (a opção padrão).

## Como os usuários acessam o conteúdo de uma pasta compartilhada com eles

<!--
<p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Delete these 2 paragraphs when the story &nbsp;<a href="https://hub.workfront.com/task/622f8d6f000897c9a4a11bdfd9b2cf34/overview">Handle email notification content when a folder is shared</a> goes to Preview:</p>
-->

Atualmente, quando você compartilha uma pasta, seus destinatários não veem a pasta na área Documentos. No entanto, eles podem acessar seus documentos executando um relatório de documento.

Para obter informações sobre como executar um relatório, consulte a seção [Relatório sobre objetos](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#reporting-on-objects) no artigo [Entender objetos no Adobe Workfront](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md). Consulte também [Criar um relatório personalizado](../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

<!--
<div class="preview" data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>Workfront sends a notification email when someone shares a document folder on an object with a user or a team. To access the folder from the email, recipients can click the folder title or the "See it in Workfront" link.</p> <note type="note">
<ul class="preview">
<li> <p>The email notification "Someone shares an object with me" or "Someone shares an object with my team" must be enabled in order for a user or team to receive a notification email about a shared folder.</p> </li>
<li> <p>When someone shares a document folder from the global Documents area, the links in the notification email take the recipient to the global Documents area. Because folders in this area are private, the shared folder is not displayed there, but the recipient can access its documents by creating a document report. </p> <p>For information about running a report, see the section <a href="../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#reporting-on-objects" class="MCXref xref">Report on objects</a> in the article <a href="../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md" class="MCXref xref">Understand objects in Adobe Workfront</a>. Also see <a href="../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">Create a custom report</a>.</p> </li>
<li> <p>Currently, it is not possible to share folders with external users.</p> </li>
</ul>
</note>
</div>
-->

## Permissões herdadas ao compartilhar um objeto que contém uma pasta

Quando você compartilha um objeto que tem uma pasta de documentos, os recipients também obtêm acesso à pasta:

* Se você conceder aos seus recipients o acesso de Visualização ao objeto principal, eles terão acesso de Visualização à pasta.
* Se você conceder aos seus destinatários acesso ao Contribute ou ao Manage para o objeto principal, eles terão acesso ao Manage para a pasta.
* Se você conceder um tipo de acesso (Exibir, Contribute ou Gerenciar) ao objeto pai e outro tipo à pasta, os destinatários terão o maior desses dois tipos de acesso aos documentos da pasta

  Por exemplo, se você compartilhar o objeto pai com acesso de Visualização e a pasta com acesso de Gerenciar, os destinatários terão acesso de Gerenciar aos documentos na pasta.

  >[!NOTE]
  >
  >Um documento anexado herda permissões somente do objeto ao qual foi anexado. Se você criar uma pasta no objeto e mover o documento para a pasta, ela herdará as permissões da pasta. Porém, se você criar uma pasta em um objeto pai ou avô e mover o documento para essa pasta, ele não herdará as permissões dessa pasta.

* Se a opção &quot;Nunca herdar acesso a documentos de projetos, tarefas, problemas etc.&quot; estiver habilitada no nível de acesso do recipient, eles não herdarão permissões para documentos em uma pasta que você compartilha com eles. Para conceder a eles acesso a um documento na pasta, você deve compartilhar o documento.

  Para obter informações sobre a opção &quot;Nunca herdar&quot;, consulte [Configurar acesso ao Adobe Workfront](../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md).

  Para obter informações sobre como compartilhar um documento, consulte [Compartilhar um documento](../../workfront-basics/grant-and-request-access-to-objects/document-permissions.md).
