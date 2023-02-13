---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Defina as configurações de um módulo em [!DNL Adobe Workfront Fusion]
description: Você deve definir as configurações para cada módulo que criar.
author: Becky
feature: Workfront Fusion
exl-id: 7e66728d-8c6f-4597-98c4-bc6d36f96911
source-git-commit: e58ff769015b8c4e34b34eea653f55a296eea371
workflow-type: tm+mt
source-wordcount: '286'
ht-degree: 1%

---

# Defina as configurações de um módulo em [!DNL Adobe Workfront Fusion]

Você deve definir as configurações para cada módulo que criar.

Por exemplo, a variável [[!DNL Dropbox] módulos](../../workfront-fusion/apps-and-their-modules/dropbox-modules.md) Os módulos exigem que você especifique a pasta de destino onde deseja fazer upload de arquivos. Para o [[!UICONTROL Email] módulos](../../workfront-fusion/apps-and-their-modules/email-modules.md) , é necessário inserir o endereço de email para o qual os emails devem ser enviados.

>[!NOTE]
>
>Além das configurações do módulo , você também pode ajustar as configurações de um cenário. Você pode renomear o cenário, alterar seu agendamento e especificar configurações adicionais, entre outras ações.

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

## Definir as configurações de um módulo

1. Adicione um novo módulo a um cenário.

   Ou

   Clique no ícone do módulo no editor de cenário, conforme descrito em [Crie um cenário em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

1. Se necessário para o módulo , crie um **[!UICONTROL Conexão]** para sua conta de usuário registrada para esse serviço, conforme descrito em [Sobre a conexão [!DNL Adobe Workfront Fusion] para um aplicativo ou serviço](../../workfront-fusion/connections/about-connecting-wf-fusion-to-app-or-service.md).
1. Em cada campo, digite o texto apropriado.

   Ou

   Clique em **[!UICONTROL Mapa]** se for exibido à direita do campo , mapeie um item de outro módulo em seu cenário.

   Parâmetros em negrito são necessários.

   Para obter informações sobre os diferentes tipos de dados de item [!DNL Workfront Fusion] pode reconhecer (como data, número e texto), consulte [Tipos de dados de item em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/item-data-types.md).

1. (Condicional) Se o módulo tiver opções avançadas que você deseja exibir e usar, selecione **[!UICONTROL Mostrar configurações avançadas]**.
