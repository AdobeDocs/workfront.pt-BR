---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Definir as configurações de um módulo no [!DNL Adobe Workfront Fusion]
description: Você deve definir as configurações para cada módulo criado.
author: Becky
feature: Workfront Fusion
exl-id: 7e66728d-8c6f-4597-98c4-bc6d36f96911
source-git-commit: f11af8d9d1e5fa65c2efb4d882d25f9e13784611
workflow-type: tm+mt
source-wordcount: '329'
ht-degree: 1%

---

# Definir as configurações de um módulo no [!DNL Adobe Workfront Fusion]

Você deve definir as configurações para cada módulo criado.

Por exemplo, a variável [[!DNL Dropbox] módulos](../../workfront-fusion/apps-and-their-modules/dropbox-modules.md) Os módulos exigem que você especifique a pasta de destino na qual deseja fazer upload dos arquivos. Para o [[!UICONTROL E-mail] módulos](../../workfront-fusion/apps-and-their-modules/email-modules.md) , é necessário inserir o endereço de email para onde os emails devem ser enviados.

>[!NOTE]
>
>Além das configurações do módulo, você também pode ajustar as configurações de um cenário. É possível renomear o cenário, alterar seu agendamento e especificar configurações adicionais, entre outras ações.

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

## Definir as configurações de um módulo

1. Adicione um novo módulo a um cenário.

   Ou

   Clique no ícone do módulo no editor de cenários, conforme descrito em [Criar um cenário no [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

1. Se necessário para o módulo, crie um **[!UICONTROL Conexão]** para sua conta de usuário registrada para esse serviço específico, conforme descrito em [Visão geral das conexões](../../workfront-fusion/connections/about-connecting-wf-fusion-to-app-or-service.md).
1. Em cada campo, digite o texto apropriado.

   Ou

   Clique em **[!UICONTROL Mapa]** se ele aparecer à direita do campo, mapeie um item de outro módulo no seu cenário.

   Parâmetros em negrito são necessários.

   Para obter informações sobre os diferentes tipos de dados do item [!DNL Workfront Fusion] reconhecer (como data, número e texto), consulte [Tipos de dados de item no [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/item-data-types.md).

1. (Condicional) Se o módulo tiver opções avançadas que você deseja exibir e usar, selecione **[!UICONTROL Mostrar configurações avançadas]**.
