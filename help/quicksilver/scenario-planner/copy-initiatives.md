---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Copiar Iniciativas no Planejador de Cenários
description: É possível criar iniciativas copiando as existentes. Você pode copiar iniciativas em um plano que criar ou em um plano que alguém compartilhar com você.
author: Alina
feature: Workfront Scenario Planner
exl-id: 0aadb074-69c3-4229-a01a-7cabdb87e7cb
source-git-commit: aa2e9a012a60ab10e2d027dedae520b5e06686c7
workflow-type: tm+mt
source-wordcount: '467'
ht-degree: 0%

---

# Copiar iniciativas no [!DNL Scenario Planner]

<!--Audited: 07/2024-->

É possível criar iniciativas copiando as existentes. Você pode copiar iniciativas em um plano que criar ou em um plano que alguém compartilhar com você.

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
</table>-->

## Copiar iniciativas

Considere o seguinte ao copiar iniciativas:

* Copiar uma iniciativa coloca a cópia no mesmo plano da iniciativa original.
* Copiar uma iniciativa copia e adiciona as seguintes informações da iniciativa original à nova iniciativa:

   * [!UICONTROL Duração]
   * [!UICONTROL Funções de trabalho]
   * [!UICONTROL Pessoas] e [!UICONTROL Custos Fixos]
   * [!UICONTROL Benefício Planejado]

* Copiar uma iniciativa pode modificar as seguintes informações do plano, se as informações existirem na iniciativa original:

   * Quantidade necessária de funções de trabalho
   * [!UICONTROL Custos]
   * [!UICONTROL Utilização do Plano]
   * Utilização da função de trabalho
   * [!UICONTROL Valor Líquido]

* Copiar uma iniciativa que foi criada ao importar um projeto ou que foi publicada em um projeto pelo menos uma vez tem as seguintes implicações:

   * Não duplica o projeto associado à iniciativa.
   * Ela não conecta a iniciativa copiada ao projeto.
   * Ela não modifica a seção [!DNL Scenario Planner] no projeto para projetos que foram publicados pelo menos uma vez.

  Para obter informações sobre como publicar iniciativas em projetos, consulte [Atualizar ou criar projetos publicando iniciativas em [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md).

  Para obter informações sobre como criar iniciativas importando projetos, consulte [Importar projetos para planos na [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md).

## Copiar iniciativas

{{step1-to-scenario-planner}}

Uma lista de planos é exibida.

1. Clique no nome de um plano para abri-lo e localize as iniciativas que deseja copiar.
1. Selecione a caixa à esquerda da iniciativa ou iniciativas que deseja copiar e clique em **[!UICONTROL Copiar]** no menu exibido na parte inferior do plano.

   ![Copiar iniciativa](assets/bottom-manage-initiative-menu-350x45.png)

   [!DNL Workfront] copia as iniciativas imediatamente e as coloca abaixo da última iniciativa selecionada.

   O nome da iniciativa copiada é *[!UICONTROL Cópia de]`<Name of original initiative>`*.

   >[!NOTE]
   >
   >Dependendo de onde você inserir as novas iniciativas, os números de iniciativas existentes podem mudar.

1. Atualize o nome da iniciativa copiada.

   >[!TIP]
   >
   >Recomendamos que você sempre atualize o nome da iniciativa para evitar confusão caso deseje copiá-las novamente.

1. (Opcional) Atualize a prioridade de suas iniciativas recém-criadas.

   Para obter informações sobre como priorizar iniciativas, consulte [Atualizar prioridades de iniciativa no [!DNL Scenario Planner]](../scenario-planner/prioritize-initiatives.md).

1. Clique em **[!UICONTROL Salvar Plano]** para salvar suas alterações.
