---
content-type: reference
product-area: documents;workfront-integrations
navigation-topic: documents-navigation-topic
title: Criar uma pasta vinculada ao Experience Manager Assets ou Assets Essentials
description: É possível criar uma pasta vinculada ao Experience Manager Assets ou ao Assets Essentials no Workfront.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: eb2b3b21-bc0b-45d3-85fa-1715cf927cb7
source-git-commit: 90eb99fa46e706a53427f995d484e2fb42e9c293
workflow-type: tm+mt
source-wordcount: '488'
ht-degree: 11%

---

# Criar uma pasta vinculada ao Experience Manager Assets ou Assets Essentials

É possível criar uma pasta vinculada ao Experience Manager Assets ou ao Assets Essentials no Workfront. Como a pasta está vinculada, qualquer ativo adicionado à pasta será exibido automaticamente no Workfront e no Experience Manager. Não é necessário enviar manualmente o ativo se ele estiver em uma pasta vinculada.

Se um ativo for excluído ou movido de uma pasta vinculada dentro do Experience Manager Assets ou do Assets Essentials, a Workfront manterá uma cópia do ativo na área Projeto > Documentos.

>[!NOTE]
>
>Essa funcionalidade não está disponível na área de novos documentos.<br>
>Se sua organização usar armazenamento corporativo, você verá a nova área de documentos ao acessar documentos no Workfront. A partir daí, você pode adicionar ativos do Experience Manager Assets ou do Assets Essentials, mas não poderá criar uma pasta vinculada.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo.

<table>
  <tr>
   <td><strong>Pacote do Adobe Workfront</strong>
   </td>
   <td>Qualquer
   </td>
  </tr>
  <tr>
   <td><strong>licenças do Adobe Workfront</strong>
   </td>
   <td>
   <p>Padrão</p>
   <p>Plano</p>
   </td>
  </tr>
  <tr>
   <td><strong>Produtos adicionais</strong>
   </td>
   <td>Você deve ter o Experience Manager Assets as a Cloud Service ou o Assets Essentials e deve ser adicionado ao produto como usuário.
   </td>
  </tr>
  <tr>
   <td><strong>Permissões do Experience Manager</strong>
   </td>
   <td>Você deve ter acesso de gravação à pasta de destino na integração do Experience Manager.
   </td>
  </tr>
  <tr>
   <td><strong>Configurações de nível de acesso</strong>
   </td>
   <td>Você deve ser um administrador do Workfront para configurar uma integração com o Experience Manager. Após a configuração, os usuários com uma licença de Plano podem configurar pastas vinculadas em projetos individuais.
   </td>
  </tr>
</table>

Para obter mais detalhes sobre as informações contidas nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Pré-requisitos

Antes de começar,

* O administrador do Workfront deve configurar uma integração do Experience Manager. Para obter mais informações, consulte [Configurar a integração do Experience Manager Assets as a Cloud Service](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md) ou [Configurar a integração do Experience Manager Assets Essentials](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).


## Criar uma pasta vinculada

A pasta vinculada é criada no local especificado pelo administrador do Workfront quando ele configura a integração. Cada integração pode ter apenas um local de pasta para pastas vinculadas.

O nome da pasta vinculada é criado automaticamente com base no Portfolio, Programa, Projeto associado a ele e não pode ser alterado. Se o projeto não estiver associado a um Portfolio ou Programa, a pasta vinculada exibirá o nome do projeto e a data de criação.

>[!NOTE]
>
>You cannot create a new document or proof version inside of a linked folder.


To create a linked folder:

1. Go to the Project where you want the folder.
1. Select **Add New**, then go to the Experience manager integration your administrator set up.

   >[!NOTE]
   >
   >The Workfront administrator can choose any name for this integration, so it might not specifically mention Experience Manager Assets or Assets Essentials.

1. Select **Create linked folder**. The system automatically creates a folder in Experience Manager based on the location specified when the integration was set up.
   ![create a linked folder](assets/linked-folder.png)
