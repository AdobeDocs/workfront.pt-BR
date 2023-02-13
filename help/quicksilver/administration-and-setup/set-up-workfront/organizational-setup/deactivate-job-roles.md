---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: organization-setup
title: Desativar funções de trabalho
description: Como um [!DNL Adobe Workfront] administrador ou um usuário com acesso administrativo às Funções de trabalho, você pode desativar funções de trabalho que se tornam obsoletas em seu sistema. Ao desativar uma função de trabalho em vez de excluí-la, você pode manter qualquer informação histórica associada a ela.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 934cef1a-8157-45db-b000-24a08a94dd18
source-git-commit: b6f6964bb80f172849434c669df2b0ecd735a590
workflow-type: tm+mt
source-wordcount: '690'
ht-degree: 0%

---

# Desativar funções de trabalho

Como um [!DNL Adobe Workfront] administrador ou um usuário com acesso administrativo às Funções de trabalho, você pode desativar funções de trabalho que se tornam obsoletas em seu sistema. Ao desativar uma função de trabalho em vez de excluí-la, você pode manter qualquer informação histórica associada a ela.

Também é possível reativar funções de trabalho que foram desativadas anteriormente.

## Requisitos de acesso

Você deve ter o seguinte:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plano da [!UICONTROL Adobe Workfront]*</td> 
   <td> <p>Qualquer Um </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da [!UICONTROL Adobe Workfront]*</td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Acesso administrativo às funções de trabalho</p> <p><b>OBSERVAÇÃO</b>: Se ainda não tiver acesso, pergunte ao seu [!DNL Workfront] administrador se eles definirem restrições adicionais em seu nível de acesso. Para obter informações sobre como uma [!DNL Workfront] administrador pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com seu [!DNL Workfront] administrador.

## O impacto da desativação de funções de trabalho

Se você desativar uma função de trabalho, ela não será mais exibida nas seguintes áreas:

* O [!UICONTROL Atribuições] campo typeforward (para tarefas, tarefas de modelo, emissões, aprovações e regras de roteamento)
* O [!UICONTROL Atribuições] campos em listas e relatórios
* Perfis de usuário

   >[!NOTE]
   >
   >Quando você adiciona uma nova função a um usuário, uma função de trabalho desativada não é exibida. Mas continua sendo exibido no [!UICONTROL Função principal] e [!UICONTROL Outras funções] campos se o usuário foi associado à função de trabalho antes de ser desativado.

* O [!UICONTROL Compartilhamento] caixa de diálogo para objetos, incluindo atribuição de modelo de layout
* Digitar campos avançados em formulários personalizados
* O [!UICONTROL Membros do Pool] em [!UICONTROL Pools de Recursos]
* O [!UICONTROL Função da Tarefa] campo de um [!UICONTROL Taxa de Faturamento] editar tela quando um usuário estiver substituindo as taxas de faturamento de projetos
* O [!UICONTROL Adicionar atribuição ao quadro Kanban] caixa de diálogo em um projeto
* O [!UICONTROL Função da Tarefa] campo de um plano ou de uma iniciativa quando alguém estiver usando a variável [!DNL Adobe Workfront Scenario Planner].

   O [!DNL Scenario Planner] está disponível somente no novo [!DNL Adobe Workfront] e requer uma licença adicional. Para obter informações sobre o [!DNL Workfront Scenario Planner], consulte [O [!DNL Scenario Planner] visão geral](../../../scenario-planner/scenario-planner-overview.md).

>[!TIP]
>
>As funções desativadas sempre são exibidas nos filtros em listas, relatórios e outras ferramentas, como a [!DNL Workload Balancer].

## Considerações antes de desativar uma função de trabalho

É melhor desativar em vez de excluir funções de trabalho que se tornam obsoletas para que você possa manter todas as informações históricas associadas a funções que você possa ter usado no passado.

>[!NOTE]
>
>Qualquer trabalho atribuído à função de trabalho antes da desativação permanece atribuído.

Recomendamos que você faça o seguinte antes de desativar uma função de trabalho não utilizada:

* Crie relatórios para quaisquer objetos que estejam atribuídos à função que você planeja desativar e reatribuí-los a uma função de trabalho ativa. Para obter informações sobre como criar relatórios, consulte [Criar um relatório](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md).

   >[!TIP]
   >
   >Você pode criar um relatório para filtrar quaisquer tarefas ou problemas em que a função desativada esteja atribuída. Em seguida, use o relatório para reatribuir tarefas ou problemas pendentes a uma função ativa.

* Faça um inventário de todos os processos de aprovação, caminhos de aprovação atuais e regras de roteamento ou outros objetos atribuídos à função de trabalho que você planeja desativar e reatribuí-los a uma função ativa.

   >[!TIP]
   >
   >Ao usar filas de solicitações, se você desativar uma função de trabalho atribuída como o destinatário padrão em uma regra de roteamento, a função permanecerá e as solicitações ainda serão roteadas para a função desativada. Recomendamos atualizar as regras de roteamento com funções ativas antes de desativar a equipe.

   Para obter informações sobre como criar processos de aprovação e regras de roteamento, consulte os seguintes artigos:

   * [Criar um processo de aprovação para itens de trabalho](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md)
   * [Criar regras de roteamento](../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md)

## Desativar uma função de trabalho

1. Clique no botão **[!UICONTROL Menu principal]** ícone ![](assets/main-menu-icon.png) no canto superior direito de [!DNL Adobe Workfront], depois clique em **[!UICONTROL Configuração]** ![](assets/gear-icon-settings.png).

1. No painel esquerdo, clique em &#x200B; **[!UICONTROL Funções do Trabalho].**
1. (Opcional) Na seção **[!UICONTROL Filtro]** , selecione **[!UICONTROL Ativo]** para exibir somente funções de job ativas.
1. Clique no nome da função de trabalho que deseja desativar.
1. No **[!UICONTROL Está ativo]** , selecione **[!UICONTROL Não]**.

   ![](assets/deactivate-job-role-edit-role-box-nwe.png)

1. Clique em **[!UICONTROL Salvar alterações]**.

   A função de trabalho é desativada e não pode mais ser atribuída ao trabalho, associada aos modelos de layout e assim por diante. Para obter informações sobre todos os usos de funções de cargo em [!DNL Workfront], consulte [Visão geral da função de trabalho](../../../administration-and-setup/set-up-workfront/organizational-setup/job-role-overview.md).
