---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Métodos de solicitação HTTP em [!DNL Adobe Workfront Fusion]
description: Ao configurar uma chamada de API em um módulo, é necessário preencher o campo para o método de solicitação HTTP.
author: Becky
feature: Workfront Fusion
exl-id: 20b3c0f4-4a4c-4ba0-8570-ac39573ef1c0
source-git-commit: e58ff769015b8c4e34b34eea653f55a296eea371
workflow-type: tm+mt
source-wordcount: '354'
ht-degree: 0%

---

# Métodos de solicitação HTTP em [!DNL Adobe Workfront Fusion]

Ao configurar uma chamada de API em um módulo, é necessário preencher o campo para o método de solicitação HTTP.

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

## Métodos HTTP

Use um dos métodos HTTP a seguir.

* **[!UICONTROL GET]**: Recupera dados de um servidor da Web com base em seus parâmetros. [!UICONTROL GET] solicita uma representação do recurso especificado e recebe uma [!UICONTROL 200 OK] mensagem de resposta com o conteúdo solicitado, se bem-sucedido.
* **[!UICONTROL POST]**: Envia dados para um servidor da Web com base em seus parâmetros. [!UICONTROL POST] as solicitações incluem ações como carregar um arquivo. Vários [!UICONTROL POST]pode resultar em resultados diferentes de um único [!UICONTROL POST], portanto, tenha cuidado ao enviar várias [!UICONTROL POST]s. Se uma [!UICONTROL POST] for bem-sucedido, você receberá uma [!UICONTROL 200 OK] mensagem de resposta.
* **[!UICONTROL PUT]**: Envia dados para um local no servidor da Web com base em seus parâmetros. [!UICONTROL PUT] as solicitações incluem ações como carregar um arquivo. A diferença entre uma [!UICONTROL PUT] e [!UICONTROL POST] é que PUT é idempotente, o que significa que o resultado de um único sucesso [!UICONTROL PUT] é igual a muitos idênticos [!UICONTROL PUT]s. Se um PUT for bem-sucedido, você receberá uma mensagem de resposta 200 (geralmente 201 ou 204).
* **[!UICONTROL PATCH]**: (Não disponível para alguns módulos de chamada de API) Aplica modificações parciais a um recurso em um servidor da Web com base em seus parâmetros. [!UICONTROL PATCH] não é idempotente, o que significa que o resultado de vários [!UICONTROL PATCH]O pode ter consequências não intencionais. Se uma [!UICONTROL PATCH] for bem-sucedido, você receberá uma mensagem de resposta 200 (geralmente 204).
* **[!UICONTROL DELETE]**: Exclui o recurso especificado do servidor da Web com base em seus parâmetros (se o recurso existir). Se uma [!UICONTROL DELETE] for bem-sucedido, você receberá uma mensagem de resposta 200 OK.
