---
product-area: calendars
navigation-topic: calendars-navigation-topic
title: Usar campos de data personalizados em um relatório de calendário
description: Um relatório de calendário é um relatório dinâmico que fornece uma representação visual do seu trabalho. Você pode usar campos de data personalizados em um relatório de calendário para tarefas, problemas e projetos.
author: Lisa
feature: Reports and Dashboards
exl-id: 40cc8628-7641-41ce-b8e5-7f5ed5ad36c7
source-git-commit: 880e82546ac0ca80be60f03db31b99ad1778c35a
workflow-type: tm+mt
source-wordcount: '696'
ht-degree: 1%

---

# Usar campos de data personalizados em um relatório de calendário

A [!UICONTROL calendário] relatório é um relatório dinâmico que fornece uma representação visual do seu trabalho. Você pode usar campos de data personalizados em um relatório de calendário para os seguintes objetos:

* Tarefas
* Problemas
* Projetos

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas deste artigo:

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
   <td> <p>[!UICONTROL Plano] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurações de nível de acesso*</strong></td> 
   <td> <p>[!UICONTROL Editar] acesso a [!UICONTROL Relatórios], [!UICONTROL Painéis] e [!UICONTROL Calendários]</p> <p>Observação: se você ainda não tiver acesso, pergunte ao seu [!DNL Workfront] administrador se eles definirem restrições adicionais no seu nível de acesso. Para obter informações sobre como uma [!DNL Workfront] administrador pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Permissões de objeto</strong></td> 
   <td> <p>Acesso [!UICONTROL Gerenciar] ao relatório de calendário</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir que plano, tipo de licença ou acesso você tem, entre em contato com o [!DNL Workfront] administrador.

## Pré-requisitos

1. É necessário ter campos de data personalizados e um valor dentro do campo disponível em [!DNL Workfront] instância. Se você não tiver um formulário personalizado configurado com datas personalizadas, siga as instruções nas duas primeiras seções em [Criar ou editar um formulário personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).
1. Anexe o formulário personalizado a um projeto, tarefa ou problema que você planeja adicionar ao calendário e especifique uma data. Para obter mais informações, consulte [Adicionar um formulário personalizado a um objeto](../../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

## Configurar o grupo de itens

Você pode escolher como deseja que o grupo de itens seja exibido no calendário.

1. Clique em **[!UICONTROL Menu principal]** ícone ![](assets/main-menu-icon.png) no canto superior direito de [!DNL Adobe Workfront]e, em seguida, clique em **[!UICONTROL Calendários]**.

1. Selecione o calendário ao qual deseja adicionar um novo grupo de itens.\
   Ou\
   Clique em **[!UICONTROL + Novo calendário]** e insira o nome do calendário.

   >[!NOTE]
   >
   >Você deve ter [!UICONTROL Editar] acesso a [!UICONTROL Relatórios], [!UICONTROL Painéis], e [!UICONTROL Calendários] em seu nível de acesso para criar um relatório de calendário.

1. À esquerda, clique em **[!UICONTROL Adicionar ao calendário]** e, em seguida, clique em **[!UICONTROL Adicionar itens avançados]**.

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
      <td>Escolher <strong>[!UICONTROL Datas personalizadas]</strong>.<br></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL No calendário, mostrar]</strong></td>
      <td><p>Escolha como deseja que as datas sejam exibidas:</p>
       <ul>
        <li><strong>[!UICONTROL Data Única]</strong>: o calendário exibe o objeto em uma única data.</li>
        <li><strong>[!UICONTROL Duração] (Início ao Fim)</strong>: o calendário exibe o objeto durante um período de dias.<br><p>Observação: se você escolher <strong>[!UICONTROL Duração]</strong>, a data de término especificada deve ser posterior à data de início ou o item não será exibido no calendário.</p></li>
       </ul></td>
     </tr>
     <tr data-mc-conditions="">
      <td role="rowheader"><strong>[!UICONTROL Datas Personalizadas]</strong></td>
      <td><p>Insira o nome da data personalizada anexada ao objeto que você deseja rastrear.</p><p><strong>NOTA:</strong> A pesquisa pelo nome de data personalizado é limitada a 50 resultados para evitar problemas de desempenho.</td>
     </tr>
    </tbody>
   </table>

1. Prossiga para a seção a seguir.

## Adicionar objetos ao grupo de itens

Depois de configurar como deseja que os itens sejam exibidos, você precisa adicionar os objetos que deseja ver no calendário ao agrupamento.

1. No **[!UICONTROL O que você deseja adicionar ao calendário?]** , selecione

   * **[!UICONTROL Tarefas]**
   * **[!UICONTROL Projetos]**
   * **[!UICONTROL Problemas]**

1. Clique em **[!UICONTROL Adicionar tarefas]**, **[!UICONTROL Adicionar Projetos]** ou **[!UICONTROL Adicionar Problemas]**, dependendo do tipo de objeto que você está adicionando ao calendário.\
   ![Selecionar objeto para o calendário](assets/field-name.png)

1. No menu suspenso, comece digitando o nome do campo e selecione a origem do campo do objeto que deseja exibir no calendário (por exemplo, **[!UICONTROL Tarefas atrasadas]**).
1. Definir uma declaração de condição para o agrupamento de calendário.

   ![Declaração de condição](assets/condition-statement-calendar.png)

   Para saber mais sobre a configuração de condições, consulte [Filtro e modificadores de condição](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

1. (Opcional) Especifique objetos adicionais para o agrupamento de calendário repetindo as Etapas de 1 a 4.
1. No **[!UICONTROL Definir os rótulos de Tarefas/Projetos/Problemas para serem...]** selecione como os objetos deste agrupamento de calendário são rotulados no calendário.

   >[!NOTE]
   >
   >Se as opções de rótulo padrão não estiverem disponíveis para um determinado objeto, o nome do objeto será exibido. Por exemplo, quando a variável [!UICONTROL Tarefa pai] rótulo estiver selecionado e não houver nenhuma tarefa pai associada ao objeto, [!DNL Adobe Workfront] exibe o nome do objeto que você está exibindo no calendário.

1. Clique em **[!UICONTROL Salvar]**.
