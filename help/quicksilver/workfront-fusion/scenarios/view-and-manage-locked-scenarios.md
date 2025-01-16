---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Gerenciar cenários bloqueados em  [!DNL Adobe Workfront Fusion]
description: A documentação do Adobe Workfront Fusion foi movida para um novo local. Este artigo foi descontinuado, mas contém um link para o novo artigo que aborda essa funcionalidade.
author: Becky
feature: Workfront Fusion
exl-id: 5fccf336-d904-43fe-ad4a-c3ce76dbcad0
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '409'
ht-degree: 0%

---

# Gerenciar cenários bloqueados em [!DNL Adobe Workfront Fusion]

>[!IMPORTANT]
>
>A documentação do Adobe Workfront Fusion foi movida para um novo local.
>
>As informações neste artigo agora podem ser encontradas no artigo:
>
>* [Gerenciar cenários bloqueados](https://experienceleague.adobe.com/docs/workfront-fusion/using/manage-scenarios/view-manage-locked-scenario.html)
>
>Atualize todos os marcadores.
>
>Este artigo não está mais sendo atualizado e será removido em breve.

Em alguns casos, um cenário pode estar temporariamente bloqueado em [!DNL Workfront Fusion]. As execuções bloqueadas serão automaticamente desbloqueadas dentro de 2 a 4 horas. Também é possível desbloquear cenários manualmente.

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
  <td> <p>[!UICONTROL [!DNL Workfront Fusion] para Automação e Integração do Trabalho] </p><p>[!UICONTROL [!DNL Workfront Fusion] para Automação de Trabalho] </p>  </td>    </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">Produto</td> 
   <td>Sua organização deve comprar o [!DNL Adobe Workfront Fusion] e o [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo.</td> 
  </tr> 
 </tbody> 
</table>

Para saber que plano, tipo de licença ou acesso você tem, contate o administrador do [!DNL Workfront].

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
1. Selecione **[!UICONTROL Desbloquear execução]**.
1. Clique em **[!UICONTROL Desbloquear]**.
