---
title: Compartilhar um documento
content-type: reference
product-area: user-management
navigation-topic: grant-and-request-access-to-objects
description: Seu administrador Adobe Systems Workfront concede aos usuários acesso para visualização ou editar documentos ao atribuir níveis de acesso, como explicado em Conceder acesso a documentos.
author: Courtney
feature: Get Started with Workfront
exl-id: c83a3184-4af0-4897-985b-29f7ee3a0b73
source-git-commit: 7f8c9b9f63770d6364f0eb1b9c23e4648dacaf93
workflow-type: tm+mt
source-wordcount: '1387'
ht-degree: 5%

---

# Compartilhar um documento

O administrador da Workfront controla quem pode visualização ou editar documentos na área Níveis de acesso na Configuração. Para obter mais informações, consulte [Conceder acesso a documentos](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-documents.md).

Os usuários também podem compartilhar documentos que carregaram ou terem acesso, dando a outros permissão para visualização ou gerenciar eles.

* As permissões se aplicam a itens individuais e definem quais ações alguém pode tomar.
* A pessoa que faz upload de uma documento recebe automaticamente controle total (Gerenciar permissões).
* Para compartilhar uma pasta inteira, consulte [Compartilhar uma pasta](../../workfront-basics/grant-and-request-access-to-objects/share-a-document-folder.md) documento.

>[!NOTE]
>
>Se o instância da Workfront usar Adobe Systems armazenamento empresarial, você não poderá compartilhar documentos individuais. Em vez disso, você concede acesso no nível do projeto. Lembre-se de que o compartilhamento do projeto pode conceder acesso a informações confidenciais do projeto curtir finanicals, dependendo do nível de permissão escolhidos.



## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacote do Adobe Workfront</td> 
   <td> <p>Qualquer </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">licença da Adobe Systems Workfront</td> 
   <td> <p>Padrão</p> 
   <p>Trabalho ou maior</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Exibir acesso ou superior aos objetos que deseja compartilhar</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Exibir permissões ou superior aos objetos que deseja compartilhar</p></td> 
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

   * **** Exibir: o usuário pode revisar e compartilhar a documento.
   * **Gerenciar**: o usuário tem acesso total ao documento sem direitos administrativos, que são concedidos no nível de acesso (também inclui todas as permissões de Exibição).

1. (Opcional) Clique no ícone de opções avançadas ao lado do nível de permissão que você concedeu para configurar permissões específicas no documento.

   ![Opções avançadas de permissão configuradas](assets/advanced-options-icon.png)

1. (Opcional) Para desativar as permissões herdadas para os objetos filho do documento, clique em **Desativar** embutido com **Permissões herdadas**.

1. (Condicional) Para copiar o link público que permite compartilhar o documento com usuários externos, clique em **Copiar link público**.

   >[!CAUTION]
   >
   >Recomendamos que você tenha cuidado ao compartilhar uma documento contendo informações confidenciais com usuários externos. Isso permite que eles visualização informações sem ser um usuário da Workfront ou parte de sua organização.

1. Clique em **Salvar**.

## Compartilhar documentos em massa

{{step1-to-documents}}

1. **No guia Todos os documentos** na **página documentos**, mantenha **Comando** (Mac) ou **Ctrl** (Windows) no teclado e clique em cada documento que deseja compartilhar.

1. Na parte superior do página, clique no **ícone**![Compartilhar](assets/share-icon.png). O modal de compartilhamento é aberto.

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

## Compartilhamento de documento com a Adobe Systems enterprise armazenamento

A Workfront está em transição para a solução Adobe Systems enterprise armazenamento em solicitar para fornecer maior conectividade com produtos Adobe Creative Cloud. Os clientes existentes serão transferidos para o novo modelo em fases. Para obter mais informações sobre os benefícios da Adobe Systems armazenamento empresarial, visita [Adobe Systems visão geral](/help/quicksilver/review-and-approve-work/esm-overview.md) armazenamento empresarial.

Se sua instância da Workfront usar Adobe Systems armazenamento empresarial, você não poderá compartilhar documentos individuais diretamente. Em vez disso, você deve conceder acesso no nível do projeto.

>[!IMPORTANT]
>
>O compartilhamento de um projeto também pode dar aos usuários acesso a informações confidenciais do projeto, como finanças, dependendo do permissão nível escolhido.
>
>Certifique-se de revisar permissão configurações cuidadosamente antes de compartilhar.

## Permissões para documentos

As permissões são específicas de um item na Workfront e definem quais ações se pode tomar sobre esse item. Para obter informações sobre permissões de objeto, consulte [Visão geral das permissões de compartilhamento em objetos](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

A tabela a seguir exibe quais permissões você pode conceder aos usuários ao permitir que eles visualização ou gerenciar documentos:

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
   <td scope="row">Detalhes do documento do Editar</td> 
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
   <td scope="row">Compartilhar todo o sistema*</td> 
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
   <td scope="row">Adicionar/Remover</td> 
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

&#42; A ação é compartilhada por documentos e pastas de documentos.

&#42;&#42; Você deve ter uma licença de prova separada associada ao seu conta Workfront para poder prova documentos. Entre em contato com sua gerente de conta sobre a aquisição de uma licença de prova. Para obter mais informações sobre provas no Workfront, consulte [Prova](../../review-and-approve-work/proofing/proofing.md).

## Considerações sobre o compartilhamento de documentos

Além das considerações abaixo, consulte [também a Visão geral das permissões de compartilhamento em objetos](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

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
  >Recomendamos que você tenha cuidado ao compartilhar com usuários externos um objeto que contém informações confidenciais. Isso permite que eles visualização informações sem ser um usuário da Workfront ou parte de sua organização.

* Você pode compartilhar um documento com alguém que não tem um conta da Workfront, adicionando seus endereços de e-mail no campo Fornecer documento acesso ao campo.
* Ao compartilhar um documento, os usuários têm o mesmo acesso a todas as versões do documento e todas as provas documento.\
  Para obter mais informações sobre provas no Workfront, consulte a [seção Prova.](../../review-and-approve-work/proofing/proofing.md)

* Você pode herdar permissões para documentos dos objetos aos quais estão associados. O administrador da Workfront pode restringir a herança de permissões de documentos no nível de acesso.

  Para obter mais informações sobre como restringir permissões herdadas em documentos, consulte [Criar ou modifique os níveis de acesso personalizados](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

  Você pode remover manualmente as permissões herdadas no documentos. Para obter mais informações, consulte [Remover permissões de objetos](../../workfront-basics/grant-and-request-access-to-objects/remove-permissions-from-objects.md)

* Um documento anexado herda permissões somente do objeto em que estava anexado. Se você criar uma pasta no objeto e mover a documento para a pasta, ela herda as permissões da pasta. Mas, se você criar uma pasta em um objeto pai ou avô e mover a documento para essa pasta, ela não herda as permissões dessa pasta.