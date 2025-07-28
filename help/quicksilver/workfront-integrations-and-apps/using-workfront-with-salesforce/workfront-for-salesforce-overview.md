---
content-type: overview
product-area: workfront-integrations
navigation-topic: workfront-for-salesforce
title: Visão geral do Adobe Workfront para Salesforce
description: Você pode instalar o [!DNL Adobe Workfront] for Salesforce para permitir que seus usuários do Salesforce enviem [!DNL Workfront] solicitações e criem projetos automaticamente sem sair do Salesforce.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 65d4cdae-1d34-4a8a-a1c0-706cd41fc75e
source-git-commit: f9af669b023309abc132421f35a2ece974e796b0
workflow-type: tm+mt
source-wordcount: '538'
ht-degree: 0%

---

# Visão geral das [!DNL Adobe Workfront for Salesforce]

<!-- Audited: 5/2025 -->

>[!IMPORTANT]
>
>Para fornecer integrações mais estáveis e escaláveis, estamos mudando para uma abordagem de integração moderna e flexível usando a Automação e Integração do Workfront (Fusion). Como parte desse processo de transição, a integração do Workfront para Salesforce não estará disponível após **28 de fevereiro de 2026**.
>
>Recomendamos usar a Automação e integração do Workfront para as necessidades de integração de sua organização com o Salesforce.
>
>Para obter uma visão geral da Automação e Integração do Workfront, consulte [Visão geral do Adobe Workfront Fusion](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview).
>
>Para obter informações sobre os recursos específicos dos módulos de Automação e Integração do Workfront para Salesforce, consulte [módulos do Salesforce](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/salesforce-modules).

Você pode instalar o [!DNL Adobe Workfront for Salesforce] para permitir que seus usuários do [!DNL Salesforce] enviem [!DNL Workfront] solicitações e criem projetos automaticamente sem sair do [!DNL Salesforce].

Como administrador [!DNL Workfront], você pode baixar e configurar [!DNL Workfront for Salesforce]. Em seguida, você pode compartilhá-lo com todos os outros usuários do [!DNL Salesforce].

Para obter mais informações sobre como instalar o [!DNL Workfront for Salesforce], consulte [Instalar [!DNL Adobe Workfront for Salesforce]](../../workfront-integrations-and-apps/using-workfront-with-salesforce/install-workfront-for-salesforce.md).

Para obter mais informações sobre como configurar a seção [!DNL Workfront] em [!DNL Salesforce] para todos os usuários, consulte [Configurar a [!DNL Adobe Workfront] seção para [!DNL Salesforce] usuários](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md).

>[!NOTE]
>
>É necessário um Plano [!UICONTROL Pro] [!DNL Workfront] para usar este recurso. Para obter mais informações sobre os vários planos disponíveis, consulte [[!DNL Workfront] Planos.](https://business.adobe.com/products/workfront/pricing.html)

## Requisitos de acesso

Você deve ter o seguinte acesso para usar a funcionalidade descrita neste artigo:

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plano</td> 
   <td> <p>[!UICONTROL Pro] ou superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licença</td> 
   <td> <p>Novo: Padrão<p>
   <p>Ou</p>
   <p>Atual: Plano</p>


</td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## [!DNL Workfront for Salesforce]

Você pode fazer o seguinte ao usar o [!DNL Workfront for Salesforce]:

* Crie manualmente novas solicitações [!DNL Workfront] de [!DNL Salesforce] em uma Oportunidade ou em uma Conta.

  Para obter mais informações, consulte [Enviar [!DNL Adobe Workfront] solicitações de [!DNL Salesforce] objetos](../../workfront-integrations-and-apps/using-workfront-with-salesforce/submit-workfront-requests-from-salesforce-objects.md).

* Acione automaticamente a criação de projetos em [!DNL Workfront] quando determinados critérios forem atendidos em [!DNL Salesforce]. O administrador do sistema [!DNL Salesforce] deve configurar acionadores para criar projetos a partir de [!DNL Salesforce].

  Para obter mais informações sobre como criar projetos do [!DNL Workfront] a partir do [!DNL Salesforce], consulte [Criar [!DNL Adobe Workfront] projetos a partir do [!DNL Salesforce] objetos](../../workfront-integrations-and-apps/using-workfront-with-salesforce/create-wf-projects-from-salesforce-objects.md).

Considere o seguinte ao trabalhar com [!DNL Workfront] para [!DNL Salesforce]:

* Oferecemos suporte às estruturas [!DNL Salesforce Classic] e [!DNL Lightning Experience].
* Os itens só podem ser criados de [!DNL Salesforce] a [!DNL Workfront].
* Você pode exibir algumas informações sobre os [!DNL Workfront] itens em [!DNL Salesforce]. Essas informações não podem ser personalizadas.

  Para obter uma lista de [!DNL Workfront] campos que você pode visualizar a partir de [!DNL Salesforce], consulte [Enviar [!DNL Adobe Workfront] solicitações de [!DNL Salesforce] objetos](../../workfront-integrations-and-apps/using-workfront-with-salesforce/submit-workfront-requests-from-salesforce-objects.md) e [Criar [!DNL Adobe Workfront] projetos de [!DNL Salesforce] objetos](../../workfront-integrations-and-apps/using-workfront-with-salesforce/create-wf-projects-from-salesforce-objects.md).

* Você pode acessar diretamente os itens vinculados ao [!DNL Salesforce] clicando no link [!UICONTROL Ir para o Salesforce] do Workfront.

  Você não pode exibir nenhuma informação sobre os [!DNL Salesforce] itens em [!DNL Workfront], mas há um link no Workfront que direciona você ao item no Salesforce para que você possa analisá-lo lá.

  [!UICONTROL O link Ir para o Salesforce] é exibido nas seguintes áreas:

   * A seção [!UICONTROL Detalhes] de um projeto ou problema.
   * O cabeçalho de um projeto ou um problema.

     O administrador do sistema ou do grupo deve adicionar o campo [!UICONTROL Integrações] ao Modelo de Layout para exibir o link [!UICONTROL Ir para o Salesforce] no cabeçalho do projeto ou do problema.
   * O painel [!DNL Summary] de um problema ao selecionar o problema em uma lista, depois de clicar em [!UICONTROL Abrir resumo] ![ícone do painel Resumo](assets/summary-panel-icon.png) na barra de ferramentas da lista.

     >[!NOTE]
     >
     >O link [!UICONTROL Ir para o Salesforce] está visível para todos os usuários [!DNL Workfront] que podem exibir o projeto ou o problema. Você deve ter uma conta [!DNL Salesforce] para poder acessar a Oportunidade [!DNL Salesforce] ou a Conta onde o problema foi registrado.

* A atualização de campos em um item em um aplicativo não atualiza nenhuma informação sobre itens vinculados em outro aplicativo.
