---
product-area: documents;workfront-integrations
navigation-topic: workfront-for-adobe-creative-cloud
title: Usar a extensão Workfront para Illustrator e InDesign
description: Você pode usar a Extensão do Workfront para exportar conteúdo digital salvo e criado no Adobe Illustrator e Adobe InDesign para o Workfront. Isso acelera o processo de revisão e aprovação de documentos.
author: Courtney
feature: Workfront Integrations and Apps, Digital Content and Documents
exl-id: 40945eac-e8de-42af-b6ba-f3082c208e02
source-git-commit: 147a5b5d508e1ea01d18d981f9157439a643cf55
workflow-type: tm+mt
source-wordcount: '3056'
ht-degree: 0%

---

# Usar a extensão Workfront para Illustrator e InDesign

>[!IMPORTANT]
>
>Estamos substituindo a extensão Workfront para Illustrator e InDesign por [plugins Creative Cloud atualizados](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-cc-install-toc.md). A partir do final de 2022, essa extensão não será mais suportada e estará disponível como está.


Você pode usar a Extensão do Workfront para exportar conteúdo digital salvo e criado no Adobe Illustrator e Adobe InDesign para o Workfront. Isso acelera o processo de revisão e aprovação de documentos.

A extensão Workfront é compatível com o Adobe Creative Cloud 2017 e mais recente nos seguintes aplicativos:

* InDesign
* Illustrator
* Photoshop

   >[!NOTE]
   >
   >Recomendamos usar o novo [Adobe Workfront para Photoshop](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-cc-install-ps.md) plug-in.

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plano Adobe Workfront*</td> 
   <td> <p>Pro ou superior</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Trabalho ou superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produto</td> 
   <td>Você deve ter uma licença da Adobe Creative Cloud além de uma licença da Workfront.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Edite o acesso ao objeto com o qual deseja interagir.</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

## Faça logon na extensão do Workfront a partir do Illustrator ou InDesign {#log-in-to-workfront-extension-from-illustrator-or-indesign}

Ao fazer logon no Workfront a partir de um dos aplicativos do Adobe suportados, você faz logon em todos os aplicativos do Adobe suportados.

1. Vá para o aplicativo Adobe, onde deseja usar a extensão Workfront.

   Para obter uma lista de formatos compatíveis para cada aplicativo suportado, consulte [Formatos de arquivo exportados suportados](#supported-exported-file-formats) neste artigo.

1. Clique em **Window** > **Extensões** > Workfront.

1. (Opcional) Arraste o painel Workfront até a posição desejada no aplicativo Adobe.
1. Siga as instruções para fazer logon no Workfront.

   >[!NOTE]
   >
   >* O Workfront se conecta ao Adobe Creative Cloud usando o OAuth 2.0, um padrão seguro usado pela maioria das integrações baseadas na Web para a autenticação e a autorização dos usuários.
   >* Quando for solicitado a inserir o [domínio ou host] da sua conta Workfront, digite-a usando este formato: *sua empresa&#39;sDomain.my.workfront.com*. O domínio de sua empresa geralmente é o nome de sua empresa.


   Uma lista de itens de trabalho atribuídos a você é exibida se o projeto tiver um status atual. Se uma lista não for exibida, faça logon no Workfront.

   As tarefas pessoais estão listadas em **Sem projeto**.

## Fazer upload de um arquivo para um projeto, tarefa ou problema do Workfront {#upload-a-file-to-a-workfront-project-task-or-issue}

Você pode fazer upload de um arquivo do seu sistema de arquivos de computador ou exportar um arquivo aberto atualmente em um aplicativo Adobe Creative Cloud para um projeto, tarefa ou problema do Workfront. 

Considere o seguinte ao carregar ou exportar um arquivo do Adobe Creative Cloud:

* Seu Nível de acesso deve permitir o upload de documentos para a Workfront. Para obter mais informações, consulte [Conceder acesso a documentos](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-documents.md).
* Você deve ter permissões para fazer upload de documentos para o item em que deseja. Para obter mais informações, consulte [Visão geral do compartilhamento de permissões em objetos](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).
* O arquivo é carregado na área Documentos do objeto Workfront selecionado.
* Não é possível exportar um documento para a área Documentos no Menu principal ![](assets/main-menu-icon.png) de um aplicativo Adobe Creative Cloud.

Esta seção explica o seguinte:

* [Carregar um arquivo](#upload-a-file)
* [Exportar um arquivo atualmente aberto no Illustrator ou InDesign](#export-a-file-currently-open-in-illustrator-or-indesign)
* [Fazer upload de uma nova versão de um arquivo do Illustrator ou InDesign](#upload-a-new-version-of-a-file-from-illustrator-or-indesign)

### Carregar um arquivo {#upload-a-file}

Você pode fazer upload de seus arquivos para um projeto, tarefa ou problema sem sair do aplicativo Adobe Creative Cloud.

1. Se você não vir a extensão do Workfront ao abrir seu aplicativo Adobe Creative Cloud, clique em **Window** > **Extensões** > Workfront.

   Uma lista de itens de trabalho atribuídos a você é exibida se o projeto tiver um status atual. Se uma lista não for exibida, faça logon no Workfront.

   As tarefas pessoais estão listadas em **Sem projeto**.

1. Clique no nome do projeto, tarefa ou problema para o qual deseja fazer upload do arquivo.

   Você pode pesquisar por isso digitando o nome no **Pesquisar** e selecionando **Projeto**, **Tarefa** ou **Problema** no menu suspenso à direita do **Pesquisar** caixa. Se o nome do item de trabalho não aparecer na lista, pressione **Enter** para pesquisar todos os itens do Workfront que você tem acesso para visualizar.

1. Clique em **Selecionar** no canto inferior direito da extensão do Workfront.
1. No **Clique para selecionar o formato** no menu suspenso , clique no formato no qual deseja salvar o arquivo no Workfront.

   Para obter uma lista de formatos compatíveis para cada aplicativo suportado, consulte [Formatos de arquivo exportados suportados](#supported-exported-file-formats) neste artigo.

1. (Condicional) Se o item de trabalho no qual você deseja fazer upload do arquivo tiver pastas de documento, selecione uma pasta de documento no **Clique para selecionar uma pasta de documento** e clique em **Selecionar**.

1. Clique em **Carregar um arquivo local**.
1. No **Abrir arquivo** for exibida, encontre o arquivo em seu sistema de arquivos e clique em **Abrir**.

1. (Opcional) Digite um novo nome para o arquivo. 

   ![](assets/rename-file-uploading.png)

1. Clique em **Upload**.

   No Workfront, o documento agora é listado na área Documentos do projeto, tarefa ou problema especificado.  

1. (Opcional) Clique no nome do documento para abrir a página Detalhes do documento no Workfront.

   O Workfront é aberto em uma nova guia do navegador.

### Exportar um arquivo atualmente aberto no Illustrator ou InDesign {#export-a-file-currently-open-in-illustrator-or-indesign}

1. Em um aplicativo do Adobe Creative Cloud compatível, abra um arquivo que deseja exportar para o Workfront. 
1. Se a extensão do Workfront não for exibida, clique em **Window** > **Extensões** > Workfront.

   Uma lista de itens de trabalho atribuídos a você é exibida se o projeto tiver um status atual. Se uma lista não for exibida, faça logon no Workfront.

   As tarefas pessoais estão listadas em **Sem projeto**.

1. Clique no nome do projeto, tarefa ou problema para o qual deseja exportar o arquivo.

   Você pode pesquisar por isso digitando o nome no **Pesquisar** e selecionando **Projeto**, **Tarefa** ou **Problema** no menu suspenso à direita do **Pesquisar** caixa. Se o nome do item de trabalho não aparecer na lista, pressione **Enter** para pesquisar todos os itens do Workfront que você tem acesso para visualizar.

1. No **Clique para selecionar o formato** no menu suspenso , clique no formato no qual deseja salvar o arquivo no Workfront.

   Para obter uma lista de formatos compatíveis para cada aplicativo suportado, consulte [Formatos de arquivo exportados suportados](#supported-exported-file-formats) neste artigo.

1. (Condicional) Se o item de trabalho no qual você deseja fazer upload do arquivo tiver pastas de documento, selecione uma pasta de documento no **Clique para selecionar uma pasta de documento** e clique em **Selecionar**.
1. (Opcional) Para renomear o documento, clique no nome do documento e digite um novo nome.

   ![](assets/rename-doc-exporting.png)

1. Clique em **Exportar**. 

   Uma mensagem é exibida para confirmar que o documento foi exportado com êxito para o Workfront.

   No Workfront, o documento é listado na área Documentos do objeto especificado no Workfront.

1. (Opcional) Clique no nome do documento para acessá-lo no Workfront.

   ![adobe_document_with_name_highlight.PNG](assets/adobe-document-with-name-highlight-350x251.png)

   O Workfront é aberto em uma nova guia do navegador.

### Fazer upload de uma nova versão de um arquivo do Illustrator ou InDesign {#upload-a-new-version-of-a-file-from-illustrator-or-indesign}

1. Se quiser exportar um arquivo no qual você está trabalhando em um aplicativo Adobe compatível como uma nova versão de um arquivo no Workfront, abra o arquivo no aplicativo Adobe. 
1. Se a extensão do Workfront não for exibida, clique em **Window** > **Extensões** > Workfront.

   Uma lista de itens de trabalho atribuídos a você é exibida se o projeto tiver um status atual. Se uma lista não for exibida, faça logon no Workfront.

   As tarefas pessoais estão listadas em **Sem projeto**.

1. Clique no nome do projeto, tarefa ou problema em que o documento existente é listado.

   Você pode pesquisar por isso digitando o nome no **Pesquisar** e selecionando **Projeto**, **Tarefa** ou **Problema** no menu suspenso à direita do **Pesquisar** caixa. Se o nome do item de trabalho não aparecer na lista, pressione **Enter** para pesquisar todos os itens do Workfront que você tem acesso para visualizar.

   Todos os documentos carregados em projetos, tarefas ou problemas são exibidos em uma lista, independentemente de terem sido carregados do aplicativo Adobe.

1.  
1. No **Clique para selecionar o formato** no menu suspenso , clique no formato no qual deseja salvar o arquivo no Workfront.

   Isso é necessário se você estiver exportando um arquivo aberto no aplicativo Adobe. Para obter uma lista de formatos compatíveis para cada aplicativo suportado, consulte [Formatos de arquivo exportados suportados](#supported-exported-file-formats) neste artigo.

1. Se estiver exportando um arquivo aberto no aplicativo Adobe como uma nova versão do documento do Workfront selecionado, clique em **Exportar**.

   Ou

   Se quiser carregar um arquivo do seu sistema de arquivos do computador como uma nova versão do documento do Workfront selecionado, clique em **Carregar um arquivo local**, encontre o arquivo na caixa exibida, clique em **Abrir**, depois clique em **Upload**.

1. (Opcional) Clique no nome do documento para ver sua nova versão no Workfront. 

   >[!NOTE]
   >
   >O nome do documento no Workfront é preenchido por padrão e não pode ser editado. Também não é alterado para o nome do arquivo que você carrega ou exporta como uma nova versão.
   >
   >
   >![](assets/doc-name-cant-be-changed.png)

## Comentário em um documento Workfront do Illustrator ou InDesign {#comment-on-a-workfront-document-from-illustrator-or-indesign}

Você pode adicionar comentários diretamente a um documento do Workfront em um aplicativo Adobe. No Workfront, seus comentários são exibidos na área Atualizações do documento e na área Atualizações do item do Workfront em que o documento é salvo. 

1. Abra um dos aplicativos Adobe suportados.
1. Se a extensão do Workfront não for exibida, clique em **Window** > **Extensões** > Workfront.

   Uma lista de itens de trabalho atribuídos a você é exibida se o projeto tiver um status atual. Se uma lista não for exibida, faça logon no Workfront.

   As tarefas pessoais estão listadas em **Sem projeto**.

1. Clique no projeto, tarefa ou problema em que o documento existente está listado.

   Você pode pesquisar por isso digitando o nome no **Pesquisar** e selecionando **Projeto**, **Tarefa** ou **Problema** no menu suspenso à direita do **Pesquisar** caixa. Se o nome do item de trabalho não aparecer na lista, pressione **Enter** para pesquisar todos os itens do Workfront que você tem acesso para visualizar.

1. Clique no nome do documento existente e, em seguida, clique em **Selecionar** no canto inferior direito da extensão do Workfront.
1. Clique no botão **Comentário** e digite a atualização na caixa exibida.

1. (Opcional) Para incluir outros usuários ou equipes do Workfront no comentário, comece a digitar o nome de um usuário ou de uma equipe no **Notificar pessoas ou equipes** , em seguida, clique no nome quando ele for exibido na lista suspensa.
1. (Opcional) Para solicitar aprovação no documento, selecione **Fazer uma solicitação de aprovação**.
1. Clique em **Atualizar**.

   Uma atualização é postada na guia Atualizações do documento. Os usuários do Workfront que você incluir no comentário recebem uma notificação no aplicativo e, dependendo de como o Workfront é configurado, também podem receber uma notificação por email.

   Para obter mais informações sobre notificações no Workfront, consulte [Exibir e gerenciar notificações no aplicativo](../../workfront-basics/using-notifications/view-and-manage-in-app-notifications.md). 

   Para obter mais informações sobre o recebimento de notificações por email, consulte [Notificações do Adobe Workfront](../../workfront-basics/using-notifications/wf-notifications.md).

## Solicitar aprovação de documento do Illustrator ou InDesign

Você pode solicitar uma aprovação de documento do Workfront diretamente de um aplicativo Adobe.

Você pode solicitar uma aprovação de documento das seguintes entidades:

* Um usuário do Workfront
* Um usuário externo sem uma conta do Workfront

Você pode solicitar uma aprovação em um documento de um aplicativo Adobe das seguintes maneiras:

* Ao anexar um aprovador ao documento.
* Ao comentar um documento, notificando a pessoa quando você faz um comentário. e anexá-los como aprovadores ao documento.

   Para obter informações sobre solicitar uma aprovação ao comentar um documento, consulte [Comentário em um documento Workfront do Illustrator ou InDesign](#comment-on-a-workfront-document-from-illustrator-or-indesign) neste artigo.

Para solicitar uma aprovação em um documento de um aplicativo Adobe:

1. Abra um dos aplicativos Adobe suportados.
1. Se a extensão do Workfront não for exibida, clique em **Window** > **Extensões** > Workfront.

   Uma lista de itens de trabalho atribuídos a você é exibida se o projeto tiver um status atual. Se uma lista não for exibida, faça logon no Workfront.

   As tarefas pessoais estão listadas em **Sem projeto**.

1. Clique no projeto, tarefa ou problema em que o documento existente está listado e, em seguida, clique no nome do documento existente.

   Você pode pesquisar por isso digitando o nome no **Pesquisar** e selecionando **Projeto**, **Tarefa** ou **Problema** no menu suspenso à direita do **Pesquisar** caixa. Se o nome do item de trabalho não aparecer na lista, pressione **Enter** para pesquisar todos os itens do Workfront que você tem acesso para visualizar.

1. Clique no nome do documento existente e, em seguida, clique em **Selecionar** no canto inferior direito da extensão do Workfront.
1. Clique no botão **Aprovação** guia .
1. Para adicionar um aprovador, na **Comece digitando uma caixa de nome** siga um destes procedimentos:

   * Digite o nome de um aprovador e selecione-o quando ele for exibido na lista.

      ![](assets/adobe-cc-adding-a-doc-approver-350x189.png)

   * Digite o endereço de email de um usuário externo.

1. Clique em **Solicitar aprovação**.

   Os usuários do Workfront que você incluir no comentário ou adicionar como aprovador recebem uma notificação no aplicativo e, dependendo de como o Workfront é configurado, também podem receber uma notificação por email.\
   Usuários externos recebem uma notificação por email de onde podem tomar uma decisão sobre a aprovação.

   Para obter informações sobre notificações no Workfront, consulte [Exibir e gerenciar notificações no aplicativo](../../workfront-basics/using-notifications/view-and-manage-in-app-notifications.md). Para obter informações sobre o recebimento de notificações por email, consulte [Notificações do Adobe Workfront](../../workfront-basics/using-notifications/wf-notifications.md).

## Gerar uma prova do Illustrator ou InDesign {#generate-a-proof-from-illustrator-or-indesign}

Se sua organização usar modelos de Fluxo de trabalho automatizado, você poderá gerar uma prova para um documento criado em um aplicativo do Adobe sem sair do aplicativo. Para obter informações sobre como criar provas, consulte [Criar provas](../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-proofs--in-wf.md). Para obter informações sobre modelos de Fluxo de trabalho automatizado, consulte [Templates de workflows automatizados](../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md#automate) em [Visão geral do fluxo de trabalho automatizado](../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md).

1. Abra um dos aplicativos Adobe suportados.
1. Se a extensão do Workfront não for exibida, clique em **Window** > **Extensões** > Workfront.

   Uma lista de itens de trabalho atribuídos a você é exibida se o projeto tiver um status atual. Se uma lista não for exibida, faça logon no Workfront.

   As tarefas pessoais estão listadas em **Sem projeto**.

1. Se o documento já estiver carregado no Workfront, selecione o projeto, a tarefa ou o problema na extensão do Workfront em que o documento está listado e clique no nome do documento.

   Ou

   Faça upload de um documento do Adobe para um objeto Workfront, conforme descrito na seção [Fazer upload de um arquivo para um projeto, tarefa ou problema do Workfront](#upload-a-file-to-a-workfront-project-task-or-issue) neste artigo, clique no nome do documento.

1. No **Clique para selecionar o formato** no menu suspenso , clique no formato no qual deseja salvar o arquivo no Workfront.

   Alguns formatos não estarão disponíveis após habilitar a funcionalidade de prova na etapa seguinte. Para obter mais informações, consulte [Formatos de arquivo exportados suportados](#supported-exported-file-formats) neste artigo.

1. Clique em **Fazer upload como uma nova prova** para habilitá-lo.
1. Selecione o **Modelo de fluxo de trabalho** você deseja que as pessoas usem enquanto revisam o documento.

   O administrador do Workfront configura os modelos de Fluxo de trabalho automatizado, conforme descrito em . Consulte o administrador em caso de dúvidas.

   1. Adicione pelo menos um **Novo recipient** para cada estágio no Modelo de fluxo de trabalho.

      Você pode começar a digitar um nome e selecioná-lo ao visualizá-lo na lista suspensa exibida.

   1. Especifique a **Função de prova** e a frequência de **Alertas por email** para cada recipient que você adicionar.

   1. (Opcional) Na seção **Notificação por e-mail** selecione se deseja enviar uma notificação por email com uma mensagem personalizada opcional sobre a prova para todos os recipients de prova adicionados.

1. Clique em **Criar prova**.

   Você pode visualizar o progresso do processo de criação de prova. Um alerta é exibido quando ele terminar de gerar. Você pode abrir a tarefa onde criou a prova e ela está listada lá.

## Fazer upload de uma nova versão de uma prova sem sair do Illustrator ou do InDesign

1. Clique em um documento existente que tenha uma prova e, em seguida, clique em **Selecionar** no canto inferior direito.
1. Clique em **Fazer upload como uma nova versão de prova** para habilitá-lo.
1. (Opcional) Selecione o **Modelo de fluxo de trabalho** você deseja que as pessoas usem a medida que revisam a nova versão.

   Se você não selecionar um modelo diferente, o modelo selecionado para a versão anterior permanecerá em vigor. Além disso, se você modificou o modelo para a versão anterior, as alterações entrarão em vigor para a nova versão.

   O administrador do Workfront configura os modelos de Fluxo de trabalho automatizado, conforme descrito em . Consulte o administrador em caso de dúvidas.

   1. Adicione pelo menos um **Novo recipient** para cada estágio no Modelo de fluxo de trabalho.

      Você pode começar a digitar um nome e selecioná-lo ao visualizá-lo na lista suspensa exibida.

   1. Especifique a **Função de prova** e a frequência de **Alertas por email** para cada recipient que você adicionar.
   1. (Opcional) Na seção **Notificação por e-mail** selecione se deseja enviar uma notificação por email com uma mensagem personalizada opcional sobre a prova para todos os recipients de prova adicionados.

1. Clique em **Criar nova versão de prova**.

   Você pode visualizar o progresso do processo de criação de prova. Um alerta é exibido quando ele terminar de gerar. Você pode abrir a tarefa onde criou a prova e ela está listada lá.

## Faça logoff da extensão do Workfront

1. No aplicativo Adobe, clique em **Window** > **Extensões** > Workfront.

1. Clique no botão **Mais** menu ![](assets/more-menu.png) no canto superior direito do painel.

1. (Opcional) Clique em **Feedback** para abrir uma breve pesquisa e enviar ao Workfront seus comentários sobre o Workfront for Adobe Creative Cloud. 
1. Clique em **Logout**.\
   A tela Logon é exibida. Para obter informações sobre como fazer logon, consulte [Faça logon na extensão do Workfront a partir do Illustrator ou InDesign](#log-in-to-workfront-extension-from-illustrator-or-indesign) neste artigo.

## Formatos de arquivo exportados suportados {#supported-exported-file-formats}

* [Formatos de arquivo exportados compatíveis com o Adobe InDesign](#supported-exported-file-formats-for-adobe-indesign)
* [Formatos de arquivo exportados compatíveis com o Adobe Illustrator](#supported-exported-file-formats-for-adobe-illustrator)

### Formatos de arquivo exportados compatíveis com o Adobe InDesign  {#supported-exported-file-formats-for-adobe-indesign}

O Workfront oferece suporte aos seguintes formatos de arquivo para exportar um arquivo do InDesign para o Workfront:

* EPS - PostScript encapsulado
* EPUB - Publicação eletrônica de layout fixo
* EPUB - Publicação eletrônica reembolsável &#42;
* HTML - Linguagem de marcação de HyperText
* IDML - Linguagem de marcação de InDesign &#42;
* JPG, JPEG - Grupo misto de peritos fotográficos
* PDF - Arquivo de documento portátil Adobe
* PNG - Gráficos de rede portáteis
* SWF - Flash Player &#42;
* XML - Linguagem de marcação extensível &#42;

&#42; Este formato de arquivo não está disponível quando **Carregar uma nova prova** estiver ativado (para obter informações sobre essa opção, consulte [Gerar uma prova do Illustrator ou InDesign](#generate-a-proof-from-illustrator-or-indesign) neste artigo). Se este formato de arquivo já estiver selecionado antes de habilitar **Carregar uma nova prova**, o sistema altera o formato do arquivo para PDF. É possível selecionar um formato diferente na lista.

### Formatos de arquivo exportados compatíveis com o Adobe Illustrator  {#supported-exported-file-formats-for-adobe-illustrator}

O Workfront oferece suporte aos seguintes formatos de arquivo para exportar um arquivo do Illustrator para o Workfront:

* DWG - Desenho do AutoCAD, Arquivo de Intercâmbio do AutoCAD &#42;
* JPG, JPEG - Grupo misto de peritos fotográficos
* PNG - Gráficos de rede portáteis
* PSD - Documento Photoshop
* SWF - Flash Player &#42;
* TIFF - Formato de arquivo de imagem com tags

&#42; Este formato de arquivo não está disponível quando **Carregar uma nova prova** estiver ativado (para obter informações sobre essa opção, consulte [Gerar uma prova do Illustrator ou InDesign](#generate-a-proof-from-illustrator-or-indesign) neste artigo). Se este formato de arquivo já estiver selecionado antes de habilitar **Carregar uma nova prova**, o sistema altera o formato do arquivo para PNG. É possível selecionar um formato diferente na lista.
