---
title: Visão geral dos espaços de trabalho
description: Um espaço de trabalho é uma coleção de tipos de registro usados por uma equipe e representa o ciclo de vida do trabalho da equipe. Você pode personalizar totalmente os espaços de trabalho no Adobe Workfront Planning para corresponder aos fluxos de trabalho de suas unidades organizacionais.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: b80d5ccf-4d22-49f2-89b6-bb9678a353c2
source-git-commit: 4692dc6f7ab840bb43f3788126471425e9f8a396
workflow-type: tm+mt
source-wordcount: '390'
ht-degree: 4%

---

# Visão geral dos espaços de trabalho

<!--
<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>
-->

{{planning-important-intro}}

Um espaço de trabalho é uma coleção de tipos de registro usados por uma unidade organizacional e representa o ciclo de vida e os processos de trabalho da unidade. Você pode personalizar totalmente os espaços de trabalho no Adobe Workfront Planning.

<!--update screenshot with preview-->

![Conta de administrador da página de aterrissagem do Workspaces](assets/workspaces-landing-page-admin-account.png)

## Considerações sobre espaços de trabalho

* Você pode criar espaços de trabalho para unidades organizacionais específicas na sua organização, para corresponder à maneira exclusiva como cada unidade funciona.
* O Workfront Planning não vem com nenhum espaço de trabalho pré-configurado. Você deve criá-los de acordo com as necessidades de sua organização.
* Você pode criar espaços de trabalho das seguintes maneiras:

   * Do zero
   * Uso de um template. Os modelos contêm um número pré-configurado de tipos de registro e seus campos.
   * Uso da Designer do Planning habilitada por IA. Este recurso atualmente está no Beta.
   * Uso de um pacote de modelo de vários espaços de trabalho.

  Para obter informações, consulte [Criar espaços de trabalho](/help/quicksilver/planning/architecture/create-workspaces.md).

* Os espaços de trabalho são estruturas nas quais suas unidades organizacionais (uma equipe, grupo, departamento ou divisão) trabalham. Elas não podem ser associadas a campos. Somente os tipos de registro em um espaço de trabalho podem ser associados a campos.

  Para obter informações, consulte [Visão geral dos tipos de registro](/help/quicksilver/planning/architecture/overview-of-record-types.md).
* Dependendo da sua licença do Workfront, os espaços de trabalho são exibidos nas seguintes guias na área do Planning:

   * Para administradores do sistema, os espaços de trabalho são exibidos nas seguintes guias:

      * **Espaços de trabalho em que estou**: exibe os espaços de trabalho que você criou ou os espaços de trabalho que são compartilhados com você.
      * **Outros espaços de trabalho**: exibe todos os outros espaços de trabalho no sistema.

     <!--
      * <span class="preview">**Sample workspaces**: Displays built-in examples of best-practice workspaces. You cannot edit the workspaces, record types, or add records, but you can add, edit, and share views with others.</span> (************TEST THIS WITH SYSTEM ADMINS AND STANDARD USERS**********)
      -->

   * Para todos os outros usuários, os espaços de trabalho que eles criaram e os espaços de trabalho que outros compartilharam com eles são exibidos na área Espaços de trabalho.

  <!--

    ******************* If Standard users can see the Sample workspaces, then replace the last bullet with this: 

   * For all other users:

        * (****************what is the name of this tab????*******) Workspaces they created and workspaces others shared with them display in the Workspaces area. 
        * <span class="preview">**Sample workspaces**: Displays built-in examples of best-practice workspaces. You cannot edit the workspaces, record types, or add records, but you can add, edit, and share views with others.</span>
    
    -->

  <!--      
    >[!NOTE]
    >
    ><span class="preview">We recommend to not edit the sample workspaces, but instead to use them as a reference to create your own. Use the multi-workspace template bundle to create workspaces identical to the ones listed in the Sample workspaces tab. For information, see the section "Create multiple workspaces using a best-practice multi-workspace template bundle" in the article [Create workspaces](/help/quicksilver/planning/architecture/create-workspaces.md). </span> 
    -->

* Os tipos de registro que um espaço de trabalho contém devem refletir o ciclo de vida do trabalho e os conceitos de uma unidade organizacional.

  Por exemplo, se os objetos de trabalho de uma unidade forem campanhas, produtos e regiões, o espaço de trabalho dessa unidade deverá conter os tipos de registro Campanha, Produto e Região.
* Ao criar um espaço de trabalho, somente você tem permissão para acessar e gerenciar seu espaço de trabalho. Você deve compartilhá-lo com outros usuários para que eles colaborem com você no mesmo espaço.

  Para obter informações, consulte [Compartilhar um espaço de trabalho](/help/quicksilver/planning/access/share-workspaces.md).

  Os administradores do sistema podem gerenciar todos os espaços de trabalho, mesmo aqueles que não criaram.

<!--make this live with the GA: * There is no limit for how many workspaces you can create in your environment. However, we recommend not to have too many workspaces, as they could become hard to manage and your workflows might be too fragmented.-->

* Há limites para a quantidade de objetos do espaço de trabalho que você pode criar na instância do Workfront Planning. Para obter informações, consulte [visão geral das limitações de objetos do Adobe Workfront Planning](/help/quicksilver/planning/general/limitations-overview.md).
