---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Configurar a integração do Experience Manager Assets Essentials
description: Conecte seu trabalho com seu conteúdo no Experience Manager Assets Essentials - EDITE-ME.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: abaa76e2-bbf1-47d0-8bdc-4e950df4f7ea
source-git-commit: b874cb1a99840db11d6d55c86b7f779aa3e6ef35
workflow-type: tm+mt
source-wordcount: '531'
ht-degree: 5%

---

# Configurar a integração do Experience Manager Assets Essentials

Conecte seu trabalho com seu conteúdo no Experience Manager Assets Essentials &#x200B;:

* Envie ativos e metadados do Adobe Workfront para o Experience Manager Assets Essentials &#x200B;
* Vincule ativos do Experience Manager Assets Essentials a seus projetos e tarefas no Workfront &#x200B;
* Facilitar os fluxos de trabalho de controle de versão para ativos enviados ao Experience Manager Assets Essentials

Também é possível conectar vários repositórios Experience Manager Assets a um ambiente Workfront ou vários ambientes Workfront a um repositório Experience Manager Assets por meio de IDs de organização. Siga as instruções de configuração neste artigo para cada integração que você deseja configurar.

## Requisitos de acesso

Você deve ter o seguinte:

<table>
  <tr>
   <td><strong>Plano Adobe Workfront*</strong>
   </td>
   <td>Qualquer Um
   </td>
  </tr>
  <tr>
   <td><strong>Licenças Adobe Workfront*</strong>
   </td>
   <td>Plano
   </td>
  </tr>
  <tr>
   <td><strong>licença Experience Manager</strong>
   </td>
   <td>Padrão
   </td>
  </tr>
  <tr>
   <td><strong>Produto</strong>
   </td>
   <td>Você deve ter o Experience Manager Assets Essentials e deve ser adicionado ao produto como usuário no Admin Console.
   </td>
  </tr>
  <tr>
   <td><strong>Configurações de nível de acesso</strong>
   </td>
   <td>Você deve ser um administrador do Workfront. Para obter informações sobre administradores do Workfront, consulte <strong>Conceder ao usuário acesso administrativo total</strong>.
   </td>
  </tr>
</table>


*Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.


## Configurar a integração

1. Clique no botão **Menu principal** no canto superior direito do Adobe Workfront, em seguida, clique em **Configuração**.
1. Selecionar  **Documentos** ![ícone de documentos](assets/document-icon.png) no painel esquerdo e selecione **Integração do Experience Manager**.
1. Selecionar **Adicionar integração de Experience Manager**.
1. Especifique o seguinte:

   <table>
   <tr>
      <td><strong>Nome</strong>
      </td>
      <td>Insira o nome que deseja que os usuários vejam no botão Add new na área Documents .
      </td>
   </tr>
   <tr>
      <td><strong>URL de navegação</strong>
      </td>
      <td>O sistema preenche automaticamente o URL de navegação. Esse URL é usado para vincular à instância do Assets Essentials de sua organização no Menu principal para acesso rápido.
      </td>
   </tr>
   <tr>
      <td>
      <strong>Repositório Experience Manager Assets</strong>
      </td>
      <td>
      O sistema preenche automaticamente o repositório do Experience Manager associado à ID da organização.
      </td>
   </tr>
   </table>

1. Clique em **Salvar** ou vá para a [Configurar metadados (opcional)](#set-up-metadata-optional) neste artigo.


## Configurar metadados (opcional)

Mapeie dados de objetos do Workfront para campos de mídia do Experience Manager Assets. Os metadados são mapeados quando um ativo é enviado por push do Workfront pela primeira vez.


### Pré-requisitos

Antes de começar, você deve

* Configure um esquema de metadados no Experience Manager Assets Essentials, conforme explicado em [Configurar o mapeamento de metadados de ativos entre o Adobe Workfront e a Experience Manager Assets](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/assets/integrations/configure-asset-metadata-mapping.html?lang=en).
* (Opcional) Configure campos de formulário personalizados no Workfront. O Workfront tem muitos campos personalizados incorporados que podem ser usados. No entanto, também é possível criar seus próprios campos personalizados. Para obter mais informações, consulte [Criar ou editar um formulário personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).


### Ativos

Os metadados mapeiam quando um ativo é enviado do Workfront pela primeira vez. Documentos com os campos incorporados ou personalizados mapeiam automaticamente para os campos especificados na primeira vez que um ativo é enviado para o Experience Manager Assets Essentials.

1. No **Campo Workfront** escolha um campo Workfront incorporado ou personalizado.
   >[!NOTE]
   >
   >Você pode mapear um único campo do Workfront para vários campos do Experience Manager Assets. Não é possível mapear vários campos do Workfront para um único campo do Experience Manager Assets.
1. No **Experience Manager** escolha um campo Experience Manager Assets.
1. Repita as etapas 1 e 2 conforme necessário.
   ![habilitar metadados](assets/metadata-assets-essentials.png)
1. Clique em **Salvar** ou vá para a [Configurar pastas vinculadas (opcional)](#set-up-linked-folders-optional) neste artigo.


## Configurar pastas vinculadas (opcional)

{{setup-linked-folder}}
