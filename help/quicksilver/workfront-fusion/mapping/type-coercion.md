---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: mapping
title: Coação de tipo no Adobe Workfront Fusion
description: Este documento descreve como [!DNL Adobe Workfront Fusion] O se comporta em situações em que recebe valores em formatos de dados esperados e inesperados.
author: Becky
feature: Workfront Fusion
exl-id: 847a17c9-bd67-4132-81a8-2a5fe8d516cb
source-git-commit: 97f91d663df86341a079894cff04d07c18b7bf08
workflow-type: tm+mt
source-wordcount: '590'
ht-degree: 1%

---

# Coação de tipo em [!DNL Adobe Workfront Fusion]

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] para automação e integração de trabalho] </p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produto</td> 
   <td>Sua organização deve comprar [!DNL Adobe Workfront Fusion] bem como [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo.</td> 
  </tr> 
 </tbody> 
</table>

Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com seu [!DNL Workfront] administrador.

Para obter informações sobre [!DNL Adobe Workfront Fusion] licenças, consulte [[!DNL Adobe Workfront Fusion] licenças](../../workfront-fusion/get-started/license-automation-vs-integration.md).

### Coação de tipo

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
   <td>array </td> 
   <td>array </td> 
   <td> <p>O valor é passado inalterado.</p> </td> 
  </tr> 
  <tr> 
   <td>array </td> 
   <td>other </td> 
   <td> <p>Se o valor recebido não for do tipo de matriz, [!DNL Workfront Fusion] criará uma matriz e o primeiro (e o único) elemento será o valor recebido.</p> </td> 
  </tr> 
  <tr> 
   <td>booleano </td> 
   <td>booleano </td> 
   <td> <p>O valor é passado inalterado.</p> </td> 
  </tr> 
  <tr> 
   <td>booleano </td> 
   <td>número </td> 
   <td> <p>O valor é convertido em Sim lógico, mesmo se o valor for 0.</p> </td> 
  </tr> 
  <tr> 
   <td>booleano </td> 
   <td>texto </td> 
   <td> <p>Se o valor for igual a false ou se o valor estiver vazio, ele será convertido em Não lógico. Caso contrário, será convertido em Sim lógico.</p> </td> 
  </tr> 
  <tr> 
   <td>booleano </td> 
   <td>other </td> 
   <td> <p>O valor é convertido em Sim lógico sempre que o valor recebido existir (não é nulo).</p> </td> 
  </tr> 
  <tr> 
   <td>buffer </td> 
   <td>buffer </td> 
   <td> <p>O valor é passado inalterado somente se a página de código estiver conforme esperado. Se a página de código for diferente, [!DNL Workfront Fusion] O tentará converter o valor recebido na página de códigos solicitada. Se essa conversão não for suportada, [!DNL Workfront Fusion] retornará um erro de validação.</p> </td> 
  </tr> 
  <tr> 
   <td>buffer </td> 
   <td>booleano </td> 
   <td> <p>O valor é convertido em texto (true/false) e, em seguida, em dados binários seguindo as etapas mencionadas acima para conversão em texto.</p> </td> 
  </tr> 
  <tr> 
   <td>buffer </td> 
   <td>data </td> 
   <td> <p>O valor é convertido em texto ISO 8601 e, em seguida, em dados binários seguindo as etapas mencionadas para conversão em texto.</p> </td> 
  </tr> 
  <tr> 
   <td>buffer </td> 
   <td>número </td> 
   <td> <p>O valor é convertido em texto e, em seguida, em dados binários seguindo as etapas mencionadas acima para conversão em texto.</p> </td> 
  </tr> 
  <tr> 
   <td>buffer </td> 
   <td>texto </td> 
   <td> <p>O valor é convertido em dados binários e codificado conforme esperado. Se a codificação esperada não for especificada, a codificação utf8 será usada.</p> </td> 
  </tr> 
  <tr> 
   <td>buffer </td> 
   <td>other </td> 
   <td> <p>[!DNL Workfront Fusion] retorna um erro de validação.</p> </td> 
  </tr> 
  <tr> 
   <td>coleção </td> 
   <td>coleção </td> 
   <td> <p>O valor é passado inalterado.</p> </td> 
  </tr> 
  <tr> 
   <td>coleção </td> 
   <td>other </td> 
   <td> <p>[!DNL Workfront Fusion] retorna um erro de validação.</p> </td> 
  </tr> 
  <tr> 
   <td>data </td> 
   <td>data </td> 
   <td> <p>O valor é passado inalterado.</p> </td> 
  </tr> 
  <tr> 
   <td>data </td> 
   <td>texto </td> 
   <td> <p>[!DNL Workfront Fusion] O tentará converter o texto em uma data. Se a conversão falhar, retornará um erro de validação. A data deve conter dia, mês e ano. A data pode conter a hora e o fuso horário. O fuso horário padrão é baseado em suas configurações. Exemplos:</p> <p><code>2016-06-20T17:26:44.356Z</code> </p> <p><code>2016-06-20 19:26:44 GMT+02:00</code> </p> <p><code>2016-06-20 19:26+0200</code> </p> <p><code>2016-06-20 17:26:44</code> </p> <p><code>2016-06-20</code> </p> <p><code>2016/06/20 17:26:44</code> </p> <p><code>2016/06/20 19:26:44+02:00</code> </p> <p><code>2016/06/20 17:26</code> </p> <p><code>2016/06/20 5:26 PM</code> </p> <p><code>2016/06/20</code> </p> <p><code>06/20/2016 17:26:44</code> </p> <p><code>06/20/2016 19:26:44+02:00</code> </p> <p><code>06/20/2016 17:26</code> </p> <p><code>06/20/2016 5:26 PM</code> </p> <p><code>06/20/2016</code> </p> <p><code>20.6.2016 17:26:44</code> </p> <p><code>20.6.2016 19:26:44+02:00</code> </p> <p><code>20.6.2016 17:26</code> </p> <p><code>20.6.2016</code> </p> </td> 
  </tr> 
  <tr> 
   <td>data </td> 
   <td>other </td> 
   <td> <p>[!DNL Workfront Fusion] retorna um erro de validação.</p> </td> 
  </tr> 
  <tr> 
   <td>número </td> 
   <td>número </td> 
   <td> <p>O valor é passado inalterado.</p> </td> 
  </tr> 
  <tr> 
   <td>número </td> 
   <td>texto </td> 
   <td> <p>[!DNL Workfront Fusion] O tentará converter o texto em um número. Se a conversão falhar, retornará um erro de validação.</p> </td> 
  </tr> 
  <tr> 
   <td>número </td> 
   <td>other </td> 
   <td> <p>[!DNL Workfront Fusion] retorna um erro de validação.</p> </td> 
  </tr> 
  <tr> 
   <td>texto </td> 
   <td>texto </td> 
   <td> <p>O valor é passado inalterado.</p> </td> 
  </tr> 
  <tr> 
   <td>texto </td> 
   <td>array </td> 
   <td> <p>Se a matriz em questão suportar conversão em texto, o valor será convertido. Caso contrário, [!DNL Workfront Fusion] retornará um erro de validação.</p> </td> 
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
   <td>other </td> 
   <td> <p>[!DNL Workfront Fusion] retorna um erro de validação.</p> </td> 
  </tr> 
  <tr> 
   <td>hora </td> 
   <td>hora </td> 
   <td> <p>O valor é passado inalterado.</p> </td> 
  </tr> 
  <tr> 
   <td>hora </td> 
   <td>texto </td> 
   <td> <p>[!DNL Workfront Fusion] tentará converter o tempo em horas:minutes:formato de segundos. Se a conversão falhar, retornará um erro de validação.</p> </td> 
  </tr> 
  <tr> 
   <td>hora </td> 
   <td>other </td> 
   <td> <p>[!DNL Workfront Fusion] retorna um erro de validação.</p> </td> 
  </tr> 
 </tbody> 
</table>
