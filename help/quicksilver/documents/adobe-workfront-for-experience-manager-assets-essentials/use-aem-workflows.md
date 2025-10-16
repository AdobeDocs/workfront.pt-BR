---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Usar fluxos de trabalho na integração do Experience Manager Assets Essentials
description: Usar fluxos de trabalho na integração do Experience Manager Assets Essentials
author: Courtney, Becky
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: 4c1e5ec1-3fd1-4527-ba8a-9db1a2350f69
source-git-commit: 430751f0e38c6c45145c965398990ee3652f36fe
workflow-type: tm+mt
source-wordcount: '1012'
ht-degree: 0%

---

# Usar fluxos de trabalho na integração do Experience Manager Assets

Um fluxo de trabalho é um conjunto de ações que conectam o Workfront ao Adobe Experience Manager as a Cloud Service. Um administrador do Workfront pode configurar fluxos de trabalho no Workfront e atribuí-los a Modelos de projeto.

Quando um Projeto é criado usando um Modelo de projeto ao qual um fluxo de trabalho é atribuído, as ações definidas no fluxo de trabalho são acionadas.

>[!NOTE]
>
>Os fluxos de trabalho estão disponíveis somente em uma integração com o Adobe Experience Manager as a Cloud Service. Não estão disponíveis em integrações com o Adobe Experience Manager Assets Essentials.


## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacote do Adobe Workfront</td> 
   <td> <p> Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenças do Adobe Workfront</td> 
   <td> 
   <p>Colaborador ou superior</p> 
   <p>Solicitação ou superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produtos adicionais</td> 
   <td>Você deve ter o Experience Manager as a Cloud Service ou o Assets Essentials e deve ser adicionado ao produto como usuário na Admin Console.</td> 
  </tr> 
   <tr> 
    <td role="rowheader">Permissões do Experience Manager</td> 
    <td>Você deve ter acesso de gravação à pasta.</td> 
   </tr>
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Editar acesso a documentos</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Exibir acesso ou superior</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Pré-requisitos

Antes de começar,

* O administrador do Workfront deve configurar os workflows em uma integração com o Adobe Experience Manager. Para obter mais informações, consulte [Configurar a integração do Experience Manager Assets as a Cloud Service](../../administration-and-setup/configure-integrations/configure-aacs-integration.md#set-up-workflows-optional).

## Adicionar um fluxo de trabalho a um modelo

É possível adicionar um fluxo de trabalho a um modelo de projeto. O fluxo de trabalho será aplicado a qualquer projeto criado a partir do modelo.

1. Abra um modelo clicando em **Modelos** no Menu Principal e selecionando o modelo na lista.
1. Clique em **Experience Manager Assets** no painel de navegação esquerdo.

   >[!NOTE]
   >
   >Se a seção Experience Manager Assets não estiver visível na navegação à esquerda, o administrador do Workfront não ativou os workflows da organização. <!--Is this right?-->

1. No campo **Selecionar uma integração para fluxos de trabalho automatizados**, selecione a integração com os fluxos de trabalho que deseja usar para projetos criados a partir deste modelo.
1. (Opcional) Edite quaisquer valores de fluxo de trabalho que deseja aplicar aos projetos criados a partir deste modelo.

   Para obter instruções sobre fluxos de trabalho específicos, consulte [Editar valores de fluxo de trabalho em um projeto](#edit-workflow-values-in-a-project) neste artigo.

   Somente os workflows que foram ativados na área Experience Manager da Configuração estão disponíveis em modelos ou projetos.

1. As alterações são salvas automaticamente. <!-- do they though??-->

## Adicionar um fluxo de trabalho a um projeto

Você pode adicionar um fluxo de trabalho ao criar um projeto ou adicionar um fluxo de trabalho a um projeto existente. Em ambos os casos, você usará um modelo de projeto para adicionar o fluxo de trabalho.

### Adicionar um fluxo de trabalho ao criar um projeto

1. Comece a criar um projeto.

   Para obter instruções, consulte [Criar um projeto usando um modelo](/help/quicksilver/manage-work/projects/create-projects/create-project-from-template.md).

1. Ao selecionar um modelo para o projeto, selecione o modelo que contém os fluxos de trabalho que deseja usar para esse projeto.
1. (Opcional) Edite quaisquer valores de fluxo de trabalho para o projeto, conforme descrito em [Editar valores de fluxo de trabalho em um projeto](#edit-workflow-values-in-a-project).

   Somente os workflows que foram ativados na área Experience Manager da Configuração estão disponíveis em modelos ou projetos.


### Adicionar um fluxo de trabalho a um projeto existente

>[!NOTE]
>
>Os fluxos de trabalho executados quando um projeto é criado (como criação de pasta vinculada) não são executados quando o modelo é anexado a um projeto existente. Eles só são executados quando um projeto é criado a partir de um modelo.

1. Comece a adicionar um modelo ao projeto.

   Para obter instruções, consulte [Anexar um modelo a um projeto](/help/quicksilver/manage-work/projects/create-and-manage-templates/attach-template-to-project.md).

1. Ao selecionar um modelo para o projeto, selecione o modelo que contém os fluxos de trabalho que deseja usar para esse projeto.
1. (Opcional) Edite quaisquer valores de fluxo de trabalho para o projeto, conforme descrito em [Editar valores de fluxo de trabalho em um projeto](#edit-workflow-values-in-a-project).

   Somente os workflows que foram ativados na área Experience Manager da Configuração estão disponíveis em modelos ou projetos.



### Editar valores de fluxo de trabalho em um projeto

É possível editar valores de fluxo de trabalho no nível do projeto. Os valores do fluxo de trabalho no nível do projeto substituem os valores definidos no modelo do projeto, que substitui os valores padrão definidos na integração do Adobe Experience Manager Assets.

Todos os valores de workflow podem ser encontrados em:

* A seção Workflows ou pastas vinculadas da janela Criar projeto ou Editar projeto.
* A seção Adobe Experience Manager da navegação à esquerda.


  >[!NOTE]
  >
  >Se essas áreas não estiverem visíveis, o administrador do Workfront não ativou os Fluxos de trabalho para sua organização.



#### Pastas vinculadas

>[!NOTE]
>
>Como as pastas vinculadas são criadas quando o projeto é criado, a edição do fluxo de trabalho da pasta vinculada em um projeto existente não é eficaz. A edição desses valores ao criar um projeto funciona conforme esperado.

Para editar o fluxo de trabalho de pastas vinculadas:

1. Ative ou desative a **[!UICONTROL Criar pasta vinculada]** conforme desejado. Se você ativá-lo, poderá editar a configuração da pasta vinculada.

   Para obter detalhes sobre a configuração da pasta vinculada, consulte [Criar pastas vinculadas do Adobe Experience Manager](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md#create-adobe-experience-manager-linked-folders) no artigo [Configurar a integração do [!UICONTROL Experience Manager Assets as a Cloud Service]](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md).

1. (Opcional) Se quiser que a árvore de pastas seja criada somente se determinados valores estiverem presentes em um formulário personalizado anexado ao projeto, clique em **Aplicar filtro** para essa árvore de pastas e selecione o formulário personalizado que contém o campo, o campo e o valor do campo. Se o campo no formulário personalizado anexado ao novo projeto contiver o valor escolhido, a árvore de pastas será criada.
1. (Opcional) Ao configurar nomes de pastas, você pode selecionar entre as seguintes opções:

   * **Nome**: digite um nome para a pasta.

   * **Dados do objeto**: selecione a origem do nome da pasta, como Nome do projeto.

   * **Dados de formulário personalizados**: selecione os dados de formulário personalizados a serem usados como o nome da pasta.

     O uso de dados de formulário personalizados para nomes de pastas está disponível somente no nível do modelo e não pode ser configurado no nível de integração.

     Se um nome de pasta for definido como dados personalizados que não existem no personalizado para anexado ao projeto, uma ID aleatória será atribuída como o nome da pasta.

1. Para exibir a árvore de pastas, clique no ícone **Visualizar** ![Visualizar](assets/preview-icon.png)
1. Clique em **[!UICONTROL Salvar]**.

#### Publicar ativos

Para editar o fluxo de trabalho de publicação de ativos:

1. Ative ou desative o **Publicar ativos automaticamente**, conforme desejado.
1. (Condicional) Se você estiver ativando a publicação, selecione se deseja publicar no serviço de publicação, no portal de marcas ou em ambos.
1. Clique em **[!UICONTROL Salvar]**.
