---
product-area: calendars
navigation-topic: calendars-navigation-topic
title: Usar datas projetadas em um relatório de calendário
description: Um relatório de calendário é um relatório dinâmico que fornece uma representação visual do seu trabalho. Você pode usar os campos Data prevista em um relatório de calendário para tarefas, problemas e projetos.
author: Lisa
feature: Reports and Dashboards
exl-id: 39e16f0b-c10d-429e-9eb5-d4847c7e4ed9
source-git-commit: e5a3024b1657942cd7abdfff76a7a6795127a4f5
workflow-type: tm+mt
source-wordcount: '655'
ht-degree: 1%

---

# Use [!UICONTROL Datas Projetadas] em um relatório de calendário

Um relatório de calendário é um relatório dinâmico que fornece uma representação visual do seu trabalho. Você pode usar os campos Data prevista em um relatório de calendário para os seguintes objetos:

* Tarefas
* Problemas
* Projetos

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront plan*]</strong></td> 
   <td> <p>Qualquer Um</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licença*</strong></td> 
   <td> <p>[!UICONTROL Plan] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurações de nível de acesso*</strong></td> 
   <td> <p>[!UICONTROL ] Editar acesso aos [!UICONTROL Relatórios], [!UICONTROL Painéis] e [!UICONTROL Calendários]</p> <p>Observação: Se ainda não tiver acesso, pergunte ao seu [!DNL Workfront] administrador se eles definirem restrições adicionais em seu nível de acesso. Para obter informações sobre como uma [!DNL Workfront] administrador pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Permissões de objeto</strong></td> 
   <td> <p>Acesso ao [!UICONTROL Gerenciar] relatório de calendário</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com seu [!DNL Workfront] administrador.

## Configurar o grupo de itens

Você pode escolher como deseja que o grupo de itens seja exibido no seu calendário.

1. Clique no botão **[!UICONTROL Menu principal]** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront, em seguida, clique em **[!UICONTROL Calendários]**.

1. Selecione o calendário ao qual deseja adicionar um novo grupo de itens.\
   Ou\
   Clique em **[!UICONTROL + Novo calendário]** e insira o nome do calendário.

   >[!NOTE]
   >
   >Você deve ter [!UICONTROL Editar] acesso a [!UICONTROL Relatórios], [!UICONTROL Painéis]e [!UICONTROL Calendários] no seu nível de acesso para criar um relatório de calendário.

1. À esquerda, clique em **[!UICONTROL Adicionar ao Calendário]**, depois clique em **[!UICONTROL Adicionar itens avançados]**.

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
      <td role="rowheader"><strong>[!UICONTROL Campo de data]</strong></td>
      <td><p>Choose <strong>[!UICONTROL Datas projetadas]</strong>. Para obter mais informações sobre Datas Projetadas, consulte </p>
       <ul>
        <li><a href="../../../manage-work/projects/planning-a-project/project-projected-start-date.md" class="MCXref xref">Visão geral da data de início prevista do projeto</a></li>
        <li><a href="../../../manage-work/projects/planning-a-project/project-projected-completion-date.md" class="MCXref xref">Visão geral da data de conclusão projetada para projetos, tarefas e problemas</a><br></li>
       </ul></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL No calendário, mostrar]</strong></td>
      <td><p>Escolha como deseja que as datas sejam exibidas:</p>
       <ul>
        <li><strong>[!UICONTROL Somente Data de início]</strong>: O calendário exibe o objeto em uma única data.</li>
        <li><strong>[!UICONTROL Somente Data Final]</strong>: O calendário exibe o objeto em uma única data.</li>
        <li><strong>[!UICONTROL Duração] (Início ao fim)</strong>: O calendário exibe o objeto ao longo de um período de dias.</li>
       </ul></td>
     </tr>
     <tr data-mc-conditions="">
      <td role="rowheader"><strong>[!UICONTROL Alternar para datas reais quando disponível]</strong></td>
      <td><p>O calendário muda automaticamente para datas reais quando estão disponíveis. <br>Choose <strong>[!UICONTROL Sim]</strong> ou <strong>[!UICONTROL n.o]</strong> para alternar para datas reais, quando disponível. Para obter mais informações sobre Datas reais, consulte</p>
       <ul>
        <li><a href="../../../manage-work/projects/planning-a-project/project-actual-start-date.md" class="MCXref xref">Visão geral da data de início real do projeto </a></li>
        <li><a href="../../../manage-work/projects/planning-a-project/project-actual-completion-date.md" class="MCXref xref">Visão geral da data de conclusão real do projeto </a></li>
       </ul></td>
     </tr>
    </tbody>
   </table>

1. Prossiga para a seção a seguir.

## Adicionar objetos ao grupo de itens

Depois de configurar como deseja que os itens sejam exibidos, é necessário adicionar os objetos que deseja ver no calendário ao agrupamento.

1. No **[!UICONTROL O que deseja adicionar ao calendário?]** seção , selecione

   * **[!UICONTROL Tarefas]**
   * **[!UICONTROL Projetos]**
   * **[!UICONTROL Problemas]**

1. Clique em **[!UICONTROL Adicionar Tarefas]**, **[!UICONTROL Adicionar projetos]** ou **[!UICONTROL Adicionar problemas]**, dependendo do tipo de objeto que você está adicionando ao calendário.\
   ![Selecionar objeto para calendário](assets/field-name.png)

1. No menu suspenso , comece a digitar o nome do campo e selecione a fonte do campo do objeto que deseja exibir no calendário (por exemplo, **[!UICONTROL Tarefas atrasadas]**).
1. Defina uma declaração de condição para o agrupamento do calendário.

   ![Instrução de condição](assets/condition-statement-calendar.png)

   Para saber mais sobre as condições de configuração, consulte [Modificadores de filtro e condição](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

1. (Opcional) Especifique objetos adicionais para o agrupamento do calendário repetindo as Etapas 1 a 4.
1. No **[!UICONTROL Defina os rótulos Tarefas/Projetos/Problemas para que sejam..]** , selecione como os objetos neste agrupamento de calendário são rotulados no calendário.

   >[!NOTE]
   >
   >Se as opções de rótulo padrão não estiverem disponíveis para um determinado objeto, o nome do objeto será exibido. Por exemplo, quando o rótulo Tarefa pai é selecionado e não há nenhuma tarefa pai associada ao objeto, [!DNL Adobe Workfront] exibe o nome do objeto que você está visualizando no calendário.

1. Clique em **[!UICONTROL Salvar]**.
