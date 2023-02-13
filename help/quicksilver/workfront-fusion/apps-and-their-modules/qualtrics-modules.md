---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: conector
navigation-topic: apps-and-their-modules
title: Módulos Qualtrics
description: Em um [!DNL Adobe Workfront Fusion] você pode automatizar workflows que usam o Qualtrics, bem como conectá-lo a vários aplicativos e serviços de terceiros.
author: Becky
feature: Workfront Fusion
exl-id: 146802cd-b863-4c93-b767-50e05892c4de
source-git-commit: c57a796ccbfb36bce58d49345e7515dd524604c5
workflow-type: tm+mt
source-wordcount: '275'
ht-degree: 0%

---

# Módulos Qualtrics

Em um [!DNL Adobe Workfront Fusion] , é possível automatizar workflows que usam [!DNL Qualtrics], bem como conectá-lo a vários aplicativos e serviços de terceiros.

Se precisar de instruções para criar um cenário, consulte [Crie um cenário em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

Para obter informações sobre módulos, consulte [Módulos em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## Requisitos de acesso

Você deve ter o seguinte acesso para usar a funcionalidade neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plano*</td>
  <td> <p>[!UICONTROL Pro] ou superior</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licença*</td>
   <td> <p>[!UICONTROL Plano], [!UICONTROL Trabalho]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licença**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] para automação e integração de trabalho] </p> </td> 
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

Para usar [!DNL Qualtrics] módulos, você deve ter um [!UICONTROL Qualtrics] conta.

## Conexão [!DNL Qualtrics] para [!DNL Workfront Fusion]

Você pode criar uma conexão com o [!DNL Qualtrics] conta diretamente de dentro de uma [!UICONTROL Qualtrics] módulo.

1. Em qualquer [!UICONTROL Qualtrics] módulo, clique em **[!UICONTROL Adicionar]** ao lado do [!UICONTROL Conexão] campo.
1. Insira as seguintes informações:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Nome da conexão]</p> </td> 
      <td> <p>Digite um nome para a nova conexão.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL ID do data center] </td> 
      <td>Usar o formato <code>&lt;Data Center ID>.qualtrics.com</code>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Chave da API]</td> 
      <td>Para localizar a chave de API, consulte <a href="https://api.qualtrics.com/instructions/docs/Instructions/api-key-authentication.md">Autenticação de token de API</a> no [!DNL Qualtrics] documentação.</td> 
     </tr> 
    </tbody> 
   </table>

1. Clique em **[!UICONTROL Continuar]** para criar a conexão e retornar ao módulo .

## [!DNL Qualtrics] módulos e seus campos

Os seguintes módulos estão disponíveis para a variável [!DNL Qualtrics] conector:

* [!UICONTROL Assista a Nova Resposta da Pesquisa]
* [!UICONTROL Criar um Contato de Diretório]
* [!UICONTROL Excluir um Contato de Diretório]
* [!UICONTROL Obter um Contato de Diretório]
* [!UICONTROL Atualizar um Contato de Diretório]
* [!UICONTROL Criar uma Nova Distribuição de Pesquisa por SMS]
* [!UICONTROL Distribuir uma Pesquisa por Email]
* [!UICONTROL Efetuar uma chamada de API]
* [!UICONTROL Listar Contatos do Diretório]
