---
content-type: overview
product-area: workfront-integrations
navigation-topic: workfront-for-salesforce
title: Visão geral do Adobe Workfront for Salesforce
description: Você pode instalar o [!DNL Adobe Workfront] for Salesforce para permitir que seus usuários do Salesforce enviem [!DNL Workfront] solicitações e criem projetos automaticamente sem sair do Salesforce.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 65d4cdae-1d34-4a8a-a1c0-706cd41fc75e
source-git-commit: 5b889633a96d634a359181bfd53ec106b0f3705c
workflow-type: tm+mt
source-wordcount: '434'
ht-degree: 0%

---

# Visão geral de [!DNL Adobe Workfront for Salesforce]

É necessário um Plano [!UICONTROL Pro] [!DNL Workfront] para usar este recurso. Para obter mais informações sobre os vários planos disponíveis, consulte [[!DNL Workfront] Planos.](https://www.workfront.com/plans)

Você pode instalar o [!DNL Adobe Workfront for Salesforce] para permitir que seus usuários do [!DNL Salesforce] enviem [!DNL Workfront] solicitações e criem projetos automaticamente sem sair do [!DNL Salesforce].

Como administrador [!DNL Workfront], você pode baixar e configurar [!DNL Workfront for Salesforce]. Em seguida, é possível compartilhá-lo com todos os outros [!DNL Salesforce] usuários.

Para obter mais informações sobre como instalar o [!DNL Workfront for Salesforce], consulte [Instalar [!DNL Adobe Workfront for Salesforce]](../../workfront-integrations-and-apps/using-workfront-with-salesforce/install-workfront-for-salesforce.md).\
Para obter mais informações sobre como configurar a seção [!DNL Workfront] em [!DNL Salesforce] para todos os usuários, consulte [Configurar a [!DNL Adobe Workfront] seção para [!DNL Salesforce] usuários](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md).

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
   <td> <p>[!UICONTROL Plano]</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qual plano, tipo de licença ou acesso você tem, contate o administrador do [!DNL Workfront].

## [!DNL Workfront for Salesforce]

Você pode fazer o seguinte ao usar o [!DNL Workfront for Salesforce]:

* Crie manualmente novas solicitações [!DNL Workfront] de [!DNL Salesforce] em uma Oportunidade ou em uma Conta.

  Para obter mais informações sobre como criar [!DNL Workfront] solicitações de [!DNL Salesforce], consulte [Enviar [!DNL Adobe Workfront] solicitações de [!DNL Salesforce] objetos](../../workfront-integrations-and-apps/using-workfront-with-salesforce/submit-workfront-requests-from-salesforce-objects.md).

* Acione automaticamente a criação de projetos em [!DNL Workfront] quando determinados critérios forem atendidos em [!DNL Salesforce]. O administrador do sistema [!DNL Salesforce] deve configurar acionadores para criar projetos a partir de [!DNL Salesforce].

  Para obter mais informações sobre como criar projetos do [!DNL Workfront] a partir do [!DNL Salesforce], consulte [Criar [!DNL Adobe Workfront] projetos a partir do [!DNL Salesforce] objetos](../../workfront-integrations-and-apps/using-workfront-with-salesforce/create-wf-projects-from-salesforce-objects.md).

Considere o seguinte ao trabalhar com [!DNL Workfront] para [!DNL Salesforce]:

* Oferecemos suporte às estruturas [!DNL Salesforce Classic] e [!DNL Lightning Experience].
* Os itens só podem ser criados de [!DNL Salesforce] em [!DNL Workfront].
* Você pode exibir algumas informações sobre os [!DNL Workfront] itens em [!DNL Salesforce].

  Essas informações não podem ser personalizadas.

  Para obter uma lista de [!DNL Workfront] campos que você pode visualizar a partir de [!DNL Salesforce], consulte [Enviar [!DNL Adobe Workfront] solicitações de [!DNL Salesforce] objetos](../../workfront-integrations-and-apps/using-workfront-with-salesforce/submit-workfront-requests-from-salesforce-objects.md) e [Criar [!DNL Adobe Workfront] projetos de [!DNL Salesforce] objetos](../../workfront-integrations-and-apps/using-workfront-with-salesforce/create-wf-projects-from-salesforce-objects.md).

* Você pode acessar diretamente os itens vinculados ao [!DNL Salesforce] clicando no link **[!UICONTROL Ir para o Salesforce]** no Workfront.

  Você não pode exibir nenhuma informação sobre os [!DNL Salesforce] itens em [!DNL Workfront], mas você tem um link para o item [!UICONTROL Salesforce] de [!DNL Workfront] para analisá-lo em [!DNL Salesforce].

  [!UICONTROL O link **Ir para o Salesforce**] é exibido nas seguintes áreas:

   * A seção [!UICONTROL Detalhes] de um projeto ou problema do e
   * O cabeçalho de um projeto ou um problema.

     O administrador do sistema ou do grupo deve adicionar o campo [!UICONTROL Integrações] ao Modelo de Layout para exibir o link [!UICONTROL Ir para o Salesforce] no cabeçalho do projeto ou do problema.
   * O painel [!DNL Summary] de um problema ao selecionar o problema em uma lista, depois de clicar em [!UICONTROL Abrir resumo] ![](assets/summary-panel-icon.png) na barra de ferramentas da lista.

     >[!NOTE]
     >
     >O link [!UICONTROL Ir para o Salesforce] está visível para todos os usuários [!DNL Workfront] que podem ver o projeto ou o problema. Você deve ter uma conta [!DNL Salesforce] para poder acessar a Oportunidade [!DNL Salesforce] ou a Conta onde o problema foi registrado.

* A atualização de campos em um item em um aplicativo não atualiza nenhuma informação sobre itens vinculados em outro aplicativo.
