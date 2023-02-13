---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Adicione um filtro a um cenário em [!DNL Adobe] Workfront Fusion
description: Em alguns cenários, você precisa trabalhar somente com pacotes que atendem a critérios específicos. Os filtros permitem selecionar esses pacotes.
author: Becky
feature: Workfront Fusion
exl-id: 114ab37f-71e0-494e-9f3d-93ff5a9d13ba
source-git-commit: 59941ea1ce523a0d1036138a83f771b058049b34
workflow-type: tm+mt
source-wordcount: '528'
ht-degree: 0%

---

# Adicione um filtro a um cenário em [!DNL Adobe Workfront Fusion]

Em alguns cenários, você precisa trabalhar somente com pacotes que atendem a critérios específicos. Os filtros permitem selecionar esses pacotes.

<!--

For example, you could create a scenario with the [!UICONTROL Watch records] trigger for [!DNL Salesforce] to capture only records containing a specific word written by a specific author.

-->

Você pode adicionar um filtro entre dois módulos e verificar se os pacotes recebidos dos módulos anteriores atendem a condições de filtro específicas:

* Se o fizerem, os pacotes passarão para o próximo módulo no cenário.
* Caso contrário, o processamento dos pacotes terminará.

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

Para obter informações sobre [!DNL Adobe Workfront Fusion] licenças, consulte [[!DNL Adobe Workfront Fusion] licenças](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Pré-requisitos

Você deve adicionar ambos os módulos a um cenário antes de poder adicionar um filtro entre eles.

## Adicione um filtro entre dois módulos:

1. Clique em **[!UICONTROL Cenários]** ![](assets/scenarios-icon.png) no painel esquerdo, selecione o cenário para abri-lo.
1. No canto superior direito da janela, clique em **[!UICONTROL Editar]**.
1. Clique na linha de conexão entre os módulos.
1. Na caixa exibida, digite uma **[!UICONTROL Rótulo]** para o filtro .
1. Definir um filtro **[!UICONTROL Condição]**.

   Você pode inserir um ou dois operandos nas duas caixas. Se você inserir operandos em ambas as caixas, poderá selecionar um operador no menu suspenso entre eles para especificar a relação entre eles.

   >[!TIP]
   >
   >Nos campos de operando, é possível inserir valores da mesma forma que você os mapearia, conforme descrito em [Mapear informações de um módulo para outro no [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

   Por exemplo, se você deseja que o filtro encontre arquivos em [!DNL Adobe Workfront] terminar com XML e passá-los para [!DNL Dropbox], insira **[!UICONTROL Nome do arquivo]** na primeira caixa e .**[!UICONTROL xml]** na segunda caixa. No menu suspenso entre elas, você selecionaria **[!UICONTROL Termina com (não diferencia maiúsculas de minúsculas)]**. Esse filtro seria aplicado aos pacotes de entrada do primeiro módulo (Workfront). Somente pacotes contendo arquivos XML passariam para o próximo módulo ([!DNL Dropbox]).

   ![](assets/set-up-filter-box-350x368.jpg)

1. Clique em **[!DNL OK]**.

## Copiar um filtro

Atualmente, o editor de cenário não inclui um recurso para copiar um filtro.

>[!NOTE]
>
>Se você copiar os módulos em qualquer lado do filtro, o filtro também será copiado.
>
>Para obter mais informações sobre cópia de módulos, consulte [Copie módulos ou cenários em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/copy-modules-or-scenarios.md)

Para copiar um filtro sem copiar módulos, você pode usar [!DNL Google] Chrome para a seguinte solução alternativa:

1. Instale o [!UICONTROL [!DNL Adobe Workfront Fusion] DevTool Chrome] extensão.
1. Em [!DNL Workfront Fusion], abra o cenário .
1. Clique no menu de três pontos do Chrome e, em seguida, clique em **[!UICONTROL Mais ferramentas*]* > **[!UICONTROL Ferramentas do desenvolvedor]**.

1. No [!UICONTROL Ferramentas do desenvolvedor] painel exibido, na barra de menus na parte superior, clique no botão [!UICONTROL Workfront Fusion] guia .

   ![](assets/copy-a-filter-350x174.png)

1. Clique no botão **[!UICONTROL Ferramentas]** ícone ![](assets/devtools-tools-icon.png) na barra lateral esquerda.

1. Clique em **[!UICONTROL Copiar Filtro]**, em seguida, configure o **[!UICONTROL Copiar Filtro]** no painel lateral direito:

   1. Defina as **[!UICONTROL Módulo de origem]** como o módulo logo após o filtro que você deseja copiar.
   1. Defina as **[!UICONTROL Módulo Target]** como o módulo antes do filtro que você deseja copiar.

1. Clique em **[!UICONTROL Executar]**.
