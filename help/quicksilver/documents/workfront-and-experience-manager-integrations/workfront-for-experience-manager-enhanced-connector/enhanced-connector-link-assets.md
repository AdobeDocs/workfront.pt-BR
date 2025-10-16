---
title: Vincular ativos e pastas ao conector aprimorado
description: Você pode vincular um ativo ou pasta do Experience Manager Assets a qualquer objeto do Workfront que suporte documentos.
author: Courtney
draft: Probably
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: 35c80f6a-419b-4237-8139-f59ab7bbd5c7
source-git-commit: 3f9a824780f2ded914d461a473aef3b6ecfa8701
workflow-type: tm+mt
source-wordcount: '519'
ht-degree: 0%

---


# Vincular ativos e pastas ao conector aprimorado

Você pode vincular um ativo ou pasta do Experience Manager Assets a qualquer objeto do Workfront que suporte documentos. O Assets enviado do Experience Manager Assets não conta para o armazenamento geral de documentos no Workfront. Os documentos carregados e enviados do Workfront para o Experience Manager Assets contam para o armazenamento geral.


>[!NOTE]
>
>Os arquivos do Excel vinculados por meio do conector aprimorado não podem ser visualizados no Workfront. Você deve baixar o arquivo para acessá-lo.

## Requisitos de acesso

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
   <td> 
   <p>Colaborador ou superior</p>
   <p>Solicitação ou superior</p> 
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produtos adicionais</td> 
   <td>Experience Manager Assets </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a documentos</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Acesso de visualização ou superior em um documento</p> </td> 
  </tr> 
 </tbody> 
</table>


Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

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

   ![Selecione um ativo](assets/select-an-asset.png)

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

   ![Selecionar uma pasta](assets/select-a-folder.png)

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

   ![Selecione um ativo](assets/select-an-asset.png)

1. Clique em **Link**.
