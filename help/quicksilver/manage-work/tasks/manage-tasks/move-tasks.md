---
product-area: projects
navigation-topic: manage-tasks
title: Mover tarefas
description: Você pode mover tarefas para projetos diferentes ou para tarefas principais diferentes no Adobe Workfront.
author: Alina
feature: Work Management
exl-id: 93295d70-a6cf-46ca-b621-228fa6c983f5
source-git-commit: 421fd012c2ce6a4ae0b11fe343c279d1a3fd551c
workflow-type: tm+mt
source-wordcount: '1488'
ht-degree: 2%

---

# Mover tarefas

Você pode mover tarefas no Adobe Workfront entre os seguintes objetos:

* Uma tarefa ad hoc para um projeto.
* Uma tarefa de um projeto para outro projeto.
* Uma tarefa de um projeto em um pai diferente em outro projeto.
* Uma tarefa dentro do mesmo projeto sob um pai diferente.

Você pode mover uma tarefa no nível da tarefa ou pode mover uma tarefa de uma lista de tarefas.
Você pode mover uma única tarefa ou pode mover várias tarefas de uma lista de tarefas de cada vez.

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as ações neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront*</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenças da Adobe Workfront*</td> 
   <td> <p>Novo plano: Padrão </p> 
 <p>ou</p>  
<p>Plano atual: Trabalho ou superior </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a tarefas e projetos</p> <p><b>Nota</b>

Se você ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões para as tarefas</p> <p>Permissões do Contribute ou superiores para o projeto com a capacidade de adicionar tarefas</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Para descobrir que plano, tipo de licença ou acesso você tem, entre em contato com o administrador do Workfront.

## Considerações para mover tarefas

Considere o seguinte ao mover uma tarefa:

* Quando você move uma tarefa de um projeto para outro, as datas da tarefa podem ser recalculadas. O recálculo levará em consideração o cronograma que o novo projeto usa e as informações de Cronograma de início do projeto.

* Você pode optar por mover alguns itens associados à tarefa para a tarefa movida durante o processo de movimentação. No entanto, por padrão, os seguintes objetos são transferidos para a tarefa movida:

   * Problemas
   * Horas registradas
   * Comentários do usuário
   * Formulários personalizados e informações de campos personalizados
   * Subtarefas

Os seguintes itens não são movidos com a tarefa, por padrão:

* Etapas

## Mover tarefas em uma lista

1. Vá para o projeto que contém a(s) tarefa(s) que deseja mover.
1. Clique em **Tarefas** no painel esquerdo para exibir a lista de tarefas.
1. Clique em **Modo de plano** ícone ![](assets/plan-mode-icon.png) e assegurar que o **Salvamento automático** for ativado, selecione a tarefa ou tarefas que deseja mover.

   ![](assets/autosave-icon-on-highlighted-350x202.png)

   >[!IMPORTANT]
   >
   >Não é possível mover tarefas quando a variável **Salvamento automático** alternância desativada.

1. (Opcional e condicional) Se quiser mover as tarefas selecionadas no mesmo projeto, clique nas tarefas selecionadas, arraste-as e solte-as no local em que deseja movê-las no projeto.

   Depois de soltar as tarefas no local correto no projeto, as alterações feitas na hierarquia de tarefas são salvas imediatamente. Todas as informações associadas a cada tarefa são movidas com as tarefas.

1. (Condicional) Selecione a(s) tarefa(s) que deseja mover e siga um destes procedimentos:

   * Clique em **Mais** menu ![](assets/qs-more-menu.png) na parte superior da lista de tarefas, em seguida, clique em **Mover para**.
   * Clique com o botão direito do mouse nas tarefas selecionadas e clique em **Mover para**.
   * Ao selecionar uma tarefa, clique no botão **Mais** menu ![](assets/more-icon-task-list.png) ao lado do nome da tarefa na lista, em seguida, clique em **Mover para**.

   ![](assets/move-task-in-list-nwe-350x119.png)

   A caixa Mover Tarefa é exibida

1. Continue movendo a tarefa, conforme descrito na seção [Mover uma tarefa no nível da tarefa](#move-a-task-at-the-task-level) neste artigo, começando na Etapa 4.

   <!--
   is this still accurate?!
   -->

## Mover uma tarefa no nível da tarefa {#move-a-task-at-the-task-level}

Além de mover tarefas de uma lista de tarefas, você também pode mover uma tarefa no nível da tarefa, depois de abri-la.

1. Encontre uma tarefa em seu sistema Workfront procurando por ela.
1. Clique no nome da tarefa para abri-la.
1. Clique em **Mais** menu suspenso ![](assets/qs-more-menu.png) ao lado do nome da tarefa e clique em **Mover para**. A caixa Mover Tarefa é exibida.

   ![](assets/move-task-at-task-level-nwe-350x222.png)

1. (Opcional) Atualize a **Nome da tarefa**. A tarefa é movida com o novo nome no novo local. A Workfront não registra o nome original da tarefa.

   >[!TIP]
   >
   >O campo Nome da tarefa fica esmaecido e não pode ser editado ao selecionar a movimentação de várias tarefas em uma lista. Você pode passar o mouse sobre o campo Nome da tarefa e uma lista de todas as tarefas selecionadas é exibida.
   >
   >
   >![](assets/move-task-multiple-tasks-box-with-list-of-task-names-nwe-350x142.png)

1. Digite o nome do **Projeto de destino** para onde deseja mover a tarefa na **Selecionar projeto de destino** campo.

   Se desejar mover a tarefa dentro do mesmo projeto, digite o nome do projeto atual.

   >[!TIP]
   >
   >* O nome do projeto diferencia maiúsculas de minúsculas.
   >* Você também pode começar a digitar o número de referência ou inserir a ID do projeto. Isso pode ajudá-lo a distinguir entre projetos com nomes idênticos.
   >* Somente 100 projetos são exibidos na lista.

1. (Condicional) Clique em **Solicitar acesso** para solicitar acesso ao projeto, se você não tiver acesso ao projeto selecionado.
1. (Condicional) Continue a mover a tarefa para o projeto de destino selecionado sem solicitar acesso se tiver acesso para adicionar tarefas a uma das tarefas no projeto de destino.

   ![](assets/move-task-request-access-from-project-nwe-350x120.png)

   >[!TIP]
   >
   >Mensagens semelhantes serão exibidas se o projeto selecionado estiver com aprovação pendente, concluído ou inativo, quando o administrador do Workfront impedir a adição de tarefas a esses projetos. Para obter mais informações, consulte [Configurar preferências de projeto em todo o sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

1. (Opcional) Clique em **Opções** no painel esquerdo

   Ou

   Role para baixo até **Opções** na caixa Mover tarefa e, em seguida, desmarque qualquer um dos itens listados na tabela abaixo para removê-los das tarefas movidas. Todas as opções são selecionadas por padrão.

   >[!IMPORTANT]
   >
   >Desmarcar itens na lista Opções resulta em perda de dados. As informações da tarefa existente serão removidas e não poderão ser recuperadas.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Selecionar tudo</td> 
      <td>Desmarque essa opção para remover todas as informações da tarefa ao movê-la para seu novo local. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Dt Restr</td> 
      <td> <p>A restrição da tarefa é definida como O Mais Breve Possível ou O Mais Tarde Possível com base na configuração do Modo de Cronograma do projeto.</p> <p> Quando selecionada, a restrição atual da tarefa é transferida com a tarefa. </p> 
      <p><b>Nota</b>

   Ao mover ou copiar uma tarefa com restrições específicas de data para outro projeto e as datas de restrição da tarefa estiverem fora das datas do novo projeto, a Restrição de Tarefa será alterada para O Mais Breve Possível ou O Mais Tarde Possível ou as datas de Início Planejado ou de Conclusão Planejada dos projetos serão ajustadas.

   Veja a seguir exemplos de restrições específicas de data:
   <ul>
      <li> Início em</li>
      <li> Precisa Terminar Em</li>
      <li> Não Iniciar Antes De</li>
      <li> Não Iniciar Depois De</li>
      </ul>

   Para obter informações sobre restrições de tarefa e como restrições de tarefa ou datas de projeto podem ser afetadas, consulte <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">Visão geral de Restrição de Tarefa</a> e procure por uma restrição específica.</p> </td>
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
      <td>O status da tarefa é New. Caso contrário, o status da tarefa existente será preservado. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Informações financeiras</td> 
      <td>As informações financeiras da tarefa são removidas e o Workfront atualiza o Tipo de Custo da tarefa para Sem Custo e o Tipo de Receita da tarefa como Não Faturável. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Todos os predecessores</td> 
      <td> <p>Quando selecionada, a dependência se torna uma predecessora entre projetos quando você move a tarefa para outro projeto. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Documentos</td> 
      <td> <p>Os documentos anexados à tarefa não são transferidos para a tarefa movida. Isso inclui versões, provas e documentos vinculados.</p> <p>Isso não inclui aprovações de documentos. Aprovações de documentos nunca podem ser movidas quando uma tarefa é movida.</p> 
      <b>NOTA</b>

   Se você optar por não mover os documentos com a tarefa, eles serão excluídos e colocados na Lixeira por 30 dias. Um administrador pode restaurá-los e eles serão restaurados na tarefa movida.

   Se a tarefa for excluída depois de movida, os documentos restaurados serão colocados na área Documentos da página do usuário do administrador que os restaura.

   </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Notificações de Lembrete</td> 
      <td>Os lembretes de tarefa não são transferidos para a tarefa movida. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Despesas</td> 
      <td>As despesas registradas na tarefa não são transferidas para a tarefa movida. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Permissões</td> 
      <td> <p>O Workfront remove os nomes de todas as entidades exibidas na lista Compartilhamento da tarefa. </p> </td> 
     </tr> 
    </tbody> 
   </table>



1. (Opcional) Clique em **Selecionar pai** no painel esquerdo

   Ou

   Role para a **Selecionar pai** e selecione a tarefa no projeto de destino que você deseja que se torne a principal da tarefa movida.

   >[!TIP]
   >
   >Ao selecionar para mover várias tarefas em uma lista, todas as tarefas selecionadas se tornam as filhas da tarefa principal selecionada.

   Selecione um pai seguindo um destes procedimentos:

   * Na lista de tarefas, selecione um dos pais no plano de projeto.
   * Clique no ícone de pesquisa ![Ícone de pesquisa](assets/search-icon.png) e procure uma tarefa pai por nome.

   A tarefa é exibida na lista.

   ![Selecionar tarefa pai ao mover uma tarefa com funcionalidade de pesquisa ](assets/select-parent-when-moving-tasks-with-search-functionality-nwe-350x110.png)

1. Selecione o botão de opção do pai depois de encontrá-lo.

   Se você não selecionar uma tarefa pai, as tarefas serão movidas como tarefas principais em vez de subtarefas e serão colocadas no final da lista de tarefas no projeto de destino.

1. Clique em **Mover tarefa**

   Ou

   Clique em **Mover tarefas** ao selecionar várias tarefas em uma lista.

   As tarefas movidas agora estão no projeto especificado e são subtarefas de uma tarefa pai ou as últimas tarefas do projeto.
