---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Gerenciar cenários bloqueados no [!DNL Adobe Workfront Fusion]
description: Gerenciar cenários bloqueados no [!DNL Adobe Workfront Fusion]
author: Becky
feature: Workfront Fusion
exl-id: 014434dc-7548-42d1-bacd-89ddf627b647
source-git-commit: 9050684504f2335f5631f63978a9f65c25fd8d5f
workflow-type: tm+mt
source-wordcount: '333'
ht-degree: 0%

---

# Gerenciar cenários bloqueados no [!DNL Adobe Workfront Fusion]

Em alguns casos, um cenário pode estar temporariamente bloqueado [!DNL Workfront Fusion]. As execuções bloqueadas serão automaticamente desbloqueadas dentro de 2 a 4 horas. Também é possível desbloquear cenários manualmente.

>[!IMPORTANT]
>
>Desbloquear um cenário manualmente pode causar erros nas execuções de um cenário.

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
  <td> <p>[!UICONTROL [!DNL Workfront Fusion] para Automação e integração do trabalho] </p><p>[!UICONTROL [!DNL Workfront Fusion] para automação de trabalho] </p>  </td>    </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">Produto</td> 
   <td>Sua organização deve comprar [!DNL Adobe Workfront Fusion] bem como [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo.</td> 
  </tr> 
 </tbody> 
</table>

Para descobrir que plano, tipo de licença ou acesso você tem, entre em contato com o [!DNL Workfront] administrador.

Para obter informações sobre [!DNL Adobe Workfront Fusion] licenças, consulte [[!DNL Adobe Workfront Fusion] licenças](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Noções básicas sobre cenários bloqueados

Os cenários podem ser bloqueados por vários motivos.

O Workfront Fusion não oferece suporte ao processamento paralelo de cenários agendados. Esses cenários são bloqueados no início da execução do cenário e desbloqueados quando ele é concluído. Se a execução for interrompida, o cenário pode não ser desbloqueado. Isso pode ocorrer quando um usuário força manualmente o cenário ou quando há um problema no sistema.

Além disso, a equipe de engenharia do Workfront Fusion pode bloquear um cenário porque ele está causando desempenho ou outros problemas.

Independentemente da causa de um cenário bloqueado, o cenário será desbloqueado automaticamente de 2 a 4 horas após ser bloqueado.

## Desbloquear um cenário bloqueado

Cenários bloqueados serão desbloqueados de 2 a 4 horas a partir do momento em que foram bloqueados. É possível desbloquear um cenário manualmente antes de seu desbloqueio automático ser agendado.

Desbloquear um cenário manualmente pode causar erros nas execuções de um cenário. Recomendamos desbloquear manualmente os cenários somente quando um cenário está bloqueado devido à execução e interrupção de execuções como parte do design do cenário. Em outras circunstâncias, recomendamos que você aguarde até que o cenário seja desbloqueado automaticamente.

>[!IMPORTANT]
>
>Desbloquear um cenário manualmente pode causar erros nas execuções de um cenário.

1. Vá para a página Detalhes do cenário do cenário bloqueado.
1. Clique em **[!UICONTROL Opções]** no canto superior direito da tela.
1. Selecionar **[!UICONTROL Desbloquear execução]**.
1. Clique em **[!UICONTROL Desbloquear]**.
