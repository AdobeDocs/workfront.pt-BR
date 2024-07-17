---
product-area: projects
navigation-topic: manage-tasks
title: Editar tarefas em uma lista
description: É possível editar as informações da tarefa em uma lista de tarefas editando os campos exibidos na lista. Para obter informações sobre outras maneiras de editar tarefas, consulte Editar tarefas.
author: Alina
feature: Work Management
exl-id: 2af81907-3657-459e-b780-65983e224ca8
source-git-commit: 1da2e6448f7ac6f4bd5bd76846fbfc1a23c3da77
workflow-type: tm+mt
source-wordcount: '2848'
ht-degree: 2%

---

# Editar tarefas em uma lista {#edit-tasks-in-a-list}

É possível editar as informações da tarefa em uma lista de tarefas editando os campos exibidos na lista. Para obter informações sobre outras maneiras de editar tarefas, consulte [Editar tarefas](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront*</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Trabalhar ou superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a tarefas e projetos</p> <p>Observação: se você ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode alterar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Contribute ou permissões mais altas para a tarefa e o projeto</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso aos objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qual plano, tipo de licença ou acesso você tem, contate o administrador do Workfront.

## Considerações sobre a edição de tarefas em uma lista {#considerations-about-editing-tasks-in-a-list}

Editar tarefas em uma lista é uma maneira rápida de fazer alterações em várias tarefas simultaneamente, com uma visão clara de como as alterações podem afetar a linha do tempo do projeto.

Leve em consideração o seguinte ao editar tarefas em uma lista:

* Ao contrário da necessidade de gerenciar permissões para a tarefa ao editá-la na caixa Editar, você pode editar uma tarefa em uma lista somente com permissões Contribute para a tarefa. Isso permite editar as seguintes informações limitadas para a tarefa:

   * Descrição
   * Status
   * Percentual concluído
   * Informações do formulário personalizado

     >[!NOTE]
     >
     >Você pode editar um campo personalizado de tarefa em uma lista somente se tiver permissões para atualizar o campo.

   * Registrar horas
   * Modificar Atribuições
   * Exibir informações financeiras
   * Adicionar despesas, tarefas ou problemas

* É possível editar uma tarefa nas seguintes listas:

   * A seção Tarefas do projeto
   * A seção Subtarefas do projeto
   * Um relatório de tarefa

     >[!NOTE]
     >
     >Por padrão, o Workfront salva automaticamente suas alterações em tarefas na seção Subtarefas ou em um relatório de tarefas.

* Você pode controlar quando o Workfront salva as alterações feitas nas tarefas em uma lista. Suas alterações podem ser salvas automaticamente ou manualmente.

  Para obter informações sobre como configurar quando o Workfront salva as alterações feitas nas tarefas de uma lista, consulte a seção [Selecionar uma opção de salvamento ao editar tarefas em uma lista](#select-a-save-option-when-editing-tasks-in-a-list) neste artigo.

* Outros usuários devem atualizar suas páginas antes de visualizarem as atualizações feitas em uma tarefa.

## Selecione uma opção para salvar ao editar tarefas em uma lista {#select-a-save-option-when-editing-tasks-in-a-list}

Você pode decidir onde as alterações feitas nas tarefas de uma lista são salvas automaticamente, à medida que ocorrem, ou se deseja salvar manualmente cada alteração.

>[!IMPORTANT]
>
>Dependendo de você salvar as tarefas automática ou manualmente, é possível substituir as informações de outra pessoa à medida que você edita tarefas em uma lista. Para obter informações sobre como o Workfront salva alterações em tarefas que você faz simultaneamente com outros usuários, consulte [Visão geral de como salvar alterações simultâneas em uma lista de tarefas](../../../manage-work/tasks/manage-tasks/save-concurrent-changes-in-a-task-list.md).

Quando você salva as alterações em uma lista de um projeto que tem Automático ou Automático e Ao alterar selecionado como o Tipo de atualização, o Workfront atualiza a linha do tempo do projeto, juntamente com todas as dependências no projeto e entre projetos. Os cálculos de linha de tempo podem levar muito tempo se o projeto for grande ou se houver muitas dependências. Alguns métodos de edição de uma lista de tarefas podem ser mais rápidos que outros, dependendo do método selecionado para salvar as alterações.

Você pode controlar quando o Workfront salva as alterações feitas nas tarefas em uma lista. Existem os seguintes cenários: 

* Você pode fazer com que o Workfront salve as alterações automaticamente após cada atualização.

  Para obter informações, consulte a seção [Editar tarefas em uma lista e salvar automaticamente as alterações](#edit-tasks-in-a-list-and-automatically-save-changes) neste artigo.

* É possível ter controle sobre quando você aplica várias alterações de uma vez usando manualmente um botão Salvar.

  Para obter informações, consulte a seção [Editar tarefas em uma lista e salvar manualmente as alterações](#edit-tasks-in-a-list-and-manually-save-changes) neste artigo.

### Editar tarefas em uma lista e salvar as alterações automaticamente {#edit-tasks-in-a-list-and-automatically-save-changes}

>[!TIP]
>
>Salvar as alterações e todas as dependências do projeto pode ser mais lento se o projeto tiver mais de 2000 tarefas ou se tiver muitas dependências.

Leve em consideração o seguinte ao salvar as alterações da lista de tarefas automaticamente:

* É possível aplicar uma visualização personalizada à lista de tarefas e editar quaisquer campos relacionados à tarefa que você tenha acesso para atualizar.
* Não é possível reverter as alterações salvas automaticamente. Esta é a configuração padrão.
* O Workfront recalcula a linha do tempo do projeto e todas as dependências entre projetos e no projeto automaticamente após cada alteração, quando o Tipo de atualização do projeto é Automático ou Automático e Mediante alteração. Para obter informações sobre o Tipo de Atualização do projeto, consulte [Selecionar o Tipo de Atualização do projeto](../../../manage-work/projects/manage-projects/select-project-update-type.md).

Para editar tarefas em uma lista e salvar alterações automaticamente:

1. Vá para o projeto e clique na seção **Tarefas**.
1. Clique no menu **Modo de plano** ![](assets/qs-list-mode-or-save-mode-icon-small.png) na parte superior da lista e verifique se a opção **Salvamento automático** está selecionada.

   ![](assets/autosave-setting-enabled-quicksilver-task-list-350x308.png)

1. Edite qualquer campo que você tenha permissões para atualizar manualmente.

   ![](assets/inline-editing-a-task-350x26.png)

1. (Opcional) Pressione **Escape** para cancelar suas alterações.
1. Pressione Enter para salvar as alterações nas tarefas e na linha do tempo do projeto.
1. (Opcional) Clique com o botão direito do mouse em uma tarefa que você deseja modificar.

   Ou

   Clique no menu ![](assets/more-icon-task-list.png) **Mais** à direita do nome da tarefa.

1. (Opcional) Selecione entre as seguintes opções:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Abrir em uma nova guia</strong></td> 
      <td>Abre a tarefa em uma nova guia do navegador. </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Editar</strong></td> 
      <td><p>Abre a caixa <strong>Editar Tarefa</strong>, onde você pode editar a tarefa.</p><p>Para obter informações sobre como editar uma tarefa, consulte <a href="#edit-tasks-in-a-list" class="MCXref xref">Editar tarefas em uma lista</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Excluir</td> 
      <td><p>Exclui a tarefa.</p><p>Para obter informações sobre como excluir tarefas, consulte <a href="../../../manage-work/tasks/manage-tasks/delete-tasks.md" class="MCXref xref">Excluir tarefas</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Aumentar Recuo</td> 
      <td><p>Recua a tarefa em um nível. </p><p>Essa opção é exibida somente em tarefas independentes.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Diminuir recuo</td> 
      <td><p>Aplica recuo para a esquerda à tarefa em um nível. </p><p>Essa opção é exibida somente em tarefas filho. </p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Inserir tarefa acima</td> 
      <td>Insere uma tarefa acima da tarefa selecionada.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Inserir tarefa entre</td> 
      <td>Insere uma tarefa na tarefa selecionada</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Duplicar</td> 
      <td><p>Cria uma versão duplicada da tarefa no mesmo projeto. </p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Copiar para</td> 
      <td><p>Copia a tarefa para outro projeto.</p><p>Para obter informações sobre como copiar e duplicar tarefas, consulte <a href="../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md" class="MCXref xref">Copiar e duplicar tarefas</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Move Para</td> 
      <td><p>Move a tarefa para outro projeto.</p><p>Para obter informações sobre como mover tarefas, consulte <a href="../../../manage-work/tasks/manage-tasks/move-tasks.md" class="MCXref xref">Mover tarefas</a>.</p></td> 
     </tr> 
    </tbody> 
   </table>

   As alterações são salvas automaticamente e não podem ser revertidas.

### Editar tarefas em uma lista e salvar as alterações manualmente {#edit-tasks-in-a-list-and-manually-save-changes}

Você pode salvar manualmente as alterações feitas nas tarefas de uma lista. Ao salvar as alterações dessa maneira, você tem a flexibilidade de revertê-las antes de salvar.

>[!TIP]
>
>* Não é possível reverter as alterações feitas em tarefas em uma lista ao editá-las na seção Subtarefas ou em um relatório de tarefa.
>* Não há limitações no número de alterações que podem ser revertidas. É possível reverter todas elas uma por uma até atingir o estado original das tarefas.
>

Leve em consideração o seguinte ao salvar manualmente as alterações em uma lista de tarefas:

* Para salvar as alterações da lista de tarefas manualmente, você precisa de permissões para Gerenciar as tarefas e o projeto.
* Não é possível editar o projeto. A opção para editar o projeto está desativada.
* Não é possível atualizar as informações no cabeçalho do projeto. Você só pode fazer o seguinte ao salvar manualmente as alterações na lista de tarefas:

   * Inscreva-se no projeto.
   * Adicione o projeto à lista de favoritos.
   * Abra uma tarefa clicando no seu nome na lista.

* Edite as tarefas em massa. O ícone Editar é desativado ao selecionar várias tarefas.
* O Workfront aciona notificações sobre as alterações feitas nas tarefas somente após você salvar as alterações.

Há duas maneiras de salvar manualmente as alterações em tarefas de uma lista. Estas duas formas são descritas abaixo.

* [Salve as alterações manualmente em uma lista de tarefas ao selecionar a opção Salvar manualmente Padrão](#save-changes-in-a-task-list-manually-when-you-select-the-manual-save-standard-option)
* [Salvar as alterações em uma lista de tarefas manualmente ao selecionar a opção Salvar manualmente o planejamento de linha do tempo](#save-changes-in-a-task-list-manually-when-you-select-the-manual-save-timeline-planning-option)

#### Salvar alterações manualmente em uma lista de tarefas ao selecionar a opção Salvar manualmente Padrão {#save-changes-in-a-task-list-manually-when-you-select-the-manual-save-standard-option}

>[!TIP]
>
>Se o seu projeto tiver mais de 2000 tarefas, ou se tiver muitas dependências, pode demorar um pouco para identificar visualmente as alterações que você faz nas tarefas e como essas alterações afetam todas as dependências do projeto. Nesse caso, salvar as alterações pode levar mais tempo se o projeto tiver mais de 2000 tarefas ou se tiver muitas dependências.

Considere o seguinte ao atualizar tarefas em uma lista após selecionar a opção Salvar manualmente padrão:

* Aplique um modo de exibição personalizado à lista de tarefas e edite quaisquer campos relacionados à tarefa que você tenha permissões para Gerenciar nesse modo de exibição.
* O Workfront calcula a linha do tempo do projeto e todas as dependências entre projetos e no projeto depois de clicar em Salvar, quando o Tipo de atualização do projeto for Automático ou Automático e Mediante alteração. Para obter informações sobre o Tipo de Atualização do projeto, consulte [Selecionar o Tipo de Atualização do projeto](../../../manage-work/projects/manage-projects/select-project-update-type.md).

Para editar tarefas em uma lista ao selecionar a opção Salvar manualmente padrão:

1. Vá para um projeto e clique na seção **Tarefas**.
1. Clique no menu ![](assets/qs-list-mode-or-save-mode-icon-small.png) do **Modo do Plano** na parte superior da lista e selecione **Salvar manualmente** e clique em **Padrão** > **Aplicar**.

   ![](assets/manual-standard-setting-enabled-quicksilver-task-list-350x493.png)

   Uma configuração da barra de ferramentas é exibida com opções para desfazer, refazer e salvar as alterações.

   ![](assets/undo,-redo,-save,-and-cancel-widget-for-task-list-350x65.png)

1. Clique dentro de qualquer campo que você tenha permissões para atualizar manualmente. O campo se torna editável e você pode fazer suas alterações.

   ![](assets/inline-editing-a-task-350x26.png)

1. Pressione Enter para salvar temporariamente as alterações feitas.
1. (Opcional) Clique no **ícone Desfazer** ![](assets/undo-icon-on-task-list.png) para reverter uma alteração e retornar um campo ao seu estado original.
1. (Opcional e condicional) Clique no **ícone Refazer** ![](assets/redo-icon-on-task-list.png) para restaurar a alteração que você reverteu.

1. (Opcional) Clique com o botão direito do mouse em uma tarefa que deseja modificar.

   Ou

   Clique no menu ![](assets/more-icon-task-list.png) **Mais**.

1. (Opcional) Selecione entre as seguintes opções:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Abrir em uma nova guia</strong> </td> 
      <td>Abre a tarefa em uma nova guia do navegador. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Excluir</td> 
      <td>Para obter informações sobre como excluir tarefas, consulte <a href="../../../manage-work/tasks/manage-tasks/delete-tasks.md" class="MCXref xref">Excluir tarefas</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Aumentar Recuo</td> 
      <td> <p>Recua a tarefa em um nível. </p> <p>Essa opção é exibida somente em tarefas independentes.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Diminuir recuo</td> 
      <td> <p>Aplica recuo para a esquerda à tarefa em um nível. </p> <p>Essa opção é exibida somente em tarefas filho. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Inserir tarefa acima</td> 
      <td>Insere uma tarefa acima da tarefa selecionada.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Inserir tarefa entre</td> 
      <td>Insere uma tarefa na tarefa selecionada</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Duplicar</td> 
      <td> <p>Cria uma versão duplicada da tarefa no mesmo projeto. </p> <p>Para obter informações sobre como copiar e duplicar tarefas, consulte <a href="../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md" class="MCXref xref">Copiar e duplicar tarefas</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. O Workfront atualiza todas as dependências entre projetos e dentro de projetos ao fazer alterações na linha do tempo de tarefas.
1. Clique em **Salvar** quando quiser manter as alterações da tarefa permanentemente e salvar a linha do tempo do projeto.

#### Salvar as alterações em uma lista de tarefas manualmente ao selecionar a opção Salvar manualmente o planejamento de linha do tempo {#save-changes-in-a-task-list-manually-when-you-select-the-manual-save-timeline-planning-option}

Salvar as alterações e todas as dependências do projeto é mais rápido. Isso não está disponível para projetos com mais de 2000 tarefas.

>[!IMPORTANT]
>
>Recomendamos que você use essa opção ao editar uma grande lista de tarefas com mais de algumas centenas que tenham muitas dependências. Usar essa opção permite identificar visualmente as alterações com muito mais rapidez do que com a opção de salvamento manual.

Considere o seguinte ao usar a opção Planejamento de linha do tempo de salvamento manual em uma lista de tarefas:

* Não é possível aplicar a opção Planejamento de linha do tempo de salvamento manual a projetos com mais de 2000 tarefas.
* Não é possível aplicar um modo de exibição, filtro ou agrupamento personalizado à lista de tarefas. Os menus suspensos Exibição, Filtro e Agrupamento, bem como o ícone Exibição Agile, estão desativados. A exibição aplicada por padrão contém um número limitado de campos.
* A linha do tempo do projeto e todas as dependências no projeto são calculadas automaticamente após cada alteração quando o Tipo de atualização do projeto é Automático ou Automático e Mediante alteração.
* As dependências entre projetos são calculadas depois que você clica em Salvar, quando o Tipo de Atualização do projeto é Automático ou Automático e Mediante Alteração. Para obter informações sobre o Tipo de Atualização do projeto, consulte [Selecionar o Tipo de Atualização do projeto](../../../manage-work/projects/manage-projects/select-project-update-type.md).

Para editar tarefas em uma lista ao usar a opção Salvar manualmente o planejamento de linha do tempo:

1. Vá para um projeto e clique na seção **Tarefas**.
1. Clique no menu ![](assets/qs-list-mode-or-save-mode-icon-small.png) do **Modo de Plano** na parte superior da lista e selecione **Salvar manualmente** e clique em **Planejamento de Linha do Tempo**> **Aplicar**.

   Essa opção fica esmaecida para projetos com mais de 2000 tarefas.

   ![](assets/manual-timeline-planning-setting-enabled-quicksilver-task-list-350x490.png)

   >[!TIP]
   >
   >Ao sair desta página, o Workfront reativa a opção de Salvamento automático.

   Observe as seguintes alterações na lista:

   * Os menus suspensos Exibir, Agrupamento e Filtro são removidos e a exibição é substituída pelos seguintes campos:

      * Número da Tarefa
      * Nome da tarefa
      * Tipo de Restrição
      * Duração
      * Data de início planejado
      * Data de conclusão planejada
      * Predecessoras
      * Atribuições
      * Status
      * Percentual concluído

   * O ícone de visualização Agile é removido.
   * Uma configuração da barra de ferramentas é exibida com opções para desfazer, refazer e salvar as alterações.

     ![](assets/undo,-redo,-save,-and-cancel-widget-for-task-list-350x65.png)

1. Edite qualquer campo que você tenha permissões para atualizar manualmente.

   ![](assets/inline-editing-a-task-350x26.png)

1. Pressione Enter para salvar temporariamente as alterações feitas.
1. (Opcional) Clique no **ícone Desfazer** ![](assets/undo-icon-on-task-list.png) para reverter uma alteração e retornar um campo ao seu estado original.
1. (Opcional e condicional) Clique no **ícone Refazer** ![](assets/redo-icon-on-task-list.png) para restaurar a alteração que você reverteu.

1. (Opcional) Clique com o botão direito do mouse em uma tarefa que você deseja modificar

   Ou

   Clique no menu ![](assets/more-icon-task-list.png) **Mais**.

1. Selecione entre as seguintes opções:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Abrir em uma nova guia</strong> </td> 
      <td>Abre a tarefa em uma nova guia do navegador. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Excluir</td> 
      <td>Para obter informações sobre como excluir tarefas, consulte <a href="../../../manage-work/tasks/manage-tasks/delete-tasks.md" class="MCXref xref">Excluir tarefas</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Aumentar Recuo</td> 
      <td> <p>Recua a tarefa em um nível. </p> <p>Essa opção é exibida somente em tarefas independentes.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Diminuir recuo</td> 
      <td> <p>Aplica recuo para a esquerda à tarefa em um nível. </p> <p>Essa opção é exibida somente em tarefas filho. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Inserir tarefa acima</td> 
      <td>Insere uma tarefa acima da tarefa selecionada.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Inserir tarefa entre</td> 
      <td>Insere uma tarefa na tarefa selecionada</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Duplicar</td> 
      <td> <p>Cria uma versão duplicada da tarefa no mesmo projeto. </p> <p>Para obter informações sobre como copiar e duplicar tarefas, consulte <a href="../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md" class="MCXref xref">Copiar e duplicar tarefas</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. O Workfront atualiza todas as dependências entre projetos e no projeto ao alterar a linha do tempo de uma tarefa.
1. Clique em **Salvar** quando quiser manter as alterações da tarefa permanentemente e salvar a linha do tempo do projeto.

## Editar uma tarefa em uma lista usando o Resumo

1. Vá para o projeto que contém as tarefas que você deseja editar.
1. Clique em **Tarefas** no painel esquerdo.

   A lista de tarefas no projeto é exibida.

1. Clique no menu Mais ![](assets/more-icon-task-list.png) depois do nome da tarefa e em **Abrir Resumo**. Selecione a tarefa que deseja editar e clique no **ícone Abrir resumo** ![](assets/qs-open-summary-icon-in-new-toolbar-small.png), no canto superior direito da lista.

   O **Resumo** é aberto.

   ![](assets/qs-task-right-panel-in-a-task-list-350x328.png)

1. (Opcional) Clique no ícone **X** no canto superior direito do Resumo para fechar o painel e editar as tarefas em linha.

   Siga as etapas sobre como editar uma tarefa em uma lista para editar a tarefa em linha.

   Para obter informações sobre como editar a tarefa em uma lista, consulte [Considerações sobre como editar tarefas em uma lista](#considerations-about-editing-tasks-in-a-list) neste artigo.

1. (Opcional) Digite uma atualização para a tarefa na área **Atualizações**.
1. Clique em qualquer um dos ícones ou áreas a seguir para acessar a tarefa e editar as informações no nível da tarefa:

   | Documentos | Clique **Clique aqui para adicionar** para adicionar documentos à tarefa. |
   |---|---|
   | Detalhes | Clique em para atualizar as informações sobre a tarefa. |
   | Formulários personalizados | Clique em para adicionar ou remover o Forms personalizado ou atualizar as informações nos formulários. |
   | Horas | Clique para registrar horas. |
   | Aprovações | Clique em para adicionar aprovações de tarefas. |

   {style="table-layout:auto"}

1. Clique no botão Voltar do navegador para retornar à lista de tarefas quando terminar de atualizar a tarefa.

## Editar tarefas em massa

É possível editar várias tarefas de uma só vez. Verifique se você tem permissões de gerenciamento para as tarefas para poder editá-las.

1. Vá para um projeto que contenha tarefas que você deseja editar em massa.
1. Clique em **Tarefas** no painel esquerdo.
1. Verifique se a opção **Salvar automaticamente** está selecionada.

   >[!IMPORTANT]
   >
   >Não é possível editar tarefas em massa ao salvar tarefas manualmente.

   Para obter mais informações sobre como salvar alterações em tarefas de uma lista, consulte a seção [Considerações sobre a edição de tarefas em uma lista](#considerations-about-editing-tasks-in-a-list) neste artigo.

1. Selecione várias tarefas na lista de tarefas.
1. Clique no **ícone Editar** ![](assets/qs-edit-icon.png).

   A caixa de diálogo **Editar Tarefas** é aberta.

1. Especifique as informações que deseja alterar para todas as tarefas selecionadas.

   A edição de informações em todas as tarefas é idêntica à edição de informações em uma tarefa. Se você quiser editar a Duração da tarefa, as tarefas selecionadas deverão ter a mesma Restrição de Tarefa; caso contrário, o campo **Duração** não será preenchido.

   Para obter mais informações sobre como editar uma tarefa, consulte [Editar tarefas](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

   >[!NOTE]
   >
   >As informações que você está alterando em todas as tarefas selecionadas substituirão as informações existentes em tarefas individuais, exceto pelo campo **Atribuições**. Adicionar um novo destinatário na edição em massa adicionará este destinatário a todas as tarefas selecionadas. Se outros atribuídos forem atribuídos às tarefas selecionadas, eles permanecerão atribuídos, além daquele adicionado por meio da edição em massa.

1. Clique em **Forms Personalizado** para editar os formulários personalizados anexados a todas as tarefas selecionadas. Somente formulários personalizados ativos são exibidos na lista.

   Se as tarefas selecionadas não tiverem formulários personalizados comuns, nenhum formulário será listado nesta seção.

   É possível editar apenas os campos nos formulários que estão anexados a todas as tarefas selecionadas e que você tem permissão para editar.

1. (Opcional) Na seção Forms Personalizado, selecione a opção **Recalcular Expressões Personalizadas** para garantir que todos os Campos Personalizados Calculados que estão nos formulários personalizados anexados às tarefas selecionadas estejam atualizados.
1. Clique em **Salvar alterações**.

   Todas as alterações feitas agora estão visíveis em todas as tarefas selecionadas.

Para obter informações sobre a edição de formulários personalizados em massa, consulte a seção &quot;Editar vários Forms personalizados ao editar objetos em massa&quot; em [Gerenciar formulários personalizados anexados a objetos](../../../workfront-basics/work-with-custom-forms/manage-custom-forms-attached-to-objects.md).
