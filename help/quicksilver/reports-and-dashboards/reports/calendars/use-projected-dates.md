---
product-area: calendars
navigation-topic: calendars-navigation-topic
title: Usar datas projetadas em um relatório de calendário
description: Um relatório de calendário é um relatório dinâmico que fornece uma representação visual do seu trabalho. Você pode usar os campos Data projetada em um relatório de calendário para tarefas, problemas e projetos.
author: Lisa
feature: Reports and Dashboards
exl-id: 39e16f0b-c10d-429e-9eb5-d4847c7e4ed9
source-git-commit: d90459cb4f6fb1960552f0ab174e963582312b5c
workflow-type: tm+mt
source-wordcount: '609'
ht-degree: 1%

---

# Usar [!UICONTROL Datas Projetadas] em um relatório de calendário

Um relatório de calendário é um relatório dinâmico que fornece uma representação visual do seu trabalho. Você pode usar os campos Data projetada em um relatório de calendário para os seguintes objetos:

* Tarefas
* Problemas
* Projetos

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront plan]</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licença</td> 
   <td><p>Novo: Padrão</p>
       <p>ou</p>
       <p>Atual: Plano</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>[!UICONTROL Editar] acesso a [!UICONTROL Relatórios], [!UICONTROL Painéis] e [!UICONTROL Calendários]</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td>Acesso [!UICONTROL Gerenciar] ao relatório de calendário</td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Configurar o grupo de itens

Você pode escolher como deseja que o grupo de itens seja exibido no calendário.

{{step1-to-calendars}}

1. Selecione o calendário ao qual deseja adicionar um novo grupo de itens.
Ou
Clique em **[!UICONTROL + Novo calendário]** e digite o nome do calendário.

   >[!NOTE]
   >
   >Você deve ter acesso de [!UICONTROL Edição] a [!UICONTROL Relatórios], [!UICONTROL Painéis] e [!UICONTROL Calendários] no seu nível de acesso para criar um relatório de calendário.

1. À esquerda, clique em **[!UICONTROL Adicionar ao Calendário]** e em **[!UICONTROL Adicionar itens avançados]**.

1. Especifique o seguinte:

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Nomear este grupo de itens]</strong></td>
      <td>Digite um nome para o grupo de itens.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Cor]</strong></td>
      <td>Selecione uma cor para o grupo de itens. Todos os itens são exibidos na cor selecionada no relatório de calendário.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Campo de Data]</strong></td>
      <td><p>Escolha <strong>[!UICONTROL Datas Projetadas]</strong>. Para obter mais informações sobre Datas Projetadas, consulte </p>
       <ul>
        <li><a href="../../../manage-work/projects/planning-a-project/project-projected-start-date.md" class="MCXref xref">Visão Geral da Data de Início Projetada do projeto</a></li>
        <li><a href="../../../manage-work/projects/planning-a-project/project-projected-completion-date.md" class="MCXref xref">Visão geral da Data de conclusão projetada para projetos, tarefas e problemas</a><br></li>
       </ul></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL No calendário, mostrar]</strong></td>
      <td><p>Escolha como deseja que as datas sejam exibidas:</p>
       <ul>
        <li><strong>[!UICONTROL Somente Data de Início]</strong>: o calendário exibe o objeto em uma única data.</li>
        <li><strong>[!UICONTROL Somente Data de Término]</strong>: o calendário exibe o objeto em uma única data.</li>
        <li><strong>[!UICONTROL Duration] (Início ao Fim)</strong>: o calendário exibe o objeto durante um período de dias.</li>
       </ul></td>
     </tr>
     <tr data-mc-conditions="">
      <td role="rowheader"><strong>[!UICONTROL Alternar para Datas Reais quando disponível]</strong></td>
      <td><p>O calendário alterna automaticamente para datas reais quando elas estão disponíveis. <br>Escolha <strong>[!UICONTROL Sim]</strong> ou <strong>[!UICONTROL Não]</strong> para alternar para datas reais quando disponíveis. Para obter mais informações sobre Datas Reais, consulte</p>
       <ul>
        <li><a href="../../../manage-work/projects/planning-a-project/project-actual-start-date.md" class="MCXref xref">Visão Geral da Data de Início Efetivo do projeto </a></li>
        <li><a href="../../../manage-work/projects/planning-a-project/project-actual-completion-date.md" class="MCXref xref">Visão geral da Data de Término Efetivo do projeto </a></li>
       </ul></td>
     </tr>
    </tbody>
   </table>

1. Prossiga para a seção a seguir.

## Adicionar objetos ao grupo de itens

Depois de configurar como deseja que os itens sejam exibidos, você precisa adicionar os objetos que deseja ver no calendário ao agrupamento.

1. No **[!UICONTROL O que você deseja adicionar ao calendário?seção]**, selecione

   * **[!UICONTROL Tarefas]**
   * **[!UICONTROL Projetos]**
   * **[!UICONTROL Problemas]**

1. Clique em **[!UICONTROL Adicionar Tarefas]**, **[!UICONTROL Adicionar Projetos]** ou **[!UICONTROL Adicionar Problemas]**, dependendo do tipo de objeto que você está adicionando ao calendário.
   ![Selecionar objeto para o calendário](assets/field-name.png)

1. No menu suspenso, comece digitando o nome do campo e selecione a origem do campo do objeto que deseja exibir no calendário (por exemplo, **[!UICONTROL Tarefas atrasadas]**).
1. Definir uma declaração de condição para o agrupamento de calendário.

   ![Declaração de condição](assets/condition-statement-calendar.png)

   Para saber mais sobre como definir condições, consulte [Filtro e modificadores de condição](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

1. (Opcional) Especifique objetos adicionais para o agrupamento de calendário repetindo as Etapas de 1 a 4.
1. No campo **[!UICONTROL Definir os rótulos de Tarefas/Projetos/Problemas para...]**, selecione como os objetos neste agrupamento de calendário são rotulados no calendário.

   >[!NOTE]
   >
   >Se as opções de rótulo padrão não estiverem disponíveis para um determinado objeto, o nome do objeto será exibido. Por exemplo, quando o rótulo Tarefa Pai é selecionado e não há nenhuma tarefa pai associada ao objeto, [!DNL Adobe Workfront] exibe o nome do objeto que você está visualizando no calendário.

1. Clique em **[!UICONTROL Salvar]**.
