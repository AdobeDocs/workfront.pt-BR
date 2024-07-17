---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: organization-setup
title: Desativar funções de trabalho
description: Como administrador [!DNL Adobe Workfront] ou usuário com acesso administrativo a Funções de Trabalho, você pode desativar funções de trabalho que se tornam obsoletas no sistema. Ao desativar uma função de trabalho em vez de excluí-la, você pode manter todas as informações históricas associadas a ela.
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

Como administrador do [!DNL Adobe Workfront] ou usuário com acesso administrativo às Funções de Trabalho, você pode desativar funções de trabalho que se tornam obsoletas no sistema. Ao desativar uma função de trabalho em vez de excluí-la, você pode manter todas as informações históricas associadas a ela.

Você também pode reativar funções de trabalho que foram desativadas anteriormente.

## Requisitos de acesso

Você deve ter o seguinte:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plano [!UICONTROL Adobe Workfront]*</td> 
   <td> <p>Qualquer </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da [!UICONTROL Adobe Workfront]*</td> 
   <td>[!UICONTROL Plano]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Acesso administrativo a funções de trabalho</p> <p><b>OBSERVAÇÃO</b>: se você ainda não tiver acesso, pergunte ao administrador do [!DNL Workfront] se ele definiu restrições adicionais no seu nível de acesso. Para obter informações sobre como um administrador do [!DNL Workfront] pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qual plano, tipo de licença ou acesso você tem, contate o administrador do [!DNL Workfront].

## O impacto da desativação de funções de trabalho

Se você desativar uma função de trabalho, ela não será mais exibida nas seguintes áreas:

* O campo [!UICONTROL Atribuições] do tipo digitação antecipada (para tarefas, tarefas de modelo, problemas, aprovações e regras de roteamento)
* Os campos [!UICONTROL Atribuições] em listas e relatórios
* Perfis de usuário

  >[!NOTE]
  >
  >Quando você adiciona uma nova função a um usuário, uma função de trabalho desativada não é exibida. Mas ele continua a ser exibido nos campos [!UICONTROL Função principal] e [!UICONTROL Outras funções] se o usuário tiver sido associado à função de trabalho antes de ser desativado.

* A caixa de diálogo [!UICONTROL Compartilhamento] para objetos, incluindo atribuição de modelo de layout
* Campos de digitação antecipada em formulários personalizados
* O campo [!UICONTROL Membros do Pool] em [!UICONTROL Pools de Recursos]
* O campo [!UICONTROL Função de trabalho] de uma tela de edição [!UICONTROL Taxa de Cobrança] quando um usuário substitui taxas de cobrança para projetos
* A caixa de diálogo [!UICONTROL Adicionar atribuição ao Quadro Kanban] em um projeto
* O campo [!UICONTROL Função de Trabalho] de um plano ou iniciativa quando alguém estiver usando o [!DNL Adobe Workfront Scenario Planner].

  O [!DNL Scenario Planner] está disponível somente na nova experiência do [!DNL Adobe Workfront] e requer uma licença adicional. Para obter informações sobre [!DNL Workfront Scenario Planner], consulte [A [!DNL Scenario Planner] visão geral](../../../scenario-planner/scenario-planner-overview.md).

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

1. Clique no ícone ![](assets/main-menu-icon.png) do **[!UICONTROL Menu Principal]** no canto superior direito de [!DNL Adobe Workfront] e em **[!UICONTROL Configurar]** ![](assets/gear-icon-settings.png).

1. No painel esquerdo, clique em&#x200B; **[!UICONTROL Funções de trabalho].**
1. (Opcional) No menu suspenso **[!UICONTROL Filtro]**, selecione **[!UICONTROL Ativo]** para exibir somente as funções de trabalho ativas.
1. Clique no nome da função de trabalho que deseja desativar.
1. No menu suspenso **[!UICONTROL Está ativo]**, selecione **[!UICONTROL Não]**.

   ![](assets/deactivate-job-role-edit-role-box-nwe.png)

1. Clique em **[!UICONTROL Salvar alterações]**.

   A função de trabalho está desativada e não pode mais ser atribuída para trabalho, associada a modelos de layout e assim por diante. Para obter informações sobre todos os usos de funções de trabalho em [!DNL Workfront], consulte [Visão geral da função de trabalho](../../../administration-and-setup/set-up-workfront/organizational-setup/job-role-overview.md).
