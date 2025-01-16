---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Administração de Modelos do Adobe Workfront Fusion
description: A documentação do Adobe Workfront Fusion foi movida para um novo local. Este artigo foi descontinuado, mas contém um link para o novo artigo que aborda essa funcionalidade.
author: Becky
feature: Workfront Fusion
exl-id: 63c14183-0d22-44f3-87e5-c311cfbf5540
source-git-commit: 8163f9f12bb27bbc8adfde34fc1e1f0f8c8be7f9
workflow-type: tm+mt
source-wordcount: '686'
ht-degree: 0%

---

# Administração de modelos [!DNL Adobe Workfront Fusion]

>[!IMPORTANT]
>
>A documentação do Adobe Workfront Fusion foi movida para um novo local.
>
>As informações neste artigo agora podem ser encontradas nos artigos:
>
>* [Aprovar ou desaprovar modelos para a guia Público](https://experienceleague.adobe.com/docs/workfront-fusion/using/set-up-and-manage-fusion/manage-templates-admin/approve-templates.html)
>* [Editar modelos](https://experienceleague.adobe.com/docs/workfront-fusion/using/set-up-and-manage-fusion/manage-templates-admin/edit-templates.html)
>
>Atualize todos os marcadores.
>
>Este artigo não está mais sendo atualizado e será removido em breve.

Se você for um administrador, terá permissão para exibir, modificar, renomear, publicar, aprovar e excluir modelos criados por outros. Você pode executar essas ações na página [!UICONTROL Modelos] na área [!DNL Adobe Workfront Fusion Administration].

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
   <p>Requisito de licença atual: nenhum requisito de licença [!DNL Workfront Fusion].</p>
   <p>Ou</p>
   <p>Requisito de licença herdada: [!UICONTROL [!DNL Workfront Fusion] para Automação e Integração do Trabalho], [!UICONTROL [!DNL Workfront Fusion] para Automação do Trabalho]</p>
   </td>  
  </tr> 
  <tr> 
   <td role="rowheader">Produto</td> 
   <td>
   <p>Requisito atual do produto: se você tiver o Plano [!DNL Adobe Workfront] da [!UICONTROL Select] ou da [!UICONTROL Prime], sua organização deve comprar o [!DNL Adobe Workfront Fusion] e o [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo. [!DNL Workfront Fusion] está incluído no plano [!DNL Workfront] da [!UICONTROL Ultimate].</p>
   <p>Ou</p>
   <p>Requisito de produto herdado: sua organização deve comprar o [!DNL Adobe Workfront Fusion] e o [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo.</p>
   </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Você deve ser um administrador do Workfront Fusion para sua organização.</p> </td> 
  </tr> 
 </tbody> 
</table>

Para saber que plano, tipo de licença ou acesso você tem, contate o administrador do [!DNL Workfront].

Para obter informações sobre [!DNL Adobe Workfront Fusion] licenças, consulte [[!DNL Adobe Workfront Fusion] licenças](../../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Exibir modelos [!DNL Workfront Fusion] como administrador [!DNL Workfront Fusion]

Para exibir uma tabela de todos os modelos criados e seus status:

1. Clique em **[!UICONTROL Administração]** no painel de navegação esquerdo para abrir a área [!UICONTROL Administração].

   >[!NOTE]
   >
   >A área Administração é visível somente para administradores do Workfront Fusion.

1. Clique em **[!UICONTROL Modelos]** no painel de navegação esquerdo.

Há três colunas relacionadas ao status de publicação dos modelos. Uma marca de seleção em uma coluna indica o seguinte:

* **[!UICONTROL Publicado]**: esses modelos estão visíveis atualmente na guia [!UICONTROL Modelos de equipe] da interface do usuário.
* **[!UICONTROL Aprovação solicitada]**: esses modelos estão aguardando sua aprovação. Atualmente, eles estão visíveis na guia [!UICONTROL Modelos de equipe] da interface.
* **[!UICONTROL Aprovado]**: esses modelos foram aprovados. Atualmente, eles estão visíveis na guia [!UICONTROL Modelos públicos] da interface padrão.

>[!NOTE]
>
>Modelos com a marca de seleção na coluna [!UICONTROL Aprovação solicitada] e na coluna [!UICONTROL Aprovado] já foram aprovados e tornaram-se públicos, mas há uma versão mais recente deles aguardando sua aprovação.

## Editar modelos de [!DNL Workfront Fusion] como administrador

1. Clique em **[!UICONTROL Administração]** no painel de navegação esquerdo para abrir a área [!UICONTROL Administração].
1. Clique em **[!UICONTROL Modelos]** no painel de navegação esquerdo.
1. Clique em **[!UICONTROL Detalhe]** à direita do modelo que deseja editar.

Agora você pode editar o modelo, de modo semelhante a editar um modelo como um usuário não administrador. Entretanto, nas [!UICONTROL Opções] no canto superior direito, há uma opção adicional: o diagrama de SVG que fornece o código de SVG. Além disso, o processo de publicação é o mesmo que no caso de um usuário padrão. Consulte a seção Publicação e compartilhamento de modelos para obter mais detalhes.

Para obter informações sobre opções de modelo específicas que podem ser editadas, consulte [Criar novos modelos em [!DNL Adobe Workfront Fusion]](../../../workfront-fusion/scenarios/templates/create-new-fusion-templates.md).

Para obter informações sobre a publicação de modelos, consulte [Publish e compartilhar [!DNL Adobe Workfront Fusion] modelos](../../../workfront-fusion/scenarios/templates/publish-and-share-fusion-templates.md).

## Aprovar ou desaprovar [!DNL Workfront Fusion] modelos

A aprovação de um modelo o torna visível na guia [!UICONTROL Modelos públicos] e disponível para todos os usuários. Desaprovar um modelo o remove da guia [!UICONTROL Modelos públicos] e o disponibiliza somente para a equipe que o criou.

1. Clique em **[!UICONTROL Administração]** no painel de navegação esquerdo para abrir a área [!UICONTROL Administração].
1. Clique em **[!UICONTROL Modelos]** no painel de navegação esquerdo.
1. Se quiser aprovar um modelo, clique em **[!UICONTROL Aprovar]** à direita do modelo.
1. Se quiser desaprovar um modelo, clique em **[!UICONTROL Desaprovar]** à direita do modelo.

>[!NOTE]
>
>Se você estiver aprovando o modelo que foi aprovado anteriormente e editado, sua segunda aprovação substituirá o modelo original.

## Clonar um cenário como modelo

Como administrador, você tem a capacidade de clonar um cenário como gabarito.

Para obter instruções sobre como clonar um cenário como modelo, consulte [Criar um modelo a partir de um cenário](../../../workfront-fusion/scenarios/templates/create-new-fusion-templates.md#create-a-template-from-a-scenario) em [Criar novos modelos [!DNL Adobe Workfront Fusion]](../../../workfront-fusion/scenarios/templates/create-new-fusion-templates.md)
