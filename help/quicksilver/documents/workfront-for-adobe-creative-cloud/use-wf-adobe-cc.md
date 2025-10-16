---
product-area: documents;workfront-integrations
navigation-topic: workfront-for-adobe-creative-cloud
title: Usar a extensão do Workfront para Illustrator e InDesign
description: Você pode usar a extensão Workfront para exportar conteúdo digital salvo e criado no Adobe Illustrator e Adobe InDesign para o Workfront. Isso acelera o processo de revisão e aprovação de documentos.
author: Courtney
feature: Workfront Integrations and Apps, Digital Content and Documents
exl-id: 40945eac-e8de-42af-b6ba-f3082c208e02
source-git-commit: 3f9a824780f2ded914d461a473aef3b6ecfa8701
workflow-type: tm+mt
source-wordcount: '3069'
ht-degree: 0%

---

# Usar a extensão do Workfront para Illustrator e InDesign

<!--Audited: 01/2024-->

>[!IMPORTANT]
>
>Estamos substituindo a extensão do Workfront para Illustrator e InDesign por [plug-ins atualizados do Creative Cloud](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-cc-install-toc.md). A partir do final de 2022, essa extensão não será mais suportada e estará disponível como está.

Você pode usar a extensão Workfront para exportar conteúdo digital salvo e criado no Adobe Illustrator e Adobe InDesign para o Workfront. Isso acelera o processo de revisão e aprovação de documentos.

A extensão do Workfront é compatível com o Adobe Creative Cloud 2017 e mais recente nos seguintes aplicativos:

* InDesign
* Illustrator
* Photoshop

  >[!NOTE]
  >
  >Recomendamos usar o novo plug-in [Adobe Workfront para Photoshop](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-cc-install-ps.md).

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacote do Adobe Workfront</td> 
   <td> <p>Qualquer</p>
 </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td> 
      <p>Standard</p> 
   <p>Trabalhar ou superior</p>
</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produtos adicionais</td> 
   <td>Você deve ter uma licença do Adobe Creative Cloud além de uma licença do Workfront.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Edite o acesso ao objeto com o qual você deseja interagir.</p>  </td> 
  </tr> 
 </tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Faça logon na extensão Workfront a partir do Illustrator ou InDesign {#log-in-to-workfront-extension-from-illustrator-or-indesign}

Ao fazer logon no Workfront a partir de um dos aplicativos compatíveis da Adobe, você é conectado a todos os aplicativos compatíveis da Adobe.

1. Vá para o aplicativo do Adobe onde deseja usar a extensão do Workfront.

   Para obter uma lista de formatos com suporte para cada aplicativo, consulte [Formatos de arquivo exportados com suporte](#supported-exported-file-formats) neste artigo.

1. Clique em **Janela** > **Extensões** > Workfront.

1. (Opcional) Arraste o painel Workfront até a posição em que deseja exibi-lo no aplicativo do Adobe.
1. Siga as instruções para fazer logon no Workfront.

   >[!NOTE]
   >
   >* O Workfront se conecta ao Adobe Creative Cloud usando o OAuth 2.0, um padrão seguro usado pela maioria das integrações baseadas na Web para a autenticação e autorização dos usuários.
   >* Quando for solicitado que você insira o [domínio ou host] de sua conta do Workfront, digite-o usando este formato:`yourCompany'sDomain.my.workfront.com`. O domínio da sua empresa geralmente é o nome da sua empresa.

   Uma lista de itens de trabalho atribuídos a você é exibida se o projeto tiver um status atual. Se uma lista não for exibida, faça logon no Workfront.

   As tarefas pessoais estão listadas em **Nenhum projeto**.

## Fazer upload de um arquivo para um projeto, tarefa ou problema do Workfront {#upload-a-file-to-a-workfront-project-task-or-issue}

Você pode fazer upload de um arquivo do sistema de arquivos do seu computador ou exportar um arquivo atualmente aberto em um aplicativo do Adobe Creative Cloud para um projeto, tarefa ou problema do Workfront. 

Considere o seguinte ao fazer upload ou exportar um arquivo do Adobe Creative Cloud:

* Seu nível de acesso deve permitir o upload de documentos para o Workfront. Para obter mais informações, consulte [Conceder acesso a documentos](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-documents.md).
* Você deve ter permissões para carregar documentos no item em que deseja carregá-los. Para obter mais informações, consulte [Visão geral das permissões de compartilhamento em objetos](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).
* O arquivo é carregado na área Documentos para o objeto Workfront selecionado.
* Não é possível exportar um documento para a área Documentos do ![ícone Menu Principal](assets/main-menu-icon.png) de um aplicativo do Adobe Creative Cloud.

As seções a seguir explicam o seguinte:

* [Carregar um arquivo](#upload-a-file)
* [Exportar um arquivo atualmente aberto no Illustrator ou no InDesign](#export-a-file-currently-open-in-illustrator-or-indesign)
* [Fazer upload de uma nova versão de um arquivo do Illustrator ou InDesign](#upload-a-new-version-of-a-file-from-illustrator-or-indesign)

### Carregar um arquivo {#upload-a-file}

Você pode fazer upload de arquivos para um projeto, tarefa ou problema sem sair do aplicativo do Adobe Creative Cloud.

1. Se você não vir a extensão do Workfront ao abrir o aplicativo do Adobe Creative Cloud, clique em **Janela** > **Extensões** > **Workfront**.

   Uma lista de itens de trabalho atribuídos a você é exibida se o projeto estiver em um status atual. Se uma lista não for exibida, faça logon no Workfront.

   As tarefas pessoais estão listadas em **Nenhum projeto**.

1. Clique no nome do projeto, tarefa ou problema para o qual deseja fazer upload do arquivo.

   Você pode pesquisar digitando o nome na caixa **Pesquisar** e selecionando **Projeto**, **Tarefa** ou **Problema** no menu suspenso à direita da caixa **Pesquisar**. Se o nome do item de trabalho não aparecer na lista, pressione **Enter** para pesquisar todos os itens de Workfront aos quais você tem acesso para visualizar.

1. Clique em **Selecionar** no canto inferior direito da extensão do Workfront.
1. No menu suspenso **Clique para selecionar o formato**, clique no formato no qual deseja salvar o arquivo no Workfront.

   Para obter uma lista de formatos com suporte para cada aplicativo, consulte [Formatos de arquivo exportados com suporte](#supported-exported-file-formats) neste artigo.

1. (Condicional) Se o item de trabalho no qual você deseja carregar o arquivo tiver pastas de documentos, selecione uma pasta de documentos no campo **Clique para selecionar uma pasta de documentos** e clique em **Selecionar**.

1. Clique em **Carregar um arquivo local**.
1. Na caixa **Abrir Arquivo**, localize o arquivo em seu sistema de arquivos e clique em **Abrir**.

1. (Opcional) Digite um novo nome para o arquivo.

   ![Renomear arquivo](assets/rename-file-uploading.png)

1. Clique em **Carregar**.

   No Workfront, o documento agora está listado na área Documentos do projeto, tarefa ou problema selecionado.

1. (Opcional) Clique no nome do documento para abrir sua página Detalhes do documento no Workfront.

   O Workfront é aberto em uma nova guia do navegador.

### Exportar um arquivo aberto no momento no Illustrator ou no InDesign {#export-a-file-currently-open-in-illustrator-or-indesign}

1. Em um aplicativo Adobe Creative Cloud compatível, abra um arquivo que gostaria de exportar para o Workfront.
1. Se a extensão do Workfront não for exibida, clique em **Janela** > **Extensões** > **Workfront**.

   Uma lista de itens de trabalho atribuídos a você é exibida se o projeto estiver em um status atual. Se uma lista não for exibida, faça logon no Workfront.

   As tarefas pessoais estão listadas em **Nenhum projeto**.

1. Clique no nome do projeto, tarefa ou problema para o qual deseja exportar o arquivo.

   Você pode pesquisar digitando o nome na caixa **Pesquisar** e selecionando **Projeto**, **Tarefa** ou **Problema** no menu suspenso à direita da caixa **Pesquisar**. Se o nome do item de trabalho não aparecer na lista, pressione **Enter** para pesquisar todos os itens de Workfront aos quais você tem acesso para visualizar.

1. No menu suspenso **Clique para selecionar o formato**, clique no formato no qual deseja salvar o arquivo no Workfront.

   Para obter uma lista de formatos com suporte para cada aplicativo, consulte [Formatos de arquivo exportados com suporte](#supported-exported-file-formats) neste artigo.

1. (Condicional) Se o item de trabalho no qual você deseja carregar o arquivo tiver pastas de documentos, selecione uma pasta de documentos no campo **Clique para selecionar uma pasta de documentos** e clique em **Selecionar**.
1. (Opcional) Para renomear o documento, clique no nome do documento e digite um novo nome.

   ![Renomear documento ao exportar](assets/rename-doc-exporting.png)

1. Clique em **Exportar**.

   Uma mensagem é exibida para confirmar que o documento foi exportado com êxito para o Workfront.

   No Workfront, o documento é listado na área Documentos do objeto especificado no Workfront.

1. (Opcional) Clique no nome do documento para acessá-lo no Workfront.

   ![adobe_document_with_name_highlight.PNG](assets/adobe-document-with-name-highlight-350x251.png)

   O Workfront é aberto em uma nova guia do navegador.

### Fazer upload de uma nova versão de um arquivo do Illustrator ou InDesign {#upload-a-new-version-of-a-file-from-illustrator-or-indesign}

1. Se quiser exportar um arquivo em que está trabalhando em um aplicativo Adobe compatível como uma nova versão de um arquivo no Workfront, abra o arquivo no aplicativo Adobe.
1. Se a extensão do Workfront não for exibida, clique em **Janela** > **Extensões** > **Workfront**.

   Uma lista de itens de trabalho atribuídos a você é exibida se o projeto tiver um status atual. Se uma lista não for exibida, faça logon no Workfront.

   As tarefas pessoais estão listadas em **Nenhum projeto**.

1. Clique no nome do projeto, tarefa ou problema onde o documento existente está listado.

   Você pode pesquisar digitando o nome na caixa **Pesquisar** e selecionando **Projeto**, **Tarefa** ou **Problema** no menu suspenso à direita da caixa **Pesquisar**. Se o nome do item de trabalho não aparecer na lista, pressione **Enter** para pesquisar todos os itens de Workfront aos quais você tem acesso para visualizar.

   Todos os documentos carregados para projetos, tarefas ou problemas são exibidos em uma lista, independentemente de terem sido carregados por meio do aplicativo do Adobe.

1. No menu suspenso **Clique para selecionar o formato**, clique no formato no qual deseja salvar o arquivo no Workfront.

   Isso é necessário se estiver exportando um arquivo aberto no aplicativo do Adobe. Para obter uma lista de formatos com suporte para cada aplicativo, consulte [Formatos de arquivo exportados com suporte](#supported-exported-file-formats) neste artigo.

1. Se estiver exportando um arquivo aberto no aplicativo Adobe como uma nova versão do documento Workfront selecionado, clique em **Exportar**.

   Ou

   Para carregar um arquivo do sistema de arquivos do seu computador como uma nova versão do documento do Workfront selecionado, clique em **Carregar um arquivo local**, localize o arquivo na caixa exibida, clique em **Abrir** e em **Carregar**.

1. (Opcional) Clique no nome do documento para ver sua nova versão no Workfront.

   >[!NOTE]
   >
   >O nome do documento no Workfront é preenchido por padrão e não pode ser editado. Além disso, não altera o nome do arquivo que você carrega ou exporta como uma nova versão.
   >
   >
   >![O nome do documento não pode ser alterado](assets/doc-name-cant-be-changed.png)

## Comentar em um documento do Workfront no Illustrator ou InDesign {#comment-on-a-workfront-document-from-illustrator-or-indesign}

Você pode adicionar comentários diretamente a um documento do Workfront em um aplicativo do Adobe. No Workfront, os comentários são exibidos na área Atualizações do documento e na área Atualizações para o item do Workfront em que o documento foi salvo.

1. Abra um dos aplicativos Adobe compatíveis.
1. Se a extensão do Workfront não for exibida, clique em **Janela** > **Extensões** > **Workfront**.

   Uma lista de itens de trabalho atribuídos a você é exibida se o projeto tiver um status atual. Se uma lista não for exibida, faça logon no Workfront.

   As tarefas pessoais estão listadas em **Nenhum projeto**.

1. Clique no projeto, tarefa ou problema onde o documento existente está listado.

   Você pode pesquisar digitando o nome na caixa **Pesquisar** e selecionando **Projeto**, **Tarefa** ou **Problema** no menu suspenso à direita da caixa **Pesquisar**. Se o nome do item de trabalho não aparecer na lista, pressione **Enter** para pesquisar todos os itens de Workfront aos quais você tem acesso para visualizar.

1. Clique no nome do documento existente e em **Selecionar** no canto inferior direito da extensão do Workfront.
1. Clique na guia **Comentário** e digite sua atualização na caixa.

1. (Opcional) Para incluir outros usuários ou equipes do Workfront no comentário, comece digitando o nome de um usuário ou equipe na caixa **Notificar pessoas ou equipes** e, em seguida, clique no nome quando ele aparecer na lista suspensa.
1. (Opcional) Para solicitar aprovação no documento, selecione **Fazer uma solicitação de aprovação**.
1. Clique **Atualizar**.

   Uma atualização é postada na guia Atualizações do documento. Os usuários do Workfront incluídos no comentário recebem uma notificação no aplicativo e, dependendo de como o Workfront é configurado, também podem receber uma notificação por email.

   Para obter mais informações sobre notificações no Workfront, consulte [Exibir e gerenciar notificações no aplicativo](../../workfront-basics/using-notifications/view-and-manage-in-app-notifications.md).

   Para obter mais informações sobre como receber notificações por email, consulte [notificações do Adobe Workfront](../../workfront-basics/using-notifications/wf-notifications.md).

## Solicitar uma aprovação de documento do Illustrator ou do InDesign

Você pode solicitar uma aprovação de documento do Workfront diretamente de um aplicativo do Adobe.

Você pode solicitar uma aprovação de documento às seguintes entidades:

* Um usuário do Workfront
* Um usuário externo sem uma conta do Workfront

Você pode solicitar uma aprovação em um documento de um aplicativo do Adobe das seguintes maneiras:

* Anexando um aprovador ao documento.
* Ao comentar em um documento, notificar a pessoa quando você fizer um comentário e anexá-lo como um aprovador do documento.

  Para obter informações sobre como solicitar uma aprovação ao comentar em um documento, consulte a seção [Comentar em um documento do Workfront do Illustrator ou do InDesign](#comment-on-a-workfront-document-from-illustrator-or-indesign) neste artigo.

Para solicitar uma aprovação em um documento de um aplicativo do Adobe:

1. Abra um dos aplicativos Adobe compatíveis.
1. Se a extensão do Workfront não for exibida, clique em **Janela** > **Extensões** > **Workfront**.

   Uma lista de itens de trabalho atribuídos a você é exibida se o projeto tiver um status atual. Se uma lista não for exibida, faça logon no Workfront.

   As tarefas pessoais estão listadas em **Nenhum projeto**.

1. Clique no projeto, tarefa ou problema em que o documento existente está listado e clique no nome do documento existente.

   Você pode pesquisar digitando o nome na caixa **Pesquisar** e selecionando **Projeto**, **Tarefa** ou **Problema** no menu suspenso à direita da caixa **Pesquisar**. Se o nome do item de trabalho não aparecer na lista, pressione **Enter** para pesquisar todos os itens de Workfront aos quais você tem acesso para visualizar.

1. Clique no nome do documento existente e em **Selecionar** no canto inferior direito da extensão do Workfront.
1. Clique na guia **Aprovação**.
1. Para adicionar um aprovador, na **caixa de nome de Comece a digitar**, siga um destes procedimentos:

   * Digite o nome de um aprovador e selecione-o quando ele for exibido na lista.

     ![Adicionar um aprovador de documento](assets/adobe-cc-adding-a-doc-approver-350x189.png)

   * Digite o endereço de email de um usuário externo.

1. Clique em **Solicitar Aprovação**.

   Os usuários do Workfront incluídos no comentário ou adicionados como aprovadores recebem uma notificação no aplicativo e, dependendo de como o Workfront é configurado, também podem receber uma notificação por email.\
   Os usuários externos recebem uma notificação por email de onde podem tomar uma decisão sobre a aprovação.

   Para obter informações sobre notificações no Workfront, consulte [Exibir e gerenciar notificações no aplicativo](../../workfront-basics/using-notifications/view-and-manage-in-app-notifications.md). Para obter informações sobre como receber notificações por email, consulte [notificações do Adobe Workfront](../../workfront-basics/using-notifications/wf-notifications.md).

## Gerar uma prova pelo Illustrator ou InDesign {#generate-a-proof-from-illustrator-or-indesign}

Se sua organização usar modelos de fluxo de trabalho automatizado, você poderá gerar uma prova para um documento criado em um aplicativo do Adobe sem sair do aplicativo. Para obter informações sobre como criar provas, consulte [Criar provas](../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-proofs-in-wf.md). Para obter informações sobre modelos de Fluxo de Trabalho Automatizado, consulte [modelos de Fluxo de Trabalho Automatizado](../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md#automate) na [visão geral do Fluxo de Trabalho Automatizado](../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md).

1. Abra um dos aplicativos Adobe compatíveis.
1. Se a extensão do Workfront não for exibida, clique em **Janela** > **Extensões** > Workfront.

   Uma lista de itens de trabalho atribuídos a você é exibida se o projeto tiver um status atual. Se uma lista não for exibida, faça logon no Workfront.

   As tarefas pessoais estão listadas em **Nenhum projeto**.

1. Se o documento já tiver sido carregado para o Workfront, selecione o projeto, tarefa ou problema na extensão do Workfront em que o documento está listado e clique no nome do documento.

   Ou

   Carregue um documento do Adobe para um objeto do Workfront, conforme descrito na seção [Carregue um arquivo para um projeto, tarefa ou problema do Workfront](#upload-a-file-to-a-workfront-project-task-or-issue) neste artigo, em seguida, clique no nome do documento.

1. No menu suspenso **Clique para selecionar o formato**, clique no formato no qual deseja salvar o arquivo no Workfront.

   Alguns formatos não estão disponíveis depois de habilitar a funcionalidade de prova na etapa seguinte a este. Para obter mais informações, consulte [Formatos de arquivo exportados com suporte](#supported-exported-file-formats) neste artigo.

1. Clique em **Carregar como uma nova prova** para habilitá-la.
1. Selecione o **Modelo de Fluxo de Trabalho** que você deseja que as pessoas usem ao revisar o documento.

   O administrador do Workfront configura os modelos de Fluxo de Trabalho Automatizado, conforme descrito em [Criar e gerenciar modelos de Fluxo de Trabalho Automatizado](/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/create-manage-automated-workflow-templates.md). Consulte o administrador se tiver dúvidas.

   1. Adicione pelo menos um **Novo destinatário** a cada estágio no Modelo de Fluxo de Trabalho.

      Você pode começar a digitar um nome e selecioná-lo quando o vir na lista suspensa exibida.

   1. Especifique a **função de prova** e a frequência de **alertas de email** para cada destinatário adicionado.

   1. (Opcional) Na seção **Notificação por email**, selecione se deseja enviar uma notificação por email com uma mensagem personalizada opcional sobre a prova para todos os destinatários de prova adicionados.

1. Clique em **Criar prova**.

   É possível visualizar o progresso do processo de criação de prova. Um alerta é exibido quando a geração é concluída. É possível abrir a tarefa em que você criou a prova e ela está listada lá.

## Fazer upload de uma nova versão de uma prova sem sair do Illustrator ou do InDesign

1. Clique em um documento existente que tenha uma prova e em **Selecionar** no canto inferior direito.
1. Clique em **Carregar como uma nova versão de prova** para habilitá-la.
1. (Opcional) Selecione o **Modelo de fluxo de trabalho** que você deseja que as pessoas usem ao revisar a nova versão.

   Se você não selecionar um modelo diferente, o modelo selecionado para a versão anterior permanecerá em vigor. Além disso, se você tiver modificado o modelo para a versão anterior, as alterações estarão em vigor para a nova versão.

   O administrador do Workfront configura os modelos de Fluxo de Trabalho Automatizado, conforme descrito em [Criar e gerenciar modelos de Fluxo de Trabalho Automatizado](/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/create-manage-automated-workflow-templates.md). Consulte o administrador se tiver dúvidas.

   1. Adicione pelo menos um **Novo destinatário** a cada estágio no Modelo de Fluxo de Trabalho.

      Você pode começar a digitar um nome e selecioná-lo quando o vir na lista suspensa exibida.

   1. Especifique a **função de prova** e a frequência de **alertas de email** para cada destinatário adicionado.
   1. (Opcional) Na seção **Notificação por email**, selecione se deseja enviar uma notificação por email com uma mensagem personalizada opcional sobre a prova para todos os destinatários de prova adicionados.

1. Clique em **Criar nova versão de prova**.

   É possível visualizar o progresso do processo de criação de prova. Um alerta é exibido quando a geração é concluída. É possível abrir a tarefa em que você criou a prova e ela está listada lá.

## Faça logout da extensão do Workfront

1. No aplicativo Adobe, clique em **Janela** > **Extensões** > **Workfront**.

1. Clique no menu **Mais** ![Mais menu](assets/more-menu.png) no canto superior direito do painel.

1. (Opcional) Clique em **Feedback** para abrir uma breve pesquisa e enviar à Workfront seus comentários sobre o Workfront para Adobe Creative Cloud.
1. Clique em **Logout**.\
   A tela Login (Login) é exibida. Para obter informações sobre como fazer logon, consulte [Fazer logon na extensão do Workfront da Illustrator ou do InDesign](#log-in-to-workfront-extension-from-illustrator-or-indesign) neste artigo.

## Formatos de arquivo exportados com suporte {#supported-exported-file-formats}

* [Formatos de Arquivo Exportados com Suporte para o Adobe InDesign](#supported-exported-file-formats-for-adobe-indesign)
* [Formatos de arquivo exportados compatíveis com o Adobe Illustrator](#supported-exported-file-formats-for-adobe-illustrator)

### Formatos de arquivo exportados com suporte para o Adobe InDesign  {#supported-exported-file-formats-for-adobe-indesign}

O Workfront é compatível com os seguintes formatos de arquivo para exportar arquivos do InDesign para o Workfront:

* EPS - PostScript encapsulado
* EPUB - Publicação eletrônica de layout fixo
* EPUB - Publicação eletrônica refluível &#42;
* HTML - Linguagem de marcação de hipertexto
* IDML - Linguagem de marcação do InDesign &#42;
* JPG, JPEG - Grupo conjunto de especialistas em fotografia
* PDF - Arquivo de documento portátil Adobe
* PNG - Portable Network Graphics
* SWF - Flash Player &#42;
* XML - Linguagem de Marcação Extensível &#42;

&#42; Este formato de arquivo não está disponível quando **Carregar uma nova prova** está habilitado (para obter informações sobre esta opção, consulte [Gerar uma prova do Illustrator ou do InDesign](#generate-a-proof-from-illustrator-or-indesign) neste artigo). Se este formato de arquivo já estiver selecionado antes de habilitar **Carregar uma nova prova**, o sistema alterará o formato de arquivo para PDF. Você pode selecionar um formato diferente na lista.

### Formatos de arquivo exportados compatíveis com o Adobe Illustrator  {#supported-exported-file-formats-for-adobe-illustrator}

O Workfront é compatível com os seguintes formatos de arquivo para exportar arquivos do Illustrator para o Workfront:

* DWG - Desenho do AutoCAD, Arquivo de Intercâmbio do AutoCAD &#42;
* JPG, JPEG - Grupo conjunto de especialistas em fotografia
* PNG - Portable Network Graphics
* PSD - Documento Photoshop
* SWF - Flash Player &#42;
* TIFF - Formato de arquivo de imagem marcado

&#42; Este formato de arquivo não está disponível quando **Carregar uma nova prova** está habilitado (para obter informações sobre esta opção, consulte [Gerar uma prova do Illustrator ou do InDesign](#generate-a-proof-from-illustrator-or-indesign) neste artigo). Se esse formato de arquivo já estiver selecionado antes de você habilitar **Carregar uma nova prova**, o sistema alterará o formato de arquivo para PNG. Você pode selecionar um formato diferente na lista.
