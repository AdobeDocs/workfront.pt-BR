---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Métodos de solicitação HTTP em [!DNL Adobe Workfront Fusion]
description: Ao configurar uma chamada de API em um módulo do, é necessário preencher o campo do método de solicitação HTTP.
author: Becky
feature: Workfront Fusion
exl-id: 20b3c0f4-4a4c-4ba0-8570-ac39573ef1c0
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '402'
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

## Métodos HTTP

Use um dos seguintes métodos HTTP.

* **[!UICONTROL GET]**: recupera dados de um servidor Web com base em seus parâmetros. [!UICONTROL GET] solicita uma representação do recurso especificado e recebe uma [!UICONTROL 200 OK] mensagem de resposta com o conteúdo solicitado em caso de sucesso.
* **[!UICONTROL POST]**: envia dados a um servidor Web com base em seus parâmetros. [!UICONTROL POST] As solicitações incluem ações como carregar um arquivo. Múltiplo [!UICONTROL POST]s pode resultar em um resultado diferente de um único [!UICONTROL POST], portanto, tenha cuidado ao enviar vários [!UICONTROL POST]s. Se uma [!UICONTROL POST] for bem-sucedido, você receberá um [!UICONTROL 200 OK] mensagem de resposta.
* **[!UICONTROL PUT]**: envia dados a um local no servidor Web com base em seus parâmetros. [!UICONTROL PUT] As solicitações incluem ações como carregar um arquivo. A diferença entre um [!UICONTROL PUT] e [!UICONTROL POST] é que o PUT é idempotente, o que significa que o resultado de um único sucesso [!UICONTROL PUT] é o mesmo que muitos [!UICONTROL PUT]s. Se um PUT for bem-sucedido, você receberá uma mensagem de resposta 200 (geralmente 201 ou 204).
* **[!UICONTROL PATCH]**: (Não disponível para alguns módulos de chamada de API) Aplica modificações parciais a um recurso em um servidor Web com base em seus parâmetros. [!UICONTROL PATCH] não é idempotente, o que significa que o resultado de vários [!UICONTROL PATCH]Isso pode ter consequências não intencionais. Se um [!UICONTROL PATCH] for bem-sucedido, você receberá uma mensagem de resposta 200 (geralmente 204).
* **[!UICONTROL DELETE]**: exclui o recurso especificado do servidor Web com base em seus parâmetros (se o recurso existir). Se um [!UICONTROL DELETE] for bem-sucedido, você receberá uma mensagem de resposta 200 OK.
