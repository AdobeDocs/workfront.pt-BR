---
product-area: projects
navigation-topic: manage-tasks
title: Editar tarefas em uma lista
description: É possível editar as informações da tarefa em uma lista de tarefas editando os campos exibidos na lista. Para obter informações sobre outras maneiras de editar tarefas, consulte Editar tarefas.
author: Alina
feature: Work Management
exl-id: 2af81907-3657-459e-b780-65983e224ca8
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '2828'
ht-degree: 2%

---

# Editar tarefas em uma lista {#edit-tasks-in-a-list}

É possível editar as informações da tarefa em uma lista de tarefas editando os campos exibidos na lista. Para obter informações sobre outras maneiras de editar tarefas, consulte [Editar tarefas](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

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
   <td> <p>Editar acesso a Tarefas e Projetos</p> <p>Observação: Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode alterar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Contribuir com permissões ou permissões mais altas para a tarefa e o projeto</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

## Considerações sobre edição de tarefas em uma lista {#considerations-about-editing-tasks-in-a-list}

Editar tarefas em uma lista é uma maneira rápida de fazer alterações em várias tarefas simultaneamente, com uma exibição clara de como suas alterações podem afetar a linha do tempo do projeto.

Considere o seguinte ao editar tarefas em uma lista:

* Ao contrário da necessidade de permissões de gerenciamento para a tarefa ao editá-la na Caixa de edição, é possível editar uma tarefa em uma lista somente com permissões do Contribute para a tarefa. Isso permite editar as seguintes informações limitadas para a tarefa:

   * Descrição
   * Status
   * Percentual concluído
   * Informações do formulário personalizado

      >[!NOTE]
      >
      >É possível editar um campo personalizado de tarefa em uma lista somente se você tiver permissões para atualizar o campo.

   * Horas de registro
   * Modificar Atribuições
   * Exibir informações financeiras
   * Adicionar despesas, tarefas ou problemas

* É possível editar uma tarefa nas seguintes listas:

   * A seção Tarefas do projeto
   * A seção Subtarefas do projeto
   * Um relatório de tarefas

      >[!NOTE]
      >
      >Por padrão, o Workfront salva automaticamente as alterações nas tarefas na seção Subtarefas ou em um relatório de tarefa.

* Você pode controlar quando o Workfront salva as alterações feitas nas tarefas em uma lista. As alterações podem ser salvas automaticamente ou manualmente.

   Para obter informações sobre como configurar quando o Workfront salva as alterações feitas em tarefas em uma lista, consulte o [Selecionar uma opção de salvar ao editar tarefas em uma lista](#select-a-save-option-when-editing-tasks-in-a-list) neste artigo.

## Selecionar uma opção de salvar ao editar tarefas em uma lista {#select-a-save-option-when-editing-tasks-in-a-list}

Você pode decidir onde as alterações feitas nas tarefas de uma lista são salvas automaticamente, à medida que ocorrem, ou se deseja salvar manualmente cada alteração.

>[!IMPORTANT]
>
>Dependendo de as tarefas serem salvas automática ou manualmente, você pode substituir as informações de outra pessoa enquanto edita tarefas em uma lista. Para obter informações sobre como o Workfront salva alterações em tarefas realizadas simultaneamente com outros usuários, consulte [Visão geral de salvar alterações simultâneas em uma lista de tarefas](../../../manage-work/tasks/manage-tasks/save-concurrent-changes-in-a-task-list.md).

Ao salvar suas alterações em uma lista de um projeto que tenha as opções Automático ou Automático e On Change selecionadas como Tipo de atualização, o Workfront atualiza a linha do tempo do projeto, juntamente com todas as dependências dentro do projeto e entre projetos. Os cálculos da linha do tempo podem levar muito tempo se o projeto for grande ou se houver muitas dependências. Alguns métodos de edição de uma lista de tarefas podem ser mais rápidos que outros, dependendo do método selecionado para salvar suas alterações.

Você pode controlar quando o Workfront salva as alterações feitas nas tarefas em uma lista. Os seguintes cenários existem: 

* Depois de cada atualização, o Workfront pode salvar as alterações automaticamente.

   Para obter mais informações, consulte a seção [Editar tarefas em uma lista e salvar automaticamente as alterações](#edit-tasks-in-a-list-and-automatically-save-changes) neste artigo.

* Você pode ter controle sobre quando aplicar várias alterações de cada vez usando manualmente um botão Salvar.

   Para obter mais informações, consulte a seção [Editar tarefas em uma lista e salvar manualmente as alterações](#edit-tasks-in-a-list-and-manually-save-changes) neste artigo.

### Editar tarefas em uma lista e salvar automaticamente as alterações {#edit-tasks-in-a-list-and-automatically-save-changes}

>[!TIP]
>
>Salvar as alterações e todas as dependências do projeto podem ser mais lentas se o projeto tiver mais de 2000 tarefas ou se tiver muitas dependências.

Considere o seguinte ao salvar as alterações da lista de tarefas automaticamente:

* Você pode aplicar uma exibição personalizada à lista de tarefas e editar quaisquer campos relacionados a tarefas aos quais tenha acesso para atualizar.
* Não é possível reverter as alterações salvas automaticamente. Esta é a configuração padrão.
* O Workfront recalcula a linha do tempo do projeto e todas as dependências entre projetos e dentro do projeto automaticamente após cada alteração, quando o Tipo de atualização do projeto é Automático ou Automático e On Change. Para obter informações sobre o Tipo de Atualização do projeto, consulte [Selecione o Tipo de Atualização do projeto](../../../manage-work/projects/manage-projects/select-project-update-type.md).

Para editar tarefas em uma lista e salvar as alterações automaticamente:

1. Vá para o projeto e clique no botão **Tarefas** seção.
1. Clique no botão **Menu Modo de plano** ![](assets/qs-list-mode-or-save-mode-icon-small.png) na parte superior da lista e verifique se a variável **Salvar automaticamente** está selecionada.

   ![](assets/autosave-setting-enabled-quicksilver-task-list-350x308.png)

1. Edite qualquer campo com permissões para atualizar manualmente.

   ![](assets/inline-editing-a-task-350x26.png)

1. (Opcional) Pressione **Escape** para cancelar as alterações.
1. Pressione Enter para salvar as alterações nas tarefas e na linha do tempo do projeto.
1. (Opcional) Clique com o botão direito do mouse em uma tarefa que deseja modificar.

   Ou

   Clique no botão **Mais** menu ![](assets/more-icon-task-list.png) à direita do nome da tarefa.

1. (Opcional) Selecione uma das seguintes opções:

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
      <td><p>Abre a variável <strong>Editar tarefa</strong> , onde é possível editar a tarefa.</p><p>Para obter informações sobre como editar uma tarefa, consulte <a href="#edit-tasks-in-a-list" class="MCXref xref">Editar tarefas em uma lista</a>.</p></td> 
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
      <td><p>Ultrapassa a tarefa em um nível. </p><p>Essa opção é exibida somente em tarefas secundárias. </p></td> 
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
      <td><p>Copia a tarefa para outro projeto.</p><p>Para obter informações sobre cópia e duplicação de tarefas, consulte <a href="../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md" class="MCXref xref">Copiar e duplicar tarefas</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Move Para</td> 
      <td><p>Move a tarefa para outro projeto.</p><p>Para obter informações sobre como mover tarefas, consulte <a href="../../../manage-work/tasks/manage-tasks/move-tasks.md" class="MCXref xref">Mover tarefas</a>.</p></td> 
     </tr> 
    </tbody> 
   </table>

   As alterações são salvas automaticamente e não é possível revertê-las.

### Editar tarefas em uma lista e salvar manualmente as alterações {#edit-tasks-in-a-list-and-manually-save-changes}

Você pode salvar manualmente as alterações feitas em tarefas em uma lista. Ao salvar as alterações dessa maneira, você tem a flexibilidade de revertê-las antes de salvar.

>[!TIP]
>
>* Não é possível reverter as alterações feitas em tarefas em uma lista ao editá-las na seção Subtarefas ou em um relatório de tarefa.
>* Não há limitações para quantas alterações você pode reverter. É possível reverter todos eles um por um até atingir o estado original das tarefas.
>


Considere o seguinte ao salvar as alterações em uma lista de tarefas manualmente:

* Para salvar as alterações da lista de tarefas manualmente, você precisa de permissões para gerenciar as tarefas e o projeto.
* Não é possível editar o projeto. A opção para editar o projeto está desativada.
* Não é possível atualizar informações no cabeçalho do projeto. Você só pode fazer o seguinte ao salvar manualmente as alterações na lista de tarefas:

   * Assine o projeto.
   * Adicione o projeto à lista de favoritos.
   * Abra uma tarefa clicando no seu nome na lista.

* Edite as tarefas em massa. O ícone Editar é desativado ao selecionar várias tarefas.
* O Workfront aciona notificações sobre as alterações feitas nas tarefas somente depois que você salva as alterações.

Há duas maneiras de salvar manualmente as alterações em tarefas em uma lista. Essas duas maneiras são descritas abaixo.

* [Salve as alterações em uma lista de tarefas manualmente ao selecionar a opção Salvar padrão manual](#save-changes-in-a-task-list-manually-when-you-select-the-manual-save-standard-option)
* [Salve as alterações em uma lista de tarefas manualmente ao selecionar a opção Salvar Manual do Planejamento de Linha do Tempo](#save-changes-in-a-task-list-manually-when-you-select-the-manual-save-timeline-planning-option)

#### Salve as alterações em uma lista de tarefas manualmente ao selecionar a opção Salvar padrão manual {#save-changes-in-a-task-list-manually-when-you-select-the-manual-save-standard-option}

>[!TIP]
>
>Se o projeto tiver mais de 2000 tarefas ou se tiver muitas dependências, pode demorar algum tempo para identificar visualmente as alterações feitas nas tarefas e como essas alterações afetam todas as dependências do projeto. Nesse caso, salvar as alterações pode demorar mais se o projeto tiver mais de 2000 tarefas ou se tiver muitas dependências.

Considere o seguinte ao atualizar tarefas em uma lista depois de selecionar a opção Salvar padrão manual :

* Você pode aplicar uma exibição personalizada à lista de tarefas e editar quaisquer campos relacionados a tarefas que tenha permissões para gerenciar nessa visualização.
* O Workfront calcula a linha do tempo do projeto e todas as dependências dentro do projeto e entre projetos depois que você clica em Salvar, quando o Tipo de atualização do projeto é Automático ou Automático e On Change. Para obter informações sobre o Tipo de Atualização do projeto, consulte [Selecione o Tipo de Atualização do projeto](../../../manage-work/projects/manage-projects/select-project-update-type.md).

Para editar tarefas em uma lista ao selecionar a opção Salvar Manual Padrão:

1. Vá para um projeto e clique no botão **Tarefas** seção .
1. Clique no botão **Modo de Plano** menu ![](assets/qs-list-mode-or-save-mode-icon-small.png) na parte superior da lista e selecione **Salvar manualmente**, depois clique em **Padrão** > **Aplicar**.

   ![](assets/manual-standard-setting-enabled-quicksilver-task-list-350x493.png)

   Uma configuração da barra de ferramentas é exibida com opções para desfazer, refazer e salvar as alterações.

   ![](assets/undo,-redo,-save,-and-cancel-widget-for-task-list-350x65.png)

1. Clique dentro de qualquer campo com permissões para atualizar manualmente. O campo se torna editável e você pode fazer as alterações.

   ![](assets/inline-editing-a-task-350x26.png)

1. Pressione Enter para salvar temporariamente as alterações feitas.
1. (Opcional) Clique no botão **Ícone Desfazer** ![](assets/undo-icon-on-task-list.png) para reverter uma alteração e retornar um campo ao seu estado original.
1. (Opcional e condicional) Clique no botão **Ícone Refazer** ![](assets/redo-icon-on-task-list.png) para restaurar a alteração revertida.

1. (Opcional) Clique com o botão direito do mouse em uma tarefa que deseja modificar.

   Ou

   Clique no botão **Mais** menu ![](assets/more-icon-task-list.png).

1. (Opcional) Selecione uma das seguintes opções:

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
      <td> <p>Ultrapassa a tarefa em um nível. </p> <p>Essa opção é exibida somente em tarefas secundárias. </p> </td> 
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
      <td> <p>Cria uma versão duplicada da tarefa no mesmo projeto. </p> <p>Para obter informações sobre cópia e duplicação de tarefas, consulte <a href="../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md" class="MCXref xref">Copiar e duplicar tarefas</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. O Workfront atualiza todas as dependências dentro do projeto e entre projetos ao fazer alterações na linha do tempo das tarefas.
1. Clique em **Salvar** quando quiser manter a tarefa alterada permanentemente e salvar a linha do tempo do projeto.

#### Salve as alterações em uma lista de tarefas manualmente ao selecionar a opção Salvar Manual do Planejamento de Linha do Tempo {#save-changes-in-a-task-list-manually-when-you-select-the-manual-save-timeline-planning-option}

Salvar as alterações e todas as dependências do projeto é mais rápido. Isso não está disponível para projetos com mais de 2000 tarefas.

>[!IMPORTANT]
>
>Recomendamos que você use essa opção ao editar uma grande lista de tarefas com mais de algumas centenas que têm muitas dependências. Usar essa opção permite identificar visualmente suas alterações muito mais rapidamente do que usar a opção Salvar manual .

Considere o seguinte ao usar a opção Salvar planejamento de linha do tempo manual em uma lista de tarefas:

* Não é possível aplicar a opção de salvamento Manual do Planejamento de Linha do Tempo a projetos com mais de 2000 tarefas.
* Não é possível aplicar uma exibição, filtro ou agrupamento personalizado à lista de tarefas. Os menus suspensos Exibição, Filtro e Agrupamento , bem como o ícone Exibição ágil , estão desativados. A exibição aplicada por padrão contém um número limitado de campos.
* A linha do tempo do projeto e todas as dependências no projeto são calculadas automaticamente após cada alteração quando o Tipo de atualização do projeto é Automático ou Automático e On Change.
* As dependências entre projetos são calculadas depois que você clica em Salvar, quando o Tipo de atualização do projeto é Automático ou Automático e On Change. Para obter informações sobre o Tipo de Atualização do projeto, consulte [Selecione o Tipo de Atualização do projeto](../../../manage-work/projects/manage-projects/select-project-update-type.md).

Para editar tarefas em uma lista ao usar a opção Salvar Manual do Planejamento de Linha do Tempo:

1. Vá para um projeto e clique no botão **Tarefas** seção.
1. Clique no botão **Modo de Plano** menu ![](assets/qs-list-mode-or-save-mode-icon-small.png) na parte superior da lista e selecione **Salvar manualmente**, depois clique em **Planejamento de linha do tempo**> **Aplicar**.

   Essa opção está esmaecida para projetos com mais de 2000 tarefas.

   ![](assets/manual-timeline-planning-setting-enabled-quicksilver-task-list-350x490.png)

   >[!TIP]
   >
   >Ao sair desta página, o Workfront reativa a opção Salvar automaticamente.

   Observe as seguintes alterações na lista:

   * Os menus suspensos Exibição, Agrupamento e Filtro são removidos e a exibição é substituída pelos seguintes campos:

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
   * O ícone de Visualização ágil é removido.
   * Uma configuração da barra de ferramentas é exibida com opções para desfazer, refazer e salvar as alterações.

      ![](assets/undo,-redo,-save,-and-cancel-widget-for-task-list-350x65.png)


1. Edite qualquer campo com permissões para atualizar manualmente.

   ![](assets/inline-editing-a-task-350x26.png)

1. Pressione Enter para salvar temporariamente as alterações feitas.
1. (Opcional) Clique no botão **Ícone Desfazer** ![](assets/undo-icon-on-task-list.png) para reverter uma alteração e retornar um campo ao seu estado original.
1. (Opcional e condicional) Clique no botão **Ícone Refazer** ![](assets/redo-icon-on-task-list.png) para restabelecer a alteração que você inverteu.

1. (Opcional) Clique com o botão direito do mouse em uma tarefa que deseja modificar

   Ou

   Clique no botão **Mais** menu ![](assets/more-icon-task-list.png).

1. Selecione dentre as seguintes opções:

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
      <td> <p>Ultrapassa a tarefa em um nível. </p> <p>Essa opção é exibida somente em tarefas secundárias. </p> </td> 
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
      <td> <p>Cria uma versão duplicada da tarefa no mesmo projeto. </p> <p>Para obter informações sobre cópia e duplicação de tarefas, consulte <a href="../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md" class="MCXref xref">Copiar e duplicar tarefas</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. O Workfront atualiza todas as dependências dentro do projeto e entre projetos ao alterar a linha do tempo de uma tarefa.
1. Clique em **Salvar** quando quiser manter a tarefa alterada permanentemente e salvar a linha do tempo do projeto.

## Editar uma tarefa em uma lista usando o Resumo

1. Vá para o projeto que contém as tarefas que deseja editar.
1. Clique em **Tarefas** no painel esquerdo.

   A lista de tarefas no projeto é exibida.

1. Clique no menu Mais ![](assets/more-icon-task-list.png) depois do nome da tarefa, clique em **Abrir resumo**. Selecione a tarefa que deseja editar e clique no botão **Ícone Abrir resumo** ![](assets/qs-open-summary-icon-in-new-toolbar-small.png) no canto superior direito da lista.

   O **Resumo** é aberto.

   ![](assets/qs-task-right-panel-in-a-task-list-350x328.png)

1. (Opcional) Clique no botão **Ícone X** no canto superior direito do Resumo para fechar o painel e editar as tarefas em linha.

   Siga as etapas sobre como editar uma tarefa em uma lista para editar a tarefa em linha.

   Para obter informações sobre como editar a tarefa em uma lista, consulte [Considerações sobre edição de tarefas em uma lista](#considerations-about-editing-tasks-in-a-list) neste artigo.

1. (Opcional) Digite uma atualização para a tarefa na função **Atualizações** área.
1. Clique em qualquer um dos ícones ou áreas a seguir para ir para a tarefa e editar informações no nível da tarefa:

   | Documentos | Clique em **Clique aqui para adicionar** para adicionar documentos à tarefa. |
   |---|---|
   | Detalhes | Clique em para atualizar informações sobre a tarefa. |
   | Formulários personalizados | Clique em para adicionar ou remover Forms personalizado ou para atualizar informações nos formulários. |
   | Horas | Clique em para registrar horas. |
   | Aprovações | Clique em para adicionar aprovações de tarefa. |

   {style=&quot;table-layout:auto&quot;}

1. Clique no botão Voltar do navegador para retornar à lista de tarefas quando terminar de atualizar a tarefa.

## Editar tarefas em massa

É possível editar várias tarefas ao mesmo tempo. Certifique-se de ter permissões de gerenciamento para as tarefas a fim de editá-las.

1. Vá para um projeto que contém tarefas que você deseja editar em massa.
1. Clique em **Tarefas** no painel esquerdo.
1. Certifique-se de que **Salvar automaticamente** está selecionada.

   >[!IMPORTANT]
   >
   >Não é possível editar tarefas em massa ao salvar tarefas manualmente.

   Para obter mais informações sobre como salvar alterações em tarefas em uma lista, consulte a seção [Considerações sobre edição de tarefas em uma lista](#considerations-about-editing-tasks-in-a-list) neste artigo.

1. Selecione várias tarefas na lista de tarefas.
1. Clique no botão **Ícone Editar** ![](assets/qs-edit-icon.png).

   O **Editar Tarefas** será aberta.

1. Especifique as informações que deseja alterar para todas as tarefas selecionadas.

   Editar as informações em todas as tarefas é idêntico à edição de informações em uma tarefa. Se você quiser editar a Duração da tarefa, as tarefas selecionadas deverão ter a mesma Restrição de Tarefa; caso contrário, a variável **Duração** campo não é preenchido.

   Para obter mais informações sobre como editar uma tarefa, consulte [Editar tarefas](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

   >[!NOTE]
   >
   >As informações que você está alterando em todas as tarefas selecionadas substituirão as informações existentes em tarefas individuais, exceto para a variável **Atribuições** campo. Adicionar um novo destinatário na edição em massa adicionará esse destinatário a todas as tarefas selecionadas. Se outros destinatários forem atribuídos às tarefas selecionadas, eles continuarão atribuídos além do que foi adicionado por meio da edição em massa.

1. Clique em **Forms personalizada** para editar os formulários personalizados anexados a todas as tarefas selecionadas. Somente os formulários personalizados ativos são exibidos na lista.

   Se as tarefas selecionadas não tiverem formulários personalizados comuns, nenhum formulário será listado nesta seção.

   É possível editar apenas os campos nos formulários que estão anexados a todas as tarefas selecionadas e que você tem permissões para editar.

1. (Opcional) Na seção Forms personalizado , selecione o **Recalcular expressões personalizadas** para garantir que todos os campos personalizados calculados que estão nos formulários personalizados anexados às tarefas selecionadas estejam atualizados.
1. Clique em **Salvar alterações**.

   Todas as alterações feitas agora estão visíveis em todas as tarefas selecionadas.

Para obter informações sobre edição de itens em massa de formulários personalizados, consulte a seção &quot;Editar vários Forms personalizados ao editar objetos em massa&quot; em [Gerenciar formulários personalizados anexados a objetos](../../../workfront-basics/work-with-custom-forms/manage-custom-forms-attached-to-objects.md).
