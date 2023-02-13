---
product-area: documents;workfront-integrations
navigation-topic: workfront-for-experience-manager-enhanced-connector
title: Enviar um documento com o conector aprimorado
description: Você pode enviar documentos do Workfront para o Experience Manager Assets. Os documentos carregados e enviados do Workfront para o Experience Manager Assets ainda contam em relação ao armazenamento geral de documentos. Os ativos vinculados do Experience Manager Assets não contam para o armazenamento geral.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: d687d2db-28e0-45e8-9d60-8419921f02e9
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '453'
ht-degree: 1%

---

# Enviar um documento com o conector aprimorado

Você pode enviar documentos do Workfront para o Experience Manager Assets. Os documentos carregados e enviados do Workfront para o Experience Manager Assets ainda contam em relação ao armazenamento geral de documentos. Os ativos vinculados do Experience Manager Assets não contam para o armazenamento geral.

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
   <td> <p>Editar acesso a documentos</p> <p>Observação: Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Exibir acesso ou superior em Documentos</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

## Pré-requisitos

Antes de começar, você deve

* Instale o Workfront para o conector Experience Manager enhanced.

## Enviar um documento para a Experience Manager Assets

Quando um usuário envia um documento do Workfront para o Experience Manager Assets, os metadados mapeados são transferidos ao longo do documento. Se configurado, os metadados são sincronizados continuamente cada vez que uma alteração é feita.

Para enviar um documento:

1. Vá para o **Documentos** no Workfront e selecione o documento que deseja enviar.
1. Clique em **Enviar para** e escolha a integração do Experience Manager Assets configurada pelo administrador.

   >[!NOTE]
   >
   >Qualquer nome pode ser escolhido para essa integração, portanto, pode não mencionar especificamente o Experience Manager Assets.

   ![](assets/copy-of-send-to-in-toolbar-350x149.png)

1. Escolha para onde deseja direcionar o ativo e clique em **Selecionar pasta**.
1. Ao encontrar o destino desejado, clique em **Salvar**.

## Enviar uma nova versão para o Experience Manager Assets

Você pode adicionar uma nova versão a um documento que tenha carregado anteriormente no Workfront. Para obter mais informações, consulte [Fazer upload de uma nova versão de um documento](../../../documents/managing-documents/upload-new-document-version.md). Depois que a versão mais recente for carregada, você poderá enviá-la para o Experience Manager Assets. Se um campo mapeado no Workfront tiver sido alterado, a nova versão atualizará os metadados no Experience Manager Assets quando ele enviar.

Para enviar a versão mais recente:

1. Vá para o **Documentos** no Workfront e localize o documento.
1. Clique em **Enviar para** e escolha a integração do Experience Manager Assets configurada pelo administrador.

   >[!NOTE]
   >
   >Qualquer nome pode ser escolhido para essa integração, portanto, pode não mencionar especificamente o Experience Manager Assets.

   ![](assets/copy-of-send-to-in-toolbar-350x149.png)

1. Clique em **Salvar**. A nova versão salva no mesmo local que a versão anterior.
