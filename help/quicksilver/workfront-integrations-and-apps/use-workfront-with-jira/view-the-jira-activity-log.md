---
product-area: workfront-integrations;setup
navigation-topic: workfront-for-jira
title: Exibir o log de atividades do Jira
description: Como administrador do  [!DNL Jira] , você pode exibir as exceções e erros que ocorrem durante a sincronização ou criação dos tíquetes entre o  [!DNL Adobe Workfront] e o [!DNL Jira] em um Log de atividades.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 3e66c8e3-94b7-4153-abbb-32b872b9402b
source-git-commit: b1b55b8046aa771abb2cceda333940ccf827356a
workflow-type: tm+mt
source-wordcount: '347'
ht-degree: 0%

---

# Exibir o [!UICONTROL [!DNL Jira] Log de Atividades]

>[!IMPORTANT]
>
>Para fornecer integrações mais estáveis e escaláveis, estamos mudando para uma abordagem de integração moderna e flexível usando a Automação e Integração do Workfront (Fusion). Como parte desse processo de transição, a integração do Workfront para Jira não estará disponível após **28 de fevereiro de 2026**.
>
>Recomendamos usar a Automação e integração do Workfront para as necessidades de integração de sua organização com o Jira.
>
>Para obter uma visão geral da Automação e Integração do Workfront, consulte [Visão geral do Adobe Workfront Fusion](https://experienceleague.adobe.com/pt-br/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview).
>
>Para obter informações sobre os recursos específicos dos módulos de Automação e Integração do Workfront para Jira, consulte [módulos do Software Jira](https://experienceleague.adobe.com/pt-br/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/jira-software-modules).

<!--

>[!IMPORTANT]
>
>To deliver more stable and scalable integrations, we're shifting to a modern, flexible integration approach using Workfront Automation and Integration (Fusion). As part of this transition process, the Workfront for Jira integration will not be available after **February 28, 2026**. 
>
>We recommend using Workfront Automation and Integration for your organization's integration needs with Jira. 
>
>Eight ready-to-use Workfront Automation and Integration templates for Jira will be available by August to help replicate common workflows and accelerate implementation. Templates are fully customizable to meet specific business needs and can be extended as requirements evolve. 
> 
>For an overview of Workfront Automation and Integration, see [Adobe Workfront Fusion overview](https://experienceleague.adobe.com/pt-br/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview). 
>
>For information about the specific capabilities of the Workfront Automation and Integration modules for Jira, see [Jira Software modules](https://experienceleague.adobe.com/pt-br/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/jira-software-modules). 

-->

Como administrador do [!DNL Jira], você pode exibir as exceções e erros que ocorrem durante a sincronização ou criação dos tíquetes entre [!DNL Adobe Workfront] e [!DNL Jira] em um [!UICONTROL Log de Atividades].

Você pode ver até 500 itens no Registro de atividades e eles são listados começando com os mais recentes.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacote do Adobe Workfront</td> 
   <td><p>Qualquer</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td><p>Standard </p>
       <p>Plano </p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Acesso à Jira</td> 
   <td> <p>Acesso de administrador do sistema</p> <p>Importante: recomendamos que você crie contas de administrador do sistema separadas no Jira e no Workfront para se dedicar a essa integração, em vez de usar as existentes que podem ser anexadas aos usuários.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Você deve ser um administrador do Workfront.</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

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
