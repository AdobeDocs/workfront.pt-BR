---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: organization-setup
title: Desativar funções de trabalho
description: Como um [!DNL Adobe Workfront] administrador ou um usuário com acesso administrativo a Funções de trabalho, você pode desativar funções de trabalho que se tornam obsoletas no sistema. Ao desativar uma função de trabalho em vez de excluí-la, você pode manter todas as informações históricas associadas a ela.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 934cef1a-8157-45db-b000-24a08a94dd18
source-git-commit: 9c0160dc5e43f36b65d9f2d4a3498a9c5f39f6f1
workflow-type: tm+mt
source-wordcount: '692'
ht-degree: 0%

---

# Desativar funções de trabalho

Como um [!DNL Adobe Workfront] administrador ou um usuário com acesso administrativo a Funções de trabalho, você pode desativar funções de trabalho que se tornam obsoletas no sistema. Ao desativar uma função de trabalho em vez de excluí-la, você pode manter todas as informações históricas associadas a ela.

Você também pode reativar funções de trabalho que foram desativadas anteriormente.

## Requisitos de acesso

Você deve ter o seguinte:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plano [!UICONTROL Adobe Workfront]*</td> 
   <td> <p>Qualquer Um </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da [!UICONTROL Adobe Workfront]*</td> 
   <td>[!UICONTROL Plano]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Acesso administrativo a funções de trabalho</p> <p><b>NOTA</b>: Se ainda não tiver acesso, pergunte ao seu [!DNL Workfront] administrador se eles definirem restrições adicionais no seu nível de acesso. Para obter informações sobre como uma [!DNL Workfront] administrador pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir que plano, tipo de licença ou acesso você tem, entre em contato com o [!DNL Workfront] administrador.

## O impacto da desativação de funções de trabalho

Se você desativar uma função de trabalho, ela não será mais exibida nas seguintes áreas:

* A variável [!UICONTROL Atribuições] campo de digitação antecipada (para tarefas, tarefas de modelo, problemas, aprovações e regras de roteamento)
* A variável [!UICONTROL Atribuições] campos em listas e relatórios
* Perfis de usuário

   >[!NOTE]
   >
   >Quando você adiciona uma nova função a um usuário, uma função de trabalho desativada não é exibida. Mas continua a ser exibido no [!UICONTROL Função Primária] e [!UICONTROL Outras Funções] se o usuário estava associado à função de trabalho antes de ser desativado.

* A variável [!UICONTROL Compartilhamento] caixa de diálogo para objetos, incluindo atribuição de modelo de layout
* Campos de digitação antecipada em formulários personalizados
* A variável [!UICONTROL Membros do pool] campo em [!UICONTROL Conjuntos de recursos]
* A variável [!UICONTROL Função de trabalho] campo de a [!UICONTROL Taxa de cobrança] editar tela quando um usuário estiver substituindo taxas de faturamento de projetos
* A variável [!UICONTROL Adicionar atribuição ao quadro Kanban] em um projeto
* A variável [!UICONTROL Função de trabalho] campo de um plano ou de uma iniciativa quando alguém estiver usando o [!DNL Adobe Workfront Scenario Planner].

   A variável [!DNL Scenario Planner] está disponível somente no novo [!DNL Adobe Workfront] e exige uma licença adicional. Para obter informações sobre o [!DNL Workfront Scenario Planner], consulte [A variável [!DNL Scenario Planner] visão geral](../../../scenario-planner/scenario-planner-overview.md).

>[!TIP]
>
>As funções desativadas sempre são exibidas em filtros em listas, relatórios e outras ferramentas, como o [!UICONTROL Balanceador de carga de trabalho].

## Considerações antes de desativar uma função de trabalho

É melhor desativar, em vez de excluir, as funções de trabalho que se tornam obsoletas para que você possa manter todas as informações históricas associadas às funções que você pode ter usado no passado.

>[!NOTE]
>
>Qualquer trabalho atribuído à função de trabalho antes da desativação permanece atribuído.

Recomendamos que você faça o seguinte antes de desativar uma função de trabalho não usada:

* Crie relatórios para quaisquer objetos atribuídos à função que você planeja desativar e reatribua-os a uma função de trabalho ativa. Para obter informações sobre a criação de relatórios, consulte [Criar um relatório](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md).

   >[!TIP]
   >
   >É possível criar um relatório para filtrar qualquer tarefa ou problema ao qual a função desativada esteja atribuída. Em seguida, use o relatório para reatribuir tarefas ou problemas pendentes a uma função ativa.

* Faça um inventário de todos os processos de aprovação, caminhos de aprovação atuais e regras de encaminhamento ou outros objetos atribuídos à função de trabalho que você planeja desativar e reatribua-os a uma função ativa.

   >[!TIP]
   >
   >Ao usar filas de solicitações, se você desativar uma função de trabalho atribuída como o destinatário padrão em uma regra de roteamento, a função permanecerá e as solicitações ainda serão encaminhadas para a função desativada. Recomendamos atualizar as regras de roteamento com funções ativas antes de desativar a equipe.

   Para obter informações sobre como criar processos de aprovação e regras de roteamento, consulte os seguintes artigos:

   * [Criar um processo de aprovação para itens de trabalho](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md)
   * [Criar Regras de Encaminhamento](../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md)

## Desativar uma função de trabalho

1. Clique em **[!UICONTROL Menu principal]** ícone ![](assets/main-menu-icon.png) no canto superior direito de [!DNL Adobe Workfront]e, em seguida, clique em **[!UICONTROL Configuração]** ![](assets/gear-icon-settings.png).

1. No painel esquerdo, clique em&#x200B; **[!UICONTROL Funções de trabalho].**
1. (Opcional) Na **[!UICONTROL Filtro]** selecione **[!UICONTROL Ativo]** para exibir apenas as funções de trabalho ativas.
1. Clique no nome da função de trabalho que deseja desativar.
1. No **[!UICONTROL Está ativo]** selecione **[!UICONTROL Não]**.

   ![](assets/deactivate-job-role-edit-role-box-nwe.png)

1. Clique em **[!UICONTROL Salvar alterações]**.

   A função de trabalho está desativada e não pode mais ser atribuída para trabalho, associada a modelos de layout e assim por diante. Para obter informações sobre todos os usos de funções de trabalho no [!DNL Workfront], consulte [Visão geral das funções de trabalho](../../../administration-and-setup/set-up-workfront/organizational-setup/job-role-overview.md).
