---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Programar um cenário no Adobe Workfront Fusion
description: A documentação do Adobe Workfront Fusion foi movida para um novo local. Este artigo foi descontinuado, mas contém um link para o novo artigo que aborda essa funcionalidade.
author: Becky
feature: Workfront Fusion
exl-id: bce89abe-ec37-4705-a88f-de62c8b27f49
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '632'
ht-degree: 0%

---

# Agendar um cenário em [!DNL Adobe Workfront Fusion]

>[!IMPORTANT]
>
>A documentação do Adobe Workfront Fusion foi movida para um novo local.
>
>As informações neste artigo agora podem ser encontradas no artigo:
>
>* [Agendar um cenário](https://experienceleague.adobe.com/docs/workfront-fusion/using/create-scenarios/configure-scenario-settings/schedule-a-scenario.html)
>
>Atualize todos os marcadores.
>
>Este artigo não está mais sendo atualizado e será removido em breve.

Por padrão, um cenário é executado a cada 15 minutos. Você pode alterar isso definindo quando e com que frequência um cenário ativado é executado. Os cenários de fusão podem ser agendados para execução com uma frequência de até 5 minutos.

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
   <p>Requisito de licença herdada: [!UICONTROL [!DNL Workfront Fusion] para Automação e Integração do Trabalho], [!UICONTROL [!DNL Workfront Fusion] para Automação do Trabalho]</p>
   </td>    </tr> 
  <tr> 
   <td role="rowheader">Produto</td> 
   <td>
   <p>Requisito atual do produto: se você tiver o Plano [!DNL Adobe Workfront] da [!UICONTROL Select] ou da [!UICONTROL Prime], sua organização deve comprar o [!DNL Adobe Workfront Fusion] e o [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo. [!DNL Workfront Fusion] está incluído no plano [!DNL Workfront] da [!UICONTROL Ultimate].</p>
   <p>Ou</p>
   <p>Requisito de produto herdado: sua organização deve comprar o [!DNL Adobe Workfront Fusion] e o [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Para saber que plano, tipo de licença ou acesso você tem, contate o administrador do [!DNL Workfront].

Para obter informações sobre [!DNL Adobe Workfront Fusion] licenças, consulte [[!DNL Adobe Workfront Fusion] licenças](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Agendar um cenário

1. No canto superior direito da página Detalhes do cenário, clique em **[!UICONTROL Opções]** > **[!UICONTROL Agendamento]**

   Ou

   Clique no ícone (relógio) **[!UICONTROL Agendamento]** no módulo de gatilho do cenário.

1. Insira informações nos seguintes campos:

   <table style="table-layout:auto">   
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Executar cenário]</td> 
      <td> <p>Selecione a frequência na qual deseja executar o cenário e selecione o intervalo.</p> 
       <ul> 
        <li> <p><strong>[!UICONTROL Em intervalos regulares]</strong> </p> <p>Insira o número de minutos entre execuções. O valor padrão é 15 minutos.</p> </li> 
        <li> <p><strong>[!UICONTROL Once]</strong> </p> <p>Insira a data e a hora em que deseja que o cenário seja executado. Use o formato <code>MM/DD/YYYY h:mm A</code>. Exemplo: <code>06/25/2019 11:00 PM</code>.</p> </li> 
        <li> <p><strong>[!UICONTROL Todo dia]</strong> </p> <p>Informe a hora em que deseja que o cenário seja executado. Use o formato <code>h:mm A</code>. Exemplo: <code>11:00 PM</code>.</p> </li> 
        <li> <p><strong></strong>{UICONTROL Dias da semana </p> <p>Dias: Selecione os dias da semana em que deseja que o cenário seja executado. Você pode selecionar um ou mais dias.</p> <p>Hora: Informe a hora em que deseja que o cenário seja executado nos dias selecionados. Use o formato <code>h:mm A</code>. Exemplo: <code>11:00 PM</code></p> </li> 
        <li> <p><strong>[!UICONTROL Dias do mês]</strong> </p> <p>Dias: Selecione os dias do mês em que deseja que o cenário seja executado. Você pode selecionar um ou mais dias.</p> <p>Hora: Informe a hora em que deseja que o cenário seja executado nos dias selecionados. Use o formato <code>h:mm A</code>. Exemplo: <code>11:00 PM</code></p> </li> 
        <li> <p><strong>[!UICONTROL Datas Especificadas]</strong> </p> <p>Meses: Selecione os meses em que deseja executar o cenário. Você pode selecionar um ou mais meses.</p> <p>Dias: Selecione os dias do mês em que deseja que o cenário seja executado. Você pode selecionar um ou mais dias.</p> <p>Hora: Informe a hora em que deseja que o cenário seja executado nos dias selecionados. Use o formato <code>h:mm A</code>. Exemplo: <code>11:00 PM</code></p> </li> 
       </ul> <p>Nota: Uma data deve existir para que um cenário seja executado nessa data. Por exemplo, um cenário agendado para somente o dia 31 do mês não será executado em fevereiro, abril, junho, setembro ou novembro, pois esses meses não têm um dia 31.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Agendamento avançado]</td> 
      <td>Você pode definir intervalos de tempo específicos durante os quais seu cenário deve ser executado. Você pode especificar intervalos de hora do dia, dias da semana ou meses. Para cada intervalo, clique em <strong>[!UICONTROL Adicionar]</strong> e preencha os campos conforme descrito no campo [!UICONTROL Executar cenário].</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Iniciar]</td> 
      <td>Informe a data e a hora após as quais deseja que o cenário seja executado. Use o formato <code>MM/DD/YYYY h:mm A</code>. Exemplo: <code>06/25/2019 11:00 PM</code>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Fim]</td> 
      <td>Informe a data e a hora antes da qual deseja que o cenário seja executado. Use o formato <code>MM/DD/YYYY h:mm A</code>. Exemplo: <code>06/25/2019 11:00 PM</code>.</td> 
     </tr> 
    </tbody> 
   </table>

1. Clique em **[!UICONTROL OK]** para salvar as configurações do agendamento e retornar ao cenário.
