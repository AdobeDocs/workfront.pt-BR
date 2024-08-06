---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Escolha onde um módulo de acionador é iniciado no Adobe Workfront Fusion
description: Alguns módulos de acionamento permitem selecionar o primeiro pacote a partir do qual deseja que a recuperação de pacotes seja iniciada.
author: Becky
feature: Workfront Fusion
exl-id: 5ab7cac4-8d50-4be0-b26b-b832544f18f7
source-git-commit: 489ed23fe0d7945753b59810ff9da084bd3e92e4
workflow-type: tm+mt
source-wordcount: '386'
ht-degree: 1%

---

# Escolha onde um módulo de acionador inicia em [!DNL Adobe Workfront Fusion]

Alguns módulos de acionamento permitem selecionar o primeiro pacote a partir do qual deseja que a recuperação de pacotes seja iniciada.

Você também pode especificar se deseja recuperar todos os pacotes ou apenas os pacotes de após uma data específica.

Para obter mais informações sobre módulos de acionador, consulte a seção [Módulos de acionador](../../workfront-fusion/modules/module-types.md#triggers) no artigo [Tipos de módulos](../../workfront-fusion/modules/module-types.md).

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

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

+++

## Escolher onde um módulo de acionador é iniciado

1. Salve um módulo de acionamento.

   Ou

   Altere as configurações do módulo do acionador conforme descrito em [Definir configurações de um módulo no [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/modules/configure-a-modules-settings.md).

   Ou

   Clique com o botão direito do mouse no ícone do módulo do acionador no [!UICONTROL Editor de cenários], conforme descrito em [Criar um cenário no [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

1. Na caixa **[!UICONTROL Escolher onde começar]**, selecione uma opção.

   ![](assets/choose-where-to-start-350x346.jpg)

   As opções exibidas dependem das possibilidades de um determinado serviço. Elas podem incluir o seguinte:

   <table style="table-layout:auto">
        <tr>
            <td>[!UICONTROL De agora em diante] (padrão)</td>
            <td>Recupera todos os pacotes adicionados ou atualizados (dependendo das configurações) a partir de agora</td>
        </tr>
        <tr>
            <td>[!UICONTROL De após uma data específica]</td>
            <td>Recupera todos os pacotes adicionados ou atualizados (dependendo das configurações) após uma data/hora especificada</td>
        </tr>
        <tr>
            <td>[!UICONTROL Com ID maior ou igual a um valor específico]</td>
            <td>Recupera todos os pacotes com uma ID maior ou igual a uma ID especificada</td> 
        </tr>
        <tr>
            <td>[!UICONTROL Todos os pacotes]</td>
            <td>Recupera todos os pacotes disponíveis</td>
        </tr>
        <tr>
            <td>[!UICONTROL Selecionar o primeiro pacote]</td>
            <td>Permite selecionar o primeiro pacote a partir do qual a recuperação de pacotes deve começar</td>
        </tr>
   </table>
