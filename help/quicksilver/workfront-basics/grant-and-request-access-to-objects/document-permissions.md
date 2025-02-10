---
title: Compartilhar um documento
content-type: reference
product-area: user-management
navigation-topic: grant-and-request-access-to-objects
description: O administrador do Adobe Workfront concede aos usuários acesso para visualizar ou editar documentos quando eles atribuírem níveis de acesso, conforme explicado em Conceder acesso a documentos.
author: Alina
feature: Get Started with Workfront
exl-id: c83a3184-4af0-4897-985b-29f7ee3a0b73
source-git-commit: b4e90918c5f499638d0cf5355dc75c3ceca48293
workflow-type: tm+mt
source-wordcount: '640'
ht-degree: 1%

---

# Compartilhar um documento

<span class="preview">As informações destacadas nesta página referem-se a funcionalidades que ainda não estão disponíveis. Ele está disponível somente no ambiente de Pré-visualização da Sandbox.</span>

O administrador do Adobe Workfront concede aos usuários acesso para visualizar ou editar documentos quando eles atribuírem níveis de acesso, conforme explicado em [Conceder acesso a documentos](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-documents.md).

O nível de acesso que o administrador do Workfront concede aos usuários permite que eles visualizem ou editem documentos. Além disso, outros usuários também podem conceder a outros usuários permissões para exibir ou gerenciar documentos específicos que eles próprios carregaram ou que têm acesso para compartilhar.

As permissões são específicas a um item no Workfront e definem quais ações podem ser executadas nesse item. Para obter informações sobre permissões de objeto, consulte [Visão geral das permissões de compartilhamento em objetos](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

Por padrão, o usuário que carrega um documento no Workfront tem permissões de gerenciamento.

Para obter informações sobre como compartilhar uma pasta de documentos inteira, consulte [Compartilhar uma pasta de documentos](../../workfront-basics/grant-and-request-access-to-objects/share-a-document-folder.md).

## Considerações sobre o compartilhamento de documentos

Além das considerações abaixo, consulte também [Visão geral das permissões de compartilhamento em objetos](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

>[!NOTE]
>
>Um administrador do Workfront pode adicionar ou remover permissões a qualquer item no sistema, para todos os usuários, sem ser o proprietário desses itens.

* O compartilhamento de um documento é semelhante ao compartilhamento de qualquer outro objeto no Workfront. Para obter informações sobre como compartilhar documentos no Workfront, consulte [Compartilhar um objeto](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md).
* Você pode conceder as seguintes permissões a documentos:

   * Exibir
   * Gerenciar

  <span class="preview">Na visualização:
  ![](assets/document-permissions.png)
</span>

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

## Permissões de documento

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
   <td>✓ µ</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Editar detalhes do documento</td> 
   <td>✓ µ</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Excluir*</td> 
   <td>✓ µ</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Baixar</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
  </tr> 
  <tr> 
   <td scope="row">Check-out</td> 
   <td>✓ µ</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Adicionar aprovadores</td> 
   <td>✓ µ</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Aprovar documento</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
  </tr> 
  <tr> 
   <td scope="row">Anexar Formulário Personalizado</td> 
   <td>✓ µ</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Editar campos personalizados</td> 
   <td>✓ µ</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Mover para (objeto)</td> 
   <td>✓ µ</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Enviar para (integração)</td> 
   <td>✓ µ</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Atualizações/ Comentários</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
  </tr> 
  <tr> 
   <td scope="row">Carregar nova versão</td> 
   <td>✓ µ</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Excluir versão</td> 
   <td>✓ µ</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Visualizar documento(s)</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
  </tr> 
  <tr> 
   <td scope="row">Visualização</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
  </tr> 
  <tr> 
   <td scope="row">Prova**</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
  </tr> 
  <tr> 
   <td scope="row">Gerar prova**</td> 
   <td>✓ µ</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Remover prova**</td> 
   <td>✓ µ</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Compartilhar*</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
  </tr> 
  <tr> 
   <td scope="row">Compartilhe com todo o sistema*</td> 
   <td>✓ µ</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Compartilhar documentos publicamente*</td> 
   <td>✓ µ</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Compartilhar com um endereço de email externo</td> 
   <td> </td> 
   <td>✓ µ</td> 
  </tr> 
  <tr> 
   <td scope="row">Adicionar/ Remover</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
  </tr> 
  <tr> 
   <td scope="row">Renomear</td> 
   <td>✓ µ</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Link (com integração)</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
  </tr> 
  <tr> 
   <td scope="row">Desvincular (com integração)</td> 
   <td>✓ µ</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

A ação &#42; é compartilhada por Documentos e Pastas de Documentos.

&#42;&#42; É necessário ter uma licença de comprovação separada associada à sua conta da Workfront para poder comprovar documentos. Entre em contato com seu gerente de conta para obter uma licença de comprovação. Para obter mais informações sobre revisões no Workfront, consulte [Revisão](../../review-and-approve-work/proofing/proofing.md).
