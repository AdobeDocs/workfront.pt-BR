---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Adicionar um filtro a um cenário no [!DNL Adobe] Workfront Fusion
description: Em alguns cenários, é necessário trabalhar somente com pacotes que atendam a critérios específicos. Os filtros permitem selecionar esses pacotes.
author: Becky
feature: Workfront Fusion
exl-id: 114ab37f-71e0-494e-9f3d-93ff5a9d13ba
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '576'
ht-degree: 0%

---

# Adicionar um filtro a um cenário no [!DNL Adobe Workfront Fusion]

Em alguns cenários, é necessário trabalhar somente com pacotes que atendam a critérios específicos. Os filtros permitem selecionar esses pacotes.

<!--

For example, you could create a scenario with the [!UICONTROL Watch records] trigger for [!DNL Salesforce] to capture only records containing a specific word written by a specific author.

-->

Você pode adicionar um filtro entre dois módulos e verificar se os pacotes recebidos dos módulos anteriores atendem a condições de filtro específicas:

* Se isso acontecer, os pacotes serão transmitidos para o próximo módulo no cenário.
* Caso contrário, o processamento dos pacotes será encerrado.

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

Para obter informações sobre [!DNL Adobe Workfront Fusion] licenças, consulte [[!DNL Adobe Workfront Fusion] licenças](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Pré-requisitos

Você deve adicionar ambos os módulos a um cenário antes de poder adicionar um filtro entre eles.

## Adicione um filtro entre dois módulos:

1. Clique em **[!UICONTROL Cenários]** ![](assets/scenarios-icon.png) no painel esquerdo, selecione o cenário para abri-lo.
1. No canto superior direito da janela, clique em **[!UICONTROL Editar]**.
1. Clique na linha de conexão entre os módulos.
1. Na caixa exibida, digite um **[!UICONTROL Rótulo]** para o filtro.
1. Definir um filtro **[!UICONTROL Condição]**.

   É possível inserir um ou dois operandos nas duas caixas. Se você inserir operandos em ambas as caixas, será possível selecionar um operador no menu suspenso entre elas para especificar a relação entre elas.

   >[!TIP]
   >
   >Nos campos de operando, você pode inserir valores da mesma maneira que os mapearia, conforme descrito em [Mapear informações de um módulo para outro no [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

   Por exemplo, se você deseja que o filtro localize arquivos em [!DNL Adobe Workfront] terminando com XML e transmitindo-as para [!DNL Dropbox], você digitaria **[!UICONTROL Nome do arquivo]** na primeira caixa e .**[!UICONTROL xml]** na segunda caixa. No menu suspenso entre elas, você selecionaria **[!UICONTROL Termina com (não diferencia maiúsculas de minúsculas)]**. Esse filtro se aplicaria aos pacotes recebidos do primeiro módulo (Workfront). Somente pacotes contendo arquivos XML passariam para o próximo módulo ([!DNL Dropbox]).

   ![](assets/set-up-filter-box-350x368.jpg)

1. Clique em **[!DNL OK]**.

## Copiar um filtro

Atualmente, o editor de cenários não inclui um recurso para copiar um filtro.

>[!NOTE]
>
>Se você copiar os módulos em ambos os lados do filtro, o filtro também será copiado.
>
>Para obter mais informações sobre a cópia de módulos, consulte [Copiar módulos ou cenários no [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/copy-modules-or-scenarios.md)

Para copiar um filtro sem copiar módulos, é possível usar [!DNL Google] Chrome para a seguinte solução alternativa:

1. Instale o [!UICONTROL [!DNL Adobe Workfront Fusion] DevTool Chrome] extensão.
1. Entrada [!DNL Workfront Fusion], abra o cenário.
1. Clique no menu de três pontos do Chrome e clique em **[!UICONTROL Mais ferramentas*]* > **[!UICONTROL Ferramentas do desenvolvedor]**.

1. No [!UICONTROL Ferramentas do desenvolvedor] painel que for exibido, na barra de menus na parte superior, clique na guia [!UICONTROL Workfront Fusion] guia.

   ![](assets/copy-a-filter-350x174.png)

1. Clique em **[!UICONTROL Ferramentas]** ícone ![](assets/devtools-tools-icon.png) na barra lateral esquerda.

1. Clique em **[!UICONTROL Copiar Filtro]**, em seguida, configure o **[!UICONTROL Copiar Filtro]** no painel direito:

   1. Defina o **[!UICONTROL Módulo de origem]** como o módulo logo após o filtro que você deseja copiar.
   1. Defina o **[!UICONTROL Módulo do Target]** como o módulo, antes do filtro que você deseja copiar.

1. Clique em **[!UICONTROL Executar]**.
