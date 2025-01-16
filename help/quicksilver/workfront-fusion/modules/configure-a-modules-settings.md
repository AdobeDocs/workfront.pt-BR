---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Definir as configurações de um módulo no  [!DNL Adobe Workfront Fusion]
description: A documentação do Adobe Workfront Fusion foi movida para um novo local. Este artigo foi descontinuado, mas contém um link para o novo artigo que aborda essa funcionalidade.
author: Becky
feature: Workfront Fusion
exl-id: 7e66728d-8c6f-4597-98c4-bc6d36f96911
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '394'
ht-degree: 1%

---

# Definir as configurações de um módulo no [!DNL Adobe Workfront Fusion]

>[!IMPORTANT]
>
>A documentação do Adobe Workfront Fusion foi movida para um novo local.
>
>As informações neste artigo agora podem ser encontradas no artigo:
>
>* [Configurar um módulo](https://experienceleague.adobe.com/docs/workfront-fusion/using/create-scenarios/add-modules/configure-a-modules-settings.html)
>
>Atualize todos os marcadores.
>
>Este artigo não está mais sendo atualizado e será removido em breve.

Você deve definir as configurações para cada módulo criado.

Por exemplo, os módulos [[!DNL Dropbox] modules](../../workfront-fusion/apps-and-their-modules/dropbox-modules.md) exigem que você especifique a pasta de destino para onde deseja carregar arquivos. Para os módulos [[!UICONTROL Email]](../../workfront-fusion/apps-and-their-modules/email-modules.md), é necessário inserir o endereço de email para o qual os emails devem ser enviados.

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
   <p>Requisito de licença atual: nenhum requisito de licença [!DNL Workfront Fusion].</p>
   <p>Ou</p>
   <p>Requisito de licença herdada: [!UICONTROL [!DNL Workfront Fusion] para Automação e Integração do Trabalho] </p>
   </td> 
  </tr> 
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

## Definir as configurações de um módulo

1. Adicione um novo módulo a um cenário.

   Ou

   Clique no ícone do módulo no editor de cenários, conforme descrito em [Criar um cenário em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

1. Se necessário para o módulo, crie uma **[!UICONTROL Conexão]** para sua conta de usuário registrada para esse serviço específico, conforme descrito na [Visão geral das conexões](../../workfront-fusion/connections/about-connecting-wf-fusion-to-app-or-service.md).
1. Em cada campo, digite o texto apropriado.

   Ou

   Clique em **[!UICONTROL Mapear]** se ele aparecer à direita do campo, em seguida, mapeie um item de outro módulo no seu cenário.

   Parâmetros em negrito são necessários.

   Para obter informações sobre os diferentes tipos de dados de item que [!DNL Workfront Fusion] pode reconhecer (como data, número e texto), consulte [Tipos de dados de item em  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/item-data-types.md).

1. (Condicional) Se o módulo tiver opções avançadas que você deseja exibir e usar, selecione **[!UICONTROL Mostrar configurações avançadas]**.
