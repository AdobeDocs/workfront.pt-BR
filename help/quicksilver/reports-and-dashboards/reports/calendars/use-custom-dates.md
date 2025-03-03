---
product-area: calendars
navigation-topic: calendars-navigation-topic
title: Usar campos de data personalizados em um relatório de calendário
description: Um relatório de calendário é um relatório dinâmico que fornece uma representação visual do seu trabalho. Você pode usar campos de data personalizados em um relatório de calendário para tarefas, problemas e projetos.
author: Lisa
feature: Reports and Dashboards
exl-id: 40cc8628-7641-41ce-b8e5-7f5ed5ad36c7
source-git-commit: 40bbb198216b2806154f83730d8afedd5f355a3e
workflow-type: tm+mt
source-wordcount: '1104'
ht-degree: 1%

---

# Usar campos de data personalizados em um relatório de calendário

<span class="preview">As informações destacadas nesta página referem-se a funcionalidades que ainda não estão disponíveis. Ele está disponível somente no ambiente de Pré-visualização da Sandbox.</span>

Um relatório de [!UICONTROL calendário] é um relatório dinâmico que fornece uma representação visual do seu trabalho. Você pode usar campos de data personalizados em um relatório de calendário para os seguintes objetos:

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

## Pré-requisitos

1. Você deve ter campos de data personalizados e um valor dentro do campo disponível em sua instância [!DNL Workfront]. Se você não tiver um formulário personalizado configurado com datas personalizadas, siga as instruções em [Criar um formulário personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).
1. Anexe o formulário personalizado a um projeto, tarefa ou problema que você planeja adicionar ao calendário e especifique uma data. Para obter mais informações, consulte [Adicionar um formulário personalizado a um objeto](../../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

## Configurar o grupo de itens na Produção

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
      <td>Escolha <strong>[!UICONTROL Datas personalizadas]</strong>.<br></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL No calendário, mostrar]</strong></td>
      <td><p>Escolha como deseja que as datas sejam exibidas:</p>
       <ul>
        <li><strong>[!UICONTROL Data Única]</strong>: o calendário exibe o objeto em uma única data.</li>
        <li><strong>[!UICONTROL Duration] (Início ao Fim)</strong>: o calendário exibe o objeto durante um período de dias.<br><p>Observação: se você escolher <strong>[!UICONTROL Duration]</strong>, a data de término especificada deverá ser posterior à data de início, caso contrário o item não será exibido no calendário.</p></li>
       </ul></td>
     </tr>
     <tr data-mc-conditions="">
      <td role="rowheader"><strong>[!UICONTROL Datas Personalizadas]</strong></td>
      <td><p>Insira o nome da data personalizada anexada ao objeto que você deseja rastrear.</p><p><strong>OBSERVAÇÃO:</strong> a pesquisa pelo nome de data personalizado está limitada a 50 resultados para evitar problemas de desempenho.</td>
     </tr>
    </tbody>
   </table>

1. Prossiga para a seção a seguir.

## Adicionar objetos ao grupo de itens na produção

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
   >Se as opções de rótulo padrão não estiverem disponíveis para um determinado objeto, o nome do objeto será exibido. Por exemplo, quando o rótulo [!UICONTROL Tarefa pai] é selecionado e não há nenhuma tarefa pai associada ao objeto, [!DNL Adobe Workfront] exibe o nome do objeto que você está visualizando no calendário.

1. Clique em **[!UICONTROL Salvar]**.

<div class="preview">

## Configurar o grupo de itens na Visualização

Você pode escolher como deseja que o grupo de itens seja exibido no calendário.

{{step1-to-calendars}}

1. Selecione o calendário ao qual deseja adicionar um novo grupo de itens, clique no menu Mais e **Editar**.
Ou
Clique em **[!UICONTROL + Novo calendário]**, digite o nome do projeto e clique em **[!UICONTROL Adicionar itens avançados]**.

   >[!NOTE]
   >
   >Você deve ter acesso de [!UICONTROL Edição] a [!UICONTROL Relatórios], [!UICONTROL Painéis] e [!UICONTROL Calendários] no seu nível de acesso para criar um relatório de calendário.

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
      <td>Escolha <strong>[!UICONTROL Datas personalizadas]</strong>.<br></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL No calendário, mostrar]</strong></td>
      <td><p>Escolha como deseja que as datas sejam exibidas:</p>
       <ul>
        <li><strong>[!UICONTROL Data Única]</strong>: o calendário exibe o objeto em uma única data.</li>
        <li><strong>[!UICONTROL Duration] (Início ao Fim)</strong>: o calendário exibe o objeto durante um período de dias.<br><p>Observação: se você escolher <strong>[!UICONTROL Duration]</strong>, a data de término especificada deverá ser posterior à data de início, caso contrário o item não será exibido no calendário.</p></li>
       </ul></td>
     </tr>
     <tr data-mc-conditions="">
      <td role="rowheader"><strong>[!UICONTROL Datas Personalizadas]</strong></td>
      <td><p>Insira o nome da data personalizada anexada ao objeto que você deseja rastrear.</p><p><strong>OBSERVAÇÃO:</strong> a pesquisa pelo nome de data personalizado está limitada a 50 resultados para evitar problemas de desempenho.</td>
     </tr>
    </tbody>
   </table>

1. Prossiga para a seção a seguir.

### Adicionar objetos ao grupo de itens na Visualização

Depois de configurar como deseja que os itens sejam exibidos, você precisa adicionar os objetos que deseja ver no calendário ao agrupamento.

1. No **[!UICONTROL O que você deseja adicionar ao calendário?seção]**, selecione

   * **[!UICONTROL Tarefas]**
   * **[!UICONTROL Projetos]**
   * **[!UICONTROL Problemas]**

1. Clique em **[!UICONTROL Adicionar tarefas]**, **[!UICONTROL Adicionar projetos]**, **[!UICONTROL Adicionar problemas]** ou **Folga**, dependendo do tipo de objeto que você está adicionando ao calendário.

1. No menu suspenso, comece digitando o nome do campo e selecione a origem do campo do objeto que deseja exibir no calendário (por exemplo, **[!UICONTROL Tarefas atrasadas]**).
1. Definir uma declaração de condição para o agrupamento de calendário.


   Para saber mais sobre como definir condições, consulte [Filtro e modificadores de condição](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

   ![Selecionar objeto para o calendário](assets/calendar-field-name.png)

1. (Opcional) Especifique objetos adicionais para o agrupamento de calendário repetindo as Etapas de 1 a 4.
1. No campo **[!UICONTROL Definir os rótulos de Tarefas/Projetos/Problemas para...]**, selecione como os objetos neste agrupamento de calendário são rotulados no calendário.

   >[!NOTE]
   >
   >Se as opções de rótulo padrão não estiverem disponíveis para um determinado objeto, o nome do objeto será exibido. Por exemplo, quando o rótulo [!UICONTROL Tarefa pai] é selecionado e não há nenhuma tarefa pai associada ao objeto, [!DNL Adobe Workfront] exibe o nome do objeto que você está visualizando no calendário.

   ![definir rótulos de tarefa](assets/set-task-labels.png)
1. Clique em **[!UICONTROL Salvar]**.

</div>