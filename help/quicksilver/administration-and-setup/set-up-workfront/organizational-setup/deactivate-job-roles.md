---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: organization-setup
title: Desativar Funções
description: Como administrador [!DNL Adobe Workfront] ou usuário com acesso administrativo a Funções de Trabalho, você pode desativar funções de trabalho que se tornam obsoletas no sistema. Ao desativar uma função de trabalho em vez de excluí-la, você pode manter todas as informações históricas associadas a ela.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 934cef1a-8157-45db-b000-24a08a94dd18
source-git-commit: 15063d937a5ba9b5285c66a0987e8deea6cc6d74
workflow-type: tm+mt
source-wordcount: '643'
ht-degree: 1%

---

# Desativar funções de trabalho

Como administrador do [!DNL Adobe Workfront] ou usuário com acesso administrativo às Funções de Trabalho, você pode desativar funções de trabalho que se tornam obsoletas no sistema. Ao desativar uma função de trabalho em vez de excluí-la, você pode manter todas as informações históricas associadas a ela.

Você também pode reativar funções de trabalho que foram desativadas anteriormente.

## Requisitos de acesso

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] pacote</td> 
   <td><p>Qualquer</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] licença</td> 
   <td><p>[!UICONTROL Padrão]</p>
       <p>[!UICONTROL Plano]</p></td>
  </tr> 
  <tr> 
   <td>Configurações de nível de acesso</td> 
   <td>Acesso administrativo a Funções de trabalho</td>
  </tr> 
 </tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

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

{{step-1-to-setup}}

1. No painel esquerdo, clique em&#x200B; **[!UICONTROL Funções de trabalho].**
1. (Opcional) No menu suspenso **[!UICONTROL Filtro]**, selecione **[!UICONTROL Ativo]** para exibir somente as funções de trabalho ativas.
1. Clique no nome da função de trabalho que deseja desativar.
1. No menu suspenso **[!UICONTROL Está ativo]**, selecione **[!UICONTROL Não]**.

   ![Desativar função de trabalho](assets/deactivate-job-role-edit-role-box-nwe.png)

1. Clique em **[!UICONTROL Salvar alterações]**.

   A função de trabalho está desativada e não pode mais ser atribuída para trabalho, associada a modelos de layout e assim por diante. Para obter informações sobre todos os usos de funções de trabalho em [!DNL Workfront], consulte [Visão geral da função de trabalho](../../../administration-and-setup/set-up-workfront/organizational-setup/job-role-overview.md).
