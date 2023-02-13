---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Escolha onde um módulo de acionador inicia no Adobe Workfront Fusion
description: Alguns módulos de acionador permitem selecionar o primeiro pacote do qual deseja iniciar a recuperação de pacotes.
author: Becky
feature: Workfront Fusion
exl-id: 5ab7cac4-8d50-4be0-b26b-b832544f18f7
source-git-commit: e58ff769015b8c4e34b34eea653f55a296eea371
workflow-type: tm+mt
source-wordcount: '327'
ht-degree: 0%

---

# Escolha onde um módulo de acionador começa em [!DNL Adobe Workfront Fusion]

Alguns módulos de acionador permitem selecionar o primeiro pacote do qual deseja iniciar a recuperação de pacotes.

Você também pode especificar se deseja recuperar todos os pacotes ou apenas os pacotes após uma data específica.

Para obter mais informações sobre módulos de acionador, consulte a seção [Módulos de acionador](../../workfront-fusion/modules/module-types.md#triggers) no artigo [Tipos de módulos](../../workfront-fusion/modules/module-types.md).

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

## Escolha onde um módulo de acionador é iniciado

1. Salve um módulo de acionador.

   Ou

   Altere as configurações do módulo de acionador, conforme descrito em [Defina as configurações de um módulo em [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/modules/configure-a-modules-settings.md).

   Ou

   Clique com o botão direito do mouse no ícone do módulo de acionador na [!UICONTROL Editor de cenário], conforme descrito em [Crie um cenário em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

1. Selecione uma opção no **[!UICONTROL Escolha onde começar]** que é exibida.

   ![](assets/choose-where-to-start-350x346.jpg)

   As opções exibidas dependem das possibilidades de um determinado serviço. Podem incluir:

   <table style="table-layout:auto">
        <tr>
            <td>[!UICONTROL A partir de agora] (padrão)</td>
            <td>Recupera todos os pacotes adicionados ou atualizados (dependendo das configurações) a partir de agora</td>
        </tr>
        <tr>
            <td>[!UICONTROL De após uma data específica]</td>
            <td>Recupera todos os pacotes adicionados ou atualizados (dependendo das configurações) após uma data/hora especificada</td>
        </tr>
        <tr>
            <td>[!UICONTROL com ID maior ou igual a um valor específico]</td>
            <td>Recupera todos os pacotes com uma ID maior ou igual a uma ID especificada</td> 
        </tr>
        <tr>
            <td>[!UICONTROL Todos os pacotes]</td>
            <td>Recupera todos os pacotes disponíveis</td>
        </tr>
        <tr>
            <td>[!UICONTROL Selecionar o primeiro pacote]</td>
            <td>Permite selecionar o primeiro pacote do qual a recuperação de pacotes deve ser iniciada</td>
        </tr>
   </table>
