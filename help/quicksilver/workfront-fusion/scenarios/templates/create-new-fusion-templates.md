---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Criar novos modelos em  [!DNL Adobe Workfront Fusion]
description: Você pode criar novos modelos de cenário no  [!DNL Adobe] Workfront Fusion.
author: Becky
feature: Workfront Fusion
exl-id: fdfa509c-30c6-431e-89f3-a4bf50261e8a
source-git-commit: f3f34e807228b299c0570e63bdf329f4e20e0340
workflow-type: tm+mt
source-wordcount: '794'
ht-degree: 0%

---

# Criar novos modelos em [!DNL Adobe Workfront Fusion]

Você pode criar novos modelos de cenário no [!DNL Adobe] Workfront Fusion.

>[!TIP]
>
>Antes de criar um novo modelo, você pode verificar a guia [!UICONTROL Modelos públicos] para garantir que o modelo que você deseja criar ainda não está disponível.

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
   <td role="rowheader">Licença [!UICONTROL Adobe Workfront Fusion]**</td> 
  <td>
   <p>Requisito de licença atual: nenhum requisito de licença [!DNL Workfront Fusion].</p>
   <p>Ou</p>
   <p>Requisito de licença herdada: [!UICONTROL [!DNL Workfront Fusion] para Automação e Integração do Trabalho], [!UICONTROL [!DNL Workfront Fusion] para Automação do Trabalho]</p>
   </td>    </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">Produto</td> 
   <td>
   <p>Requisito atual do produto: se você tiver o Plano [!DNL Adobe Workfront] da [!UICONTROL Select] ou da [!UICONTROL Prime], sua organização deve comprar o [!DNL Adobe Workfront Fusion] e o [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo. [!DNL Workfront Fusion] está incluído no plano [!DNL Workfront] do [!UICONTROL Ultimate].</p>
   <p>Ou</p>
   <p>Requisito de produto herdado: sua organização deve comprar o [!DNL Adobe Workfront Fusion] e o [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Para saber que plano, tipo de licença ou acesso você tem, contate o administrador do [!DNL Workfront].

Para obter informações sobre [!DNL Adobe Workfront Fusion] licenças, consulte [[!DNL Adobe Workfront Fusion] licenças](../../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Criar um novo modelo

Você pode criar um modelo em um processo semelhante à criação de um cenário. Os administradores do Fusion também podem criar modelos a partir de cenários existentes.

* [Criar um modelo](#build-a-template)
* [Criar um modelo a partir de um cenário](#create-a-template-from-a-scenario)

### Criar um modelo

1. Clique em **[!UICONTROL Modelos]** ![](assets/fusion-template-icon.png) no painel de navegação esquerdo.
1. Clique em **[!UICONTROL Criar um novo modelo]** no canto superior direito.
1. (Opcional) Renomeie o modelo substituindo o padrão **[!UICONTROL Novo nome do modelo]** no canto superior esquerdo.
1. (Opcional) Para alterar o idioma do modelo, clique em **[!UICONTROL Configurar um modelo]** ![](assets/fusion-scenario-settings-icon.png) e selecione o idioma no menu suspenso Idioma.

   >[!IMPORTANT]
   >
   >A seleção Languages corresponde aos idiomas disponíveis nas configurações do sistema e aborda apenas o nome do template público e sua descrição. Não é possível alterar um idioma de modelo depois que o modelo é salvo.

1. (Opcional) Para inserir uma descrição do modelo, clique em **[!UICONTROL Configurar um modelo]** ![](assets/fusion-scenario-settings-icon.png) e insira a descrição.
1. Adicione aplicativos, módulos e ferramentas da mesma forma que faria ao criar um cenário padrão.

   Para adicionar ajuda contextual aos módulos, consulte [Configurar a funcionalidade [!UICONTROL Assistente]](#set-up-wizard-functionality) neste artigo.

   Para obter mais informações sobre como criar um cenário, consulte [Criar um cenário [!DNL Adobe Workfront Fusion]](../../../workfront-fusion/scenarios/create-a-scenario.md).

   >[!NOTE]
   >
   >Se o modelo incluir módulos que exigem a adição da conexão, das credenciais ou de outras informações confidenciais de privacidade, essas informações não serão compartilhadas com os usuários do modelo.

1. (Opcional) Clique em **[!UICONTROL Executar uma vez]** para testar seu modelo.
1. Clique no ícone **[!UICONTROL Salvar]** ![](assets/save-icon.png).

>[!NOTE]
>
>Ao salvar seu modelo, você o torna visível para todos os membros da equipe. Se quiser que o modelo seja acessível fora da equipe, você deverá enviar uma solicitação para que ele seja aprovado e publicado. A solicitação é enviada ao Adobe Workfront para aprovação e, uma vez aprovada, o modelo pode ser acessado por outras pessoas fora da equipe.
>
>Para obter informações sobre a publicação de modelos, consulte [Publish e compartilhar [!DNL Adobe Workfront Fusion] modelos](/help/quicksilver/workfront-fusion/scenarios/templates/publish-and-share-fusion-templates.md).

### Criar um modelo a partir de um cenário

>[!NOTE]
>
>Você deve ser um administrador do Fusion para criar um modelo a partir de um cenário.

1. Abra a página de detalhes do cenário do cenário no qual deseja criar um cenário.
1. Clique no menu suspenso **Admin** próximo ao canto superior direito da página.
1. Selecione **Clonar como modelo**.

   O cenário é copiado em uma página Novo modelo.
1. (Opcional) Renomeie o modelo substituindo o padrão **[!UICONTROL Novo nome do modelo]** no canto superior esquerdo.
1. (Opcional) Para alterar o idioma do modelo, clique em **[!UICONTROL Configurar um modelo]** ![](assets/fusion-scenario-settings-icon.png) e selecione o idioma no menu suspenso Idioma.

   >[!IMPORTANT]
   >
   >A seleção Languages corresponde aos idiomas disponíveis nas configurações do sistema e aborda apenas o nome do template público e sua descrição. Não é possível alterar um idioma de modelo depois que o modelo é salvo.

1. (Opcional) Para inserir uma descrição do modelo, clique em **[!UICONTROL Configurar um modelo]** ![](assets/fusion-scenario-settings-icon.png) e insira a descrição.
1. Edite aplicativos, módulos e ferramentas da mesma forma que faria ao editar um cenário padrão.

   Para adicionar ajuda contextual aos módulos, consulte [Configurar a funcionalidade [!UICONTROL Assistente]](#set-up-wizard-functionality) neste artigo.

   >[!NOTE]
   >
   >Se o modelo incluir módulos que exigem a adição da conexão, das credenciais ou de outras informações confidenciais de privacidade, essas informações não serão compartilhadas com os usuários do modelo.

1. (Opcional) Clique em **[!UICONTROL Executar uma vez]** para testar seu modelo.
1. Clique no ícone **[!UICONTROL Salvar]** ![](assets/save-icon.png).

## Configurar a funcionalidade [!UICONTROL Assistente] {#set-up-wizard-functionality}

O [!DNL Workfront Fusion template] [!UICONTROL Assistente] permite que você forneça aos futuros usuários do seu modelo instruções ou informações relacionadas aos campos específicos usados nos módulos.

1. Clique no módulo adicionado ao modelo para ver os campos do módulo.
1. Localize o campo no qual você deseja adicionar informações do [!UICONTROL Assistente] e habilitar o **[!UICONTROL Uso do Assistente]** para esse campo.
1. Digite as informações que você deseja tornar visíveis para usuários no campo [!UICONTROL Ajuda].
1. (Opcional) Para permitir que os usuários vejam este texto ao usar o modelo, habilite **[!UICONTROL Usar como valor padrão]**.
1. Repita as etapas 2 a 4 para cada campo para o qual deseja fornecer informações.
1. Clique em **[!UICONTROL OK]** para salvar as alterações e fechar o módulo.
