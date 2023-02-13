---
content-type: overview
product-area: workfront-integrations
navigation-topic: workfront-for-salesforce
title: Visão geral do Adobe Workfront for Salesforce
description: Você pode instalar [!DNL Adobe Workfront] para permitir que os usuários do Salesforce enviem [!DNL Workfront] solicita e cria projetos automaticamente sem sair do Salesforce.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 65d4cdae-1d34-4a8a-a1c0-706cd41fc75e
source-git-commit: 5b889633a96d634a359181bfd53ec106b0f3705c
workflow-type: tm+mt
source-wordcount: '436'
ht-degree: 0%

---

# [!DNL Adobe Workfront for Salesforce] visão geral

A [!UICONTROL Pro] [!DNL Workfront] O plano é necessário para usar esse recurso. Para obter mais informações sobre os vários planos disponíveis, consulte [[!DNL Workfront] Planos.](https://www.workfront.com/plans)

Você pode instalar [!DNL Adobe Workfront for Salesforce] para permitir que [!DNL Salesforce] usuários a enviar [!DNL Workfront] solicita e cria projetos automaticamente sem sair [!DNL Salesforce].

Como um [!DNL Workfront] administrador, você pode baixar e configurar [!DNL Workfront for Salesforce]. Em seguida, você pode compartilhá-lo para todos os outros [!DNL Salesforce] usuários.

Para obter mais informações sobre a instalação [!DNL Workfront for Salesforce], consulte [Instalar [!DNL Adobe Workfront for Salesforce]](../../workfront-integrations-and-apps/using-workfront-with-salesforce/install-workfront-for-salesforce.md).\
Para obter mais informações sobre como configurar o [!DNL Workfront] seção em [!DNL Salesforce] para todos os usuários, consulte [Configure o [!DNL Adobe Workfront] seção para [!DNL Salesforce] usuários](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md).

## Requisitos de acesso

Você deve ter o seguinte acesso para usar a funcionalidade descrita neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plano*</td> 
   <td> <p>[!UICONTROL Pro] ou superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licença*</td> 
   <td> <p>[!UICONTROL Plan]</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com seu [!DNL Workfront] administrador.

## [!DNL Workfront for Salesforce]

Você pode fazer o seguinte ao usar [!DNL Workfront for Salesforce]:

* Criar manualmente um novo [!DNL Workfront] solicitações de [!DNL Salesforce] em uma Oportunidade ou Conta.

   Para obter mais informações sobre como criar [!DNL Workfront] solicitações de [!DNL Salesforce], consulte [Enviar [!DNL Adobe Workfront] solicitações de [!DNL Salesforce] objetos](../../workfront-integrations-and-apps/using-workfront-with-salesforce/submit-workfront-requests-from-salesforce-objects.md).

* Acione automaticamente a criação de projetos no [!DNL Workfront] quando determinados critérios forem atendidos em [!DNL Salesforce]. Seu [!DNL Salesforce] o administrador do sistema deve configurar acionadores para criar projetos do [!DNL Salesforce].

   Para obter mais informações sobre como criar [!DNL Workfront] projetos de [!DNL Salesforce], consulte [Criar [!DNL Adobe Workfront] projetos de [!DNL Salesforce] objetos](../../workfront-integrations-and-apps/using-workfront-with-salesforce/create-wf-projects-from-salesforce-objects.md).

Considere o seguinte ao trabalhar com [!DNL Workfront] para [!DNL Salesforce]:

* Apoiamos ambos [!DNL Salesforce Classic] e [!DNL Lightning Experience] quadros.
* Itens podem ser criados somente a partir de [!DNL Salesforce] em [!DNL Workfront].
* Você pode exibir algumas informações sobre o [!DNL Workfront] itens em [!DNL Salesforce].

   Essas informações não podem ser personalizadas.

   Para uma lista de [!DNL Workfront] campos que podem ser visualizados [!DNL Salesforce], consulte  [Enviar [!DNL Adobe Workfront] solicitações de [!DNL Salesforce] objetos](../../workfront-integrations-and-apps/using-workfront-with-salesforce/submit-workfront-requests-from-salesforce-objects.md)  e [Criar [!DNL Adobe Workfront] projetos de [!DNL Salesforce] objetos](../../workfront-integrations-and-apps/using-workfront-with-salesforce/create-wf-projects-from-salesforce-objects.md).

* Você pode acessar diretamente os itens vinculados ao [!DNL Salesforce] clicando no botão **[!UICONTROL Ir para o Salesforce]** link do Workfront.

   Não é possível exibir nenhuma informação sobre o [!DNL Salesforce] itens em [!DNL Workfront], mas você tem um link para a variável [!UICONTROL Salesforce] item de [!DNL Workfront] para revisá-lo em [!DNL Salesforce].

   [!UICONTROL O **Ir para o Salesforce**] é exibido nas seguintes áreas:

   * O [!UICONTROL Detalhes] seção de um projeto ou de um problema
   * O cabeçalho de um projeto ou de um problema.

      O administrador do sistema ou do grupo deve adicionar a variável [!UICONTROL Integrações] para seu Modelo de layout para exibir o [!UICONTROL Ir para o Salesforce] link no cabeçalho do projeto ou do problema.
   * O [!DNL Summary] painel de um problema ao selecionar o problema em uma lista, depois de clicar em [!UICONTROL Abrir resumo] ![](assets/summary-panel-icon.png) na barra de ferramentas da lista.

      >[!NOTE]
      >
      >O [!UICONTROL Ir para o Salesforce] link é visível para todos [!DNL Workfront] usuários que podem visualizar o projeto ou o problema. Você deve ter um [!DNL Salesforce] para poder acessar a [!DNL Salesforce] Oportunidade ou Conta em que o problema foi registrado.

* Atualizar campos em um item em um aplicativo não atualiza nenhuma informação sobre itens vinculados no outro aplicativo.
