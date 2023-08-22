---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Criar novos modelos no [!DNL Adobe Workfront Fusion]
description: Você pode criar novos modelos de cenário no [!DNL Adobe] Workfront Fusion
author: Becky
feature: Workfront Fusion
exl-id: fdfa509c-30c6-431e-89f3-a4bf50261e8a
source-git-commit: b7879e8f2d4590d6347762d66c82de293d00c995
workflow-type: tm+mt
source-wordcount: '782'
ht-degree: 0%

---

# Criar novos modelos no [!DNL Adobe Workfront Fusion]

Você pode criar novos modelos de cenário no [!DNL Adobe] Workfront Fusion

>[!TIP]
>
>Antes de criar um novo template, você pode verificar o [!UICONTROL Modelos públicos] para garantir que o modelo que você deseja criar ainda não esteja disponível.

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
   <p>Requisito de licença atual: Não [!DNL Workfront Fusion] requisito de licença.</p>
   <p>Ou</p>
   <p>Requisito de licença herdada: [!UICONTROL [!DNL Workfront Fusion] para Automação e Integração do Trabalho], [!UICONTROL [!DNL Workfront Fusion] para automação de trabalho]</p>
   </td>    </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">Produto</td> 
   <td>
   <p>Requisito atual do produto: se você tiver o [!UICONTROL Select] ou o [!UICONTROL Prime] [!DNL Adobe Workfront] Planejar, sua organização deve comprar [!DNL Adobe Workfront Fusion] bem como [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo. [!DNL Workfront Fusion] está incluído no [!UICONTROL Ultimate] [!DNL Workfront] plano.</p>
   <p>Ou</p>
   <p>Requisito de produto herdado: sua organização deve comprar [!DNL Adobe Workfront Fusion] bem como [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Para descobrir que plano, tipo de licença ou acesso você tem, entre em contato com o [!DNL Workfront] administrador.

Para obter informações sobre [!DNL Adobe Workfront Fusion] licenças, consulte [[!DNL Adobe Workfront Fusion] licenças](../../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Criar um novo modelo

Você pode criar um modelo em um processo semelhante à criação de um cenário. Os administradores do Fusion também podem criar modelos a partir de cenários existentes.

* [Criar um modelo](#build-a-template)
* [Criar um modelo a partir de um cenário](#create-a-template-from-a-scenario)

### Criar um modelo

1. Clique em **[!UICONTROL Modelos]** ![](assets/fusion-template-icon.png) no painel de navegação esquerdo.
1. Clique em **[!UICONTROL Criar um novo modelo]** no canto superior direito.
1. (Opcional) Renomeie o template substituindo o padrão **[!UICONTROL Novo nome do modelo]** no canto superior esquerdo.
1. (Opcional) Para alterar o idioma do modelo, clique em **[!UICONTROL Configurar um modelo]** ![](assets/fusion-scenario-settings-icon.png) e selecione o idioma no menu suspenso Idioma.

   >[!IMPORTANT]
   >
   >A seleção Languages corresponde aos idiomas disponíveis nas configurações do sistema e aborda apenas o nome do template público e sua descrição. Não é possível alterar um idioma de modelo depois que o modelo é salvo.

1. (Opcional) Para inserir uma descrição do modelo, clique em **[!UICONTROL Configurar um modelo]** ![](assets/fusion-scenario-settings-icon.png) e insira a descrição.
1. Adicione aplicativos, módulos e ferramentas da mesma forma que faria ao criar um cenário padrão.

   Para adicionar ajuda contextual aos módulos, consulte [Configurar [!UICONTROL Assistente] funcionalidade](#set-up-wizard-functionality) neste artigo.

   Para obter mais informações sobre a criação de um cenário, consulte [Criar um cenário no [!DNL Adobe Workfront Fusion]](../../../workfront-fusion/scenarios/create-a-scenario.md).

   >[!NOTE]
   >
   >Se o modelo incluir módulos que exigem a adição da conexão, das credenciais ou de outras informações confidenciais de privacidade, essas informações não serão compartilhadas com os usuários do modelo.

1. (Opcional) Clique em **[!UICONTROL Executar uma vez]** para testar seu modelo.
1. Clique em **[!UICONTROL Salvar]** ícone ![](assets/save-icon.png).

>[!NOTE]
>
>Ao salvar seu modelo, você o torna visível para todos os membros da equipe. Se quiser que o modelo seja acessível fora da equipe, você deverá enviar uma solicitação para que ele seja aprovado e publicado. A solicitação é enviada ao Adobe Workfront para aprovação e, uma vez aprovada, o modelo pode ser acessado por outras pessoas fora da equipe.

### Criar um modelo a partir de um cenário

>[!NOTE]
>
>Você deve ser um administrador do Fusion para criar um modelo a partir de um cenário.

1. Abra a página de detalhes do cenário do cenário no qual deseja criar um cenário.
1. Clique em **Admin** próximo ao canto superior direito da página.
1. Selecionar **Clonar como modelo**.

   O cenário é copiado em uma página Novo modelo.
1. (Opcional) Renomeie o template substituindo o padrão **[!UICONTROL Novo nome do modelo]** no canto superior esquerdo.
1. (Opcional) Para alterar o idioma do modelo, clique em **[!UICONTROL Configurar um modelo]** ![](assets/fusion-scenario-settings-icon.png) e selecione o idioma no menu suspenso Idioma.

   >[!IMPORTANT]
   >
   >A seleção Languages corresponde aos idiomas disponíveis nas configurações do sistema e aborda apenas o nome do template público e sua descrição. Não é possível alterar um idioma de modelo depois que o modelo é salvo.

1. (Opcional) Para inserir uma descrição do modelo, clique em **[!UICONTROL Configurar um modelo]** ![](assets/fusion-scenario-settings-icon.png) e insira a descrição.
1. Edite aplicativos, módulos e ferramentas da mesma forma que faria ao editar um cenário padrão.

   Para adicionar ajuda contextual aos módulos, consulte [Configurar [!UICONTROL Assistente] funcionalidade](#set-up-wizard-functionality) neste artigo.

   >[!NOTE]
   >
   >Se o modelo incluir módulos que exigem a adição da conexão, das credenciais ou de outras informações confidenciais de privacidade, essas informações não serão compartilhadas com os usuários do modelo.

1. (Opcional) Clique em **[!UICONTROL Executar uma vez]** para testar seu modelo.
1. Clique em **[!UICONTROL Salvar]** ícone ![](assets/save-icon.png).

## Configurar [!UICONTROL Assistente] funcionalidade {#set-up-wizard-functionality}

A variável [!DNL Workfront Fusion template] [!UICONTROL Assistente] O permite fornecer instruções ou informações relacionadas aos campos específicos usados nos módulos aos futuros usuários do modelo.

1. Clique no módulo adicionado ao modelo para ver os campos do módulo.
1. Localize o campo onde deseja adicionar [!UICONTROL Assistente] informações e habilitar **[!UICONTROL Uso no Assistente]** para esse campo.
1. Insira as informações que você deseja tornar visíveis para usuários na [!UICONTROL Ajuda] campo.
1. (Opcional) Para permitir que os usuários vejam esse texto ao usar o modelo, habilite **[!UICONTROL Usar como valor padrão]**.
1. Repita as etapas 2 a 4 para cada campo para o qual deseja fornecer informações.
1. Clique em **[!UICONTROL OK]** para salvar as alterações e fechar o módulo.
