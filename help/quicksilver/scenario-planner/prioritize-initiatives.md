---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Atualizar prioridades de iniciativa no Planejador de cenários
description: Priorizar iniciativas é importante porque as iniciativas recebem funções de trabalho e recursos de orçamento do plano na ordem em que estão listadas no plano.
author: Alina
feature: Workfront Scenario Planner
exl-id: 45f019de-b29c-477b-8bd1-f32ef21c1015
source-git-commit: 7cfe82eb703e2a043c264cf86c0e5424d1e33d78
workflow-type: tm+mt
source-wordcount: '545'
ht-degree: 1%

---

# Atualizar prioridades de iniciativa no [!DNL Scenario Planner]

Priorizar iniciativas é importante porque as iniciativas recebem funções de trabalho e recursos de orçamento do plano na ordem em que estão listadas no plano.

É possível priorizar iniciativas em um plano criado ou em um plano que alguém compartilhou com você.

Para obter informações sobre como criar planos, consulte [Criar e editar planos no [!DNL Scenario Planner]](../scenario-planner/create-and-edit-plans.md).

Para obter informações sobre como criar iniciativas, consulte [Criar e editar iniciativas no [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md).

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
   <p>O Planejador de cenários não está disponível para os novos planos Select ou Prime do Workfront Workfront. </p>
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

## Atualizar prioridades de iniciativa

Ao alterar a prioridade das iniciativas, você modifica a ordem de listagem no plano.

Recomendamos que você coloque iniciativas mais urgentes no topo de um plano e as mais fluidas - isso pode ser feito a qualquer momento e somente se os recursos estiverem disponíveis - na parte inferior do plano.

>[!NOTE]
>
>[!DNL Workfront] aloca recursos do plano para iniciativas na ordem em que estão listadas no plano.
>
>Por exemplo, se o plano tiver três engenheiros disponíveis e a Iniciativa 1 e a Iniciativa 2 exigirem que dois engenheiros sejam concluídos e ambos estiverem programados para o mesmo período, a Workfront associará dois engenheiros à Iniciativa 1 e um engenheiro disponível restante à Iniciativa 2. Neste caso, a Iniciativa 2 mostra que tem um conflito, porque falta um engenheiro. Às vezes, alterar a prioridade de suas iniciativas é a única maneira de evitar conflitos em um plano.

Para atualizar a prioridade da iniciativa:

{{step1-to-scenario-planner}}

Uma lista de planos é exibida.

1. Clique no nome de um plano para abri-lo e, em seguida, localize as iniciativas que deseja priorizar.
1. Clique na caixa à esquerda do nome de uma ou mais iniciativas e siga um destes procedimentos:

   * Clique na alça à esquerda dos nomes de uma das iniciativas selecionadas e arraste-a para cima ou para baixo na lista para alterar a prioridade da iniciativa.

     O Workfront exibe o número de iniciativas selecionadas.

     ![Número da iniciativa de seleção múltipla](assets/multi-select-initiative-number.png)

   * Clique na caixa **[!UICONTROL Priorizar]** na parte inferior do plano e escolha uma das seguintes opções:

      * **[!UICONTROL Superior]**: move as iniciativas selecionadas para o topo da lista de iniciativas. As iniciativas selecionadas são listadas primeiro no plano.
      * **[!UICONTROL Inferior]**: move as iniciativas selecionadas para a parte inferior da lista de iniciativas. As iniciativas selecionadas são listadas por último no plano.
      * **[!UICONTROL Selecionar um número]**: move as iniciativas selecionadas após a iniciativa que você indicar aqui.

        ![Priorizar iniciativas](assets/prioritize-initiatives-expanded-highlighted-350x171.png)

     O [!DNL Workfront] coloca imediatamente as iniciativas selecionadas onde você indica e os números de todas as iniciativas são atualizados de acordo.

1. Clique em **[!UICONTROL Salvar Plano]** para salvar suas alterações.
