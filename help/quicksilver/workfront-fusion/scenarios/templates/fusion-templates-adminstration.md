---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Administração de Modelos do Adobe Workfront Fusion
description: Se você for um administrador, terá permissão para exibir, modificar, renomear, publicar, aprovar e excluir modelos criados por outras pessoas. Você pode executar essas ações a partir do [!UICONTROL Modelos] na página [!DNL Adobe Workfront Fusion Administration] área.
author: Becky
feature: Workfront Fusion
exl-id: 63c14183-0d22-44f3-87e5-c311cfbf5540
source-git-commit: bcca026e193e66cfb92ab9a0fb1aaf1eeb6892fb
workflow-type: tm+mt
source-wordcount: '578'
ht-degree: 0%

---

# [!DNL Adobe Workfront Fusion] Administração de modelos

Se você for um administrador, terá permissão para exibir, modificar, renomear, publicar, aprovar e excluir modelos criados por outras pessoas. Você pode executar essas ações a partir do [!UICONTROL Modelos] na página [!DNL Adobe Workfront Fusion Administration] área.

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] plano*</td> 
   <td> <p>[!DNL Pro] ou superior</p> </td> 
  </tr>
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">[!DNL Adobe Workfront] licença*</td> 
    <td> <p>[!UICONTROL Plano], [!UICONTROL Trabalho]</p> </td> 
   </tr>
  <tr> 
   <td role="rowheader">Licença da [!UICONTROL Adobe Workfront Fusion]**</td> 
  <td> <p>[!UICONTROL [!DNL Workfront Fusion] para automação e integração de trabalho] </p><p>[!UICONTROL [!DNL Workfront Fusion] para Automação de Trabalho] </p>  </td>  
  </tr> 
  <tr> 
   <td role="rowheader">Produto</td> 
   <td>Sua organização deve comprar [!DNL Adobe Workfront Fusion] bem como [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Você deve ser um administrador do Workfront Fusion para sua organização.</p> </td> 
  </tr> 
 </tbody> 
</table>

Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com seu [!DNL Workfront] administrador.

Para obter informações sobre [!DNL Adobe Workfront Fusion] licenças, consulte [[!DNL Adobe Workfront Fusion] licenças](../../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Exibir [!DNL Workfront Fusion] modelos como administrador

Para exibir uma tabela de todos os modelos criados e seus status:

1. Clique em **[!UICONTROL Administração]** no painel de navegação esquerdo para abrir o [!UICONTROL Administração] área.
1. Clique em **[!UICONTROL Modelos]** no painel de navegação esquerdo.

Há três colunas relacionadas ao status de publicação dos templates. Uma marca de seleção em uma coluna indica o seguinte:

* **[!UICONTROL Publicado]**: Esses modelos estão visíveis no momento na variável [!UICONTROL Modelos de equipe] na interface do usuário.
* **[!UICONTROL Aprovação solicitada]**: Esses modelos estão aguardando sua aprovação. No momento, eles estão visíveis na variável [!UICONTROL Modelos de equipe] na interface do usuário.
* **[!UICONTROL Aprovado]**: Esses modelos foram aprovados. No momento, eles estão visíveis na variável [!UICONTROL Modelos públicos] na interface do usuário padrão.

>[!NOTE]
>
>Modelos com a marca de seleção em ambas as [!UICONTROL Aprovação solicitada] e na [!UICONTROL Aprovado] já foram aprovadas e tornadas públicas, mas há uma versão mais recente aguardando sua aprovação.

## Editar [!DNL Workfront Fusion] modelos como administrador

1. Clique em **[!UICONTROL Administração]** no painel de navegação esquerdo para abrir o [!UICONTROL Administração] área.
1. Clique em **[!UICONTROL Modelos]** no painel de navegação esquerdo.
1. Clique em **[!UICONTROL Detalhe]** à direita do modelo que deseja editar.

Agora é possível editar o modelo, de maneira semelhante à edição de um modelo como um usuário não administrador. No entanto, no [!UICONTROL Opções] no canto superior direito, há uma opção adicional - o diagrama de SVG que fornece o código de SVG. Além disso, o processo de publicação é o mesmo no caso de um usuário padrão, consulte a seção Publicação e compartilhamento de modelos para obter mais detalhes.

Para obter informações sobre opções de modelo específicas que você pode editar, consulte [Criar novos modelos em [!DNL Adobe Workfront Fusion]](../../../workfront-fusion/scenarios/templates/create-new-fusion-templates.md).

Para obter informações sobre a publicação de modelos, consulte [Publicar e compartilhar [!DNL Adobe Workfront Fusion] modelos](../../../workfront-fusion/scenarios/templates/publish-and-share-fusion-templates.md).

## Aprovar ou rejeitar [!DNL Workfront Fusion] modelos

A aprovação de um modelo o torna visível no [!UICONTROL Modelos públicos] e disponíveis para todos os usuários. Desaprovar um modelo o remove do [!UICONTROL Modelos públicos] e a disponibiliza somente para a equipe que a criou.

1. Clique em **[!UICONTROL Administração]** no painel de navegação esquerdo para abrir o [!UICONTROL Administração] área.
1. Clique em **[!UICONTROL Modelos]** no painel de navegação esquerdo.
1. Se quiser aprovar um modelo, clique em **[!UICONTROL Aprovar]** à direita do template.
1. Se quiser rejeitar um modelo, clique em **[!UICONTROL Reprovar]** à direita do template.

>[!NOTE]
>
>Se você estiver aprovando o template que foi aprovado e editado anteriormente, sua segunda aprovação substituirá o template original.

## Clonar um cenário como modelo

Como administrador, você pode clonar um cenário como modelo.

Para obter instruções sobre como clonar um cenário como modelo, consulte [Criar um modelo a partir de um cenário](../../../workfront-fusion/scenarios/templates/create-new-fusion-templates.md#create-a-template-from-a-scenario) em [Criar novos modelos em [!DNL Adobe Workfront Fusion]](../../../workfront-fusion/scenarios/templates/create-new-fusion-templates.md)
