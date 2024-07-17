---
title: Vincular ativos e pastas ao conector aprimorado
description: Você pode vincular um ativo ou pasta do Experience Manager Assets a qualquer objeto do Workfront que suporte documentos.
author: Courtney
draft: Probably
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: 35c80f6a-419b-4237-8139-f59ab7bbd5c7
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '543'
ht-degree: 0%

---

# Vincular ativos e pastas ao conector aprimorado

Você pode vincular um ativo ou pasta do Experience Manager Assets a qualquer objeto do Workfront que suporte documentos. O Assets enviado do Experience Manager Assets não conta para o armazenamento geral de documentos no Workfront. Os documentos carregados e enviados do Workfront para o Experience Manager Assets contam para o armazenamento geral.

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront*</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Solicitação ou superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produto</td> 
   <td>Experience Manager Assets </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a documentos</p> <p>Observação: se você ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Acesso de visualização ou superior em um documento</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso aos objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qual plano, tipo de licença ou acesso você tem, contate o administrador do Workfront.

## Pré-requisitos

Antes de começar, você deve

* Instale o conector aprimorado do Workfront para Experience Manager

## Vincular um ativo do Experience Manager Assets

É possível vincular um ativo do Experience Manager Assets ao Workfront. Depois que o ativo for vinculado, você poderá

* [Criar uma prova de um ativo vinculado para o Experience Manager Assets](../../../documents/workfront-and-experience-manager-integrations/workfront-for-experience-manager-enhanced-connector/enhanced-connector-proof-asset.md)
* [Fazer upload de uma nova versão de um documento](../../../documents/managing-documents/upload-new-document-version.md)

Para vincular um ativo ao Experience Manager Assets:

1. Vá para a área **Documentos** no Workfront onde deseja adicionar o documento.
1. Clique em **Adicionar novo** e escolha a integração do Experience Manager Assets configurada pelo administrador.

   >[!NOTE]
   >
   >Qualquer nome pode ser escolhido para essa integração, portanto, ele pode não mencionar especificamente o Experience Manager Assets.

1. Selecione os ativos desejados.

   ![](assets/select-an-asset.png)

1. Clique em **Link**.

## Vincular uma pasta do Experience Manager Assets

As permissões para visualizar ativos individuais dentro de uma pasta dependem das permissões do Experience Manager Assets.

Para vincular uma pasta ao Experience Manager Assets:

1. Vá para a área **Documentos** no Workfront onde deseja adicionar o documento.
1. Clique em **Adicionar novo** e escolha a integração do Experience Manager Assets configurada pelo administrador.

   >[!NOTE]
   >
   >Qualquer nome pode ser escolhido para essa integração, portanto, ele pode não mencionar especificamente o Experience Manager Assets.

1. Selecione as pastas desejadas.

   ![](assets/select-a-folder.png)

1. Clique em **Link**.

## Vincular uma nova versão do Experience Manager Assets

Você pode obter um novo ativo do Experience Manager Assets e adicioná-lo a um ativo existente como uma nova versão no Workfront. Se o documento já estiver vinculado e uma nova versão for adicionada no Experience Manager Assets, a nova versão será exibida automaticamente no Workfront.

>[!TIP]
>
>Você pode exibir todas as versões de um ativo se acessar **Detalhes do documento** > **Versões**.

Para vincular uma nova versão do Experience Manager Assets:

1. Vá para a área **Documentos** no Workfront onde deseja adicionar o documento.
1. Selecione o ativo que deseja substituir por uma nova versão. Não é possível criar uma nova versão de um ativo em uma pasta vinculada.
1. Clique em **Adicionar novo** e escolha a integração do Experience Manager Assets configurada pelo administrador.

   >[!NOTE]
   >
   >Qualquer nome pode ser escolhido para essa integração, portanto, ele pode não mencionar especificamente o Experience Manager Assets.

1. Selecione o ativo desejado.

   ![](assets/select-an-asset.png)

1. Clique em **Link**.
