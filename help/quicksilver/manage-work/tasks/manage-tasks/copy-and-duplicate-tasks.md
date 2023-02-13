---
product-area: projects
navigation-topic: manage-tasks
title: Copiar e duplicar tarefas
description: É possível copiar uma tarefa de um projeto para outro projeto ou duplicar uma tarefa no mesmo projeto.
author: Alina
feature: Work Management
exl-id: daf89062-cf58-4c39-83ff-727d969a9630
source-git-commit: 23a08c929b0a227c7a555af70ff731ef2df7a179
workflow-type: tm+mt
source-wordcount: '1670'
ht-degree: 1%

---

# Copiar e duplicar tarefas

É possível copiar uma tarefa de um projeto para outro projeto ou duplicar uma tarefa no mesmo projeto.

Você pode copiar ou duplicar uma ou várias tarefas ou tarefas pai de cada vez.

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
   <td> <p>Trabalho ou superior </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a Tarefas e Projetos</p> <p>Observação: Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões para uma tarefa </p> <p>Contribuir ou obter permissões mais altas para o projeto</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

## Considerações para copiar tarefas

Considere o seguinte ao copiar uma tarefa:

* Os problemas não são copiados com a tarefa.
* Os marcos são transferidos para a tarefa copiada e removidos da tarefa original.

Você pode copiar uma tarefa nas seguintes áreas da aplicação Web do Adobe Workfront:

* No nível da tarefa, na **Ícone Mais** ![](assets/qs-more-menu-19x7.png) à direita do nome da tarefa.

   Para obter informações, consulte o [Copiar uma tarefa no nível da tarefa](#copy-a-task-at-the-task-level) neste artigo.

* Em uma lista de tarefas, execute um dos seguintes procedimentos:

   * Clique com o botão direito do mouse no nome de uma tarefa.
   * Selecione a tarefa (ou tarefas) e expanda a **Mais** ícone ![](assets/more-icon-task-list.png) na parte superior da lista de tarefas.
   * Selecione uma tarefa e expanda o **Mais** ícone ![](assets/more-icon-task-list.png) ao lado do nome da tarefa.

      Essa opção não está disponível ao selecionar várias tarefas.
   Para obter informações, consulte o [Copiar tarefas em uma lista](#copy-tasks-in-a-list) neste artigo.

## Copiar tarefas em uma lista {#copy-tasks-in-a-list}

1. Vá para o projeto que contém a tarefa ou tarefas que deseja copiar.

   Ou

   Ir para um relatório de tarefa.

1. Clique em **Tarefas** no painel esquerdo.
1. Clique no botão **Menu Modo de plano** ![](assets/qs-list-mode-or-save-mode-icon-small.png) , em seguida **Salvar automaticamente**.

   >[!IMPORTANT]
   >
   >Você só pode copiar tarefas em uma lista quando salvar automaticamente as alterações. Para obter informações sobre como salvar opções ao editar tarefas, consulte [Editar tarefas em uma lista](../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md).

1. Selecione a tarefa ou tarefas que deseja copiar e execute um dos seguintes procedimentos:

   * Clique no botão **Menu Mais** na parte superior da lista de tarefas, em seguida, clique em **Copiar para**.
   * Clique com o botão direito do mouse nas tarefas selecionadas e depois clique em **Copiar para**.
   * Ao selecionar uma tarefa, clique no botão **Mais** menu ![](assets/more-icon-task-list.png) ao lado do nome da tarefa na lista, em seguida, clique em **Copiar para**.
   ![](assets/copy-task-in-list-nwe-350x131.png)

1. Continue copiando a tarefa, conforme descrito na seção [Copiar uma tarefa no nível da tarefa](#copy-a-task-at-the-task-level) a partir da Etapa 4.

   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   (NOTE: is this still accurate?!)
   </MadCap:conditionalText>
   -->

## Copiar uma tarefa no nível da tarefa {#copy-a-task-at-the-task-level}

Além de copiar tarefas em uma lista de tarefas, também é possível copiar uma tarefa depois de abri-la. 

1. Localize uma tarefa em seu sistema Workfront procurando por ela.
1. Clique no nome da tarefa para abri-la. 
1. Clique no botão **Mais** menu suspenso ![](assets/qs-more-menu.png) ao lado do nome da tarefa, em seguida, clique em **Copiar** **para**.

   ![](assets/taskcopy-to-at-the-task-level-nwe-350x200.png)

   A caixa Copiar tarefa é exibida.

1. (Opcional) Atualize o **Nome da tarefa**.

   >[!TIP]
   >
   >Este campo está esmaecido e não é editável ao selecionar para copiar várias tarefas em uma lista. Você pode passar o mouse sobre o campo Nome da tarefa e exibir uma lista de todas as tarefas selecionadas.
   >
   >![](assets/copy-task-multiple-tasks-box-with-list-of-task-names-nwe-350x130.png)

1. Digite o nome da função **Projeto de destino** onde você deseja copiar a tarefa na **Selecionar projeto de destino** campo. 

   >[!TIP]
   >
   >* O nome do projeto diferencia maiúsculas de minúsculas.
   >* Você também pode começar a digitar o Número de referência ou inserir a ID do projeto. Isso pode ajudar você a distinguir entre projetos com nomes idênticos.
   >* Somente 100 projetos são exibidos na lista.


   O nome do projeto atual é exibido por padrão. Se quiser copiar a tarefa no mesmo projeto, deixe este campo inalterado.

1. (Condicional) Clique em **solicitar acesso** para solicitar acesso ao projeto, se você não tiver acesso ao projeto selecionado.
1. (Condicional) Continue copiando a tarefa para o projeto de destino selecionado sem solicitar acesso se tiver acesso para adicionar tarefas a uma das tarefas no projeto de destino.

   ![](assets/copy-task-request-access-from-project-nwe-350x125.png)

   >[!TIP]
   >
   >Mensagens semelhantes são exibidas se o projeto selecionado estiver com aprovação pendente, concluído ou inativo, quando o administrador do Workfront impede a adição de tarefas a esses projetos. Para obter mais informações, consulte [Configurar preferências de projeto em todo o sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

1. Clique em **Opções** no painel esquerdo, desmarque os atributos da tarefa que você não deseja copiar com a tarefa. Todas as opções são selecionadas por padrão.

   >[!TIP]
   Selecionar e desmarcar **Selecionar tudo** cancela a seleção de todas as opções.

   Desmarque as opções a seguir para não transferi-las para a tarefa copiada. A tabela a seguir descreve o que acontece quando as opções são desmarcadas:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Dt Restr</td> 
      <td> <p>A restrição de tarefa é definida como Assim que possível ou Mais tarde possível com base na configuração do Modo de agendamento do projeto.</p> <p> Quando selecionada, a restrição atual da tarefa é transferida para a tarefa copiada. </p> <p>Observação: Ao mover ou copiar uma tarefa com restrições específicas de data para outro projeto e as datas de restrição da tarefa estiverem fora das datas do novo projeto, a Restrição de Tarefa será alterada para O mais rápido possível ou O mais tarde possível, ou as datas Planejadas de Início ou Conclusão Planejada dos projetos serão ajustadas. Alguns exemplos de restrições específicas de data são Deve começar em, Deve terminar em, Não iniciar mais cedo do que, Não iniciar mais tarde do que etc. Para obter informações sobre restrições de tarefa e como as restrições de tarefa ou datas do projeto podem ser afetadas, consulte <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">Visão geral da restrição de tarefa</a> e procure por uma restrição específica.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Atribuições</td> 
      <td> <p>Todas as atribuições são removidas da tarefa. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Processo de aprovação</td> 
      <td>Todos os processos de aprovação são removidos da tarefa.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Progresso</td> 
      <td>O status da tarefa é New. Caso contrário, a tarefa copiada manterá o status da tarefa existente.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Informações financeiras</td> 
      <td>As informações financeiras da tarefa são removidas.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Todos os antecessores</td> 
      <td> <p>Isso significa que as dependências não serão transferidas para as tarefas copiadas. </p> <p>Quando selecionados, os antecessores no grupo de tarefas copiadas são preservados, outros são excluídos.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Documentos</td> 
      <td> <p>Os documentos anexados à tarefa não são transferidos para a tarefa copiada. Isso inclui versões, provas e documentos vinculados.</p> <p>Isso não inclui aprovações de documento. As aprovações de documentos nunca podem ser copiadas quando uma tarefa é copiada.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Notificações de Lembrete</td> 
      <td>Os lembretes da tarefa não são transferidos para a tarefa copiada. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Despesas</td> 
      <td>As despesas registradas na tarefa não são transferidas para a tarefa copiada. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Permissões</td> 
      <td>O Workfront remove os nomes de todas as entidades exibidas na lista Compartilhamento da tarefa. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Dados personalizados</td> 
      <td> <p>Os valores dos campos personalizados são apagados e os formulários personalizados são transferidos para a tarefa copiada. </p> <p>Quando selecionados, os formulários e os valores dos campos personalizados são transferidos para a tarefa copiada. </p> </td> 
     </tr> 
    </tbody> 
   </table>

1.  (Opcional) Clique em **Selecionar Pai** no painel esquerdo, selecione a tarefa no projeto de destino que deseja tornar-se o pai da tarefa copiada.

   >[!TIP]
   Ao selecionar para copiar várias tarefas em uma lista, todas as tarefas selecionadas se tornam filhos do pai selecionado.

   Selecione um pai seguindo um destes procedimentos:

   * Na lista de tarefas, selecione um dos pais no plano do projeto.
   * Clique no ícone de pesquisa ![Ícone de Pesquisa](assets/search-icon.png) e procure por uma tarefa pai por nome.
   A tarefa deve aparecer na lista.

   ![Selecionar tarefa pai ao mover uma tarefa com funcionalidade de pesquisa ](assets/select-parent-when-moving-tasks-with-search-functionality-nwe-350x110.png)

1. Selecione o botão de opção do pai depois de encontrá-lo. 

   Se você não selecionar uma tarefa pai, as tarefas serão copiadas como tarefas principais em vez de subtarefas e serão colocadas no final da lista de tarefas no projeto de destino. 

1. Clique em **Copiar tarefa**

   Ou

   Clique em **Copiar tarefas** ao selecionar várias tarefas em uma lista.
As tarefas copiadas agora estão no projeto especificado e são subtarefas para a tarefa pai selecionada ou as últimas tarefas no projeto.

## Tarefas duplicadas

Você pode duplicar rapidamente uma tarefa em uma lista de tarefas, se precisar de uma tarefa idêntica no mesmo projeto.

* [Considerações para duplicação de tarefas](#considerations-for-duplicating-tasks)
* [Tarefas duplicadas](#duplicate-tasks)

### Considerações para duplicação de tarefas {#considerations-for-duplicating-tasks}

* Você pode duplicar uma tarefa em uma lista de tarefas somente quando a lista é classificada por número de tarefa.

* A nova tarefa terá o mesmo nome da tarefa original.
* Não é possível selecionar quais informações estão duplicadas para a nova tarefa. Quase todas as informações da tarefa original serão transferidas para a tarefa duplicada, incluindo o relacionamento pai, por padrão.
* Os itens a seguir não são transferidos para a nova tarefa:

   * Horas registradas
   * Notas
   * Problemas
   * Somente os antecessores que estão no mesmo grupo de tarefas copiadas também são copiados com suas tarefas sucessoras.

      **Exemplo:** Por exemplo, se você copiar a Tarefa 2 e seu antecessor, Tarefa 1, ao mesmo tempo, você terá uma cópia da Tarefa 2 e uma cópia da Tarefa 1. A cópia da Tarefa 1 será o antecessor da cópia da Tarefa 2. Mas se você copiar apenas a Tarefa 2 sem copiar o antecessor, sua cópia não terá antecessor.

* Quando você duplica uma tarefa pai, todas as tarefas filho também são duplicadas, mesmo quando as tarefas filho não estão selecionadas.
* É possível duplicar várias tarefas ao mesmo tempo.

   No entanto, não é possível duplicar várias tarefas que não são sequenciais ao mesmo tempo.

* Os marcos são movidos para a nova tarefa e removidos da tarefa original.

### Tarefas duplicadas

1. Vá para o projeto que contém a tarefa ou tarefas que deseja duplicar.
1. Clique em **Tarefas** no painel esquerdo.
1. Siga um destes procedimentos:

   * (Condicional) Clique no botão **Menu Modo de plano** ![](assets/qs-list-mode-or-save-mode-icon-small.png) > **Salvar automaticamente**, selecione as tarefas que deseja duplicar e clique no botão **Menu Mais** ![](assets/qs-more-menu-29x11.png) > **Duplicar**.

      ![](assets/duplicate-tasks-in-list-nwe-350x196.png)

   * (Condicional) Clique no botão **Menu Modo de plano** ![](assets/qs-list-mode-or-save-mode-icon-small.png) > **Salvar manualmente** > **Padrão** ou **Planejamento de linha do tempo** e faça o seguinte:

      1. Selecione a tarefa ou tarefas que deseja duplicar e clique em **Duplicar**.
      1. (Opcional) Clique em **Desfazer** para reverter as alterações e não duplicar as tarefas.
      1. (Opcional e condicional) Clique em **Refazer** se você já clicou anteriormente **Desfazer**, para manter as alterações e duplicar as tarefas.

      1. Clique em **Salvar** para salvar as alterações.
   1. Editar tarefas em uma lista
