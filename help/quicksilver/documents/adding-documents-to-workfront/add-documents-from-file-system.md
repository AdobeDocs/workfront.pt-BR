---
product-area: documents
navigation-topic: add-documents-to-workfront
title: Adicionar documentos ao Adobe Workfront a partir do seu sistema de arquivos
description: Você pode adicionar documentos a projetos, tarefas ou problemas em várias áreas no Adobe Workfront.
author: Courtney
feature: Digital Content and Documents
exl-id: 0a5f82b2-f86e-4ffa-b3a6-18221dd0e158
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 18301970abddd8ed98abccf42562d950422bfa7c
workflow-type: tm+mt
source-wordcount: '1237'
ht-degree: 5%

---

# Adicionar documentos ao Adobe Workfront a partir do seu sistema de arquivos

Atualmente, o Workfront tem duas versões da área Documentos: a área documentos herdados e a nova área documentos. A versão usada por sua organização depende do armazenamento Workfront herdado ou do armazenamento corporativo. Para obter mais informações sobre esses tipos de armazenamento, consulte [visão geral do armazenamento corporativo da Adobe](/help/quicksilver/review-and-approve-work/esm-overview.md).

Adicionar documentos ao Workfront difere, dependendo da versão da área de documentos que sua organização usa.

* [Adicionar documentos ao a partir do seu sistema de arquivos na área de documentos herdados](#add-documents-from-your-file-system-in-the-legacy-documents-area)
* [Adicionar documentos ao Workfront na nova área de documentos](#add-documents-to-workfront-in-the-new-documents-area)



## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacote do Adobe Workfront</td> 
   <td> <p> Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenças do Adobe Workfront*</td> 
   <td> 
   <p>Colaborador ou posterior</p> 
   <p>Solicitação ou posterior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Armazenamento herdado do Workfront: editar acesso a documentos</p> 
   <p>Armazenamento corporativo: o acesso de edição a documentos é ativado por padrão e não pode ser alterado</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Adicionar documentos do sistema de arquivos na área de documentos herdados

Se sua organização utiliza o Workfront Storage herdado, você verá a área de documentos herdados ao acessar documentos no Workfront. Para obter mais informações sobre o Workfront Storage, consulte [Diferenças entre o Adobe Enterprise Storage e o Workfront Storage herdado](/help/quicksilver/review-and-approve-work/esm-overview.md#differences-between-adobe-enterprise-storage-and-legacy-workfront-storage).

Você pode adicionar documentos a projetos, tarefas ou problemas nas seguintes áreas no Adobe Workfront:

* A área Documentos global
* A área Documentos de um objeto do Workfront
* Uma placa conectada em uma placa Workfront

Você também pode carregar novas versões de documentos e adicionar links a documentos de fornecedores de nuvem de terceiros, como Google Drive, Dropbox e Microsoft OneDrive. Para obter informações sobre como adicionar novas versões de documentos, consulte [Carregar uma nova versão de um documento](../../documents/managing-documents/upload-new-document-version.md). Para obter informações sobre como adicionar documentos de fornecedores de nuvem de terceiros, consulte [Vincular documentos de aplicativos externos](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

Não há restrições quanto aos tipos e tamanhos de arquivos que você pode carregar no Workfront. No entanto, para ser bem-sucedido, o upload deve ser concluído em cinco minutos e você deve ter espaço de armazenamento adequado disponível.

Se você precisar de informações sobre como carregar novas versões de um documento no Workfront, consulte [Carregar uma nova versão de um documento](../../documents/managing-documents/upload-new-document-version.md).


### Adicionar documentos ao Workfront na área de documentos herdados

Você pode adicionar novos documentos ao Workfront a partir do sistema de arquivos em sua estação de trabalho. Você também pode vincular documentos de aplicativos de terceiros, como o Google Drive e o SharePoint.

>[!IMPORTANT]
>
>* É possível carregar até 150 documentos de uma só vez.
>* Não há limite para o tamanho do arquivo.
>* Os downloads de documentos são limitados a 4 GB.

Para adicionar um documento:

1. Vá para o projeto, tarefa ou problema em que deseja adicionar um novo documento.
1. Clique na guia **Documentos** e no menu suspenso **Adicionar novo**.

   ![Adicionar novo documento](assets/add-new-doc.png)

1. Dependendo do tipo de documento que deseja adicionar, execute um dos procedimentos a seguir:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Fazer upload de documentos do sistema de arquivos na estação de trabalho</td> 
      <td> 
       <ol> 
        <li value="1">No menu suspenso <strong>Adicionar novo</strong>, selecione <strong>Documento.</strong></li> 
        <li value="2"> <p>Procure e selecione o documento que deseja adicionar do sistema de arquivos na estação de trabalho.<br></p> <p>Você pode selecionar vários documentos pressionando a tecla Shift enquanto seleciona arquivos adicionais.</p> </li> 
        <li value="3">Clique em <strong>Abrir</strong>.</li> 
       </ol> 
       <p><b>OBSERVAÇÃO</b>: você também pode arrastar e soltar arquivos diretamente do gerenciador de arquivos na lista de documentos.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Fazer upload de documentos de um aplicativo de terceiros, como o Google Drive ou o SharePoint</td> 
      <td> 
       <ol> 
        <li value="1"> <p>No menu suspenso <strong>Adicionar novo</strong>, selecione <strong>De &lt;name_of_third-party_application&gt;</strong>.</p> <p>Por exemplo, para carregar um documento do Google Drive, clique em <strong>Do Google Drive</strong>.</p> </li> 
        <li value="2"> <p>Siga as instruções para selecionar o documento no aplicativo de terceiros.<br></p> <p>Para obter mais informações sobre documentos vinculados, consulte <a href="../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md" class="MCXref xref">Vincular documentos de aplicativos externos</a>.</p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Solicitar um documento de outro usuário do Workfront</td> 
      <td> 
       <ol> 
        <li value="1">No menu suspenso <strong>Adicionar novo</strong>, selecione <strong>Solicitar um documento</strong>.</li> 
        <li value="2">Na caixa <strong>De quem você está solicitando o documento</strong>, digite o nome do usuário de quem você está solicitando o documento.</li> 
        <li value="3">Na caixa <strong>Diga a eles o que você está solicitando</strong>, digite o nome do documento.</li> 
        <li value="4"> <p>Clique em <strong>Enviar solicitação</strong>.</p> <p>Sua solicitação é exibida na guia Documentos.</p> <p>Para obter mais informações sobre a solicitação de documentos, consulte <a href="../../documents/adding-documents-to-workfront/request-a-document.md" class="MCXref xref">Solicitar um Documento</a>.</p> </li> 
       </ol> </td> 
     </tr> 
    </tbody> 
   </table>


## Adicionar documentos ao Workfront na nova área de documentos

É possível adicionar documentos a projetos, tarefas ou problemas usando o modelo de armazenamento corporativo. Para obter mais informações sobre o armazenamento corporativo, consulte [visão geral sobre o armazenamento corporativo da Adobe](/help/quicksilver/review-and-approve-work/esm-overview.md).

Funcionalidade não suportada atualmente na área de novos documentos:

* Fazendo upload de documentos para a área Documentos global
* Adicionar links para documentos de fornecedores de nuvem de terceiros, como Google Drive, Dropbox e Microsoft OneDrive.
* Solicitando documentos
* Como copiar um link para uma pasta
* Fazendo check-out de documentos
* Colar imagens da área de transferência
* Adicionar pastas inteligentes


### Adicionar documentos ao Workfront na nova área de documentos

Se sua organização usar armazenamento corporativo, você verá a nova área de documentos ao acessar documentos no Workfront. Para obter mais informações sobre o armazenamento corporativo, consulte [visão geral sobre o armazenamento corporativo da Adobe](/help/quicksilver/review-and-approve-work/esm-overview.md).

<!--
>[!IMPORTANT]
>
>* You can upload up to 150 documents at one time.
>* There is no limit on the file size. 
>* Document downloads are limited to 4GB.
-->

Para adicionar um documento:

1. Vá para o projeto, tarefa ou problema em que deseja adicionar um novo documento.
1. Clique em **Documentos** no painel esquerdo.
1. Clique em **Novo** no lado direito da página ou arraste e solte o arquivo na área designada exibida. É possível adicionar vários documentos de uma vez.

   ![Adicionar um novo documento](assets/add-new-doc-new-doc.png)

Se você precisar de informações sobre como carregar novas versões de um documento no Workfront, consulte [Carregar uma nova versão de um documento](../../documents/managing-documents/upload-new-document-version.md).

## Segurança de documentos para armazenamento corporativo

O Workfront impede que vírus e outros conteúdos mal-intencionados entrem no site através de documentos das seguintes maneiras:

**Como o Workfront detecta arquivos corrompidos**

A digitalização de documentos é ativada automaticamente para objetos que usam o modelo de armazenamento corporativo.

Todos os arquivos com menos de 500 MB são verificados quando são carregados. Arquivos com mais de 500 MB não são verificados. Se o Workfront detectar um documento corrompido, ele será removido automaticamente.

**Restrições de nome de arquivo**

Como essa integração é criada usando o armazenamento corporativo Adobe, há algumas convenções de estrutura e nomenclatura aplicadas que devem ser levadas em conta ao gerenciar projetos e documentos.

* Os nomes dos objetos devem ser exclusivos e não podem ser duplicados
* O armazenamento corporativo da Adobe requer nomes exclusivos para objetos de mesmo nível com o mesmo pai na árvore hierárquica
* Os documentos não podem ter o mesmo nome se pertencerem ao mesmo projeto
* Nomes de documentos não podem conter nenhum dos seguintes caracteres especiais: `\ / : * ? " | < >`
* Os nomes de documentos são limitados a no máximo 255 caracteres

Com essas limitações em mente, o Workfront renomeia automaticamente objetos ou documentos conforme necessário para evitar conflitos.


## Segurança de documentos para armazenamento Workfront herdado

O site do Workfront impede que vírus e outros conteúdos mal-intencionados entrem no site através de documentos das seguintes maneiras:

**Como o Workfront detecta arquivos corrompidos**

A digitalização de documentos está ativada para sua organização somente mediante solicitação.

Se a digitalização de documentos estiver ativada, os arquivos com menos de 25 MB serão examinados quando forem carregados. Arquivos com mais de 25 MB não são verificados.

Se o Workfront detectar um documento corrompido, será exibida uma mensagem indicando que o arquivo está corrompido. Você também recebe uma notificação por email quando o Workfront detecta conteúdo potencialmente malicioso e o arquivo está programado para remoção.

Os arquivos corrompidos são removidos em até 24 horas após a detecção, a menos que você os remova manualmente. Se você excluir um arquivo corrompido, o Workfront rastreia essa ação como uma atualização. Se você permitir que o Workfront o remova, nenhuma atualização será gravada.

**Restrições de nome de arquivo**

Os arquivos carregados no Workfront não podem conter determinados caracteres nos nomes de arquivo. Se um arquivo contiver qualquer um dos seguintes caracteres no nome do arquivo, eles serão removidos do nome do arquivo quando ele for carregado: `! # % * \ | ' " / ? < > { } [ ]`.
