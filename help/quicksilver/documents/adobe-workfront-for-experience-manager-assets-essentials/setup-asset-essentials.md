---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Configurar a integração do Experience Manager Assets Essentials
description: Conecte seu trabalho ao seu conteúdo no Experience Manager Assets Essentials.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: abaa76e2-bbf1-47d0-8bdc-4e950df4f7ea
source-git-commit: 1ae65d18419bf4235a7c97614b539811643110cc
workflow-type: tm+mt
source-wordcount: '635'
ht-degree: 0%

---

# Configurar a integração do Experience Manager Assets Essentials

Conecte seu trabalho ao seu conteúdo no Experience Manager Assets Essentials&#x200B;:

* Enviar ativos e metadados do Adobe Workfront para o Experience Manager Assets Essentials&#x200B;
* Vincule ativos do Experience Manager Assets Essentials aos seus projetos e tarefas na Workfront&#x200B;
* Facilitar workflows de controle de versão para ativos enviados para o Experience Manager Assets Essentials

>[!NOTE]
>
>Você também pode conectar vários repositórios Experience Manager Assets a um ambiente Workfront, ou vários ambientes Workfront a um repositório Experience Manager Assets em IDs de organização. Siga as instruções de configuração neste artigo para cada integração que você deseja configurar.

## Requisitos de acesso

Você deve ter o seguinte:

<table>
  <tr>
   <td><strong>Plano Adobe Workfront*</strong>
   </td>
   <td>Qualquer
   </td>
  </tr>
  <tr>
   <td><strong>Licenças do Adobe Workfront*</strong>
   </td>
   <td>Plano
   </td>
  </tr>
  <tr>
   <td><strong>licença de Experience Manager</strong>
   </td>
   <td>Padrão
   </td>
  </tr>
  <tr>
   <td><strong>Produto</strong>
   </td>
   <td>Você deve ter o Experience Manager Assets Essentials e ser adicionado ao produto como usuário no Admin Console.
   </td>
  </tr>
  <tr>
   <td><strong>Configurações de nível de acesso</strong>
   </td>
   <td>Você deve ser um administrador do Workfront. Para obter informações sobre administradores do Workfront, consulte <strong>Conceder a um usuário acesso administrativo total</strong>.
   </td>
  </tr>
</table>


*Para descobrir que plano, tipo de licença ou acesso você tem, entre em contato com o administrador do Workfront.


## Configurar a integração

1. Clique no ícone **Menu Principal** no canto superior direito do Adobe Workfront e em **Instalação**.
1. Selecione **Documentos** ![ícone de documentos](assets/document-icon.png) no painel esquerdo e selecione **Integração de Experience Manager**.
1. Selecione **Adicionar Integração de Experience Manager**.
1. Especifique o seguinte:

   <table>
   <tr>
      <td><strong>Nome</strong>
      </td>
      <td>Insira o nome que você deseja que os usuários vejam no botão Adicionar novo na área Documentos.
      </td>
   </tr>
   <tr>
      <td><strong>URL de Navegação</strong>
      </td>
      <td>O sistema preenche automaticamente o URL de navegação. Esse URL é usado para vincular a instância Assets Essentials da sua organização no menu principal para acesso rápido.
      </td>
   </tr>
   <tr>
      <td>
      <strong>Repositório do Experience Manager Assets</strong>
      </td>
      <td>
      O sistema preenche automaticamente o repositório de Experience Manager associado à ID da organização.
      </td>
   </tr>
   </table>

1. Clique em **Salvar** ou vá para a seção [Configurar metadados (opcional)](#set-up-metadata-optional) neste artigo.


## Configurar metadados (opcional)

Mapeie dados de objetos do Workfront para campos de mídia de ativos no Experience Manager Assets. Os metadados são mapeados quando um ativo é enviado por push do Workfront pela primeira vez.


### Pré-requisitos

Antes de começar, você deve

* Configure um esquema de metadados no Experience Manager Assets Essentials conforme explicado em [Configurar o mapeamento de metadados de ativos entre o Adobe Workfront e o Experience Manager Assets](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/assets/integrations/configure-asset-metadata-mapping.html?lang=en).
* (Opcional) Configure campos de formulário personalizados no Workfront. O Workfront tem muitos campos personalizados internos que você pode usar. No entanto, você também pode criar seus próprios campos personalizados. Para obter mais informações, consulte [Criar um formulário com o designer de formulário](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

## Campos Workfront e Experience Manager Assets compatíveis

### Palavra-chave AEM

Você pode mapear qualquer campo compatível com o Workfront para uma palavra-chave no Experience Manager Assets Essentials.

Para vincular um campo a uma palavra-chave, selecione `xcm:keywords` na lista suspensa de campos do Experience Manager Assets na área de mapeamento de metadados.

Para mapear vários campos de texto de linha única para palavras-chave, insira uma lista separada por vírgulas dos valores de palavra-chave no lado do Workfront do mapeamento de metadados e `xcm:keywords` no lado do Experience Manager Assets. Cada valor de campo mapeia para uma palavra-chave separada. Você pode usar um campo calculado para combinar vários campos do Workfront em um único campo de texto separado por vírgulas.

<!--
Look for essentials article
For more information on keywords in Experience Manager Assets, including how to create and manage keywords, see [Administering Tags]( https://experienceleague.adobe.com/docs/experience-manager-64/administering/contentmanagement/tags.html?lang=en).
-->

+++


### Ativos

Os metadados são mapeados quando um ativo é enviado por push do Workfront pela primeira vez. Documentos com campos incorporados ou personalizados são mapeados automaticamente para os campos especificados na primeira vez que um ativo é enviado ao Experience Manager Assets Essentials.

1. Na coluna **Campo do Workfront**, escolha um campo interno ou personalizado do Workfront.
   >[!NOTE]
   >
   >Você pode mapear um único campo do Workfront para vários campos do Experience Manager Assets. Não é possível mapear vários campos do Workfront para um único campo do Experience Manager Assets.
1. No campo **Experience Manager**, escolha um campo do Experience Manager Assets.

   Para mapear um campo do Workfront para uma marca Experience Manager Assets, selecione `xcm:keywords`.
1. Repita as etapas 1 e 2 conforme necessário.
   ![habilitar metadados](assets/metadata-assets-essentials.png)
1. Clique em **Salvar** ou vá para a seção [Configurar pastas vinculadas (opcional)](#set-up-linked-folders-optional) neste artigo.


## Configurar pastas vinculadas (opcional)

{{setup-linked-folder}}
