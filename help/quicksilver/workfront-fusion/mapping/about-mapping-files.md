---
content-type: overview
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: mapping
title: Sobre o mapeamento de arquivos no [!DNL Adobe Workfront Fusion]
description: Alguns módulos têm a capacidade de processar arquivos. Esses módulos podem retornar um arquivo de saída para ser enviado para processamento adicional ou exigir que um arquivo seja passado a eles para processamento. Antes que esses módulos possam trabalhar em conjunto para processar arquivos, eles devem ser mapeados um para o outro.
author: Becky
feature: Workfront Fusion
exl-id: 9ed5f176-86d8-4139-b582-c2f58aaed8d4
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '468'
ht-degree: 0%

---

# Sobre o mapeamento de arquivos no [!DNL Adobe Workfront Fusion]

Alguns módulos têm a capacidade de processar arquivos. Esses módulos podem retornar um arquivo de saída para ser enviado para processamento adicional ou exigir que um arquivo seja passado a eles para processamento. Antes que esses módulos possam trabalhar em conjunto para processar arquivos, eles devem ser mapeados um para o outro.

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
   <p>Requisito de licença herdada: [!UICONTROL [!DNL Workfront Fusion] para Automação e integração do trabalho] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produto</td> 
   <td>
   <p>Requisito atual do produto: se você tiver o [!UICONTROL Select] ou o [!UICONTROL Prime] [!DNL Adobe Workfront] Planejar, sua organização deve comprar [!DNL Adobe Workfront Fusion] bem como [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo. [!DNL Workfront Fusion] está incluído no [!UICONTROL Ultimate] [!DNL Workfront] plano.</p>
   <p>Ou</p>
   <p>Requisito de produto herdado: sua organização deve comprar [!DNL Adobe Workfront Fusion] bem como [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo.</p>
   </td> 
  </tr>  </tbody> 
</table>

Para descobrir que plano, tipo de licença ou acesso você tem, entre em contato com o [!DNL Workfront] administrador.

Para obter informações sobre [!DNL Adobe Workfront Fusion] licenças, consulte [[!DNL Adobe Workfront Fusion] licenças](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Mapeamento de arquivos

Os módulos que podem trabalhar com arquivos exigem duas informações:

* Nome do arquivo
* Conteúdo do arquivo (dados)

Ao mapear um arquivo, você escolhe os módulos no cenário a partir dos quais deseja obter os dados. O nome do arquivo e o conteúdo do arquivo são mapeados automaticamente como estão.

>[!NOTE]
>
>Se você precisar processar um arquivo de um URL, recomendamos usar o `HTTP > Get a File` para baixar o arquivo do URL e, em seguida, mapear o arquivo do `HTTP > Get a File` para o campo do módulo desejado em seu cenário.

>[!INFO]
>
>**Exemplo:** Este exemplo mostra como baixar documentos do [!DNL Adobe Workfront] para [!DNL Google Drive]. A variável [!DNL Workfront] acionador [!UICONTROL Assistir ao registro] retorna informações detalhadas sobre cada documento, incluindo seu nome e ID.
>
>O próximo módulo, [!UICONTROL Baixar documento]O baixa os dados reais para que eles possam ser carregados no Google Drive.
>
>Para mapear essas informações para [!DNL Google Drive] para que ele possa ser carregado, é necessário especificar o arquivo de origem a partir do qual as informações serão mapeadas. Se você selecionar a variável [!DNL Workfront] > [!UICONTROL Baixar documento] no arquivo de origem, [!DNL Workfront Fusion] mapeia o nome e o conteúdo do arquivo para que o documento do [!DNL Workfront] é carregado na pasta especificada do Google.
>
>![](assets/wf-download-document-350x605.png)
>
>No entanto, se você quiser renomear o arquivo, mas manter os dados como estão, poderá usar o [!UICONTROL Mapa] opção para mapear o nome do arquivo e o conteúdo do arquivo separadamente. Digite o nome completo do arquivo, incluindo a extensão. Formatos de texto e formatos binários, como fotos, vídeos e PDF, são suportados.
>
>![](assets/use-the-map-option-350x358.png)
