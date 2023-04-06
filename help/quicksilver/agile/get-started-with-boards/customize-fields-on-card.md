---
product-area: agile-and-teams
navigation-topic: customize-fields-on-card
title: Personalizar quais campos são exibidos em um cartão
description: Você pode personalizar quais campos são exibidos em um cartão desabilitando um campo para que ele não seja exibido no cartão completo ou na visualização condensada, ou ocultando um campo na visualização condensada do cartão.
author: Lisa
feature: Agile
source-git-commit: 48dc1bcbaa5755888c45fdafbd6471c9ee073a45
workflow-type: tm+mt
source-wordcount: '502'
ht-degree: 0%

---


# Personalizar quais campos são exibidos em um cartão

Por padrão, todos os campos disponíveis são exibidos em um cartão, tanto na exibição completa quando o cartão está aberto, quanto na exibição condensada do cartão no quadro. Você pode personalizar quais campos são exibidos ao:

* Desativar um campo para que ele não seja exibido em nenhuma das exibições
* Ocultar um campo na visualização de cartão condensado

Se um campo contiver um valor e você desativar o campo, o valor será retido se o campo for ativado novamente mais tarde.

Também é possível exibir campos personalizados que foram criados anteriormente. Não é possível criar e criar novos campos personalizados dentro de um quadro.

>[!NOTE]
>
>Todas as personalizações de campo feitas se aplicam apenas ao quadro em que você está trabalhando.

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] plano*</strong></td> 
   <td> <p>Qualquer Um</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licença*</strong></td> 
   <td> <p>[!UICONTROL Solicitação] ou superior</p> </td> 
  </tr>
   </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com seu [!DNL Workfront] administrador.

## Configurar cartões {#configure-cards}

1. Clique no botão **[!UICONTROL Menu principal]** ícone ![](assets/main-menu-icon.png) no canto superior direito de [!DNL Adobe Workfront], depois clique em **[!UICONTROL Quadros]**.
1. Acesse um quadro. Para obter mais informações, consulte [Criar ou editar um quadro](../../agile/get-started-with-boards/create-edit-board.md).
1. Clique em [!UICONTROL **Configurar**] à direita do quadro para abrir o painel Configurar .
1. Expandir [!UICONTROL **Cartões**].

   A maioria dos campos é ativada por padrão.

1. Desative um campo para desativá-lo em ambas as visualizações de cartão.
1. Clique no ícone Ocultar ![Ícone Ocultar](assets/eye-hide-icon.png) ao lado de um campo para ocultá-lo na exibição condensada.
1. Para exibir todos os campos em ambas as exibições, clique em [!UICONTROL **Restaurar todos os campos como padrão**].
1. Clique em [!UICONTROL **Ocultar configuração**] para fechar o painel Configurar .

## Adicionar campos personalizados aos cartões

Os campos personalizados estão disponíveis em cartões conectados. Eles só são visíveis na visualização completa do cartão, não na visualização condensada no quadro.

>[!NOTE]
>
>Ao adicionar um campo personalizado aos cartões, os dados no cartão são somente leitura.

1. Acesse um quadro e clique em [!UICONTROL **Configurar**] para abrir o painel Configurar .
1. Expandir [!UICONTROL **Cartões**].
1. Em [!UICONTROL Campos de cartão], clique em [!UICONTROL **Adicionar campo personalizado**].
1. Selecionar [!UICONTROL **Tarefa**] ou [!UICONTROL **Problema**].

   As categorias de campos disponíveis para tarefas ou problemas são exibidas. Expanda uma categoria para ver todos os campos. Também é possível procurar um campo.

   ![Procurar campo personalizado](assets/boards-search-for-custom-field.png)

   >[!NOTE]
   >
   >Os seguintes tipos de campo não estão disponíveis para adicionar cartões: Adobe XD, Imagem, PDF, Vídeo.

1. Selecione o nome do campo.
1. (Opcional) Clique em no **[!UICONTROL Valor do campo]** para alterar esse campo personalizado para outro.
1. (Opcional) Altere o **[!UICONTROL Rótulo do campo]** ao nome do campo que você deseja exibir nos cartões.
1. Quando terminar de fazer alterações, clique em [!UICONTROL **Salvar campo**].

   ![Valor e rótulo do campo personalizado](assets/save-custom-field-value-label.png)

   O campo personalizado é adicionado à lista de campos disponíveis e é ativado por padrão. Você pode desativar o campo personalizado seguindo as etapas da variável [Configurar cartões](customize-fields-on-card.md#configure-cards) seção acima, edite o campo ou exclua-o de todos os cartões.

