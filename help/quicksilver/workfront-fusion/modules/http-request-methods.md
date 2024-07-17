---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Métodos de solicitação HTTP em  [!DNL Adobe Workfront Fusion]
description: Ao configurar uma chamada de API em um módulo do, é necessário preencher o campo do método de solicitação HTTP.
author: Becky
feature: Workfront Fusion
exl-id: 20b3c0f4-4a4c-4ba0-8570-ac39573ef1c0
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '410'
ht-degree: 0%

---

# Métodos de solicitação HTTP em [!DNL Adobe Workfront Fusion]

Ao configurar uma chamada de API em um módulo do, é necessário preencher o campo do método de solicitação HTTP.

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
  </tr> 
 </tbody> 
</table>

Para saber que plano, tipo de licença ou acesso você tem, contate o administrador do [!DNL Workfront].

Para obter informações sobre [!DNL Adobe Workfront Fusion] licenças, consulte [[!DNL Adobe Workfront Fusion] licenças](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Métodos HTTP

Use um dos seguintes métodos HTTP.

* **[!UICONTROL GET]**: recupera dados de um servidor Web com base em seus parâmetros. [!UICONTROL GET] solicita uma representação do recurso especificado e recebe uma mensagem de resposta [!UICONTROL 200 OK] com o conteúdo solicitado se for bem-sucedido.
* **[!UICONTROL POST]**: envia dados para um servidor Web com base em seus parâmetros. As solicitações [!UICONTROL POST] incluem ações como carregar um arquivo. Vários [!UICONTROL POST]s podem resultar em um resultado diferente de um único [!UICONTROL POST]. Portanto, tenha cuidado ao enviar vários [!UICONTROL POST]s involuntariamente. Se um [!UICONTROL POST] for bem-sucedido, você receberá uma mensagem de resposta [!UICONTROL 200 OK].
* **[!UICONTROL PUT]**: envia dados para um local no servidor Web com base em seus parâmetros. As solicitações [!UICONTROL PUT] incluem ações como carregar um arquivo. A diferença entre um [!UICONTROL PUT] e [!UICONTROL POST] é que o PUT é idempotente, o que significa que o resultado de um único [!UICONTROL PUT] bem-sucedido é o mesmo que muitos [!UICONTROL PUT]s idênticos. Se um PUT for bem-sucedido, você receberá uma mensagem de resposta 200 (geralmente 201 ou 204).
* **[!UICONTROL PATCH]**: (Não disponível para alguns módulos de chamada de API) Aplica modificações parciais a um recurso em um servidor Web com base em seus parâmetros. [!UICONTROL PATCH] não é idempotente, o que significa que o resultado de vários [!UICONTROL PATCH]&#39;s pode ter consequências não intencionais. Se um [!UICONTROL PATCH] for bem-sucedido, você receberá uma mensagem de resposta 200 (normalmente 204).
* **[!UICONTROL DELETE]**: exclui o recurso especificado do servidor Web com base em seus parâmetros (se o recurso existir). Se um [!UICONTROL DELETE] for bem-sucedido, você receberá uma mensagem de resposta 200 OK.
