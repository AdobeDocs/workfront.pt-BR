---
product-area: projects
navigation-topic: convert-issues
title: Converter um problema em uma tarefa
description: Se for necessário trabalhar mais para concluir um problema depois que ele for enviado, você poderá converter o problema em uma tarefa no Adobe Workfront.
author: Alina
feature: Work Management
exl-id: 9d8e50ab-9fed-4ded-83e1-29dc92c37171
source-git-commit: cd0214917620e0b147d0da3402ea2d34e28bc9c3
workflow-type: tm+mt
source-wordcount: '1043'
ht-degree: 1%

---

# Converter um problema em uma tarefa

<!--Audited: 08/2025-->

Se for necessário trabalhar mais para concluir um problema depois que ele for enviado, você poderá converter o problema em uma tarefa no Adobe Workfront.

Para obter informações gerais sobre a conversão de problemas, consulte [Visão geral da conversão de problemas no Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md).

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacote do Adobe Workfront</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td> <p>Standard</p>
   <p>Trabalhar ou superior</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Editar acesso a Problemas, Tarefas e Projetos</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Exibir permissões para o problema</p> <p>Contribuir com permissões para o projeto</p> <p>Você obtém permissões Gerenciar para a tarefa depois que o problema é convertido</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


<!--Old:
<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Work or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Issues, Tasks, and Projects</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View permissions to the issue</p> <p>Contribute permissions to the project</p> <p>You obtain&nbsp;Manage permissions to the task after the issue is converted</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table> -->

## Considerações

* Há um limite de processamento de 5 minutos ao converter um problema em uma tarefa. Se o problema tiver um grande número de documentos anexados a ele e não for convertido, talvez seja necessário remover alguns dos documentos e tentar novamente.

## Converter um problema em uma tarefa

1. Vá para um projeto e clique em [!UICONTROL **Problemas**] no painel esquerdo.
1. Clique no problema que deseja converter para ir para a página de aterrissagem do problema.
1. Clique no menu [!UICONTROL **Mais**] sobre o problema e em [!UICONTROL **Converter em Tarefa**].

   ![Menu Emitir Mais](assets/qs-issue-more-menu-highlighted-350x469.png)

   >[!TIP]
   >
   >Se o problema estiver associado a um processo de aprovação ou já estiver associado a um objeto de resolução, o Workfront exibirá um aviso na parte superior da caixa [!UICONTROL Converter em Projeto] para notificá-lo de que a aprovação foi removida ou de que o objeto de resolução foi substituído durante a conversão. Para obter mais informações, consulte [Visão geral da conversão de problemas no Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md).

1. Atualize o nome da tarefa na seção [!UICONTROL Nome da Tarefa]. Por padrão, o nome da tarefa será igual ao do problema original.

   ![Converter em caixa de tarefa](assets/convert-to-task-box-nwe.png)

1. Clique em [!UICONTROL **Projeto de destino**] e comece a digitar o nome do projeto no qual você deseja colocar a nova tarefa no campo [!UICONTROL **Projeto de destino**] e selecione-o quando ele for exibido na lista. O projeto do problema é selecionado por padrão.

1. Clique em [!UICONTROL **Visão geral**] e digite uma [!UICONTROL **Descrição**] para a tarefa.

   >[!TIP]
   >
   >   Um administrador de sistema ou de grupo pode alterar a ordem das seções no painel esquerdo da caixa de conversão modificando seu modelo de layout.

1. (Opcional e condicional) Clique em [!UICONTROL **Opções**], selecione qualquer uma das opções abaixo.

   O administrador do Workfront ou o administrador de grupo deve ativar essas preferências antes que fiquem visíveis durante a conversão de problemas:

   * [!UICONTROL **Manter o problema original e vincular sua resolução a esta tarefa**]

     Se desmarcada, o problema original é excluído.

     >[!NOTE]
     >
     >Os usuários sem acesso ou permissões para excluir problemas não poderão excluir o problema como estão convertendo-o, independentemente do status dessa configuração. Para obter informações sobre acesso e permissões para problemas, consulte:
     >   
     >   * [Conceder acesso aos problemas](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md)
     >   * [Compartilhar um problema](../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md)
     >   
     >

   * [!UICONTROL **Permitir que (Nome de Usuário) tenha acesso a esta tarefa**]

     Se não estiver selecionada, o contato principal do problema não terá acesso à nova tarefa.

   * [!UICONTROL **Manter a data de conclusão planejada do problema**]

     Se desmarcada, a [!UICONTROL Data de conclusão planejada] da nova tarefa é calculada a partir da [!UICONTROL Data de início planejada] da tarefa. A [!UICONTROL Data de Início Planejada] da nova tarefa está definida de acordo com as preferências do sistema para novas tarefas.

     >[!NOTE]
     >
     >
     >As opções exibidas aqui dependem de como o administrador do Workfront as configurou para todos no sistema. Para obter mais informações, consulte [Configurar preferências de tarefas e problemas do sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).
     >
     >Ou, se os grupos de nível superior em sua organização os configurarem separadamente, as opções exibidas aqui dependerão de qual grupo está associado ao projeto selecionado na etapa 6. Para obter mais informações, consulte [Configurar preferências de tarefas e problemas para um grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

1. (Opcional) Clique em [!UICONTROL **Forms personalizado**] e anexe um formulário personalizado para a nova tarefa.

   >[!TIP]
   >
   >* Se um formulário personalizado de vários objetos anexado ao problema for configurado para uso com problemas e tarefas, todas as informações salvas no formulário serão mantidas quando você fizer a conversão, se os campos existirem tanto no problema quanto nos formulários personalizados da tarefa.
   >* Se um formulário personalizado de vários objetos com um campo calculado for anexado ao problema, bem como à tarefa, o problema e a tarefa deverão ser compatíveis com todos os campos referenciados nos campos personalizados calculados do formulário. Se houver uma incompatibilidade, uma mensagem o alertará para fazer ajustes. Para obter mais informações, consulte [Adicionar campos calculados a um formulário](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md).
   >* Se o projeto de destino tiver formulários padrão definidos no campo Forms personalizado padrão da tarefa ao editar o projeto, esses formulários de tarefa também serão adicionados à nova tarefa. Quaisquer campos personalizados comuns entre o problema original e os campos nos formulários de tarefa padrão são pré-preenchidos com informações dos campos de problema.


1. Clique em [!UICONTROL **Converter para tarefa**].

   O problema agora é uma tarefa no projeto designado, se você decidiu excluir o problema original.

   Ou

   O problema agora está vinculado à nova tarefa no projeto escolhido e será concluída quando a tarefa for concluída, se você decidir manter o problema original.

   Alguns campos de problema são transferidos para a tarefa. Para obter informações, consulte a seção [Exibir informações de problemas originais sobre projetos e tarefas](#view-original-issue-information-on-projects-and-tasks) neste artigo.

1. (Opcional) Continue editando a tarefa conforme necessário.

## Exibir informações de problemas originais em projetos e tarefas {#view-original-issue-information-on-projects-and-tasks}

Você pode exibir as informações do problema original em listas de projetos e tarefas e relatórios ou na área Detalhes do Projeto. Para obter informações sobre como criar relatórios, consulte [Criar um relatório personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

A tabela a seguir ilustra quais campos de problemas estão visíveis nas tarefas e nos projetos convertidos.

| Campos de problema | Campo de projeto ou tarefa | Lista ou relatório de projetos | Área Detalhes do projeto | Lista de tarefas ou relatório | Área Detalhes da tarefa |
|---|---|---|---|---|---|
| [!UICONTROL Nome do problema] | [!UICONTROL Nome do problema convertido] | ✔ | ✔ | ✔ | ✔ |
| [!UICONTROL Contato Primário] | [!UICONTROL Nome do Originador do Problema Convertido] | ✔ | ✔ | ✔ |  |
| [!UICONTROL Data de entrada] | [!UICONTROL Data de entrada do problema convertido] | ✔ |  | ✔ |  |


>[!CAUTION]
>
>Se o [!UICONTROL Contato Primário] de um problema for alterado ou se o problema se desvincular do projeto ou da tarefa após a conversão do problema, o [!UICONTROL Nome do Originador do Problema Convertido] não será atualizado e exibirá o [!UICONTROL Contato Primário] original do problema no momento em que ele foi convertido.
