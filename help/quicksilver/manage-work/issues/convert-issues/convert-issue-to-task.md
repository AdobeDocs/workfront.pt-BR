---
product-area: projects
navigation-topic: convert-issues
title: Converter um problema em uma tarefa no Adobe Workfront
description: Se precisar de mais trabalho para concluir um problema após o envio, é possível converter o problema em uma tarefa.
author: Alina
feature: Work Management
exl-id: 9d8e50ab-9fed-4ded-83e1-29dc92c37171
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '966'
ht-degree: 2%

---

# Converter um problema em uma tarefa no Adobe Workfront

Se precisar de mais trabalho para concluir um problema após o envio, é possível converter o problema em uma tarefa.

Para obter informações gerais sobre conversão de problemas, consulte [Visão geral da conversão de problemas no Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md).

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plano Adobe Workfront*</td> 
   <td> <p>Qualquer Um</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Trabalho ou superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a ocorrências, tarefas e projetos</p> <p>Observação: Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode alterar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Exibir permissões para o problema</p> <p>Contribuir com permissões para o projeto</p> <p>Você obtém permissões de Gerenciar para a tarefa após a conversão do problema</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

## Converter um problema em uma tarefa

1. Vá para um projeto e clique em [!UICONTROL **Problemas** ] no painel esquerdo.
1. Clique no problema que deseja converter para ir para a página de aterrissagem do problema.
1. Clique no botão [!UICONTROL **Mais**] no problema, em seguida [!UICONTROL **Converter em Tarefa**].

   ![](assets/qs-issue-more-menu-highlighted-350x469.png)

   >[!TIP]
   >
   >Se o problema estiver associado a um processo de aprovação ou já estiver associado a um objeto de resolução, o Workfront exibirá um aviso na parte superior do [!UICONTROL Converter em projeto] para notificá-lo de que a aprovação foi removida ou o objeto resolvedor foi substituído durante a conversão. Para obter mais informações, consulte [Visão geral da conversão de problemas no Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md).

1. Atualize o nome da tarefa no [!UICONTROL Nome da tarefa] seção. Por padrão, o nome da tarefa terá o mesmo nome do problema original.

   ![](assets/convert-to-task-box-nwe.png)

1. Clique em [!UICONTROL **Projeto de destino**], comece digitando o nome do projeto onde deseja colocar a nova tarefa na [!UICONTROL **Projeto de destino**] e selecione-o quando for exibido na lista. O projeto do problema é selecionado por padrão.

1. Clique em [!UICONTROL **Visão geral**] e digite a [!UICONTROL **Descrição**] para a tarefa.

   >[!TIP]
   >
   >   Um administrador de sistema ou de grupo pode alterar a ordem das seções no painel esquerdo da caixa de conversão modificando seu modelo de layout.

1. (Opcional e condicional) Clique em [!UICONTROL **Opções**] selecione qualquer uma das opções abaixo.

   O administrador do Workfront ou o administrador do grupo deve ativar essas preferências antes que elas fiquem visíveis durante a conversão dos problemas:

   * [!UICONTROL **Manter o problema original e vincular a resolução a esta tarefa**]

      Se não estiver selecionado, o problema original será excluído.

      >[!NOTE]
      >
      >Os usuários sem acesso ou permissões para excluir problemas não poderão excluir o problema à medida que o convertem, independentemente do status dessa configuração. Para obter informações sobre acesso e permissões para problemas, consulte:
      >   
      >   * [Conceder acesso a problemas](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md)
      >   * [Compartilhar um problema](../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md)


   * [!UICONTROL **Permitir que (Nome de Utilizador) tenha acesso a esta tarefa**]

      Se não estiver selecionado, o Contato Principal do problema não terá acesso à nova tarefa.

   * [!UICONTROL **Manter a data de conclusão planejada do problema**]

      Se não estiver selecionado, a variável [!UICONTROL Data de Conclusão Planejada] da nova tarefa é calculada a partir do [!UICONTROL Data de início planejada] da tarefa. O [!UICONTROL Data de início planejada] da nova tarefa é definida de acordo com as preferências do sistema para novas tarefas.

      >[!NOTE]
      >
      >
      >As opções exibidas aqui dependem de como o administrador do Workfront as configurou para todos no sistema. Para obter mais informações, consulte [Configurar preferências de emissão e tarefa em todo o sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).
      >
      >Ou, se os grupos de nível superior em sua organização os configurarem separadamente, as opções exibidas aqui dependerão de qual grupo está associado ao projeto selecionado na etapa 6. Para obter mais informações, consulte [Configurar preferências de tarefa e emissão para um grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

1. (Opcional) Clique em [!UICONTROL **Forms personalizada**] e anexe um formulário personalizado para a nova tarefa.

   >[!TIP]
   >
   >Se um formulário personalizado de vários objetos anexado ao problema for configurado para uso com problemas e tarefas, o formulário será anexado por padrão. Todas as informações salvas no formulário de problema são retidas para a tarefa ao fazer a conversão.
   >
   >Se o projeto de destino tiver qualquer formulário padrão definido no campo Forms Personalizado da Tarefa ao editar o projeto, esses formulários de tarefa também serão adicionados à nova tarefa. Todos os campos personalizados que são comuns entre a edição original e os campos nos formulários de tarefa padrão são preenchidos previamente com informações dos campos de edição.

1. Clique em [!UICONTROL **Converter em tarefa**].

   O problema agora é uma tarefa no projeto designado, se você decidir excluir o problema original.

   Ou

   O problema agora está vinculado à nova tarefa no projeto escolhido e será concluído assim que a tarefa for concluída, se você decidir manter o problema original.

   Alguns campos de emissão são transferidos para a tarefa. Para obter informações, consulte o [Exibir informações de edição original sobre projetos e tarefas](#view-original-issue-information-on-projects-and-tasks) neste artigo.

1. (Opcional) Continue editando a tarefa conforme necessário.

## Exibir informações de edição original sobre projetos e tarefas {#view-original-issue-information-on-projects-and-tasks}

Você pode exibir as informações do problema original em listas e relatórios de projeto e tarefa ou na área Detalhes do projeto . Para obter informações sobre como criar relatórios, consulte [Criar um relatório personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

A tabela a seguir ilustra quais campos de edição são visíveis nos projetos e tarefas convertidos.

| Campos de emissão | Campo Projeto ou tarefa | Lista ou relatório de projetos | Área Detalhes do projeto | Lista de tarefas ou relatório | Área Detalhes da tarefa |
|---|---|---|---|---|---|
| [!UICONTROL Nome do Problema] | [!UICONTROL Nome do problema convertido] | ✔ | ✔ | ✔ | ✔ |
| [!UICONTROL Contato Primário] | [!UICONTROL Nome do Originador da Emissão Convertido] | ✔ | ✔ | ✔ |
| [!UICONTROL Data de Entrada] | [!UICONTROL Data de entrada do problema convertido] | ✔ |  | ✔ |


>[!CAUTION]
>
>Se a variável [!UICONTROL Contato Principal] de um problema for alterado ou se o problema se tornar desvinculado do projeto ou tarefa após a conversão do problema, a variável [!UICONTROL Nome do Originador da Emissão Convertido ]não é atualizado e exibe o original [!UICONTROL Contato Principal] do problema no momento em que o problema foi convertido.
