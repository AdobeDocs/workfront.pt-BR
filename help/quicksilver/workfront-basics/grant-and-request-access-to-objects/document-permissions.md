---
title: Compartilhar um documento
content-type: reference
product-area: user-management
navigation-topic: grant-and-request-access-to-objects
description: O administrador do Adobe Workfront concede aos usuários acesso para visualizar ou editar documentos quando eles atribuírem níveis de acesso, conforme explicado em Conceder acesso a documentos.
author: Courtney
feature: Get Started with Workfront
exl-id: c83a3184-4af0-4897-985b-29f7ee3a0b73
source-git-commit: 4ae96f67b15838403ffce32317d871d6904d6d95
workflow-type: tm+mt
source-wordcount: '1387'
ht-degree: 3%

---

# Compartilhar um documento

O administrador do Workfront controla quem pode exibir ou editar documentos na área Níveis de acesso em Configurar. Para obter mais informações, consulte [Conceder acesso a documentos](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-documents.md).

Os usuários também podem compartilhar documentos aos quais fizeram upload ou têm acesso, dando a outras pessoas permissão para visualizá-los ou gerenciá-los.

* As permissões se aplicam a itens individuais e definem quais ações alguém pode realizar.
* A pessoa que carrega um documento automaticamente obtém controle total (Gerenciar permissões).
* Para compartilhar uma pasta inteira, consulte [Compartilhar uma pasta de documentos](../../workfront-basics/grant-and-request-access-to-objects/share-a-document-folder.md).

>[!NOTE]
>
>Se sua instância do Workfront usar o Adobe Enterprise Storage, você não poderá compartilhar documentos individuais. Em vez disso, você concede acesso no nível do projeto. Lembre-se de que o compartilhamento do projeto pode conceder acesso a informações confidenciais do projeto, como dados financeiros, dependendo do nível de permissão escolhido.



## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacote do Adobe Workfront</td> 
   <td> <p>Qualquer </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td> <p>Standard</p> 
   <p>Trabalhar ou superior</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Exibir o acesso ou superior aos objetos que você deseja compartilhar</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Exibir permissões ou superiores aos objetos que você deseja compartilhar</p></td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++



## Compartilhar um documento

Por padrão, o usuário que carrega um documento no Workfront tem permissões de gerenciamento.

{{step1-to-documents}}

1. Na página **Documentos**, passe o cursor do mouse sobre o documento que deseja compartilhar e clique no link **Detalhes do Documento** exibido. A página **Detalhes do documento** é aberta.

   ![Link de Detalhes do Documento](assets/document-details-link.png)

1. Clique no ícone **Mais** ![Mais ícone](assets/more-icon.png) à direita do nome do documento e em **Compartilhar**. A caixa de diálogo **Compartilhar [Nome do Documento]** é aberta.

   ![Compartilhar um documento](assets/share-a-document-350x160.png)

1. No campo **Conceder acesso ao documento para**, comece digitando o nome do usuário, da equipe, da função, do grupo ou da empresa com a qual deseja compartilhar o documento e clique no nome quando ele aparecer na lista suspensa.

   >[!TIP]
   >
   >Você só pode compartilhar um documento com usuários, equipes, funções ou empresas ativos.


1. (Opcional) Selecione o menu suspenso **Quem tem acesso** e selecione o nível de acesso do documento:

   * **Somente pessoas convidadas podem acessar:** Somente usuários convidados para o documento podem acessá-lo (padrão).
   * **Todos no sistema podem exibir**: todos os usuários do sistema podem exibir o documento sem um convite.

1. (Opcional) Para tornar o documento público, clique no ícone de engrenagem ![Selecione o ícone de engrenagem](assets/gear-icon.png) e clique na caixa alinhada com **Tornar público para usuários externos**. O botão **Copiar link público** aparece na parte inferior da caixa de diálogo.

1. Clique na lista suspensa à direita do nome do usuário e selecione o nível de permissão para este documento:

   * **Exibir**: o usuário pode revisar e compartilhar o documento.
   * **Gerenciar**: o usuário tem acesso total ao documento sem direitos administrativos, que são concedidos no nível de acesso (também inclui todas as permissões de Exibição).

1. (Opcional) Clique no ícone de opções avançadas ao lado do nível de permissão que você concedeu para configurar permissões específicas no documento.

   ![Opções avançadas de permissão configuradas](assets/advanced-options-icon.png)

1. (Opcional) Para desativar as permissões herdadas para os objetos filho do documento, clique em **Desativar** embutido com **Permissões herdadas**.

1. (Condicional) Para copiar o link público que permite compartilhar o documento com usuários externos, clique em **Copiar link público**.

   >[!CAUTION]
   >
   >Recomendamos que você tenha cuidado ao compartilhar com usuários externos um documento contendo informações confidenciais. Isso permite que eles visualizem informações sem ser um usuário da Workfront ou parte da organização.

1. Clique em **Salvar**.

## Compartilhar documentos em massa

{{step1-to-documents}}

1. Na guia **Todos os Documentos** da página **Documentos**, mantenha pressionada a tecla **Command** (Mac) ou **Ctrl** (Windows) no teclado e clique em cada documento que deseja compartilhar.

1. Na parte superior da página, clique no **ícone Compartilhar** ![ícone Compartilhar](assets/share-icon.png). O modal de compartilhamento é aberto.

   ![Ícone de compartilhamento](assets/share-documents-in-bulk.png)

1. No campo **Conceder acesso ao documento para**, comece digitando o nome do usuário, da equipe, da função, do grupo ou da empresa com a qual deseja compartilhar os documentos e clique no nome quando ele aparecer na lista suspensa.

   >[!TIP]
   >
   >Você só pode compartilhar documentos com usuários, equipes, funções ou empresas ativos.


1. (Opcional) Selecione o menu suspenso **Quem tem acesso** e selecione o nível de acesso dos documentos:

   * **Somente pessoas convidadas podem acessá-lo:** Somente usuários convidados para os documentos podem acessá-lo (Padrão).
   * **Todos no sistema podem exibir**: todos os usuários do sistema podem exibir os documentos sem um convite.

1. Clique na lista suspensa à direita do nome do usuário e selecione o nível de permissão para os documentos:

   * **Exibir**: o usuário pode revisar e compartilhar os documentos.
   * **Gerenciar**: o usuário tem acesso total aos documentos sem direitos administrativos, que são concedidos no nível de acesso (também inclui todas as permissões de Exibição).

1. (Opcional) Clique no ícone de opções avançadas ao lado do nível de permissão que você concedeu para configurar permissões específicas nos documentos.

   ![Opções avançadas de permissão configuradas](assets/advanced-options-icon.png)

1. Clique em **Salvar**.

## Compartilhamento de documentos com o armazenamento corporativo da Adobe

A Workfront está fazendo a transição para a solução de armazenamento corporativo da Adobe para fornecer maior conectividade com os produtos Adobe Creative Cloud. Os clientes existentes serão transferidos para o novo modelo em fases. Para obter mais informações sobre os benefícios do Adobe Enterprise Storage, visite [visão geral do Adobe Enterprise Storage](/help/quicksilver/review-and-approve-work/esm-overview.md).

Se sua instância do Workfront usar o armazenamento corporativo da Adobe, você não poderá compartilhar documentos individuais diretamente. Em vez disso, você deve conceder acesso no nível do projeto.

>[!IMPORTANT]
>
>O compartilhamento de um projeto também pode conceder aos usuários acesso a informações confidenciais do projeto, como finanças, dependendo do nível de permissão escolhido.
>
>Certifique-se de revisar as configurações de permissão cuidadosamente antes de compartilhar.

## Permissões de documento

As permissões são específicas a um item no Workfront e definem quais ações podem ser executadas nesse item. Para obter informações sobre permissões de objeto, consulte [Visão geral das permissões de compartilhamento em objetos](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

A tabela a seguir mostra quais permissões você pode conceder aos usuários ao permitir que eles exibam ou gerenciem documentos:

<table border="2" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Ação</strong> </p> </th> 
   <th> <p><strong>Gerenciar</strong> </p> </th> 
   <th> <p><strong>Exibir</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td scope="row">Criar</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Editar detalhes do documento</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Excluir*</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Baixar</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Check-out</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Adicionar aprovadores</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Aprovar documento</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Anexar Formulário Personalizado</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Editar campos personalizados</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Mover para (objeto)</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Enviar para (integração)</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Atualizações/ Comentários</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Carregar nova versão</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Excluir versão</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Visualizar documento(s)</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Visualização</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Prova**</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Gerar prova**</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Remover prova**</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Compartilhar*</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Compartilhe com todo o sistema*</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Compartilhar documentos publicamente*</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Compartilhar com um endereço de email externo</td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Adicionar/ Remover</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Renomear</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Link (com integração)</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Desvincular (com integração)</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

A ação &#42; é compartilhada por Documentos e Pastas de Documentos.

&#42;&#42; É necessário ter uma licença de comprovação separada associada à sua conta da Workfront para poder comprovar documentos. Entre em contato com seu gerente de conta para obter uma licença de comprovação. Para obter mais informações sobre revisões no Workfront, consulte [Revisão](../../review-and-approve-work/proofing/proofing.md).

## Considerações sobre o compartilhamento de documentos

Além das considerações abaixo, consulte também [Visão geral das permissões de compartilhamento em objetos](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

>[!NOTE]
>
>Um administrador do Workfront pode adicionar ou remover permissões a qualquer item no sistema, para todos os usuários, sem ser o proprietário desses itens.

* O compartilhamento de um documento é semelhante ao compartilhamento de qualquer outro objeto no Workfront. Para obter informações sobre como compartilhar documentos no Workfront, consulte [Compartilhar um objeto](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md).
* Você pode conceder as seguintes permissões a documentos:

   * Exibir
   * Gerenciar

* Você também pode compartilhar um documento publicamente ou em todo o sistema.

  >[!CAUTION]
  >
  >Recomendamos que você tenha cuidado ao compartilhar com usuários externos um objeto que contém informações confidenciais. Isso permite que eles visualizem informações sem ser um usuário da Workfront ou parte da organização.

* Você pode compartilhar um documento com alguém que não tenha uma conta do Workfront, adicionando o endereço de email no campo Dar acesso ao documento.
* Quando você compartilha um documento, os usuários têm o mesmo acesso a todas as versões do documento e a todas as provas do documento.\
  Para obter mais informações sobre revisões no Workfront, consulte a seção [Revisão](../../review-and-approve-work/proofing/proofing.md).

* Você pode herdar permissões para documentos dos objetos aos quais estão associados. O administrador do Workfront pode restringir a herança de permissões para documentos em seu nível de acesso.

  Para obter mais informações sobre como restringir permissões herdadas em documentos, consulte [Criar ou modificar níveis de acesso personalizados](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

  Você pode remover manualmente permissões herdadas em documentos. Para obter mais informações, consulte [Remover permissões de objetos](../../workfront-basics/grant-and-request-access-to-objects/remove-permissions-from-objects.md)

* Um documento anexado herda permissões somente do objeto ao qual foi anexado. Se você criar uma pasta no objeto e mover o documento para a pasta, ela herdará as permissões da pasta. Porém, se você criar uma pasta em um objeto pai ou avô e mover o documento para essa pasta, ele não herdará as permissões dessa pasta.