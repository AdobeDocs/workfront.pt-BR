---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Atualizar as prioridades da iniciativa no Planejador de Cenário
description: A priorização de iniciativas é importante porque as iniciativas recebem funções de emprego e recursos orçamentais do plano na ordem em que são listadas no plano.
author: Alina
feature: Workfront Scenario Planner
exl-id: 45f019de-b29c-477b-8bd1-f32ef21c1015
source-git-commit: e152c20e7b987f4bef7ffd6ee534c059f7b9bf45
workflow-type: tm+mt
source-wordcount: '536'
ht-degree: 0%

---

# Atualizar as prioridades da iniciativa no [!DNL Scenario Planner]

A priorização de iniciativas é importante porque as iniciativas recebem funções de emprego e recursos orçamentais do plano na ordem em que são listadas no plano.

Você pode priorizar iniciativas em um plano criado por você ou em um plano compartilhado por alguém com você.

Para obter informações sobre como criar planos, consulte [Crie e edite planos na [!DNL Scenario Planner]](../scenario-planner/create-and-edit-plans.md).

Para obter informações sobre como criar iniciativas, consulte [Crie e edite iniciativas na [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md).

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
   <td> <p>Você deve comprar uma licença adicional para a [!DNL Adobe Workfront Scenario Planner] para acessar a funcionalidade descrita neste artigo.</p> <p>Para obter informações sobre como obter o [!DNL Workfront Scenario Planner], consulte <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">O acesso necessário para usar o [!DNL Scenario Planner]</a>. </p> </td> 
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

## Atualizar prioridades da iniciativa

Quando você altera a prioridade das iniciativas, modifica a ordem de listagem do plano.

Recomendamos que você coloque iniciativas mais urgentes no topo de um plano e as mais fluidas - que poderiam ser feitas a qualquer momento e apenas se houver recursos disponíveis - no fim do plano.

>[!NOTE]
>
>[!DNL Workfront] atribui recursos do plano a iniciativas na ordem em que estão listadas no plano.
>
>Por exemplo, se o plano tiver 3 engenheiros e a Iniciativa 1 e a Iniciativa 2 disponíveis, cada um exigirá que dois engenheiros sejam concluídos e ambos estejam programados para o mesmo período, a Workfront associará dois engenheiros à Iniciativa 1 e um engenheiro disponível à Iniciativa 2. Neste caso, a Iniciativa 2 mostra ter um conflito, porque falta um engenheiro. Por vezes, alterar a prioridade das vossas iniciativas é a única forma de evitar conflitos num plano.

Para atualizar a prioridade da iniciativa:

1. Clique no botão **[!UICONTROL Menu principal]** ícone ![](assets/main-menu-icon.png), depois clique em [!UICONTROL Cenários].

   Uma lista de planos é exibida.

1. Clique no nome de um plano para abri-lo, depois localize as iniciativas que deseja priorizar.
1. Clique na caixa à esquerda de um ou mais nomes de iniciativas e siga um destes procedimentos:

   * Clique na alça à esquerda de um dos nomes das iniciativas selecionadas e arraste-a para cima ou para baixo na lista para alterar a prioridade da iniciativa.

      O Workfront exibe o número de iniciativas selecionadas.

      ![](assets/multi-select-initiative-number.png)

   * Clique no botão **[!UICONTROL Priorizar]** na parte inferior do plano, escolha entre as seguintes opções:

      * **[!UICONTROL Topo]**: Move as iniciativas selecionadas para o topo da lista de iniciativas. As iniciativas selecionadas são listadas primeiro no plano.
      * **[!UICONTROL Inferior]**: Move as iniciativas selecionadas para o final da lista de iniciativas. As iniciativas selecionadas são listadas por último no plano.
      * **[!UICONTROL Selecionar um número]**: Move as iniciativas selecionadas após a iniciativa indicada aqui.

         ![](assets/prioritize-initiatives-expanded-highlighted-350x171.png)
      [!DNL Workfront] O coloca imediatamente as iniciativas selecionadas, onde você indica, e o número de todas as iniciativas é atualizado adequadamente.


1. Clique em **[!UICONTROL Salvar plano]** para salvar as alterações.
