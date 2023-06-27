---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Escolha onde um módulo de acionador é iniciado no Adobe Workfront Fusion
description: Alguns módulos de acionamento permitem selecionar o primeiro pacote a partir do qual deseja que a recuperação de pacotes seja iniciada.
author: Becky
feature: Workfront Fusion
exl-id: 5ab7cac4-8d50-4be0-b26b-b832544f18f7
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '375'
ht-degree: 1%

---

# Escolha onde um módulo de acionador começa em [!DNL Adobe Workfront Fusion]

Alguns módulos de acionamento permitem selecionar o primeiro pacote a partir do qual deseja que a recuperação de pacotes seja iniciada.

Você também pode especificar se deseja recuperar todos os pacotes ou apenas os pacotes de após uma data específica.

Para obter mais informações sobre módulos de acionador, consulte a seção [Módulos de acionamento](../../workfront-fusion/modules/module-types.md#triggers) no artigo [Tipos de módulos](../../workfront-fusion/modules/module-types.md).

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

## Escolher onde um módulo de acionador é iniciado

1. Salve um módulo de acionamento.

   Ou

   Altere as configurações do módulo acionador conforme descrito em [Definir as configurações de um módulo no [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/modules/configure-a-modules-settings.md).

   Ou

   Clique com o botão direito do mouse no ícone do módulo Acionador na [!UICONTROL Editor de cenários], conforme descrito em [Criar um cenário no [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

1. Selecione uma opção no **[!UICONTROL Escolher onde começar]** que aparece.

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
