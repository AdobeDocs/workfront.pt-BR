---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Excluir iniciativas no Planejador de cenários
description: É possível excluir iniciativas em um plano que você criou ou em um plano que alguém compartilhou com você. Não é possível recuperar iniciativas excluídas.
author: Alina
feature: Workfront Scenario Planner
exl-id: 799ca02e-c513-4409-b327-1ce7d8eb19ae
source-git-commit: aa2e9a012a60ab10e2d027dedae520b5e06686c7
workflow-type: tm+mt
source-wordcount: '485'
ht-degree: 1%

---

# Excluir iniciativas no [!DNL Scenario Planner]

É possível excluir iniciativas em um plano que você criou ou em um plano que alguém compartilhou com você. Não é possível recuperar iniciativas excluídas.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] pacote</p> </td> 
   <td> 
   <p>Workfront Ultimate</p>
<p><b>Nota</b></p>
<p>Fale com o representante da Workfront se tiver um pacote do Workfront diferente.</p>
   </td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] licença</p> </td> 
   <td> <p>[!UICONTROL Light] ou superior</p> 
   <p>[!UICONTROL Review] ou superior</p> </td> 
  </tr> 
    <tr> 
   <td>Configurações de nível de acesso</td> 
   <td> <p>[!UICONTROL Editar] acesso à [!DNL Scenario Planner]</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Permissões de objeto </p> </td> 
   <td> <p>[!UICONTROL Gerenciar] permissões para um plano</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obter mais informações sobre o acesso ao Planejador de cenários, consulte [Acesso necessário para usar o [!DNL Scenario Planner]](../scenario-planner/access-needed-to-use-sp.md).

Para obter informações sobre requisitos de acesso do Workfront, consulte [Requisitos de acesso à documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] plan*</p> </td> 
   <td> <ul></li>
   <li><p>New: Ultimate </p></li>
   <p>The Scenario Planner is not available for the new Workfront Select or Workfront Prime plans. </p>
   <li><p>Current: [!UICONTROL Business] or higher</p></ul>
   </td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] license*</p> </td> 
   <td> <p>New: Light or higher</p> 
   <p>Current: [!UICONTROL Review] or higher</p> </td> 
  </tr> 
  <tr> 
   <td>Product* </td> 
   <td> <ul><li><p>For the new Workfront plans:</p><p> Adobe Workfront</li></p>
   <li><p>For the current Workfront plans: </p>
   <p>Adobe Workfront</p> <p>Adobe Workfront Scenario Planner</p></li></ul>
   
   <p>For more information, see <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">Access needed to use the [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Access level </td> 
   <td> <p>[!UICONTROL Edit] access to the [!DNL Scenario Planner]</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>Object permissions </p> </td> 
   <td> <p>[!UICONTROL Manage] permissions to a plan</p> <p>For information on requesting additional access to a plan, see <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">Request access to a plan in the [!DNL Scenario Planner]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*For information, see [Access requirements to Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). -->

## Excluir iniciativas

Considere o seguinte ao excluir iniciativas:

* Excluir uma iniciativa remove do plano a quantidade necessária de funções de trabalho e as informações de custo associadas à iniciativa.
* Excluir uma iniciativa criada com a importação de um projeto não exclui o projeto associado à iniciativa.
* Excluir uma iniciativa que foi publicada em um projeto pelo menos uma vez resulta no seguinte:

   * A iniciativa foi excluída do cenário, mas a área [!DNL Scenario Planner] permanece na seção [!UICONTROL Detalhes do Projeto].
   * Se a iniciativa excluída for a única iniciativa publicada no cenário, o indicador de que o plano foi publicado também será removido.

     Para obter informações sobre como publicar iniciativas em projetos, consulte [Atualizar ou criar projetos publicando iniciativas em [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md).

     Para obter informações sobre como criar iniciativas importando projetos, consulte [Importar projetos para planos na [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md).

É possível excluir uma iniciativa por vez ou várias iniciativas em massa.

* [Excluir uma iniciativa](#delete-one-initiative)
* [Excluir iniciativas em massa](#delete-initiatives-in-bulk)

### Excluir uma iniciativa {#delete-one-initiative}

{{step1-to-scenario-planner}}

Uma lista de planos é exibida.

1. Clique no nome de um plano para abri-lo e, em seguida, localize a iniciativa que deseja excluir.
1. Siga um destes procedimentos:

   * Clique no **[!UICONTROL Mais menu]** ![Mais menu](assets/more-menu.png) à direita do nome da iniciativa e clique em **[!UICONTROL Excluir]** > **[!UICONTROL Sim, excluir]**.

   * Selecione a caixa à esquerda da iniciativa e clique em **[!UICONTROL Excluir]** no menu flutuante exibido na parte inferior do plano e, em seguida, clique em **[!UICONTROL Sim, exclua-o]**.

   A iniciativa e suas informações de função de trabalho e custo são excluídas do plano.

1. Clique em **[!UICONTROL Salvar Plano]** para salvar suas alterações.

### Excluir iniciativas em massa {#delete-initiatives-in-bulk}

{{step1-to-scenario-planner}}

Uma lista de planos é exibida.

1. Clique no nome de um plano para abri-lo e, em seguida, localize a iniciativa que deseja excluir.
1. Marque as caixas à esquerda das iniciativas que deseja excluir e clique em **[!UICONTROL Excluir]** no menu exibido na parte inferior do plano e em **[!UICONTROL Sim, exclua-as]**.

   ![Gerenciar menu de iniciativa](assets/bottom-manage-initiative-menu-350x45.png)

   As iniciativas e suas funções de trabalho e informações de custo são excluídas do plano.

1. Clique em **[!UICONTROL Salvar Plano]** para salvar suas alterações.
