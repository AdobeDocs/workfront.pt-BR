---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Excluir iniciativas no Planejador de cenários
description: É possível excluir iniciativas em um plano que você criou ou em um plano que alguém compartilhou com você. Não é possível recuperar iniciativas excluídas.
author: Alina
feature: Workfront Scenario Planner
exl-id: 799ca02e-c513-4409-b327-1ce7d8eb19ae
source-git-commit: a79e4146ce6d076ef0e3707416a9c21d643b96e1
workflow-type: tm+mt
source-wordcount: '512'
ht-degree: 2%

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
   <td> <p>[!DNL Adobe Workfront] plano*</p> </td> 
   <td> <ul></li>
   <li><p>Novo: Ultimate </p></li>
   <p>O Planejador de cenários não está disponível para o novo Workfront Select ou Workfront Plan. </p>
   <li><p>Atual: [!UICONTROL Business] ou superior</p></ul>
   </td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] licença*</p> </td> 
   <td> <p>Novo: Claro ou superior</p> 
   <p>Atual: [!UICONTROL Review] ou posterior</p> </td> 
  </tr> 
  <tr> 
   <td>Produto* </td> 
   <td> <ul><li><p>Para os novos planos do Workfront:</p><p> Adobe Workfront</li></p>
   <li><p>Para os planos atuais do Workfront: </p>
   <p>Adobe Workfront</p> <p>Planejador de cenários do Adobe Workfront</p></li></ul>

<p>Para obter mais informações, consulte <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">Acesso necessário para usar o [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Nível de acesso </td> 
   <td> <p>[!UICONTROL Editar] acesso à [!DNL Scenario Planner]</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>Permissões de objeto </p> </td> 
   <td> <p>[!UICONTROL Gerenciar] permissões para um plano</p> <p>Para obter informações sobre como solicitar acesso adicional a um plano, consulte <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">Solicitar acesso a um plano no [!DNL Scenario Planner]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Para obter informações, consulte [Requisitos de acesso à documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

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

   * Clique no **[!UICONTROL Mais menu]** ![](assets/more-menu.png) à direita do nome da iniciativa e clique em **[!UICONTROL Excluir]** > **[!UICONTROL Sim, exclua-o]**.

   * Selecione a caixa à esquerda da iniciativa e clique em **[!UICONTROL Excluir]** no menu flutuante exibido na parte inferior do plano e, em seguida, clique em **[!UICONTROL Sim, exclua-o]**.

   A iniciativa e suas informações de função de trabalho e custo são excluídas do plano.

1. Clique em **[!UICONTROL Salvar Plano]** para salvar suas alterações.

### Excluir iniciativas em massa {#delete-initiatives-in-bulk}

{{step1-to-scenario-planner}}

Uma lista de planos é exibida.

1. Clique no nome de um plano para abri-lo e, em seguida, localize a iniciativa que deseja excluir.
1. Marque as caixas à esquerda das iniciativas que deseja excluir e clique em **[!UICONTROL Excluir]** no menu exibido na parte inferior do plano e em **[!UICONTROL Sim, exclua-as]**.

   ![](assets/bottom-manage-initiative-menu-350x45.png)

   As iniciativas e suas funções de trabalho e informações de custo são excluídas do plano.

1. Clique em **[!UICONTROL Salvar Plano]** para salvar suas alterações.
