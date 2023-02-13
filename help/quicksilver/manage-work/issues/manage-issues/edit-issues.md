---
product-area: projects
navigation-topic: manage-issues
title: Editar problemas
description: Você pode editar informações sobre problemas que você criou ou que outros usuários criaram se compartilharam os problemas com você.
author: Alina
feature: Work Management
exl-id: 1449374a-ab0d-4c98-83cd-4e511467633a
source-git-commit: 3f5e5e9832fc33d39ea5dfbbc513b80adbf113f5
workflow-type: tm+mt
source-wordcount: '2424'
ht-degree: 3%

---

# Editar problemas

Você pode editar informações sobre problemas que você criou ou que outros usuários criaram se compartilharam os problemas com você.

É possível editar um único problema ou editar problemas em uma lista. Para obter informações sobre edição de problemas em uma lista, consulte [Editar problemas em uma lista](../../../manage-work/issues/manage-issues/edit-issues-in-a-list.md).

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
   <td> <p>Solicitação ou superior</p> <p>Revisar ou obter uma licença superior para editar problemas na seção Problemas de uma tarefa ou projeto</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Nível de acesso*</td> 
   <td> <p>Editar acesso a problemas</p> <p><b>Nota</b>

Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre o acesso a problemas no Nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">Conceder acesso a problemas</a>. Para obter informações sobre como um administrador do Workfront pode alterar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>. </p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Contribua com permissões para um problema para editá-lo na área Detalhes do problema </p> <p>Gerencie permissões a um problema para editá-lo na caixa Editar problema</p> <p> Para obter informações sobre a concessão de permissões para problemas, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Compartilhar um problema </a></p> <p>Para obter informações sobre a solicitação de permissões adicionais, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

## Limitações ao editar problemas

Há algumas limitações que podem impedir problemas de edição.

* Não é possível editar problemas que estão em um Processo de Aprovação. Você só pode registrar tempo ou atualizar o status em um problema que esteja na Aprovação pendente.
* Você pode editar e adicionar documentos a problemas em um projeto que tenha o status Concluído, Inativo ou Pendente de Aprovação somente quando o administrador do Workfront ou um administrador de grupo ativou essa funcionalidade na área Preferências do projeto. Para obter informações sobre como definir preferências de projeto, consulte [Configurar preferências de projeto em todo o sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

## Editar um único problema

É possível editar um problema usando as áreas Editar ocorrência ou Detalhes da ocorrência . As etapas a seguir descrevem como editar um problema na caixa Editar edição .

1. Vá para o **Menu principal**.
1. Clique em **Projetos**, em seguida, clique no nome de um projeto para abri-lo.
1. (Opcional) Clique em **Tarefas** e, em seguida, clique no nome de uma tarefa para abri-la.
1. Clique em **Problemas** no painel esquerdo.

   ![](assets/qs-issues-icon-highlighted-on-project-350x278.png)

1. (Opcional) Para editar informações limitadas sobre um problema, clique em **Detalhes do problema** no painel esquerdo.

   ![](assets/qs-issue-details-icon-highlighted-and-expanded-on-issue-350x206.png)

   >[!NOTE]
   >
   >Dependendo de como o administrador do Workfront ou o administrador do Grupo modificou seu Modelo de layout, os campos na área Detalhes da ocorrência podem ser reorganizados ou não serem exibidos. Para obter mais informações, consulte [Personalizar a visualização de Detalhes usando um modelo de layout](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

   Para editar informações na seção Detalhes, faça o seguinte:

   1. (Opcional) Clique no botão **Recolher Tudo** ícone no canto superior direito para recolher todas as áreas.
   1. (Opcional e condicional) Quando uma área for recolhida, clique no botão **seta apontando para a direita** ![](assets/right-pointing-arrow.png) ao lado de cada área para expandir a área que você deseja editar.
   1. (Opcional) Para anexar um formulário personalizado, comece a digitar o nome de um formulário no **Adicionar formulário personalizado** , selecione-o quando for exibido na lista e clique em **Salvar alterações**.
   1. (Opcional) Clique no botão **Exportar** ícone ![](assets/export.png) para exportar as informações de formulários personalizados e Visão geral para um arquivo PDF, clique em **Exportar**. Selecione uma das opções a seguir:

      * Selecionar tudo (é exibido somente quando há pelo menos um formulário personalizado anexado)
      * Visão geral
      * O nome de um ou vários formulários personalizados

      O arquivo PDF é baixado para o computador.

      ![](assets/export-issue-details-selection-box-with-export-button-350x418.png)

      Para obter mais informações, consulte [Exportar formulários personalizados e detalhes do objeto](../../../workfront-basics/work-with-custom-forms/export-custom-forms-details.md).
   Para obter informações sobre os campos visíveis na seção Detalhes da ocorrência, continue editando o problema na caixa Editar edição , conforme descrito abaixo.

1. Para editar todas as informações sobre um problema, selecione um problema em uma lista e clique em **Editar** na parte superior da lista

   Ou

   Clique no nome de um problema em uma lista e, em seguida, clique no botão **Mais** ao lado do nome do problema, em seguida **Editar.**

   O **Editar problema** será exibida.

   >[!IMPORTANT]
   >
   >Você deve ter permissões de gerenciamento para visualizar o link Editar .

   Todos os campos de edição estão disponíveis na caixa Editar problema e são agrupados pelas áreas listadas no painel esquerdo.

1. Considere especificar informações em qualquer uma das seguintes seções:

   * [Nome do Problema](#issue-name)
   * [Visão geral](#overview)
   * [Atribuições](#assignments)
   * [Formulários personalizados](#Custom%C2%A0F)
   * [Configurações](#settings)

   >[!NOTE]
   >
   >Dependendo de como o administrador do Workfront configurar o Modelo de layout, os campos na caixa Editar ocorrência podem ser diferentes no seu ambiente. Para obter mais informações, consulte [Personalizar a visualização de Detalhes usando um modelo de layout](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

### Nome do Problema {#issue-name}

1. Comece a editar um problema conforme descrito acima.
1. Clique em **Nome do problema**.

   ![](assets/issue-name-section-edit-issue-box-nwe-350x127.png)

1. Atualize o **Nome do problema** campo.
1. Clique em **Salvar** ou continue editando as seções a seguir.

### Visão geral {#overview}

1. Comece a editar um problema conforme descrito acima.
1. Clique em **Visão geral**.

   ![](assets/overview-section-edit-issue-box-nwe-350x284.png)

1. Atualize ou revise qualquer um dos campos na tabela a seguir:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Descrição</td> 
      <td> <p>Adicione mais informações sobre o problema.</p> </td> 
     </tr> 
     <tr> 
      <td colspan="2" role="rowheader">Seção Informações básicas</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Status</td> 
      <td> <p>Selecione o status do problema. Para obter mais informações sobre status de problemas, consulte <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md" class="MCXref xref">Acesse a lista de status de problemas do sistema</a>. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Prioridade</td> 
      <td> <p>Esse é um sinalizador visual para você, que permite priorizar problemas.</p> <p>Selecione dentre as seguintes opções:</p> 
       <ul> 
        <li> <p><strong>Nenhum(a)</strong> </p> </li> 
        <li> <p><strong>Baixa</strong> </p> </li> 
        <li> <p><strong>Normal</strong> </p> </li> 
        <li> <p><strong>Alta</strong> </p> </li> 
        <li> <p><strong>Urgente</strong> </p> </li> 
       </ul> <p>Dependendo das Preferências do projeto selecionadas pelo administrador do Workfront, os nomes das prioridades podem ser diferentes para você. Para obter mais informações sobre como editar prioridades, consulte <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-customize-priorities.md" class="MCXref xref">Criar e personalizar prioridades</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Severidade</td> 
      <td> <p>Esse é um sinalizador visual para você que indica a gravidade do problema descrito no problema. As severidades são específicas para problemas. Selecione dentre as seguintes opções:</p> 
       <ul> 
        <li> <p style="font-weight: bold;">Cosmética</p> </li> 
        <li> <p style="font-weight: bold;">Causa Confusão</p> </li> 
        <li> <p style="font-weight: bold;">Problema com Solução</p> </li> 
        <li> <p style="font-weight: bold;">Problema Sem Solução</p> </li> 
        <li> <p style="font-weight: bold;">Erro Fatal</p> </li> 
       </ul> <p>Dependendo das Preferências do projeto selecionadas pelo administrador do Workfront, os nomes de gravidade podem ser diferentes para você. Para obter mais informações sobre edição de severidades, consulte <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-customize-issue-severities.md" class="MCXref xref">Criar ou personalizar severidades de problemas</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">URL</td> 
      <td> <p>Digite um link da Web que esteja relacionado às informações sobre o problema.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tipo</td> 
      <td> <p>De acordo com as Propriedades da fila selecionadas pelo gerente do projeto na área Detalhes da fila do projeto, talvez seja possível especificar o tipo da ocorrência. Selecione dentre as seguintes opções no <b>Tipo</b> menu suspenso: </p> 
       <ul> 
        <li> <p><strong>Registro de Defeito</strong> </p> </li> 
        <li> <p><strong>Pedido de alteração</strong> </p> </li> 
        <li> <p><strong>Problema</strong> </p> </li> 
        <li> <p><strong>Solicitar</strong> </p> </li> 
       </ul> <p>Dependendo das Preferências do projeto selecionadas pelo administrador do Workfront, os nomes dos tipos de problemas podem ser diferentes para você.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Contato Primário</td> 
      <td>Por padrão, o Contato principal é o criador do problema. Para modificar isso, comece a digitar o nome de qualquer usuário ativo no Workfront e selecione-o na lista. Um problema pode ter apenas um Contato Principal.<br> Se você alterar o Contato principal, o contato principal original ainda terá acesso de Gerenciar ao problema. Você deve remover manualmente esse acesso da caixa Acesso a Problemas ao compartilhar um problema.

   <b>DICA</b>

   Ao adicionar um usuário do Contato principal, observe o avatar, a função principal do usuário e seu endereço de email para distinguir entre usuários com nomes idênticos. Os usuários devem estar associados a pelo menos uma função de trabalho para exibi-la à medida que você os adiciona.


   </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Data e hora da confirmação</td> 
      <td> <p>Esta é a data em que o destinatário da emissão estima que a emissão será concluída. Somente as pessoas atribuídas podem editar este campo.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Data de início planejada</td> 
      <td>Por padrão, a Data inicial planejada é a data e a hora em que o problema foi criado. Você pode atualizar o <strong>Data de início planejada</strong> do problema. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Data e hora de conclusão previstas</td> 
      <td> Por padrão, a Data de conclusão planejada é de 24 horas a partir da Data de início planejada padrão. Por padrão, os problemas têm uma Duração de 1 dia. Você pode atualizar o <strong>Data de Conclusão Planejada</strong> do problema.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Data e hora de início reais</td> 
      <td>A Data de início real é automaticamente preenchida quando você altera o status do problema para <strong>Em Andamento</strong>. Você pode atualizar o <strong>Data de início real</strong> do problema. Você pode atualizar manualmente a data, se necessário. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Data e hora de conclusão real</td> 
      <td>A Data de Conclusão Real é automaticamente preenchida quando você altera o status do problema para <strong>Fechado</strong> ou<strong>Resolvido</strong>. Você pode atualizar o <strong>Data de conclusão real</strong> para o problema. Você pode atualizar manualmente a data, se necessário.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Resolvido por</td> 
      <td> <p>Isso mostra se o problema foi resolvido por outro objeto. Você pode selecionar se esse problema é resolvido por uma tarefa, um projeto ou outro problema no menu suspenso e começar a digitar o nome da tarefa, do projeto ou do problema que resolverá o problema. Selecione-o quando aparecer na lista.</p>

   <b>Nota</b>

   Quando você seleciona um objeto para resolver um problema, o status do problema é vinculado ao status do objeto que está resolvendo e não pode ser alterado no problema. Para obter mais informações sobre como resolver objetos, consulte <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">Visão Geral da Solução e Objetos Resolvíveis </a>.

   <b>DICA</b>

   Quando o administrador do sistema ou do grupo adiciona o campo &quot;Resolvido por&quot; a um cabeçalho personalizado de problema, o campo muda para &quot;Resolvendo problema&quot;, &quot;Resolvendo tarefa&quot; ou &quot;Resolvendo projeto&quot; quando há um objeto de resolução associado ao problema.

   Não é possível editar esse campo quando ele é exibido no cabeçalho da ocorrência. Para obter mais informações sobre como personalizar cabeçalhos de problemas, consulte <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md">Personalizar cabeçalhos de objetos usando um modelo de layout </a>
   </td> 
     </tr>

   <tr> 
      <td role="rowheader">Resolvendo problemas, solucionando tarefas ou solucionando projetos</td> 
      <td>O nome vinculado do problema, tarefa ou problema que resolve o problema.  </td> 
     </tr> 
      <tr> 
      <td role="rowheader">Isso resolve</td> 
      <td>O nome vinculado do problema que é concluído quando o problema que você está acessando é resolvido.  </td> 
     </tr>


   </tbody> 
   </table>





1. Clique em **Salvar** ou continue editando as seções a seguir.

#### Atribuições {#assignments}

1. Comece a editar o problema conforme descrito acima.
1. Clique em **Atribuições** no painel esquerdo.

   ![](assets/assignments-section-edit-issue-box-nwe-350x230.png)

1. Clique em **Pesquisar pessoas, funções e equipes** e comece a digitar o nome de um usuário, função ou equipe que deseja atribuir à tarefa, em seguida, clique nela ou pressione Enter quando ela for exibida na lista.

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ensure this is still called this; asked Anna to change it to "roles" and add a comma)</p>
   -->

   >[!NOTE]
   >
   >Se o nome do usuário contiver um caractere especial, você deverá incluir o caractere especial no campo de pesquisa.

   >[!TIP]
   >
   >Você pode atribuir vários usuários, funções de trabalho ou equipes. Você pode atribuir somente usuários ativos, funções de trabalho e equipes.
   >
   >
   >Se um usuário, uma função de trabalho ou uma equipe tiver sido atribuída antes de ser desativada, ela permanecerá atribuída ao item de trabalho. Nesse caso, recomendamos o seguinte:
   >
   >* Atribua novamente o item de trabalho aos recursos ativos.
   >* Associe os usuários em uma equipe desativada a uma equipe ativa e reatribua o item de trabalho à equipe ativa.


1. (Opcional) Indique se um destinatário é o destinatário principal do problema, passando o mouse sobre o nome do destinatário e clicando em **Tornar principal**. Uma equipe não pode ser o principal destinatário de um problema.
1. Atualize os seguintes campos:

   <table style="table-layout:auto"> 
    <col> 
    </col> 
    <col> 
    </col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Horas planejadas</td> 
      <td> <p>Essa é a quantidade de tempo real que os destinatários do problema levariam para concluí-lo. Digite o número de Horas Planejadas para o problema.<br></p> <p>Observação: Alterar as Horas Planejadas do problema não altera a Data de Conclusão Planejada. </p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Função do atribuidor</td> 
      <td> <p>Selecione uma função no <strong>Função do destinatário</strong> menu suspenso ao selecionar uma pessoa como destinatário. Esta é a função que o destinatário pode desempenhar nesta questão. </p> <p><b>DICA</b>

   Somente as funções de trabalho associadas a cada destinatário em seu perfil aparecem no menu suspenso.</p> </td>
   </tr> 
    </tbody> 
   </table>

1. Clique em **Salvar** ou continue editando as seções a seguir.

### Forms personalizada

1. Comece a editar um problema conforme descrito acima.
1. Clique em **Forms personalizada**.

   ![](assets/custom-forms-section-edit-issue-box-nwe-350x132.png)

1. No **Adicionar formulário personalizado** selecione o formulário ou formulários personalizados que deseja associar ao problema. Você deve criar os formulários personalizados antes que eles estejam disponíveis para seleção neste campo. Somente os formulários personalizados ativos são exibidos na lista. Para obter mais informações sobre como criar formulários personalizados, consulte [Criar ou editar um formulário personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md). É possível adicionar até dez formulários personalizados a um problema.

1. (Condicional) Se você anexou um formulário personalizado ao problema, edite quaisquer campos no formulário. Você deve especificar todos os campos obrigatórios antes de poder salvar o problema.

   >[!NOTE]
   >
   >Dependendo de como o Administrador do Workfront definiu as permissões para as seções em seu formulário personalizado, nem todos podem exibir ou editar os mesmos campos em um determinado formulário personalizado. As permissões para editar campos em uma seção de um formulário personalizado dependem das permissões que você tem sobre o problema em si. Para obter informações sobre como configurar permissões em seções de um formulário personalizado, consulte [Criar ou editar um formulário personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md). Para obter informações sobre como definir permissões de problemas, consulte [Compartilhar um problema](../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md).

1. Clique em **Salvar** ou continue editando a seguinte seção.

### Configurações {#settings}

1. Comece a editar um problema conforme descrito acima.
1. Clique em **Configurações**.

   ![](assets/settings-section-edit-issue-box-nwe-350x240.png)

   Atualize as seguintes informações:

   <table style="table-layout:auto"> 
    <col> 
    </col> 
    <col> 
    </col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Processo de aprovação</td> 
      <td> 
       <div> 
       <p>Selecione um processo de aprovação que você deseja associar ao problema. O administrador do Workfront deve definir Processos de aprovação no nível do sistema antes que você possa associá-los a problemas. Usuários com acesso administrativo aos processos de aprovação <span> O também pode criar processos de aprovação específicos de grupo.</span>Para obter mais informações sobre como criar Processos de Aprovação, consulte <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md" class="MCXref xref">Criar um processo de aprovação para itens de trabalho</a>. </p> 
       <p>Considere o seguinte ao adicionar processos de aprovação: </p> 
       <ul> 
       <li>Somente os processos de aprovação ativos são exibidos na lista. </li> 
       <li> <p>Os processos de aprovação em todo o sistema e específicos do grupo são exibidos na lista. Um processo de aprovação associado a um grupo diferente do do projeto não é exibido na lista.</p> <p>Importante: Se o grupo do projeto mudar, o processo de aprovação específico do grupo se tornará um processo de aprovação de uso único. Para obter mais informações sobre como as alterações no grupo do projeto ou no processo de aprovação afetam as configurações de aprovação, consulte <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/how-changes-affect-group-approvals.md" class="MCXref xref">Como as alterações de grupo e processo de aprovação afetam os processos de aprovação atribuídos</a>. </p> </li> 
       <li> <p>Você pode definir processos de aprovação padrão a serem anexados automaticamente a problemas ao criar filas de solicitação ou Tópicos da fila. Para obter informações sobre como atualizar Detalhes da fila, consulte <a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">Criar uma fila de solicitações</a>. Para obter informações sobre como criar tópicos da fila, consulte <a href="../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md" class="MCXref xref">Criar Tópicos da Fila</a>. </p> </li> 
       <li>Quando há problemas de edição em massa, os seguintes cenários existem: 
       <ul> 
       <li><p>Ao selecionar vários problemas do mesmo grupo, os processos de aprovação de nível de sistema e específicos do grupo são exibidos nesse campo.</p></li> 
       <li><p>Ao selecionar vários problemas de grupos diferentes, somente os processos de aprovação no nível do sistema serão exibidos nesse campo.</p></li> 
       <li><p>Quando qualquer um dos problemas tiver um processo de aprovação de uso único anexado, ele será substituído pelo processo de aprovação no nível do sistema ou do grupo selecionado. </p></li> 
       </ul></li> 
       </ul> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Notificações de Lembrete</td> 
      <td> <p>Marque a caixa de seleção à qual as Notificações de lembrete você gostaria de anexar a esse problema. Todas as notificações de lembrete de problemas são exibidas. O administrador do Workfront deve configurar as Notificações de lembrete antes de selecioná-las em um problema. Para obter mais informações sobre como configurar as Notificações do Lembrete, consulte <a href="../../../administration-and-setup/manage-workfront/emails/set-up-reminder-notifications.md" class="MCXref xref">Configurar notificações de lembrete</a></p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Clique em **Salvar.**

## Editar um problema no cabeçalho da edição (limitado)

Você pode editar uma quantidade limitada de informações no cabeçalho da edição.

O administrador do sistema ou do grupo pode personalizar os campos que você vê no cabeçalho do problema. Para obter mais informações, consulte [Personalizar cabeçalhos de objetos usando um modelo de layout](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md).

![](assets/issue-header-350x19.png)

Os seguintes campos são incluídos no cabeçalho da ocorrência, por padrão:

* Nome do problema
* Percentual completo
* Atribuições
* Data e hora de conclusão previstas
* Status
* Tome decisões de aprovação se você estiver definido como aprovador em um processo de aprovação atual
