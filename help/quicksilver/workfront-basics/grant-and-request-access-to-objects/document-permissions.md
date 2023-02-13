---
title: Compartilhar um documento
content-type: reference
product-area: user-management
navigation-topic: grant-and-request-access-to-objects
description: O administrador do Adobe Workfront concede aos usuários acesso para visualizar ou editar documentos ao atribuírem níveis de acesso, conforme explicado em Conceder acesso aos documentos.
author: Alina
feature: Get Started with Workfront
exl-id: c83a3184-4af0-4897-985b-29f7ee3a0b73
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '580'
ht-degree: 4%

---

# Compartilhar um documento

O administrador do Adobe Workfront concede aos usuários acesso para visualizar ou editar documentos ao atribuir níveis de acesso, como explicado em [Conceder acesso a documentos](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-documents.md).

O nível de acesso que o administrador do Workfront concede aos usuários permite que eles visualizem ou editem documentos. Além disso, outros usuários também podem conceder a outros permissões para visualizar ou gerenciar documentos específicos que eles próprios carregaram ou que tiveram acesso para compartilhar.

As permissões são específicas a um item no Workfront e definem quais ações podem ser executadas nesse item. Para obter informações sobre permissões de objeto, consulte [Visão geral do compartilhamento de permissões em objetos](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

Por padrão, o usuário que faz upload de um documento para o Workfront tem permissões de gerenciamento.

Para obter informações sobre como compartilhar uma pasta de documento inteira, consulte [Compartilhar uma pasta de documentos](../../workfront-basics/grant-and-request-access-to-objects/share-a-document-folder.md).

## Considerações sobre o compartilhamento de documentos

Além das considerações abaixo, consulte também [Visão geral do compartilhamento de permissões em objetos](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

>[!NOTE]
>
>Um administrador do Workfront pode adicionar ou remover permissões de qualquer item no sistema, para todos os usuários, sem ser o proprietário desses itens.

* O compartilhamento de um documento é semelhante ao compartilhamento de qualquer outro objeto no Workfront. Para obter informações sobre como compartilhar documentos no Workfront, consulte [Compartilhar um objeto](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md).
* Você pode conceder as seguintes permissões a documentos:

   * Exibir
   * Gerenciar

* Você também pode compartilhar um documento publicamente ou em todo o sistema.

   >[!CAUTION]
   >
   >Recomendamos que você tenha cuidado ao compartilhar um objeto contendo informações confidenciais com usuários externos. Isso permite que eles visualizem informações sem ser usuários da Workfront ou parte de sua organização.

* Você pode compartilhar um documento com alguém que não tem uma conta Workfront, adicionando seu endereço de email no campo Conceder acesso ao documento .
* Quando você compartilha um documento, os usuários têm o mesmo acesso a todas as versões do documento e todas as provas do documento.\
   Para obter mais informações sobre a prova no Workfront, consulte o [Tofing](../../review-and-approve-work/proofing/proofing.md) seção.

* É possível herdar permissões de documentos dos objetos aos quais eles estão associados. O administrador do Workfront pode restringir a herança de permissões para documentos em seu nível de acesso.

   Para obter mais informações sobre como restringir permissões herdadas em documentos, consulte [Criar ou modificar níveis de acesso personalizados](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

   Você pode remover manualmente permissões herdadas em documentos. Para obter mais informações, consulte [Remover permissões de objetos](../../workfront-basics/grant-and-request-access-to-objects/remove-permissions-from-objects.md)

* Um documento anexado herda permissões somente do objeto em que foi anexado. Se você criar uma pasta no objeto e mover o documento para a pasta, ela herdará as permissões da pasta. Mas, se você criar uma pasta em um objeto pai ou avô e mover o documento para essa pasta, ele não herdará as permissões dessa pasta.

## Permissões de documento

A tabela a seguir exibe quais permissões você pode conceder aos usuários ao permitir que eles visualizem ou gerenciem documentos:

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
   <td scope="row">Editar Detalhes do Documento</td> 
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
   <td scope="row">Adicionar Aprovadores</td> 
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
   <td scope="row">Atualizações/comentários</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Fazer upload de nova versão</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Excluir versão</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Exibir documento(s)</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Pré-visualização</td> 
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
   <td scope="row">Adicionar/remover</td> 
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

&#42; A ação é compartilhada por Documentos e Pastas de documentos.

&#42;&#42; Você deve ter uma licença de prova separada associada à conta do Workfront para poder provar documentos. Entre em contato com seu gerente de conta para obter uma licença de prova. Para obter mais informações sobre prova no Workfront, consulte [Tofing](../../review-and-approve-work/proofing/proofing.md).
