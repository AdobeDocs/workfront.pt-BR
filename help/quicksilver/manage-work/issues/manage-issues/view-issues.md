---
product-area: projects
navigation-topic: manage-issues
title: Exibir problemas
description: Você pode exibir problemas associados a um projeto, tarefa ou iteração.
author: Alina
feature: Work Management
exl-id: b6791c8f-b356-4235-8b0e-952e29a88952
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '1038'
ht-degree: 0%

---

# Exibir problemas

Você pode exibir problemas associados a um projeto, tarefa ou iteração.

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
   <td> <p>Solicitação ou superior</p> <p>Revise a licença ou uma licença superior para exibir os problemas na seção Problemas de um projeto.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Visualizar acesso a problemas</p> <p>Visualizar ou aumentar o acesso a Projetos e Tarefas</p> <p>Observação: Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre o acesso a problemas no Nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">Conceder acesso a problemas</a>. Para obter informações sobre como um administrador do Workfront pode alterar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Exibir permissões para o problema</p> <p> Para obter informações sobre a concessão de permissões para problemas, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Compartilhar um problema </a></p> <p>Para obter informações sobre a solicitação de permissões adicionais, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

## Exibir problemas com base no Status

Para exibir problemas em um projeto, tarefa ou iteração:

1. Abra um projeto, tarefa ou iteração que contenha problemas e clique em **Problemas** no painel esquerdo.

1. Para exibir todos os problemas, abrir ou fechar, clique em qualquer um dos filtros listados abaixo do **Filtro** menu suspenso.

>[!TIP]
>
>A lista de filtros varia dependendo do sistema ou do administrador de grupo selecionado para exibição nela.

* **Abrir:** Exibe os problemas que estão abertos.

   Isso inclui aqueles associados a um Objeto de Resolução e aqueles em um status Fechado - Aprovação Pendente .

   Para obter informações sobre como resolver objetos, consulte [Visão Geral da Solução e Objetos Resolvíveis](../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md).

* **Concluído:** Exibe todos os problemas que têm uma Data de Conclusão Real.
* **Todos** Exibe todos os problemas.

## Entender informações sobre problemas

Você pode exibir informações sobre um problema ao acessá-lo.

Para acessar um problema e exibir informações sobre ele:

1. Abra um projeto, tarefa ou iteração que contenha problemas e clique em **Problemas** no painel esquerdo.
1. No **Filtro** no menu suspenso , selecione o filtro para exibir os problemas que você está tentando visualizar.

   Selecione uma das opções a seguir:

   * Aberto
   * Concluídos
   * Todas

1. Clique no nome de um problema.

   Quando você tem permissões de gerenciamento para o problema, pode editar qualquer campo editável no problema e adicionar aprovações, horas ou documentos ao problema.

1. No painel esquerdo, clique em qualquer um dos itens a seguir para exibir mais informações sobre o problema:

* **Atualizações**: Você pode executar as seguintes ações :

   * Comente o problema ou responda a um comentário existente.
   * Hora do registro.
   * Altere o status do problema.

      Para obter mais informações sobre como atualizar o trabalho no Workfront, consulte [Atualizar trabalho](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

* **Documentos**: Anexe documentos ao problema. Para obter mais informações sobre como adicionar documentos ao Workfront, consulte [Adicionar documentos ao Adobe Workfront a partir do seu sistema de arquivos](../../../documents/adding-documents-to-workfront/add-documents-from-file-system.md).

* **Detalhes do problema**: Expanda este link para exibir a variável **Visão geral** e **Forms personalizada** áreas.

   Se você tiver permissões de gerenciamento para o problema e direitos de edição no formulário personalizado, poderá editar algumas informações aqui.

   Exiba ou edite os seguintes campos na **Visão geral** Área:

   * **Nome**
   * **Caminho**: o caminho pelo qual o problema foi registrado no projeto.

      Se um problema foi enviado como uma solicitação em uma fila de solicitações, os nomes do projeto, do Grupo de tópicos e do Tópico da fila são listados aqui. Este campo não pode ser editado.

      Para obter mais informações sobre como enviar solicitações, consulte [Criar e enviar solicitações do Adobe Workfront](../../../manage-work/requests/create-requests/create-submit-requests.md).

   * **Descrição**
   * **URL**: qualquer endereço da Web relacionado ao problema.
   * **Prioridade**: um sinalizador visual que permite priorizar problemas.
   * **Gravidade**: um sinalizador visual que indica a gravidade do problema descrito no problema.
   * **Contato Principal**: o contato principal padrão é o usuário que criou o problema. Este campo pode ser editado.
   * **Horas Planejadas**: exibe o tempo que levará alguém para concluir o problema. O padrão é 8 horas. Este campo pode ser editado.
   * **Horas reais**: exibe o tempo necessário para concluir o problema. Este é o momento em que alguém faz o login para o problema.
   * **Data de início planejada**: a data em que o problema está planejado para iniciar. O padrão é a data e a hora em que o problema foi criado.
   * **Data de início real**: a data e a hora em que o status da emissão foi alterado para Em andamento.
   * **Data de Conclusão Planejada**: A data em que a emissão está planejada para ser concluída.
   * **Data de conclusão real**: a data em que o problema está realmente concluído. Este campo é preenchido automaticamente quando o status do problema é alterado para Fechado ou Resolvido, ou pode ser editado manualmente.
   * **Custo real**: o custo com base nas Horas reais registradas no problema. Este campo não é editável. O Custo Real de uma emissão é calculado com base na seguinte fórmula, em que a Taxa de Custo do Usuário é a taxa de custo associada ao usuário registrando o tempo para a emissão:

      Emitir Custo Real = Horas Registradas * Taxa de Custo do Usuário

   * **Inserido por**: esse é o usuário que criou o problema. Este campo não é editável.
   * **Última atualização de**: este é o usuário que atualizou qualquer campo sobre o problema por último. Este campo não é editável.

      No **Forms personalizada** área , exibição de selecione um ou vários formulários personalizados para associar ao problema.

* **Horas**: Mostra uma lista de entradas de hora no problema.
* **Aprovações:** Mostra os caminhos de aprovação associados ao problema.

   Para obter mais informações sobre como associar aprovações a uma emissão, consulte o [Associar um processo de aprovação a um item de trabalho](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md#associating-the-approval-process-with-an-object) seção em [Criar um processo de aprovação para itens de trabalho](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

## Exibir quais projetos e tarefas têm problemas

É possível adicionar ícones na exibição de um projeto, relatório de tarefa ou lista para mostrar se eles têm problemas anexados. Adicionar ícones à exibição de um relatório ou lista é semelhante para projetos e tarefas.

Para adicionar ícones que exibem se um projeto tem problemas em um relatório de projeto:

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront.
1. Clique em **Relatório** > **Novo relatório** > **Relatório de projeto**.
1. No **Mostrar nesta coluna** , comece a digitar **Ícones de status** e, em seguida, selecione-a quando ela for exibida na lista.

1. Clique em **Salvar + Fechar** .

   Os ícones de problema são exibidos nos projetos que têm problemas na variável **Ícones de status** coluna.

   ![project_list_with_issue_icon.png](assets/project-list-with-issue-icon-350x132.png)
