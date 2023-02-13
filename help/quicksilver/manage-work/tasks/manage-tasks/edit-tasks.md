---
product-area: projects
navigation-topic: manage-tasks
title: Editar tarefas
description: Editar tarefas
author: Alina
feature: Work Management
exl-id: 572c6008-3a67-47ae-8f5d-6b871ef1f37b
source-git-commit: 9c7af82b02649f33728d05126587fb5035e9e110
workflow-type: tm+mt
source-wordcount: '3627'
ht-degree: 4%

---

# Editar tarefas

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: some information in this area is repeated in the following articles. If you need to update a fied, update it in both:</p>
<p>** Task finances in details</p>
<p>** Task information in overview)</p>
</div>
-->


É possível editar informações sobre tarefas criadas ou que você tenha permissões do Contribute ou do Gerenciar.

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plano Adobe Workfront*</td> 
   <td> <p>Qualquer Um </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Trabalho ou superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Nível de acesso*</td> 
   <td> <p>Editar acesso a Tarefas e Projetos</p> <p><b>Nota</b>

Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode alterar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> 
    <ul> 
     <li> <p>Contribua com permissões para uma tarefa para editá-la na área Detalhes da tarefa </p> </li> 
     <li> <p>Gerencie permissões em uma tarefa para editá-la na caixa Editar tarefa</p> </li> 
    </ul> 
    <ul> 
     <li> <p>Contribuir ou obter permissões mais altas para o projeto</p> </li> 
    </ul> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

## Limitações para tarefas de edição

Há algumas limitações que podem impedir a edição de tarefas.

Considere o seguinte ao editar tarefas:

* Atualizar tarefas aciona notificações para projetos que são um status Atual. Para evitar confusão para usuários atribuídos às tarefas, limite ao máximo as tarefas de edição quando o projeto estiver no status Atual.
* Não é possível editar tarefas que estão em um Processo de Aprovação. Você só pode registrar a hora ou atualizar o Status de uma tarefa em um processo de aprovação.

   ![](assets/edit-task-in-approval-process-nwe-350x148.png)

* Você pode editar e adicionar documentos a tarefas em um projeto que tenha o status Concluído, Inativo ou Pendente de Aprovação somente quando o administrador do Workfront ou um administrador de grupo ativou essa funcionalidade na área Preferências do projeto. Para obter informações sobre como definir preferências de projeto, consulte [Configurar preferências de projeto em todo o sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

* Você sempre pode editar as seguintes informações em uma tarefa quando o projeto tiver sido marcado como Concluído, Inativo ou estiver em um Processo de aprovação:

   * Tempo de registro
   * Editar despesas existentes
   * Anexar um formulário personalizado

## Editar uma tarefa em uma lista

É possível editar as informações da tarefa em uma lista de tarefas, por campos de edição em linha exibidos na visualização da lista.

Para obter informações sobre edição de tarefas em listas, consulte [Editar tarefas em uma lista](../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md).

## Editar uma tarefa em uma lista usando o Resumo

É possível editar uma tarefa em uma lista usando o painel Resumo. Para obter informações sobre como editar uma tarefa no painel Resumo, consulte a seção &quot;Editar uma tarefa no Resumo&quot; no [Editar tarefas em uma lista](../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md) artigo 10. o

## Editar uma tarefa na caixa Editar tarefa

É possível editar uma tarefa usando as áreas Editar Tarefa ou Detalhes da Tarefa. As etapas a seguir descrevem como editar uma tarefa na caixa Editar tarefa .

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront.

1. Clique em **Projetos**, em seguida, clique no nome de um projeto para abri-lo.
1. Clique em **Tarefas** no painel esquerdo.
1. Clique na tarefa que deseja editar.
1. (Opcional) Para editar informações limitadas sobre uma tarefa, clique em **Detalhes da tarefa** no painel esquerdo.

   ![](assets/nwe-task-details-expanded-350x273.png)

   Considere editar as informações nas seguintes áreas da seção Detalhes da tarefa:

   * **Visão geral**

      Essa área é expandida por padrão.

   * **Formulários personalizados**

      Os nomes dos formulários aduaneiros são exibidos somente se houver formulários personalizados anexados ao objeto.

   * **Finanças**
   >[!NOTE]
   >
   >Dependendo de como o administrador do Workfront ou o administrador do Grupo modificou seu Modelo de layout, os campos na área Detalhes da tarefa podem ser reorganizados ou não serem exibidos. Para obter mais informações, consulte [Personalizar a visualização de Detalhes usando um modelo de layout](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

   Para obter informações sobre os campos visíveis na seção Detalhes da tarefa ,

   continue editando a tarefa na caixa Editar tarefa , conforme descrito abaixo.

   Para editar informações na seção Detalhes, faça o seguinte:

   1. (Opcional) Clique no botão **Recolher Tudo** ícone ![](assets/collapse-all-icon.png) no canto superior direito para recolher todas as áreas.
   1. (Opcional e condicional) Quando uma área for recolhida, clique no botão **seta apontando para a direita** ![](assets/right-pointing-arrow.png) ao lado de cada área para expandir a área que você deseja editar.
   1. Para obter mais informações sobre a edição de informações na guia Detalhes da tarefa, consulte os seguintes artigos:

      * [Gerenciar informações da tarefa na área Visão geral de detalhes da tarefa](../../../manage-work/tasks/manage-tasks/task-information-in-overview.md)
      * [Gerenciar finanças da tarefa na seção Detalhes da tarefa](../../../manage-work/tasks/manage-tasks/task-finances-in-details.md)
   1. (Opcional) Se não houver formulários personalizados anexados à tarefa, comece a digitar o nome de um formulário no **Adicionar formulário personalizado** , selecione-o quando for exibido na lista e clique em **Salvar alterações**.
   1. (Opcional) Clique no botão **Exportar** ícone ![](assets/export.png) para exportar as informações de formulários personalizados e Visão geral para um arquivo PDF, clique em **Exportar**. Selecione uma das opções a seguir:

      * Selecionar tudo (é exibido somente quando há pelo menos um formulário personalizado anexado)
      * Visão geral
      * O nome de um ou vários formulários personalizados

      O arquivo PDF é baixado para o computador.

      ![](assets/export-issue-details-selection-box-with-export-button-350x418.png)

      Para obter mais informações, consulte [Exportar formulários personalizados e detalhes do objeto](../../../workfront-basics/work-with-custom-forms/export-custom-forms-details.md).




1. Para editar todas as informações sobre a tarefa, clique no botão **Mais** menu ![](assets/more-icon.png) ao lado do nome da tarefa, em seguida, clique em **Editar**.

   Ou

   Em uma lista de tarefas, selecione uma tarefa e clique no botão **Editar** ícone ![](assets/edit-icon.png) na parte superior da lista.

   A caixa Editar tarefa é aberta.

   >[!IMPORTANT]
   >
   >Você deve ter permissões de gerenciamento na tarefa para ver a opção Editar .

   Todos os campos de tarefa estão disponíveis na caixa Editar tarefa e são agrupados pelas áreas listadas no painel esquerdo.

   >[!NOTE]
   >
   >Dependendo de como o administrador do Workfront ou o administrador do Grupo modificou seu Modelo de layout, os campos na área Detalhes da tarefa podem ser reorganizados ou não serem exibidos. Para obter mais informações, consulte [Personalizar a visualização de Detalhes usando um modelo de layout](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

   Considere especificar informações em qualquer uma das seguintes seções:

   * [Nome da tarefa](#task-name)
   * [Visão geral](#overview)
   * [Atribuições](#assignments)
   * [Formulários personalizados](#Custom%C2%A0F)
   * [Finanças](#finance)
   * [Configurações](#settings)

   >[!NOTE]
   >
   >Dependendo de como o administrador do Workfront ou o administrador do Grupo configura nosso Modelo de layout, os campos na caixa Editar tarefa podem ser reorganizados ou não serem exibidos. Para obter mais informações, consulte [Personalizar a visualização de Detalhes usando um modelo de layout](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

### Nome da tarefa {#task-name}

1. Comece a editar sua tarefa conforme descrito acima.
1. Clique em **Nome da tarefa** no painel esquerdo.

   ![](assets/nwe-task-name-section-edit-task-box-350x122.png)

1. Atualize o nome da tarefa.

1. Clique em **Salvar** ou continue com as seções a seguir.

### Visão geral {#overview}

1. Comece a editar sua tarefa conforme descrito acima.
1. Clique em **Visão geral** no painel esquerdo.

   ![](assets/nwe-overview-section-edit-task-box-350x257.png)

1. Atualize as seguintes informações sobre a tarefa:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Descrição</td> 
      <td>Adicione informações adicionais sobre a tarefa. </td> 
     </tr> 
     <tr> 
      <td colspan="2" role="rowheader"><span style="font-weight: bold;">Seção Informações básicas</span> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Status</td> 
      <td> <p>Selecione o status da tarefa que indica em qual estágio de desenvolvimento a tarefa está.</p> <p><b>DICA</b>

   Você pode atualizar o Status da tarefa no cabeçalho da tarefa. </p> </td>
   </tr> 
     <tr> 
      <td role="rowheader">Prioridade</td> 
      <td> <p>Esse é um sinalizador visual para você, que permite priorizar suas tarefas. </p> <p>Selecione dentre as seguintes opções: </p> 
       <ul> 
      <li> <p> Nenhum(a)</p> </li> 
      <li> <p> Baixa </p> </li> 
      <li> <p>Normal </p> </li> 
      <li> <p>Alta </p> </li> 
      <li> <p> Urgente </p> </li> 
       </ul> <p>Dependendo das Preferências do projeto selecionadas pelo administrador do Workfront, os nomes das prioridades podem ser diferentes para você. Para obter informações sobre as prioridades da tarefa, consulte <a href="../../../manage-work/tasks/task-information/task-priority.md" class="MCXref xref">Atualizar Prioridade da Tarefa</a>. </p> </td> 
     </tr> 
     <tr> 
      <td colspan="2" role="rowheader"><span style="font-weight: bold;">Seção Datas e restrições da tarefa</span> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Restrição de Tarefa</td> 
      <td> <p>Decida quando a tarefa deve ser concluída especificando uma Restrição de Tarefa. </p> <p>Selecione dentre as seguintes opções: </p> 
       <ul> 
      <li> <p><span>Datas Fixas</span> </p> <p>Especifique um <strong>Início planejado</strong> e <strong>Data de Conclusão Planejada</strong>. </p> </li> 
      <li> <p><span>Precisa Iniciar Em</span> </p> <p>Especifique um <strong>Data de início planejada</strong>. </p> </li> 
      <li> <p><span>Precisa Terminar Em</span> </p> <p>Especifique um <strong>Data de Conclusão Planejada</strong>. </p> </li> 
       </ul> 
       <ul> 
      <li> <p><span>O Mais Rapidamente Possível</span></p> </li> 
      <li> <p><span>O Mais Tarde Possível</span></p> </li> 
      <li> <p><span>Momento Mais Cedo Disponível</span></p> </li> 
      <li> <p> <span>O Mais Tarde Disponível</span></p> </li> 
      <li> <p><span>Não Iniciar Depois De</span> </p> </li> 
      <li> <p>Especificar uma Data de Início Planejada</p> </li> 
      <li> <p><span>Não Iniciar Antes De</span> </p> <p>Especifique um <strong>Data de início planejada</strong>. </p> </li> 
      <li> <p> Concluir <span>Não mais tarde do que</span></p> <p>Especifique um <strong>Data de Conclusão Planejada</strong>. </p> </li> 
      <li> <p> Concluir <span>Não Anterior a</span></p> <p>Especifique um <strong>Data de Conclusão Planejada</strong></p> </li> 
       </ul> <p>Para obter mais informações sobre a Restrição de Tarefa, consulte <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">Visão geral da restrição de tarefa</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Data e hora da confirmação</td> 
      <td> <p>Esta é a data pela qual o usuário atribuído à tarefa se compromete a completá-la. Pode ser diferente da Data de conclusão planejada. Somente as pessoas atribuídas podem editar este campo. Para obter informações sobre datas de confirmação no Workfront, consulte <a href="../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md" class="MCXref xref">Visão geral da data de confirmação</a>. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Data e hora de início previstas</td> 
      <td> <p>Quando a tarefa estiver planejada para iniciar. A data de início planejada de uma tarefa é definida e influenciada por vários fatores:</p> 
       <ul> 
      <li>Dependendo da preferência em todo o sistema pela data de início planejada da tarefa, a data de início de uma nova tarefa em um projeto pode ser hoje ou a data de início do projeto, por padrão. <span>O administrador do grupo para o grupo associado ao projeto também pode definir essa preferência para o grupo.</span> Para obter mais informações sobre as preferências de tarefa no nível do sistema ou de grupo, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md" class="MCXref xref">Configurar preferências de emissão e tarefa em todo o sistema</a>.</li> 
      <li>Dependendo dos antecessores da tarefa, a data de início planejada é escolhida pelo Workfront para ser a próxima data disponível depois que os antecessores terminarem ou começarem, dependendo do relacionamento do antecessor. Para obter mais informações sobre os relacionamentos do antecessor, consulte <a href="../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md" class="MCXref xref">Visão geral dos antecessores de tarefas</a>.</li> 
      <li>O gerente do projeto ou o proprietário da tarefa podem definir manualmente a data de início planejada quando a restrição da tarefa for Datas fixas ou Deve iniciar em. Para obter mais informações sobre restrições de tarefa, consulte <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">Visão geral da restrição de tarefa</a>.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Data e hora de conclusão previstas</td> 
      <td> <p>A data de conclusão antecipada conforme mostrado quando a tarefa é planejada. A data de conclusão planejada pode ser definida por vários fatores:</p> 
       <ul> 
      <li>A data de conclusão planejada é calculada a partir da data de início planejada adicionando a Duração da tarefa à data de início planejada. Quando o gerente do projeto ou o Workfront especifica a Duração da tarefa, isso dispara uma atualização para a data de conclusão planejada. Se a data planejada for alterada, geralmente será porque a Duração da campanha foi atualizada.</li> 
      <li>O gerente do projeto ou o proprietário da tarefa podem definir manualmente a data de conclusão planejada quando a restrição da tarefa for Datas Fixas ou Deve Concluir em. Para obter mais informações sobre restrições de tarefa, consulte <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">Visão geral da restrição de tarefa</a>.</li> 
      <li>Se o Tipo de duração da tarefa for alterado e o número de recursos nas tarefas for alterado ao mesmo tempo, a data de conclusão planejada também será alterada. Para obter mais informações sobre tipos de duração, consulte <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Visão Geral da Duração da Tarefa e do Tipo de Duração</a>.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Data e hora de início reais</td> 
      <td> <p>Especifique uma Data de Início Real para a tarefa. O padrão normalmente é preenchido automaticamente quando você altera o status da tarefa para Em andamento. A data de início real também pode ser modificada manualmente pelo gerente do projeto ou pelo proprietário da tarefa. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Data e hora de conclusão real</td> 
      <td> <p>Especifique a data e a hora reais em que a tarefa é concluída. A data e a hora padrão em que uma tarefa é concluída sempre coincide com a hora real em que o status se torna Concluído. A data de conclusão real também pode ser modificada manualmente pelo gerente do projeto ou pelo proprietário da tarefa. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><b>Seção do tempo de trabalho</b></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Esforço do trabalho </td> 
      <td>

   <p>A quantidade de esforço necessária para concluir a tarefa. O gerente do projeto pode decidir usar esse campo em vez de Horas Planejadas para estimar o esforço necessário para concluir uma tarefa. Este campo fica visível somente quando as seguintes condições são atendidas:</p> 
      <ul> 
      <li> <p>A tarefa tem um Tipo de duração simples. </p> <p><b>DICA</b>

   Se você alterar o Tipo de duração da tarefa, esse campo ficará esmaecido. </p> </li>
   <li>O gerente de projeto habilitou o campo Usar Esforço de Trabalho para calcular automaticamente as Horas Planejadas da tarefa no projeto. </li> 
      </ul> 
      <p>Selecione dentre as seguintes opções:</p> 
      <ul> 
      <li>Pequena</li> 
      <li>Médio <span style="font-weight: normal;">(esse é o valor padrão para uma nova tarefa)</span></li> 
      <li>Grande</li> 
      </ul> 
      <p><b>Nota</b>

   Atualizar a quantidade de esforço poderia atualizar a tarefa Horas Planejadas. A atualização é imediata se o Tipo de atualização do projeto for Automático. Quando o Tipo de Atualização do projeto é Manual, você deve recalcular a linha do tempo para ver as Horas Planejadas atualizadas. </p>

   <p>Para obter informações sobre como usar o Esforço de Trabalho em vez de Horas Planejadas para estimar o esforço da tarefa, consulte <a href="../../../manage-work/tasks/task-information/work-effort.md" class="MCXref xref">Visão geral do esforço de trabalho</a>. </p> 
    </td> 
     </tr> 
    </tbody> 
   </table>

1. Clique em **Salvar** ou continue com as seções a seguir.

### Atribuições {#assignments}

1. Comece a editar sua tarefa conforme descrito acima.
1. Clique em **Atribuições** no painel esquerdo.

   ![](assets/nwe-assignments-section-edit-task-box-350x217.png)

1. Clique em **Pesquisar pessoas, funções e equipes** e comece a digitar o nome de um usuário, função ou equipe que deseja atribuir à tarefa, em seguida, clique nela ou pressione Enter quando ela for exibida na lista.

   >[!NOTE]
   >
   >Se o nome do usuário contiver um caractere especial, você deverá incluir o caractere especial no campo de pesquisa.

   >[!TIP]
   >
   >Você pode atribuir vários usuários, funções de trabalho ou equipes. Você pode atribuir somente usuários ativos, funções de trabalho e equipes.
   >
   >Se um usuário, uma função de trabalho ou uma equipe tiver sido atribuída antes de ser desativada, ela permanecerá atribuída ao item de trabalho. Nesse caso, recomendamos o seguinte:
   >
   >* Atribua novamente o item de trabalho aos recursos ativos.
   >* Associe os usuários em uma equipe desativada a uma equipe ativa e reatribua o item de trabalho à equipe ativa.


1. (Opcional) Indique se um destinatário é o destinatário principal da tarefa, selecionando o **Proprietário** botão de opção ao lado do nome. Uma equipe não pode ser o principal destinatário de uma tarefa.
1. (Condicional e opcional) Atualize os seguintes campos:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Tipo de Duração</td> 
      <td> <p>Isso identifica a relação entre o seguinte: </p> 
       <ul> 
      <li> <p>O número de recursos atribuídos a uma tarefa </p> </li> 
      <li> <p>O esforço total necessário para concluir a tarefa </p> </li> 
      <li> <p> A duração total da tarefa. </p> </li> 
       </ul> <p>Seu administrador do Workfront <span> ou um administrador de grupo</span> seleciona a configuração padrão Tipo de duração para as tarefas em seu sistema ou grupo. Para obter informações sobre a definição de padrões do projeto, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configurar preferências de projeto em todo o sistema</a>. </p> <p>Os Tipos de duração permitem definir atribuições de recursos consistentes com base nas necessidades da tarefa. Para obter mais informações sobre o Tipo de duração de uma tarefa, consulte <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Visão Geral da Duração da Tarefa e do Tipo de Duração</a>. </p> <p>Selecione dentre as seguintes opções: </p> 
       <ul> 
      <li> <p>Atribuição Calculada </p> </li> 
      <li> <p> Trabalho Calculado </p> </li> 
      <li> <p>Controlado pelo empenho </p> </li> 
      <li> <p>Simples</p> </li> 
       </ul> </td> 
     </tr> 
     <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
      <td role="rowheader">Duração por Ocorrência</td> 
      <td> <p>Isso é exibido somente no pai das tarefas recorrentes. Ele exibe a duração de cada tarefa recorrente. Para obter informações sobre como criar tarefas recorrentes, consulte <a href="../../../manage-work/tasks/create-tasks/create-recurring-tasks.md" class="MCXref xref">Criar tarefas recorrentes</a>. </p> <p> <b>Nota</b>

   As durações modificadas em tarefas recorrentes individuais não exibem o valor indicado neste campo. </p> </td>
   </tr> 
     <tr> 
      <td role="rowheader">Duração</td> 
      <td> 
      <div> 
      <div> 
      <p>Esse é o período de tempo durante o qual uma tarefa pode permanecer aberta antes de ser concluída. </p> 
      <p><b>IMPORTANTE</b>

   Como a duração da tarefa normalmente é a quantidade de tempo entre o Início Planejado e as Datas de Conclusão Planejadas, ela afeta a linha do tempo do projeto.</p>

   <p>Para indicar a Duração da tarefa e a unidade de tempo, faça o seguinte:</p> 
      <ul> 
      <li> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Digite a duração de tempo e selecione a partir das unidades de tempo disponíveis no menu suspenso.</p> <p><b>DICA</b></p>
      Ao atualizar a Duração das tarefas em uma lista de tarefas, você pode usar a abreviação da unidade de tempo. </p> </li> 
      </ul> 
      <p> Você pode escolher entre as opções de tempo regular ou de tempo decorrido na tabela a seguir: </p> 
      <table style="table-layout:auto"> 
      <col> 
      <col data-mc-conditions=""> 
      <tbody> 
      <tr> 
      <td>Unidade de tempo</td> 
      <td>Abreviação</td> 
      </tr> 
      <tr> 
      <td>Minutos</td> 
      <td>M</td> 
      </tr> 
      <tr> 
      <td>Horas</td> 
      <td>H</td> 
      </tr> 
      <tr> 
      <td>Dias. Este é o padrão. </td> 
      <td>E</td> 
      </tr> 
      <tr> 
      <td>Semanas</td> 
      <td>Q</td> 
      </tr> 
      <tr> 
      <td>Meses</td> 
      <td>T</td> 
      </tr> 
      <tr> 
      <td>Minutos corridos</td> 
      <td>EM</td> 
      </tr> 
      <tr> 
      <td>Horas corridas</td> 
      <td>EH</td> 
      </tr> 
      <tr> 
      <td>Dias corridos</td> 
      <td>ED</td> 
      </tr> 
      <tr> 
      <td>Semanas corridas</td> 
      <td>EW</td> 
      </tr> 
      <tr> 
      <td>Meses decorridos</td> 
      <td>ET</td> 
      </tr> 
      </tbody> 
   </table>

   <p><b>Nota</b>

   <p>Tempo decorrido é uma unidade de tempo para a Duração de uma tarefa. É o tempo entre a Data inicial planejada e a Data de conclusão planejada de uma tarefa que inclui feriados, finais de semana e tempo limite. Por outras palavras, o tempo decorrido é a passagem dos dias de calendário.

   O tempo normal leva em consideração feriados, finais de semana e tempo de folga e os exclui da Duração da tarefa. Para obter mais informações sobre a duração da tarefa, consulte <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Visão Geral da Duração da Tarefa e do Tipo de Duração</a>. </p>
   </div> 
   </div> </td> 
   </tr> 
   <tr> 
   <td role="rowheader">Horas planejadas</td> 
   <td> <p>Especifique a quantidade de Horas Planejadas para a tarefa, em horas. Essa é a quantidade de tempo real que os destinatários da tarefa precisariam para concluí-la. Você só pode especificar a quantidade de Horas Planejadas para uma tarefa quando o Tipo de Duração estiver definido como Atribuição Calculada. Para obter mais informações sobre tipos de duração, consulte <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Visão Geral da Duração da Tarefa e do Tipo de Duração</a>.</p> </td> 
   </tr> 
   <tr> 
   <td role="rowheader">Alocação</td> 
   <td> <p>Se a Restrição de Tarefa for Calculada pelo Trabalho ou pelo Esforço, especifique a <strong>% de alocação</strong> (porcentagem de alocação) para cada destinatário. Esse é o tempo desde o agendamento do destinatário que ele pode gastar nessa tarefa. Alterar a porcentagem de alocação para um destinatário alterará as Horas Planejadas de uma tarefa. </p> <p>Quando a Restrição de tarefa é Simples, você pode especificar o seguinte:</p> 
      <ul> 
      <li> <p>Horas de alocação de cada destinatário.</p> </li> 
      <li> <p>Horas Planejadas da tarefa</p> </li> 
      <li> <p>Duração da tarefa</p> </li> 
      </ul> </td> 
   </tr> 
   <tr> 
   <td role="rowheader">Função do atribuidor</td> 
   <td> <p>Selecione uma função no <strong>Função do destinatário</strong> menu suspenso ao selecionar uma pessoa como destinatário. Esta é a função que o destinatário pode desempenhar nesta tarefa. </p> <p><b>DICA</b>

   Somente as funções de trabalho associadas a cada destinatário em seu perfil aparecem no menu suspenso.</p> </td>
   </tr> 
      </tbody> 
      </table>

1. Clique em **Salvar** ou continue com as seções a seguir.

### Formulários personalizados

É possível definir formulários personalizados padrão a serem anexados automaticamente a tarefas quando as tarefas forem adicionadas a um projeto. Para obter informações sobre como configurar o projeto para incluir formulários personalizados de tarefas padrão para todas as novas tarefas, consulte a seção &quot;Tarefas&quot; no artigo [Editar projetos](../../../manage-work/projects/manage-projects/edit-projects.md).

1. Comece a editar a tarefa conforme descrito acima.
1. Clique em **Forms personalizada** no painel esquerdo, ou clique no nome de um formulário personalizado, se ele já estiver anexado.

   ![](assets/nwe-custom-forms-section-edit-task-box-350x127.png)

1. Clique em **Adicionar formulário personalizado** e selecione o formulário ou formulários personalizados que deseja associar à tarefa. Você deve criar os formulários personalizados antes que eles estejam disponíveis para seleção neste campo. Somente os formulários personalizados ativos são exibidos na lista.

   Para obter mais informações sobre como criar formulários personalizados, consulte [Criar ou editar um formulário personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).É possível adicionar até dez formulários personalizados a uma tarefa.

1. (Condicional) Se um formulário personalizado foi anexado à tarefa, edite quaisquer campos no formulário. Você deve especificar todos os campos obrigatórios antes de poder salvar a tarefa.

   >[!NOTE]
   >
   >Dependendo de como o administrador do Workfront definiu as permissões para as seções em seu formulário personalizado, nem todos podem exibir ou editar os mesmos campos em um determinado formulário personalizado. As permissões para editar campos em uma seção de um formulário personalizado dependem das permissões que você tem na própria tarefa. Para obter informações sobre como definir permissões de tarefa, consulte [Compartilhar uma tarefa](../../../workfront-basics/grant-and-request-access-to-objects/share-a-task.md).

1. Clique em **Salvar** ou continue com as seções a seguir.

### Finanças {#finance}

1. Comece a editar sua tarefa conforme descrito na [Editar tarefas](#Edit2) neste artigo.
1. Clique em **Finanças** no painel esquerdo.

   ![](assets/nwe-finance-section-edit-task-box-350x298.png)

1. Atualize os seguintes campos:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Tipo de Custo</td> 
      <td> <p>Especifique o Tipo de Custo da tarefa. Isso determinará como o custo da tarefa é calculado, com base no número de horas nas tarefas. </p> <p>Selecione dentre as seguintes opções: </p> 
       <ul> 
        <li> <p>Sem Custo</p> </li> 
        <li> <p>Horas por Valor de Hora Fixo </p> </li> 
        <li> <p> Horas por Valor da Hora do Recurso </p> </li> 
        <li> <p> Horas por Valor da Hora do Perfil</p> </li> 
       </ul> <p>Para obter mais informações sobre o rastreamento de custos, consulte <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Rastrear custos</a> . O administrador do Workfront ou um administrador de grupo seleciona a configuração padrão de Tipo de Custo para as tarefas em seu sistema ou grupo. Para obter informações sobre a definição de padrões do projeto, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configurar preferências de projeto em todo o sistema</a> .</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tipo de Receita</td> 
      <td> <p>Especifique o Tipo de receita para a tarefa. Isso determinará como a Receita na tarefa será calculada, com base no número de horas nas tarefas. </p> <p>Selecione dentre as seguintes opções: </p> 
       <ul> 
      <li> <p> Não Faturável </p> </li> 
      <li> <p>Horas por Valor da Hora do Recurso </p> </li> 
      <li> <p>Horas por Valor da Hora do Perfil </p> </li> 
      <li> <p>Horas por Valor de Hora Fixo </p> </li> 
      <li> <p>Horas por Valor da Hora dos Recursos, com Teto </p> </li> 
      <li> <p>Horas por Valor da Hora do Perfil, com Teto </p> </li> 
      <li> <p>Horas por Valor da Hora do Recurso mais Taxa Fixa </p> </li> 
      <li> <p>Horas por Valor da Hora do Perfil mais Taxa Fixa </p> </li> 
      <li> <p>Receita com Valor Fixo </p> </li> 
       </ul> <p>Para obter mais informações sobre o rastreamento de receita, consulte<a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">Visão Geral da Faturamento e Receita</a> . </p> <p>O administrador ou administrador de grupo da Workfront seleciona a configuração padrão Tipo de receita para as tarefas em seu sistema ou grupo. Para obter informações sobre a definição de padrões do projeto, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configurar preferências de projeto em todo o sistema</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Clique em **Salvar** ou continue com a seção a seguir.

### Configurações {#settings}

1. Comece a editar sua tarefa conforme descrito na [Editar tarefas](#Edit2) neste artigo.
1. Clique em **Configurações** no painel esquerdo.

   ![](assets/nwe-settings-section-edit-task-box-350x304.png)

1. Atualize os seguintes campos:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Modo de Acompanhamento</td> 
      <td> <p>Especifique como o status do progresso da tarefa é rastreado. </p> <p>Selecione dentre as seguintes opções: </p> 
       <ul> 
      <li> <p> Usuário deve atualizar </p> </li> 
      <li> <p>Assumir no horário </p> </li> 
      <li> <p>Ignorar avisos de atrasos</p> </li> 
      <li> <p> Preencher automaticamente </p> </li> 
      <li> <p>Predecessor </p> </li> 
       </ul> <p>Para obter mais informações sobre o Modo de rastreamento nas tarefas, consulte <a href="../../../manage-work/tasks/task-information/task-tracking-mode.md" class="MCXref xref">Visão geral do modo de rastreamento de tarefas</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Nivelamento de recurso</td> 
      <td> <p>Selecione o <strong>Excluir do Nivelamento de Recursos</strong> se desejar que os recursos atribuídos à tarefa sejam excluídos do nivelamento.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Atraso de Nivelamento</td> 
      <td> <p>Especifique o Atraso de Nivelamento, em horas. </p> <p> Para obter mais informações sobre atrasos de nivelamento, consulte <a href="../../../manage-work/tasks/task-information/task-leveling-delay.md" class="MCXref xref">Atualizar Atraso de Nivelamento de Tarefa</a>. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Processo de aprovação</td> 
      <td> <p>Selecione um processo de aprovação que você deseja associar à tarefa. O administrador do Workfront deve definir Processos de aprovação no nível do sistema antes que você possa associá-los a tarefas. Um usuário com acesso administrativo a processos de aprovação também pode criar processos de aprovação específicos do grupo. </p> <p>Para obter mais informações sobre como criar Processos de Aprovação, consulte <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md">Criar um processo de aprovação para itens de trabalho</a>. Considere o seguinte ao adicionar processos de aprovação: </p> 
       <ul>

   <li> <p>Somente os processos de aprovação ativos são exibidos na lista. </p> </li>

   <li> <p>Os processos de aprovação em todo o sistema e específicos do grupo são exibidos na lista. Um processo de aprovação associado a um grupo diferente do do projeto não é exibido na lista. </p>

   <p><b>IMPORTANTE</b>

   Se o grupo do projeto mudar, o processo de aprovação específico do grupo anexado anteriormente se tornará um processo de aprovação de uso único. Para obter mais informações sobre como as alterações no grupo do projeto ou no processo de aprovação afetam as configurações de aprovação, consulte <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/how-changes-affect-group-approvals.md">Como as alterações de grupo e processo de aprovação afetam os processos de aprovação atribuídos</a>. </p>

   </li>

   <li> <p>Você pode definir processos de aprovação padrão a serem anexados automaticamente a tarefas quando as tarefas forem adicionadas a um projeto. Para obter informações sobre como configurar o projeto para incluir processos de aprovação de tarefas padrão, consulte a seção "Tarefas" no artigo <a href="../../../manage-work/projects/manage-projects/edit-projects.md" class="MCXref xref">Editar projetos</a>. </p> </li>

   <li> <p>Quando tarefas de edição em massa, existem os seguintes cenários: </p> 
      <ul> 
      <li> <p>Ao selecionar várias tarefas do mesmo grupo, os processos de aprovação no nível do sistema e do grupo são exibidos nesse campo. </p> </li> 
      <li> <p>Ao selecionar várias tarefas de grupos diferentes, somente os processos de aprovação no nível do sistema são exibidos nesse campo. </p> </li> 
      <li> <p>Quando qualquer uma das tarefas tiver um processo de aprovação de uso único anexado, ele será substituído pelo processo de aprovação de nível de sistema ou de grupo selecionado. </p> </li>

   </ul> </li> 
      </ul> </td> 
     </tr> 
    </tbody> 
   </table>
    </li>

1. Clique em **Salvar**.

<!--notes from the table: <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this bullet stays here although the sections it might appear in are QS only, so we can use the snippet for both Qs and classic)</p>       -->

## Editar uma tarefa no cabeçalho da tarefa (limitada)

Você pode editar uma quantidade limitada de informações no cabeçalho da tarefa.

O administrador do sistema ou do grupo pode personalizar os campos que você vê no cabeçalho da tarefa. Para obter mais informações, consulte [Personalizar cabeçalhos de objetos usando um modelo de layout](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md).


![](assets/qs-task-header-without-approvals-and-with-dependecies-350x17.png)

Os seguintes campos são incluídos no cabeçalho do projeto, por padrão:

* Nomes da tarefa
* Percentual completo
* Atribuições
* Data e hora de conclusão previstas

   >[!CAUTION]
   >
   >Algumas Restrições de tarefa e outras dependências podem impedir a edição deste campo. Para obter informações sobre Restrições de Tarefa, consulte [Visão geral da restrição de tarefa](../../../manage-work/tasks/task-constraints/task-constraint-overview.md).

* Status
* Tome decisões de aprovação se você estiver definido como aprovador em um processo de aprovação atual

## Editar tarefas em massa

É possível editar tarefas em massa em uma lista e atualizar todas as informações ao mesmo tempo em que você seleciona para salvar automaticamente as alterações que você está fazendo nas tarefas da lista.

Para obter informações sobre como salvar tarefas em massa , consulte a seção &quot;Editar tarefas em massa&quot; no artigo [Editar tarefas em uma lista](../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md).
