---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Excluir iniciativas no Planejador de Cenário
description: É possível excluir iniciativas em um plano criado por você ou em um plano compartilhado por alguém com você. Não é possível recuperar iniciativas excluídas.
author: Alina
feature: Workfront Scenario Planner
exl-id: 799ca02e-c513-4409-b327-1ce7d8eb19ae
source-git-commit: 6c5be4dccff46abbed104f1f1b3c958aaf74d629
workflow-type: tm+mt
source-wordcount: '529'
ht-degree: 1%

---

# Exclua iniciativas no [!DNL Scenario Planner]

É possível excluir iniciativas em um plano criado por você ou em um plano compartilhado por alguém com você. Não é possível recuperar iniciativas excluídas.

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
   <td> <p>Você deve comprar uma licença adicional para a [!DNL Adobe Workfront Scenario Planner] para acessar a funcionalidade descrita neste artigo. </p> <p>Para obter informações sobre como obter o [!DNL Workfront Scenario Planner], consulte <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">Acesso necessário para usar o [!UICONTROL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><strong>Configurações de nível de acesso*</strong> </td> 
   <td> <p>Acesso à [!UICONTROL Editar] ou superior à [!DNL Scenario Planner]</p> <p>Observação: Se ainda não tiver acesso, pergunte ao seu [!DNL Workfront] administrador se eles definirem restrições adicionais em seu nível de acesso. Para obter informações sobre como uma [!DNL Workfront] administrador pode alterar seu nível de acesso, consulte <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><strong>Permissões de objeto</strong> </p> </td> 
   <td> <p>Permissões do [!UICONTROL Manager] para um plano</p> <p>Para obter informações sobre como solicitar acesso adicional a um plano, consulte <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">Solicitar acesso a um plano na [!DNL Scenario Planner]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Excluir iniciativas

Considere o seguinte ao excluir iniciativas:

* A exclusão de uma iniciativa remove do plano a quantidade necessária de funções de cargo e as informações de custo associadas à iniciativa.
* A exclusão de uma iniciativa criada pela importação de um projeto não exclui o projeto associado à iniciativa.
* A exclusão de uma iniciativa que tenha sido publicada em um projeto pelo menos uma vez resulta no seguinte:

   * A iniciativa é excluída do cenário, mas o cenário [!DNL Scenario Planner] a área permanece no [!UICONTROL Detalhes do projeto] seção.
   * Se a iniciativa que você exclui for a única iniciativa publicada no cenário, o indicador de que o plano foi publicado também será removido.

      Para obter informações sobre como publicar iniciativas em projetos, consulte [Atualize ou crie projetos publicando iniciativas no [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md).

      Para obter informações sobre como criar iniciativas importando projetos, consulte [Importar projetos para planos na [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md) .

É possível excluir uma iniciativa de cada vez ou excluir várias iniciativas em massa.

* [Excluir uma iniciativa](#delete-one-initiative)
* [Excluir iniciativas em massa](#delete-initiatives-in-bulk)

### Excluir uma iniciativa {#delete-one-initiative}

1. Clique no botão **[!UICONTROL Menu principal]** ícone ![](assets/main-menu-icon.png), depois clique em [!UICONTROL Cenários].

   Uma lista de planos é exibida.

1. Clique no nome de um plano para abri-lo, depois localize a iniciativa que deseja excluir.
1. Siga um destes procedimentos:

   * Clique no botão **[!UICONTROL Menu Mais]** ![](assets/more-menu.png) à direita do nome da iniciativa, em seguida, clique em **[!UICONTROL Excluir]** > **[!UICONTROL Sim, exclua]**.

   * Selecione a caixa à esquerda da iniciativa e clique em **[!UICONTROL Excluir]** no menu flutuante que aparece na parte inferior do plano, em seguida, clique em **[!UICONTROL Sim, exclua]**.

   A iniciativa, bem como o seu papel e informações sobre custos são eliminados do plano.

1. Clique em **[!UICONTROL Salvar plano]** para salvar as alterações.

### Excluir iniciativas em massa {#delete-initiatives-in-bulk}

1. Clique no botão **[!UICONTROL Menu principal]** ícone ![](assets/main-menu-icon.png), depois clique em [!UICONTROL Cenários].

   Uma lista de planos é exibida.

1. Clique no nome de um plano para abri-lo, depois localize a iniciativa que deseja excluir.
1. Selecione as caixas à esquerda das iniciativas que deseja excluir e clique em **[!UICONTROL Excluir]** no menu exibido na parte inferior do plano, clique em **[!UICONTROL Sim, exclua]**.

   ![](assets/bottom-manage-initiative-menu-350x45.png)

   As iniciativas, o seu cargo e as informações sobre custos são excluídos do plano.

1. Clique em **[!UICONTROL Salvar plano]** para salvar as alterações.
