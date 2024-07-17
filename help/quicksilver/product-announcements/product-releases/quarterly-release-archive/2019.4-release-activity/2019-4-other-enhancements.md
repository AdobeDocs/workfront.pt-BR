---
content-type: release-notes
navigation-topic: 2019-4-release-activity
title: Outras melhorias do 2019.4
description: Esta página descreve várias melhorias feitas com a versão 2019.4. Ele será disponibilizado no ambiente de Produção na semana de 11 de novembro de 2019.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: ed7488f1-2076-4160-97f3-a3da25cccd0f
source-git-commit: e1bf5fbc7dc25bf8ce472b21b9a0906530f82cf0
workflow-type: tm+mt
source-wordcount: '627'
ht-degree: 0%

---

# Outras melhorias do 2019.4

Esta página descreve várias melhorias feitas com a versão 2019.4. Ele será disponibilizado no ambiente de Produção na semana de 11 de novembro de 2019.

Para obter uma lista de todas as alterações feitas em 2019.4, consulte a [visão geral da versão 2019.4](../../../../product-announcements/product-releases/quarterly-release-archive/2019.4-release-activity/2019-4-release-activity-overview.md).

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td> <strong>Iniciar um fluxo de trabalho de comprovação automatizada de um documento Adobe CC</strong> <p>Sem sair do Adobe CC, você pode iniciar um fluxo de trabalho de prova automatizada para um documento Adobe CC criado. Para obter mais informações, consulte a seção <a href="../../../../documents/workfront-for-adobe-creative-cloud/use-wf-adobe-cc.md#generate" class="MCXref xref" xrefformat="{para}">Gerar uma prova do Illustrator ou do InDesign</a> no artigo <a href="../../../../documents/workfront-for-adobe-creative-cloud/use-wf-adobe-cc.md" class="MCXref xref" xrefformat="{para}">Usar a Extensão do Workfront para o Illustrator e o InDesign</a>.</p> </td> 
  </tr> 
  <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td><strong>Workfront G Suite add-on</strong> <p>Now you can manage Workfront objects directly from Gmail, Google Calendar, and Google Drive.</p> <p>When you open a Workfront notification email, instantly view all information about the associated object and take actions, such as reviewing content or updating a status, without leaving your Inbox.</p> <p>When you open a non-Workfront email:</p> 
     <ul> 
      <li>Convert it into a task or issue.</li> 
      <li>Associate it with a project.</li> 
      <li>Assign it as a work item.</li> 
      <li>Add it to a work item as an update.</li> 
      <li>Upload its attachments to Workfront.</li> 
     </ul> <p>Manage Workfront objects without leaving G Suite:</p> 
     <ul> 
      <li>Post updates and replies to comments.</li> 
      <li>View and manage documents associated with a task or issue.</li> 
     </ul> <p>Access and work with object details:</p> 
     <ul> 
      <li>Read the description</li> 
      <li>View the parent object</li> 
      <li>Change the status</li> 
      <li>Access custom data</li> 
      <li>Mark it as complete.</li> 
     </ul> <p>And access your Workfront Home content, including tasks, issues, approvals, and access requests, without leaving G Suite.</p> <p>For more information, see <a href="../../../../workfront-integrations-and-apps/workfront-for-g-suite/workfront-for-gsuite.md" class="MCXref xref" xrefformat="{para}">Adobe Workfront for G Suite</a>.</p> </td> 
   </tr>
  --> 
  <tr> 
   <td> <strong>Impedir endereços de email duplicados</strong> <p>Não é mais possível usar o mesmo endereço de email ao criar vários usuários no Workfront, mesmo que esses endereços variem de acordo com as letras maiúsculas e minúsculas. Por exemplo, não é possível criar um usuário com o endereço de email JohnDoe@example.com e outro usuário com o endereço de email johndoe@example.com. </p> <p>Antes dessa alteração, era compatível criar usuários com endereços de email correspondentes que diferiam somente por maiúsculas e minúsculas. </p> <p>Observação: os usuários existentes com endereços de email correspondentes que diferem apenas em maiúsculas e minúsculas precisarão ser atualizados em uma data futura. Se você tiver usuários em uma instância do Workfront com endereços de email correspondentes que diferem apenas por letras maiúsculas e minúsculas, a Workfront entrará em contato com você com informações adicionais e uma linha do tempo quando eles precisarem ser atualizados.</p> </td> 
  </tr> 
  <tr> 
   <td> 
    <div> 
     <strong>Tipos de objetos adicionais disponíveis para campos de Digitação antecipada em um formulário personalizado</strong> 
     <p>Agora, ao criar um campo personalizado Digitação antecipada, você pode associar os seguintes tipos de objetos ao campo: Usuário, Empresa, Grupo, Função de trabalho, Portfolio, Programa, Projeto e Modelo.</p> 
     <p>Anteriormente, só era possível associar o tipo de objeto Usuário a um campo personalizado Digitação antecipada.</p> 
     <p>Para obter mais informações, consulte a seção <a href="../../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md#create" class="MCXref xref" xrefformat="{para}">Criar ou editar um formulário personalizado</a> no artigo <a href="../../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref" xrefformat="{para}">Criar ou editar um formulário personalizado</a>.</p> 
    </div> </td> 
  </tr> 
  <tr> 
   <td> <strong>Nome do arquivo da última versão de um documento exibido</strong> <p>Agora, ao fazer upload de uma versão do documento com um nome de arquivo diferente do nome da versão existente, o novo nome de arquivo é exibido no Workfront.</p> <p>Anteriormente, ao adicionar uma nova versão com um nome de arquivo diferente, o nome do arquivo da versão anterior continuava a ser exibido no Workfront.</p> <p>Para obter mais informações, consulte <a href="../../../../documents/managing-documents/upload-new-document-version.md" class="MCXref xref" xrefformat="{para}">Carregar uma nova versão de um documento</a>.</p> </td> 
  </tr> 
  <tr> 
   <td> <strong>Adicionar um filtro a um campo Digitação antecipada em um formulário personalizado</strong> <p>Agora, ao adicionar um campo Digitação antecipada a um formulário personalizado, você pode adicionar um filtro para limitar os objetos que estão disponíveis quando alguém usa o campo. Por exemplo, é possível limitar o campo para que o usuário possa selecionar apenas os membros das equipes de Marketing e Vendas na organização.</p> <p>Para obter mais informações, consulte a seção Criar e adicionar um novo campo no artigo Criação de Forms personalizado.</p> </td> 
  </tr> 
  <tr> 
   <td> 
    <div> 
     <strong>Alterar o tipo de exibição de um campo em um formulário personalizado</strong> 
     <p>Agora é possível alterar o tipo de exibição de um campo em um formulário personalizado.</p> 
     <p>Por exemplo, se você criou um campo Checkboxes, é possível alterá-lo para um campo Suspenso ou um campo Radio Buttons. Esses três tipos de exibição de campo são intercambiáveis.</p> 
     <p>Ou, se você tiver criado um Campo de texto de linha única, poderá alterá-lo para um campo de texto de parágrafo. Esses dois tipos de exibição de campo são intercambiáveis.</p> 
     <p>Anteriormente, para alterar o tipo de exibição de um campo personalizado, era necessário criar um novo campo e excluir o antigo. Isso exigia a transferência de dados, o que geralmente era demorado.</p> 
     <p>Para obter mais informações, consulte <a href="../../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md#create" class="MCXref xref" xrefformat="{para}">Criar ou editar um formulário personalizado</a> no artigo <a href="../../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref" xrefformat="{para}">Criar ou editar um formulário personalizado</a></p> 
    </div> </td> 
  </tr> 
  <tr> 
   <td> 
    <div> 
     <strong>Criar calendários e relatórios de folga</strong> 
     <p>Agora você pode ver a folga do usuário para melhorar o planejamento e a execução. Você também pode adicionar novos relatórios e calendários de folga aos seus painéis para obter uma visualização em tempo real da disponibilidade do usuário.</p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>
