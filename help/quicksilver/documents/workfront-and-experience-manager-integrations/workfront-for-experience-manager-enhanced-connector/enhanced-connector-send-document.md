---
product-area: documents;workfront-integrations
navigation-topic: workfront-for-experience-manager-enhanced-connector
title: Enviar um documento com o conector aprimorado
description: Você pode enviar documentos do Workfront para o Experience Manager Assets. Os documentos carregados e enviados do Workfront para o Experience Manager Assets ainda contam com o armazenamento geral de documentos. O Assets vinculado a partir do Experience Manager Assets não conta para o armazenamento geral.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: d687d2db-28e0-45e8-9d60-8419921f02e9
source-git-commit: 3f9a824780f2ded914d461a473aef3b6ecfa8701
workflow-type: tm+mt
source-wordcount: '409'
ht-degree: 1%

---

# Enviar um documento com o conector aprimorado

Você pode enviar documentos do Workfront para o Experience Manager Assets. Os documentos carregados e enviados do Workfront para o Experience Manager Assets ainda contam com o armazenamento geral de documentos. O Assets vinculado a partir do Experience Manager Assets não conta para o armazenamento geral.

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
   <p>Solicitação ou superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produtos adicionais</td> 
   <td>Experience Manager Assets </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a documentos</p> s="MCXref xref"&gt;Crie ou modifique níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Acesso de Visualização ou superior em Documentos</p></td> 
  </tr> 
 </tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).
+++

## Pré-requisitos

Antes de começar, você deve

* Instale o conector aprimorado do Workfront para Experience Manager.

## Enviar um documento para o Experience Manager Assets

Quando um usuário envia um documento do Workfront para o Experience Manager Assets, os metadados mapeados são transferidos ao longo do documento. Se configurados, os metadados são sincronizados continuamente sempre que uma alteração é feita.

Para enviar um documento:

1. Vá para a área **Documentos** do Workfront e selecione o documento que deseja enviar.
1. Clique em **Enviar para** e escolha a integração do Experience Manager Assets configurada pelo administrador.

   >[!NOTE]
   >
   >Qualquer nome pode ser escolhido para essa integração, portanto, ele pode não mencionar especificamente o Experience Manager Assets.

   ![Enviar para](assets/copy-of-send-to-in-toolbar-350x149.png)

1. Escolha para onde deseja que o ativo vá e clique em **Selecionar pasta**.
1. Ao encontrar o destino desejado, clique em **Salvar**.

## Enviar uma nova versão para o Experience Manager Assets

É possível adicionar uma nova versão a um documento carregado anteriormente no Workfront. Para obter mais informações, consulte [Carregar uma nova versão de um documento](../../../documents/managing-documents/upload-new-document-version.md). Depois que a versão mais recente for carregada, você poderá enviá-la para o Experience Manager Assets. Se um campo mapeado no Workfront tiver sido alterado, a nova versão atualizará os metadados no Experience Manager Assets quando ele enviar.

Para enviar a versão mais recente:

1. Vá para a área **Documentos** no Workfront e localize o documento.
1. Clique em **Enviar para** e escolha a integração do Experience Manager Assets configurada pelo administrador.

   >[!NOTE]
   >
   >Qualquer nome pode ser escolhido para essa integração, portanto, ele pode não mencionar especificamente o Experience Manager Assets.

   ![Enviar para](assets/copy-of-send-to-in-toolbar-350x149.png)

1. Clique em **Salvar**. A nova versão é salva no mesmo local da versão anterior.
