---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Excluir iniciativas no Planejador de cenários
description: É possível excluir iniciativas em um plano que você criou ou em um plano que alguém compartilhou com você. Não é possível recuperar iniciativas excluídas.
author: Alina
feature: Workfront Scenario Planner
exl-id: 799ca02e-c513-4409-b327-1ce7d8eb19ae
source-git-commit: 6c5be4dccff46abbed104f1f1b3c958aaf74d629
workflow-type: tm+mt
source-wordcount: '529'
ht-degree: 0%

---

# Excluir iniciativas no [!DNL Scenario Planner]

É possível excluir iniciativas em um plano que você criou ou em um plano que alguém compartilhou com você. Não é possível recuperar iniciativas excluídas.

## Requisitos de acesso

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront]<b> plano*</b> </p> </td> 
   <td>[!UICONTROL Business] ou superior</td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront]<b> licença*</b> </p> </td> 
   <td> <p>[!UICONTROL Review] ou superior</p> </td> 
  </tr> 
  <tr> 
   <td><b>Produto</b> </td> 
   <td> <p>Você deve comprar uma licença adicional para o [!DNL Adobe Workfront Scenario Planner] acessar a funcionalidade descrita neste artigo. </p> <p>Para obter informações sobre como obter o [!DNL Workfront Scenario Planner], consulte <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">Acesso necessário para usar o [!UICONTROL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><strong>Configurações de nível de acesso*</strong> </td> 
   <td> <p>[!UICONTROL Editar] acesso ou superior à [!DNL Scenario Planner]</p> <p>Observação: se você ainda não tiver acesso, pergunte ao administrador do [!DNL Workfront] se ele definiu restrições adicionais no seu nível de acesso. Para obter informações sobre como um administrador do [!DNL Workfront] pode alterar seu nível de acesso, consulte <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><strong>Permissões de objeto</strong> </p> </td> 
   <td> <p>[!UICONTROL Gerenciar] permissões para um plano</p> <p>Para obter informações sobre como solicitar acesso adicional a um plano, consulte <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">Solicitar acesso a um plano no [!DNL Scenario Planner]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

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

1. Clique no ícone ![](assets/main-menu-icon.png) do **[!UICONTROL Menu principal]** e em [!UICONTROL Cenários].

   Uma lista de planos é exibida.

1. Clique no nome de um plano para abri-lo e, em seguida, localize a iniciativa que deseja excluir.
1. Siga um destes procedimentos:

   * Clique no **[!UICONTROL Mais menu]** ![](assets/more-menu.png) à direita do nome da iniciativa e clique em **[!UICONTROL Excluir]** > **[!UICONTROL Sim, exclua-o]**.

   * Selecione a caixa à esquerda da iniciativa e clique em **[!UICONTROL Excluir]** no menu flutuante exibido na parte inferior do plano e, em seguida, clique em **[!UICONTROL Sim, exclua-o]**.

   A iniciativa e suas informações de função de trabalho e custo são excluídas do plano.

1. Clique em **[!UICONTROL Salvar Plano]** para salvar suas alterações.

### Excluir iniciativas em massa {#delete-initiatives-in-bulk}

1. Clique no ícone ![](assets/main-menu-icon.png) do **[!UICONTROL Menu principal]** e em [!UICONTROL Cenários].

   Uma lista de planos é exibida.

1. Clique no nome de um plano para abri-lo e, em seguida, localize a iniciativa que deseja excluir.
1. Marque as caixas à esquerda das iniciativas que deseja excluir e clique em **[!UICONTROL Excluir]** no menu exibido na parte inferior do plano e em **[!UICONTROL Sim, exclua-as]**.

   ![](assets/bottom-manage-initiative-menu-350x45.png)

   As iniciativas e suas funções de trabalho e informações de custo são excluídas do plano.

1. Clique em **[!UICONTROL Salvar Plano]** para salvar suas alterações.
