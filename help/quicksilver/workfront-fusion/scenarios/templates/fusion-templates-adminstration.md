---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Administração de Modelos do Adobe Workfront Fusion
description: Se você for um administrador, terá permissão para exibir, modificar, renomear, publicar, aprovar e excluir modelos criados por outros. É possível executar essas ações a partir da [!UICONTROL Modelos] página no [!DNL Adobe Workfront Fusion Administration] área.
author: Becky
feature: Workfront Fusion
exl-id: 63c14183-0d22-44f3-87e5-c311cfbf5540
source-git-commit: a3756f9345cbc9417a6fd110306dfa50aecc81a2
workflow-type: tm+mt
source-wordcount: '626'
ht-degree: 0%

---

# [!DNL Adobe Workfront Fusion] Administração de modelos

Se você for um administrador, terá permissão para exibir, modificar, renomear, publicar, aprovar e excluir modelos criados por outros. É possível executar essas ações a partir da [!UICONTROL Modelos] página no [!DNL Adobe Workfront Fusion Administration] área.

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas deste artigo:

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
   <td role="rowheader">Licença [!UICONTROL Adobe Workfront Fusion]**</td> 
  <td>
   <p>Requisito de licença atual: Não [!DNL Workfront Fusion] requisito de licença.</p>
   <p>Ou</p>
   <p>Requisito de licença herdada: [!UICONTROL [!DNL Workfront Fusion] para Automação e Integração do Trabalho], [!UICONTROL [!DNL Workfront Fusion] para automação de trabalho]</p>
   </td>  
  </tr> 
  <tr> 
   <td role="rowheader">Produto</td> 
   <td>
   <p>Requisito atual do produto: se você tiver o [!UICONTROL Select] ou o [!UICONTROL Prime] [!DNL Adobe Workfront] Planejar, sua organização deve comprar [!DNL Adobe Workfront Fusion] bem como [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo. [!DNL Workfront Fusion] está incluído no [!UICONTROL Ultimate] [!DNL Workfront] plano.</p>
   <p>Ou</p>
   <p>Requisito de produto herdado: sua organização deve comprar [!DNL Adobe Workfront Fusion] bem como [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo.</p>
   </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Você deve ser um administrador do Workfront Fusion para sua organização.</p> </td> 
  </tr> 
 </tbody> 
</table>

Para descobrir que plano, tipo de licença ou acesso você tem, entre em contato com o [!DNL Workfront] administrador.

Para obter informações sobre [!DNL Adobe Workfront Fusion] licenças, consulte [[!DNL Adobe Workfront Fusion] licenças](../../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Exibir [!DNL Workfront Fusion] modelos como administrador

Para exibir uma tabela de todos os modelos criados e seus status:

1. Clique em **[!UICONTROL Administração]** no painel de navegação esquerdo, para abrir a janela [!UICONTROL Administração] área.
1. Clique em **[!UICONTROL Modelos]** no painel de navegação esquerdo.

Há três colunas relacionadas ao status de publicação dos modelos. Uma marca de seleção em uma coluna indica o seguinte:

* **[!UICONTROL Publicado]**: esses modelos estão visíveis no momento no [!UICONTROL Modelos de equipe] na interface do usuário.
* **[!UICONTROL Aprovação solicitada]**: esses modelos estão aguardando sua aprovação. Atualmente, eles estão visíveis na [!UICONTROL Modelos de equipe] na interface do usuário.
* **[!UICONTROL Aprovado]**: esses modelos foram aprovados. Atualmente, eles estão visíveis na [!UICONTROL Modelos públicos] na interface padrão do usuário.

>[!NOTE]
>
>Modelos com a marca de seleção em ambos [!UICONTROL Aprovação solicitada] e na [!UICONTROL Aprovado] já foram aprovadas e tornadas públicas, mas há uma versão mais recente delas aguardando sua aprovação.

## Editar [!DNL Workfront Fusion] modelos como administrador

1. Clique em **[!UICONTROL Administração]** no painel de navegação esquerdo, para abrir a janela [!UICONTROL Administração] área.
1. Clique em **[!UICONTROL Modelos]** no painel de navegação esquerdo.
1. Clique em **[!UICONTROL Detalhe]** à direita do modelo que deseja editar.

Agora você pode editar o modelo, de modo semelhante a editar um modelo como um usuário não administrador. No entanto, no [!UICONTROL Opções] no canto superior direito, há uma opção adicional - o diagrama de SVG que fornece o código de SVG. Além disso, o processo de publicação é o mesmo que no caso de um usuário padrão. Consulte a seção Publicação e compartilhamento de modelos para obter mais detalhes.

Para obter informações sobre opções de modelo específicas que podem ser editadas, consulte [Criar novos modelos no [!DNL Adobe Workfront Fusion]](../../../workfront-fusion/scenarios/templates/create-new-fusion-templates.md).

Para obter informações sobre modelos de publicação, consulte [Publicar e compartilhar [!DNL Adobe Workfront Fusion] modelos](../../../workfront-fusion/scenarios/templates/publish-and-share-fusion-templates.md).

## Aprovar ou desaprovar [!DNL Workfront Fusion] modelos

A aprovação de um modelo o torna visível no [!UICONTROL Modelos públicos] e disponível para todos os usuários. Desaprovar um modelo o remove da lista [!UICONTROL Modelos públicos] e o disponibiliza somente para a equipe que o criou.

1. Clique em **[!UICONTROL Administração]** no painel de navegação esquerdo, para abrir a janela [!UICONTROL Administração] área.
1. Clique em **[!UICONTROL Modelos]** no painel de navegação esquerdo.
1. Se quiser aprovar um modelo, clique em **[!UICONTROL Aprovar]** à direita do modelo.
1. Se quiser desaprovar um modelo, clique em **[!UICONTROL Desaprovar]** à direita do modelo.

>[!NOTE]
>
>Se você estiver aprovando o modelo que foi aprovado anteriormente e editado, sua segunda aprovação substituirá o modelo original.

## Clonar um cenário como modelo

Como administrador, você tem a capacidade de clonar um cenário como gabarito.

Para obter instruções sobre como clonar um cenário como um modelo, consulte [Criar um modelo a partir de um cenário](../../../workfront-fusion/scenarios/templates/create-new-fusion-templates.md#create-a-template-from-a-scenario) in [Criar novos modelos no [!DNL Adobe Workfront Fusion]](../../../workfront-fusion/scenarios/templates/create-new-fusion-templates.md)
