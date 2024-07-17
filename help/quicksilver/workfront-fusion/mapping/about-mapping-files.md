---
content-type: overview
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: mapping
title: Sobre o mapeamento de arquivos em [!DNL Adobe Workfront Fusion]
description: Alguns módulos têm a capacidade de processar arquivos. Esses módulos podem retornar um arquivo de saída para ser enviado para processamento adicional ou exigir que um arquivo seja passado a eles para processamento. Antes que esses módulos possam trabalhar em conjunto para processar arquivos, eles devem ser mapeados uns para os outros.
author: Becky
feature: Workfront Fusion
exl-id: 9ed5f176-86d8-4139-b582-c2f58aaed8d4
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '468'
ht-degree: 0%

---

# Sobre o mapeamento de arquivos em [!DNL Adobe Workfront Fusion]

Alguns módulos têm a capacidade de processar arquivos. Esses módulos podem retornar um arquivo de saída para ser enviado para processamento adicional ou exigir que um arquivo seja passado a eles para processamento. Antes que esses módulos possam trabalhar em conjunto para processar arquivos, eles devem ser mapeados uns para os outros.

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
   <p>Requisito de licença herdada: [!UICONTROL [!DNL Workfront Fusion] para Automação e Integração do Trabalho] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produto</td> 
   <td>
   <p>Requisito atual do produto: se você tiver o Plano [!DNL Adobe Workfront] da [!UICONTROL Select] ou da [!UICONTROL Prime], sua organização deve comprar o [!DNL Adobe Workfront Fusion] e o [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo. [!DNL Workfront Fusion] está incluído no plano [!DNL Workfront] do [!UICONTROL Ultimate].</p>
   <p>Ou</p>
   <p>Requisito de produto herdado: sua organização deve comprar o [!DNL Adobe Workfront Fusion] e o [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo.</p>
   </td> 
  </tr>  </tbody> 
</table>

Para saber que plano, tipo de licença ou acesso você tem, contate o administrador do [!DNL Workfront].

Para obter informações sobre [!DNL Adobe Workfront Fusion] licenças, consulte [[!DNL Adobe Workfront Fusion] licenças](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Mapeamento de arquivos

Os módulos que podem trabalhar com arquivos exigem duas informações:

* Nome do arquivo
* Conteúdo do arquivo (dados)

Ao mapear um arquivo, você escolhe os módulos no cenário a partir dos quais deseja obter os dados. O nome do arquivo e o conteúdo do arquivo são mapeados automaticamente como estão.

>[!NOTE]
>
>Se você precisar processar um arquivo de uma URL, recomendamos usar o módulo `HTTP > Get a File` para baixar o arquivo da URL e, em seguida, mapear o arquivo do módulo `HTTP > Get a File` para o campo do módulo desejado em seu cenário.

>[!INFO]
>
>**Exemplo:** este exemplo mostra como baixar documentos de [!DNL Adobe Workfront] para [!DNL Google Drive]. O [!DNL Workfront] acionador [!UICONTROL Registro de observação] retorna informações detalhadas sobre cada documento, incluindo seu nome e ID.
>
>O próximo módulo, [!UICONTROL Baixar Documento], baixa os dados reais para que eles possam ser carregados no Google Drive.
>
>Para mapear essas informações para [!DNL Google Drive] para que elas possam ser carregadas, é necessário especificar o arquivo de origem a partir do qual as informações serão mapeadas. Se você selecionar a opção [!DNL Workfront] > [!UICONTROL Baixar Documento] no arquivo de origem, o [!DNL Workfront Fusion] mapeará o nome do arquivo e o conteúdo do arquivo para que o documento de [!DNL Workfront] seja carregado na pasta especificada do Google.
>
>![](assets/wf-download-document-350x605.png)
>
>No entanto, se você quiser renomear o arquivo, mas manter os dados como estão, você pode usar a opção [!UICONTROL Mapear] para mapear o nome do arquivo e o conteúdo do arquivo separadamente. Digite o nome completo do arquivo, incluindo a extensão. Formatos de texto e formatos binários, como fotos, vídeos e PDF, são suportados.
>
>![](assets/use-the-map-option-350x358.png)
