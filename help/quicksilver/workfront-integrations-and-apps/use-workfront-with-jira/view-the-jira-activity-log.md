---
product-area: workfront-integrations;setup
navigation-topic: workfront-for-jira
title: Exibir o log de atividades do Jira
description: Como administrador do  [!DNL Jira] , você pode exibir as exceções e erros que ocorrem durante a sincronização ou criação dos tíquetes entre o  [!DNL Adobe Workfront] e o [!DNL Jira] em um Log de atividades.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 3e66c8e3-94b7-4153-abbb-32b872b9402b
source-git-commit: f9af669b023309abc132421f35a2ece974e796b0
workflow-type: tm+mt
source-wordcount: '431'
ht-degree: 0%

---

# Exibir o [!UICONTROL [!DNL Jira] Log de Atividades]

>[!IMPORTANT]
>
>Para fornecer integrações mais estáveis e escaláveis, estamos mudando para uma abordagem de integração moderna e flexível usando a Automação e Integração do Workfront (Fusion). Como parte desse processo de transição, a integração do Workfront para Jira não estará disponível após **28 de fevereiro de 2026**.
>
>Recomendamos usar a Automação e integração do Workfront para as necessidades de integração de sua organização com o Jira.
>
>Oito modelos de Automação e Integração do Workfront prontos para uso para Jira estarão disponíveis até agosto para ajudar a replicar fluxos de trabalho comuns e acelerar a implementação. Os modelos são totalmente personalizáveis para atender às necessidades específicas dos negócios e podem ser estendidos à medida que os requisitos evoluem.
> 
>Para obter uma visão geral da Automação e Integração do Workfront, consulte [Visão geral do Adobe Workfront Fusion](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview).
>
>Para obter informações sobre os recursos específicos dos módulos de Automação e Integração do Workfront para Jira, consulte [módulos do Software Jira](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/jira-software-modules).

Como administrador do [!DNL Jira], você pode exibir as exceções e erros que ocorrem durante a sincronização ou criação dos tíquetes entre [!DNL Adobe Workfront] e [!DNL Jira] em um [!UICONTROL Log de Atividades].

Você pode ver até 500 itens no Registro de atividades e eles são listados começando com os mais recentes.

## Requisitos de acesso

Você deve ter o seguinte:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://business.adobe.com/products/workfront/pricing.html" target="_blank">[!DNL Adobe Workfront] plano</a>*</td> 
   <td> <p>[!UICONTROL Pro] ou superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Visão geral das licenças do Adobe [!DNL Workfront]</a>*</td> 
   <td> <p>[!UICONTROL Plano]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Jira] acesso</td> 
   <td> <p>Acesso de administrador do sistema</p> <p>Importante: recomendamos que você crie contas de administrador do sistema separadas no [!DNL Jira] e no [!DNL Workfront] para se dedicar a essa integração, em vez de usar as existentes que podem estar anexadas aos usuários.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Você deve ser um administrador [!DNL Workfront]. Para obter informações sobre administradores do [!DNL Workfront], consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder a um usuário acesso administrativo total</a>.</p> <p>Observação: se você ainda não tiver acesso, pergunte ao administrador do [!DNL Workfront] se ele definiu restrições adicionais no seu nível de acesso. Para obter informações sobre como um administrador do [!DNL Workfront] pode modificar seu nível de acesso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qual plano, tipo de licença ou acesso você tem, contate o administrador do [!DNL Workfront].

## Pré-requisitos

Antes de vincular itens entre [!DNL Workfront] e [!DNL Jira], é necessário

* Instalar [!DNL Workfront for Jira]

  Para obter instruções sobre como instalar o [!DNL Workfront for Jira], consulte [Instalar [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/install-workfront-for-jira.md).

## Acessar o [!UICONTROL [!DNL Jira] Log de Atividades]:

1. Faça logon no Jira como administrador do sistema.
1. Clique em **[!UICONTROL Configurações]** no menu principal [!DNL Jira].
1. Clique em **[!UICONTROL Complementos]** e depois em **[!UICONTROL Gerenciar complementos]**.

1. Expanda o complemento **[!DNL Workfront]**.
1. Clique em **[!UICONTROL Configurar]**.
1. Faça logon em [!DNL Workfront] como administrador do sistema.
1. Selecione a guia **[!UICONTROL Log de atividades]**.

   Visualize informações sobre exceções e erros que ocorreram durante a criação de itens ou a sincronização de campos entre os dois aplicativos.

   O log inclui os seguintes campos:

   * Data da ocorrência
   * O nome do usuário no Jira
   * Número do problema no Jira
   * Uma breve descrição do erro ocorrido.
