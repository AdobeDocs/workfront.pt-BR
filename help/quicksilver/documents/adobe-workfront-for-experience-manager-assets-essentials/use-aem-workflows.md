---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Usar fluxos de trabalho na integração do Experience Manager Assets Essentials
description: Usar fluxos de trabalho na integração do Experience Manager Assets Essentials
author: Courtney, Becky
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: 4c1e5ec1-3fd1-4527-ba8a-9db1a2350f69
source-git-commit: 706e531be6f6269a927f94fee4d2c37d9367c9af
workflow-type: tm+mt
source-wordcount: '816'
ht-degree: 0%

---

# Usar fluxos de trabalho na integração do Experience Manager Assets

Um fluxo de trabalho é um conjunto de ações que conectam o Workfront ao Adobe Experience Manager as a Cloud Service. Um administrador do Workfront pode configurar fluxos de trabalho no Workfront e atribuí-los a Modelos de projeto. Quando um Projeto é criado usando um Modelo de projeto ao qual um fluxo de trabalho é atribuído, as ações definidas no fluxo de trabalho são acionadas.

>[!NOTE]
>
>Os fluxos de trabalho estão disponíveis somente em uma integração com o Adobe Experience Manager as a Cloud Service. Eles não estão disponíveis em integrações com o Adobe Experience Manager Assets Essentials.


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
   <td>Solicitação ou superior
   </td>
  </tr>
  <tr>
   <td><strong>Produto</strong>
   </td>
   <td><p>Você deve ter o Experience Manager Assets as a Cloud Service ou Assets Essentials e ser adicionado ao produto como usuário no Admin Console.</p><p>Você deve ter acesso de gravação ao repositório no Adobe Experience Manager.</p>
   </td>
  </tr>
  <tr>
   <td><strong>Configurações de nível de acesso*</strong>
   </td>
   <td>Editar acesso a documentos
<p>
<strong>Nota: </strong>Se você ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <strong>Criar ou modificar níveis de acesso personalizados</strong>.
   </td>
  </tr>
  <tr>
   <td><strong>Permissões de objeto</strong>
   </td>
   <td>Gerenciar acesso ou superior no projeto 
<p>
Para obter informações sobre como solicitar acesso adicional, consulte <strong>Solicitar acesso a objetos </strong>.
   </td>
  </tr>
</table>

## Pré-requisitos

Antes de começar,

* O administrador do Workfront deve configurar os workflows em uma integração com o Adobe Experience Manager. Para obter mais informações, consulte [Configurar a integração as a Cloud Service do Experience Manager Assets](../../administration-and-setup/configure-integrations/configure-aacs-integration.md#set-up-workflows-optional).

## Adicionar um fluxo de trabalho a um modelo

É possível adicionar um fluxo de trabalho a um modelo de projeto. O fluxo de trabalho será aplicado a qualquer projeto criado a partir do modelo.

1. Abra um template clicando em **Modelos** no Menu principal, depois selecione o modelo na lista.
1. Clique em **Experience Manager Assets** no painel de navegação esquerdo.

   >[!NOTE]
   >
   >Se a seção Experience Manager Assets não estiver visível na navegação à esquerda, o administrador do Workfront não ativou os workflows da organização. <!--Is this right?-->

1. No **Selecionar uma integração para o campo de workflows automatizados**, selecione a integração com os fluxos de trabalho que deseja usar para projetos criados a partir deste modelo.
1. (Opcional) Edite quaisquer valores de fluxo de trabalho que deseja aplicar aos projetos criados a partir deste modelo.

   Para obter instruções sobre workflows específicos, consulte [Editar valores de fluxo de trabalho em um projeto](#edit-workflow-values-in-a-project) neste artigo.

   Somente os workflows que foram ativados na área Experience Manager da Configuração estão disponíveis em modelos ou projetos.

1. As alterações são salvas automaticamente. <!-- do they though??-->

## Adicionar um fluxo de trabalho a um projeto

Você pode adicionar um fluxo de trabalho ao criar um projeto ou adicionar um fluxo de trabalho a um projeto existente. Em ambos os casos, você usará um modelo de projeto para adicionar o fluxo de trabalho.

### Adicionar um fluxo de trabalho ao criar um projeto

1. Comece a criar um projeto.

   Para obter instruções, consulte [Criar um projeto usando um modelo](/help/quicksilver/manage-work/projects/create-projects/create-project-from-template.md).

1. Ao selecionar um modelo para o projeto, selecione o modelo que contém os fluxos de trabalho que deseja usar para esse projeto.
1. (Opcional) Edite quaisquer valores de workflow para o projeto, conforme descrito em [Editar valores de fluxo de trabalho em um projeto](#edit-workflow-values-in-a-project).

   Somente os workflows que foram ativados na área Experience Manager da Configuração estão disponíveis em modelos ou projetos.


### Adicionar um fluxo de trabalho a um projeto existente

1. Comece a adicionar um modelo ao projeto.

   Para obter instruções, consulte [Anexar um modelo a um projeto](/help/quicksilver/manage-work/projects/create-and-manage-templates/attach-template-to-project.md).

1. Ao selecionar um modelo para o projeto, selecione o modelo que contém os fluxos de trabalho que deseja usar para esse projeto.
1. (Opcional) Edite quaisquer valores de workflow para o projeto, conforme descrito em [Editar valores de fluxo de trabalho em um projeto](#edit-workflow-values-in-a-project).

   Somente os workflows que foram ativados na área Experience Manager da Configuração estão disponíveis em modelos ou projetos.

### Editar valores de fluxo de trabalho em um projeto

É possível editar valores de fluxo de trabalho no nível do projeto. Os valores do fluxo de trabalho no nível do projeto substituem os valores definidos no modelo do projeto, que substitui os valores padrão definidos na integração do Adobe Experience Manager Assets.

Todos os valores de workflow podem ser encontrados em:

* A seção Workflows da janela Criar projeto ou Editar projeto.
* A seção Adobe Experience Manager da navegação à esquerda.


  >[!NOTE]
  >
  >Se essas áreas não estiverem visíveis, o administrador do Workfront não ativou os Fluxos de trabalho para sua organização.

#### Pastas vinculadas

Para editar o fluxo de trabalho de pastas vinculadas:

1. Alternar **[!UICONTROL Criar Pasta vinculada]** ligado ou desligado, conforme desejado.
1. (Condicional) Se estiver ativando pastas vinculadas, escolha um caminho de pasta para indicar onde deseja que todas as pastas vinculadas sejam associadas a essa integração.
1. Clique em **[!UICONTROL Salvar]** se você estiver usando o [!UICONTROL Criar projeto] ou [!UICONTROL Editar projeto] janela.

   Ou

   Se você estiver na [!DNL Adobe Experience Manager area], as alterações são salvas automaticamente. <!--Do they though?-->


#### Publicar ativos

Para editar o fluxo de trabalho de publicação de ativos:

1. Alternar **Publicar ativos automaticamente** ligado ou desligado, conforme desejado.
1. (Condicional) Se você estiver ativando a publicação, selecione se deseja publicar no serviço de publicação, no portal de marcas ou em ambos.
1. Clique em **[!UICONTROL Salvar]** se você estiver usando o [!UICONTROL Criar projeto] ou [!UICONTROL Editar projeto] janela.

   Ou

   Se você estiver na [!DNL Adobe Experience Manager area], as alterações são salvas automaticamente. <!--Do they though?-->


