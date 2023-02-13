---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Criar novos modelos em [!DNL Adobe Workfront Fusion]
description: Você pode criar novos modelos de cenário em [!DNL Adobe] Workfront Fusion.
author: Becky
feature: Workfront Fusion
exl-id: fdfa509c-30c6-431e-89f3-a4bf50261e8a
source-git-commit: fcaa2136310cad8ef478020a9bae34bbe5520c6d
workflow-type: tm+mt
source-wordcount: '469'
ht-degree: 0%

---

# Criar novos modelos em [!DNL Adobe Workfront Fusion]

Você pode criar novos modelos de cenário em [!DNL Adobe] Workfront Fusion.

>[!TIP]
>
>Antes de criar um novo modelo, você pode verificar a variável [!UICONTROL Modelos públicos] para garantir que o template que você deseja criar ainda não esteja disponível.

## Requisitos de acesso

Você deve ter o seguinte acesso para usar a funcionalidade neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] plano*</td> 
   <td> <p>[!DNL Pro] ou superior</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licença*</td> 
   <td> <p>[!UICONTROL Plano], [!UICONTROL Trabalho]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da [!UICONTROL Adobe Workfront Fusion]**</td> 
  <td> <p>[!UICONTROL [!DNL Workfront Fusion] para automação e integração de trabalho] </p><p>[!UICONTROL [!DNL Workfront Fusion] para Automação de Trabalho] </p>  </td>    </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">Produto</td> 
   <td>Sua organização deve comprar [!DNL Adobe Workfront Fusion] bem como [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo.</td> 
  </tr> 
 </tbody> 
</table>

Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com seu [!DNL Workfront] administrador.

Para obter informações sobre [!DNL Adobe Workfront Fusion] licenças, consulte [[!DNL Adobe Workfront Fusion] licenças](../../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Criar um novo modelo

1. Clique em **[!UICONTROL Modelos]** ![](assets/fusion-template-icon.png) no painel de navegação esquerdo.
1. Clique em **[!UICONTROL Criar um novo modelo]** no canto superior direito.
1. (Opcional) Renomeie o modelo ao substituir o padrão **[!UICONTROL Novo nome de modelo]** no canto superior esquerdo.
1. (Opcional) Para alterar o idioma do modelo, clique em **[!UICONTROL Configurar um modelo]** ![](assets/fusion-scenario-settings-icon.png) e selecione o idioma no menu suspenso Idioma .

   >[!IMPORTANT]
   >
   >A seleção de Idiomas corresponde aos idiomas disponíveis nas configurações do sistema e diz respeito somente ao nome do modelo público e sua descrição. Não é possível alterar um idioma de modelo depois que o modelo for salvo.

1. (Opcional) Para inserir uma descrição do modelo, clique em **[!UICONTROL Configurar um modelo]** ![](assets/fusion-scenario-settings-icon.png) e insira a descrição.
1. Adicione aplicativos, módulos e ferramentas da mesma maneira que faria ao criar um cenário padrão.

   Para adicionar ajuda contextual aos módulos, consulte [Configurar [!UICONTROL Assistente] funcionalidade](#set-up-wizard-functionality) neste artigo.

   Para obter mais informações sobre como criar um cenário, consulte [Crie um cenário em [!DNL Adobe Workfront Fusion]](../../../workfront-fusion/scenarios/create-a-scenario.md).

   >[!NOTE]
   >
   >Se o modelo incluir módulos que exijam a adição da conexão, credenciais ou outras informações confidenciais, essas informações não serão compartilhadas com os usuários do modelo.

1. (Opcional) Clique em **[!UICONTROL Executar uma vez]** para testar seu modelo.
1. Clique no botão **[!UICONTROL Salvar]** ícone ![](assets/save-icon.png).

>[!NOTE]
>
>Ao salvar seu modelo, você o torna visível para todos os membros da equipe. Se quiser que seu modelo seja acessível fora da equipe, publique-o e use um link compartilhado, ou peça ao administrador para aprovar e publicar o modelo.

## Configurar [!UICONTROL Assistente] funcionalidade {#set-up-wizard-functionality}

O [!DNL Workfront Fusion template] [!UICONTROL Assistente] O permite fornecer aos futuros usuários do modelo instruções ou informações relacionadas aos campos específicos usados nos módulos.

1. Clique no módulo adicionado ao template para ver os campos do módulo.
1. Localize o campo ao qual deseja adicionar [!UICONTROL Assistente] e ativar **[!UICONTROL Usar no Assistente]** para esse campo.
1. Insira as informações que você deseja tornar visíveis para os usuários no [!UICONTROL Ajuda] campo.
1. (Opcional) Para permitir que os usuários vejam esse texto ao usar o modelo, ative **[!UICONTROL Usar como valor padrão]**.
1. Repita as etapas de 2 a 4 para cada campo para o qual deseja fornecer informações.
1. Clique em **[!UICONTROL OK]** para salvar as alterações e fechar o módulo .
