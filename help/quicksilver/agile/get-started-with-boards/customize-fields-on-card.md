---
product-area: agile-and-teams
navigation-topic: customize-fields-on-card
title: Personalizar quais campos são exibidos em um cartão
description: Você pode personalizar quais campos são exibidos em um cartão desativando um campo para que ele não seja exibido no cartão completo ou na exibição condensada, ou ocultando um campo na exibição de cartão condensada.
author: Lisa
feature: Agile
exl-id: 28fa6455-04dd-4115-9ead-cb3e7c26289e
source-git-commit: 80e0a053f39991d3ed8d9bd2a11a8da2d5de588e
workflow-type: tm+mt
source-wordcount: '529'
ht-degree: 0%

---

# Personalizar quais campos são exibidos em um cartão

Por padrão, todos os campos disponíveis são exibidos em um cartão, tanto na exibição completa quando o cartão está aberto quanto na exibição condensada do cartão no quadro. Você pode personalizar quais campos serão exibidos ao:

* Desabilitação de um campo para que ele não seja exibido em nenhuma exibição
* Ocultar um campo na exibição de cartão condensado

Se um campo contiver um valor e você desativar o campo, o valor será retido se você ativar o campo novamente mais tarde.

As seções (que aparecem como as opções de navegação à esquerda nos detalhes do cartão) também estão disponíveis para exibição e ocultação.

Você também pode exibir campos personalizados criados anteriormente. Não é possível projetar e criar novos campos personalizados em um quadro.

>[!NOTE]
>
>As personalizações de campo que você fizer se aplicam somente ao painel em que está trabalhando.

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas deste artigo:

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

&#42;Para descobrir que plano, tipo de licença ou acesso você tem, entre em contato com o [!DNL Workfront] administrador.

## Configurar cartões {#configure-cards}

1. Clique em **[!UICONTROL Menu principal]** ícone ![](assets/main-menu-icon.png) no canto superior direito de [!DNL Adobe Workfront]e, em seguida, clique em **[!UICONTROL Quadros]**.
1. Acessar um quadro. Para obter informações, consulte [Criar ou editar um quadro](../../agile/get-started-with-boards/create-edit-board.md).
1. Clique em [!UICONTROL **Configurar**] à direita da placa para abrir o painel Configurar.
1. Expandir [!UICONTROL **Cartões**].

   A maioria dos campos e seções é ativada por padrão.

1. Desative um campo ou seção para desativá-lo nas duas visualizações de cartão.
1. Clique no ícone Ocultar ![Ícone Ocultar](assets/eye-hide-icon.png) ao lado de um campo ou seção para ocultá-lo na exibição condensada.
1. Para exibir todos os campos e seções em ambas as exibições, clique em [!UICONTROL **Restaurar todos os campos para o padrão**].
1. Clique em [!UICONTROL **Ocultar configuração**] para fechar o painel Configurar.

## Adicionar campos personalizados a cartões

Campos personalizados estão disponíveis em cartões conectados. Eles só são visíveis na exibição de cartão completo, não na exibição condensada no quadro.

>[!NOTE]
>
>Ao adicionar um campo personalizado a seus cartões, os dados no cartão são somente leitura.

1. Acesse um quadro e clique em [!UICONTROL **Configurar**] para abrir o painel Configurar.
1. Expandir [!UICONTROL **Cartões**].
1. Em [!UICONTROL Campos de cartão], clique em [!UICONTROL **Adicionar campo personalizado**].
1. Selecionar [!UICONTROL **Tarefa**] ou [!UICONTROL **Problema**].

   As categorias de campos disponíveis para tarefas ou problemas são exibidas. Expanda uma categoria para ver todos os campos. Também é possível pesquisar por um campo.

   ![Pesquisar campo personalizado](assets/boards-search-for-custom-field.png)

   >[!NOTE]
   >
   >Os seguintes tipos de campo não estão disponíveis para adicionar a placas: Adobe XD, Image, PDF, Video.

1. Selecione o nome do campo.
1. (Opcional) Clique no link **[!UICONTROL Valor do campo]** para alterar este campo personalizado para outro.
1. (Opcional) Altere a **[!UICONTROL Rótulo do campo]** ao nome do campo que você deseja que apareça nos cartões.
1. Quando terminar de fazer alterações, clique em [!UICONTROL **Salvar campo**].

   ![Valor e rótulo do campo personalizado](assets/save-custom-field-value-label.png)

   O campo personalizado é adicionado à lista de campos disponíveis e é ativado por padrão. Você pode desativar o campo personalizado seguindo as etapas na [Configurar cartões](customize-fields-on-card.md#configure-cards) acima, edite o campo ou exclua-o de todos os cartões.
