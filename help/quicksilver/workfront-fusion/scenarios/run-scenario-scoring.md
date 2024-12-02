---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Execute o especialista de pontuação de cenários
description: Gerenciar cenários bloqueados em  [!DNL Adobe Workfront Fusion]
author: Becky
feature: Workfront Fusion
hide: true
hidefromtoc: true
exl-id: 144c8dbd-a3e9-4267-b3db-0768dac8f384
source-git-commit: 7bc49dcd8988ef7fd781fb88eba5b03576ca7054
workflow-type: tm+mt
source-wordcount: '295'
ht-degree: 0%

---

# Execute o especialista em pontuação de cenários no Adobe Workfront Fusion

O especialista em pontuação de cenários pode ajudá-lo a garantir que seu cenário seja configurado de uma maneira que siga as práticas recomendadas. Ele verifica o cenário e fornece recomendações para sua estrutura e organização.

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

Execute o especialista de pontuação de cenários

1. Clique na guia **[!UICONTROL Cenário]** no painel esquerdo.
1. Selecione o cenário em que deseja executar o Especialista em Pontuação de Cenários.
1. Clique em qualquer lugar no cenário para entrar no editor de cenários.
1. Clique no ícone Especialista em Pontuação de Cenário ![Especialista em pontuação de cenário](assets/scoring-expert-icon.png) próximo à parte inferior da tela.

   O painel Especialista em Pontuação de Cenário é aberto.
1. Clique em **Avaliar**.

O Especialista em Pontuação de Cenários retorna uma pontuação de 10 e mostra quais verificações foram bem-sucedidas ou falharam. Se uma verificação falhar, o especialista em pontuação de cenários dará recomendações sobre como garantir que o cenário atenda a essas verificações.

![Pontuação do cenário](assets/scenario-score.png)

## Verificações de pontuação de cenário

O especialista em pontuação de cenários usa as seguintes verificações:

* O cenário deve ser nomeado.
* Todos os módulos devem ser rotulados.
* O cenário deve ser executado em um cronograma definido.

  Para obter instruções, consulte [Agendar um cenário](/help/quicksilver/workfront-fusion/scenarios/schedule-a-scenario.md).
* O tamanho do blueprint do cenário deve estar abaixo de 5 MB.

  Para obter mais informações, consulte [Medidas de proteção de desempenho do Fusion](/help/quicksilver/workfront-fusion/get-started/fusion-performance-guardrails.md#scenarios).
* Se um módulo de acionador instantâneo do Workfront for usado, ele deverá ser filtrado.

  Para obter instruções, consulte [Filtros de assinatura de evento no [!DNL Workfront] > [!UICONTROL Módulo Assistir Eventos]](/help/quicksilver/workfront-fusion/apps-and-their-modules/workfront-modules.md#event-subscription-filters-in-the-workfront--watch-events-module).

