---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: mapping
title: Coerção de tipo no Adobe Workfront Fusion
description: Este documento descreve como [!DNL Adobe Workfront Fusion] O se comporta em situações em que recebe valores em formatos de dados esperados e inesperados.
author: Becky
feature: Workfront Fusion
exl-id: 847a17c9-bd67-4132-81a8-2a5fe8d516cb
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '638'
ht-degree: 1%

---

# Coerção de tipo em [!DNL Adobe Workfront Fusion]

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
  </tr> 
 </tbody> 
</table>

Para descobrir que plano, tipo de licença ou acesso você tem, entre em contato com o [!DNL Workfront] administrador.

Para obter informações sobre [!DNL Adobe Workfront Fusion] licenças, consulte [[!DNL Adobe Workfront Fusion] licenças](../../workfront-fusion/get-started/license-automation-vs-integration.md).

### Coerção de tipo

Este documento descreve como [!DNL Adobe Workfront Fusion] O se comporta em situações em que recebe valores em formatos de dados esperados e inesperados.

<table style="table-layout:auto">
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Esperado</th> 
   <th>Recebido</th> 
   <th> <p>Descrição</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>matriz </td> 
   <td>matriz </td> 
   <td> <p>O valor é entregue inalterado.</p> </td> 
  </tr> 
  <tr> 
   <td>matriz </td> 
   <td>outro </td> 
   <td> <p>Se o valor recebido não for do tipo de matriz, [!DNL Workfront Fusion] criará uma matriz e o primeiro (e único) elemento será o valor recebido.</p> </td> 
  </tr> 
  <tr> 
   <td>booleano </td> 
   <td>booleano </td> 
   <td> <p>O valor é entregue inalterado.</p> </td> 
  </tr> 
  <tr> 
   <td>booleano </td> 
   <td>número </td> 
   <td> <p>O valor é convertido em Sim lógico, mesmo se o valor for 0.</p> </td> 
  </tr> 
  <tr> 
   <td>booleano </td> 
   <td>texto </td> 
   <td> <p>Se o valor for igual a false ou o valor estiver vazio, ele será convertido para o Nº lógico. Caso contrário, será convertido em Sim lógico.</p> </td> 
  </tr> 
  <tr> 
   <td>booleano </td> 
   <td>outro </td> 
   <td> <p>O valor é convertido em Sim lógico sempre que o valor recebido existe (não é nulo).</p> </td> 
  </tr> 
  <tr> 
   <td>buffer </td> 
   <td>buffer </td> 
   <td> <p>O valor é entregue inalterado somente se a página de código for a esperada. Se a página de código for diferente, [!DNL Workfront Fusion] tentará converter o valor recebido na página de código solicitada. Se essa conversão não for suportada, [!DNL Workfront Fusion] retornará um erro de validação.</p> </td> 
  </tr> 
  <tr> 
   <td>buffer </td> 
   <td>booleano </td> 
   <td> <p>O valor é convertido em texto (true/false) e em dados binários seguindo as etapas mencionadas acima para a conversão em texto.</p> </td> 
  </tr> 
  <tr> 
   <td>buffer </td> 
   <td>data </td> 
   <td> <p>O valor é convertido em texto ISO 8601 e em dados binários seguindo as etapas mencionadas para a conversão em texto.</p> </td> 
  </tr> 
  <tr> 
   <td>buffer </td> 
   <td>número </td> 
   <td> <p>O valor é convertido em texto e, em seguida, em dados binários seguindo as etapas mencionadas acima para converter em texto.</p> </td> 
  </tr> 
  <tr> 
   <td>buffer </td> 
   <td>texto </td> 
   <td> <p>O valor é convertido em dados binários e codificado conforme esperado. Se a codificação esperada não for especificada, a codificação utf8 será usada.</p> </td> 
  </tr> 
  <tr> 
   <td>buffer </td> 
   <td>outro </td> 
   <td> <p>[!DNL Workfront Fusion] retorna um erro de validação.</p> </td> 
  </tr> 
  <tr> 
   <td>coleção </td> 
   <td>coleção </td> 
   <td> <p>O valor é entregue inalterado.</p> </td> 
  </tr> 
  <tr> 
   <td>coleção </td> 
   <td>outro </td> 
   <td> <p>[!DNL Workfront Fusion] retorna um erro de validação.</p> </td> 
  </tr> 
  <tr> 
   <td>data </td> 
   <td>data </td> 
   <td> <p>O valor é entregue inalterado.</p> </td> 
  </tr> 
  <tr> 
   <td>data </td> 
   <td>texto </td> 
   <td> <p>[!DNL Workfront Fusion] tentará converter o texto em uma data. Se a conversão falhar, retornará um erro de validação. A data deve conter dia, mês e ano. A data pode conter a hora e o fuso horário. O fuso horário padrão é baseado em suas configurações. Exemplos:</p> <p><code>2016-06-20T17:26:44.356Z</code> </p> <p><code>2016-06-20 19:26:44 GMT+02:00</code> </p> <p><code>2016-06-20 19:26+0200</code> </p> <p><code>2016-06-20 17:26:44</code> </p> <p><code>2016-06-20</code> </p> <p><code>2016/06/20 17:26:44</code> </p> <p><code>2016/06/20 19:26:44+02:00</code> </p> <p><code>2016/06/20 17:26</code> </p> <p><code>2016/06/20 5:26 PM</code> </p> <p><code>2016/06/20</code> </p> <p><code>06/20/2016 17:26:44</code> </p> <p><code>06/20/2016 19:26:44+02:00</code> </p> <p><code>06/20/2016 17:26</code> </p> <p><code>06/20/2016 5:26 PM</code> </p> <p><code>06/20/2016</code> </p> <p><code>20.6.2016 17:26:44</code> </p> <p><code>20.6.2016 19:26:44+02:00</code> </p> <p><code>20.6.2016 17:26</code> </p> <p><code>20.6.2016</code> </p> </td> 
  </tr> 
  <tr> 
   <td>data </td> 
   <td>outro </td> 
   <td> <p>[!DNL Workfront Fusion] retorna um erro de validação.</p> </td> 
  </tr> 
  <tr> 
   <td>número </td> 
   <td>número </td> 
   <td> <p>O valor é entregue inalterado.</p> </td> 
  </tr> 
  <tr> 
   <td>número </td> 
   <td>texto </td> 
   <td> <p>[!DNL Workfront Fusion] tentará converter o texto em um número. Se a conversão falhar, retornará um erro de validação.</p> </td> 
  </tr> 
  <tr> 
   <td>número </td> 
   <td>outro </td> 
   <td> <p>[!DNL Workfront Fusion] retorna um erro de validação.</p> </td> 
  </tr> 
  <tr> 
   <td>texto </td> 
   <td>texto </td> 
   <td> <p>O valor é entregue inalterado.</p> </td> 
  </tr> 
  <tr> 
   <td>texto </td> 
   <td>matriz </td> 
   <td> <p>Se a matriz fornecida suportar conversão para texto, o valor será convertido. Caso contrário, [!DNL Workfront Fusion] retornará um erro de validação.</p> </td> 
  </tr> 
  <tr> 
   <td>texto </td> 
   <td>booleano </td> 
   <td> <p>O valor é convertido em texto (true/false).</p> </td> 
  </tr> 
  <tr> 
   <td>texto </td> 
   <td>buffer </td> 
   <td> <p>Se a codificação de texto for especificada para dados binários, o valor será convertido em texto. Caso contrário, [!DNL Workfront Fusion] retornará um erro de validação.</p> </td> 
  </tr> 
  <tr> 
   <td>texto </td> 
   <td>data </td> 
   <td> <p>O valor é convertido em texto ISO 8601.</p> </td> 
  </tr> 
  <tr> 
   <td>texto </td> 
   <td>número </td> 
   <td> <p>O valor é convertido em texto.</p> </td> 
  </tr> 
  <tr> 
   <td>texto </td> 
   <td>outro </td> 
   <td> <p>[!DNL Workfront Fusion] retorna um erro de validação.</p> </td> 
  </tr> 
  <tr> 
   <td>hora </td> 
   <td>hora </td> 
   <td> <p>O valor é entregue inalterado.</p> </td> 
  </tr> 
  <tr> 
   <td>hora </td> 
   <td>texto </td> 
   <td> <p>[!DNL Workfront Fusion] tentará converter o tempo para as horas:minutes:segundos. Se a conversão falhar, retornará um erro de validação.</p> </td> 
  </tr> 
  <tr> 
   <td>hora </td> 
   <td>outro </td> 
   <td> <p>[!DNL Workfront Fusion] retorna um erro de validação.</p> </td> 
  </tr> 
 </tbody> 
</table>
