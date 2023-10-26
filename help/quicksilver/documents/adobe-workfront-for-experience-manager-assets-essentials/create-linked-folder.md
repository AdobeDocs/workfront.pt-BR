---
content-type: reference
product-area: documents;workfront-integrations
navigation-topic: documents-navigation-topic
title: Criar uma pasta vinculada ao Experience Manager Assets ou Assets Essentials
description: É possível criar uma pasta vinculada ao Experience Manager Assets ou Assets Essentials no Workfront.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: eb2b3b21-bc0b-45d3-85fa-1715cf927cb7
source-git-commit: 1744e6f2b78c64ba2fa4856d9c6a0611404e4458
workflow-type: tm+mt
source-wordcount: '383'
ht-degree: 0%

---

# Criar uma pasta vinculada ao Experience Manager Assets ou Assets Essentials

É possível criar uma pasta vinculada ao Experience Manager Assets ou Assets Essentials no Workfront. Como a pasta está vinculada, qualquer ativo adicionado à pasta será exibido automaticamente no Workfront e no Experience Manager. Não é necessário enviar manualmente o ativo se ele estiver em uma pasta vinculada.


## Requisitos de acesso

Você deve ter o seguinte:

<table>
  <tr>
   <td><strong>plano do Adobe Workfront*</strong>
   </td>
   <td>Qualquer Um
   </td>
  </tr>
  <tr>
   <td><strong>Licenças da Adobe Workfront*</strong>
   </td>
   <td>Plano
   </td>
  </tr>
  <tr>
   <td><strong>Produto</strong>
   </td>
   <td>Você deve ter o Experience Manager Assets as a Cloud Service ou Assets Essentials e ser adicionado ao produto como usuário.
   </td>
  </tr>
  <tr>
   <td><strong>permissões de Experience Manager</strong>
   </td>
   <td>Você deve ter acesso de gravação à pasta de destino na integração do Experience Manager.
   </td>
  </tr>
  <tr>
   <td><strong>Configurações de nível de acesso</strong>
   </td>
   <td>Você deve ser um administrador do Workfront para configurar uma integração de Experience Manager. Após a configuração, os usuários com uma licença de Plano podem configurar pastas vinculadas em projetos individuais.
   </td>
  </tr>
</table>


*Para descobrir que plano, tipo de licença ou acesso você tem, entre em contato com o administrador do Workfront.


## Pré-requisitos

Antes de começar,

* O administrador do Workfront deve configurar uma integração de Experience Manager. Para obter mais informações, consulte [Configurar a integração as a Cloud Service do Experience Manager Assets](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md) ou [Configurar a integração do Experience Manager Assets Essentials](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).


## Criar uma pasta vinculada

A pasta vinculada é criada no local especificado pelo administrador do Workfront quando ele configura a integração. Cada integração pode ter apenas um local de pasta para pastas vinculadas.

O nome da pasta vinculada é criado automaticamente com base no Portfolio, Programa, Projeto associado a ele e não pode ser alterado. Se o projeto não estiver associado a um Portfolio ou Programa, a pasta vinculada exibirá o nome do projeto e a data de criação.

Para criar uma pasta vinculada:



1. Vá para o Projeto onde deseja colocar a pasta.
1. Selecionar **Adicionar novo**, em seguida, acesse a integração do Experience Manager configurada pelo administrador.

   >[!NOTE]
   >
   >O administrador do Workfront pode escolher qualquer nome para essa integração, portanto, pode ser que ele não mencione especificamente o Experience Manager Assets ou o Assets Essentials.

1. Selecionar **Criar pasta vinculada**. O sistema cria automaticamente uma pasta no Experience Manager com base no local especificado quando a integração foi configurada.
   ![criar uma pasta vinculada](assets/linked-folder.png)
