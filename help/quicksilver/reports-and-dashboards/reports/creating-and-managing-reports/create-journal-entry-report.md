---
title: Relatório sobre a área Atualizações
description: Relatório sobre a área Atualizações
author: Nolan
draft: Probably
feature: Reports and Dashboards
exl-id: ecf947ce-54d8-4103-8903-f455b1d86c39
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '2698'
ht-degree: 4%

---

# Relatório sobre a área Atualizações

O relatório Entrada do diário exibe atualizações do sistema da área Atualizações de projetos, tarefas, problemas e outros objetos que antes só estavam disponíveis por meio da API do Adobe Workfront. Embora esse seja um relatório avançado destinado a casos de uso específicos, o formato mais digerível facilita o relatório de atividades do projeto e atualizações do sistema no Workfront.

>[!TIP]
>
>O relatório Entrada de Lançamento contém apenas atualizações de sistema da área Atualizações de objetos. Para relatar os comentários deixados na área Atualizações, você deve usar o relatório de Observação .\
>Para obter mais informações sobre o relatório de Nota, consulte [Exibir todas as atualizações em um relatório de Nota](../../../workfront-basics/updating-work-items-and-viewing-updates/view-all-updates-in-a-report.md)‍

O relatório de Lançamento pode mostrar:

* Quantas alterações de status ocorreram
* Quando uma tarefa ou problema foi excluído
* Como os valores em campos personalizados importantes foram alterados durante o ciclo de vida de um projeto
* Que datas importantes mudaram ao longo do ciclo de vida de um projeto
* Se o proprietário de um projeto tiver sido alterado

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
   <td> <p>Plano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a Relatórios, Painéis, Calendários</p> <p>Editar acesso a filtros, visualizações, agrupamentos</p> <p>Observação: Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Exibir permissões para os objetos que contêm os lançamentos exibidos no relatório</p> <p>Você obterá permissões de gerenciamento para o relatório após criá-lo</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

## Pré-requisitos

Antes de executar as ações descritas neste artigo, verifique o seguinte:

* Todos os campos que deseja criar relatórios são rastreados no Workfront. Você só pode relatar dados da área Atualizações que é rastreada.

   Para saber como adicionar campos que você deseja que o Workfront rastreie, consulte [Configurar atualizações do sistema](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md).

* Todos os campos personalizados que você deseja relatar têm a configuração **Exibir alterações de campo em feeds de atualização** habilitado.

   Para saber como ativar essa configuração para um campo personalizado, consulte a seção [Criar ou editar um formulário personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md#create) no artigo [Criar ou editar um formulário personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

## Visão geral do relatório de entrada de diário

Como o relatório de Entrada de Lançamento consulta atualizações do sistema, ele pode retornar um número significativo de resultados. Por esse motivo, recomendamos que você filtre objetos específicos, como projetos, programas, portfólios, grupos e assim por diante, ao criar o relatório.

Para saber mais sobre os diferentes tipos de objetos no Workfront, consulte [Entender objetos no Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

>[!NOTE]
>
>Como o relatório de Lançamento retorna tantos dados, a exportação e a entrega programada de relatórios não são suportadas.

A exibição padrão desse relatório contém as seguintes colunas:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Campo</th> 
   <th>Explicação</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td><strong>Nome do Campo</strong> </td> 
   <td> <p><span style="font-weight: normal;">O nome do campo afetado. Dependendo de como você configurou o relatório, essa coluna pode conter Status, ID do proprietário, Nome da tarefa, Data de conclusão planejada ou outros campos.</span> </p> <p><span style="font-weight: normal;">When</span> <strong>DE</strong>:<span style="font-weight: normal;"> é exibido nessa coluna, indica que o campo listado é um campo personalizado.</span></p> </td> 
  </tr> 
  <tr> 
   <td><strong>Trocar Tipo</strong> </td> 
   <td> <p>O tipo de alteração feita no campo afetado. Dependendo das regras de filtro que você configurou e das ações executadas pelos usuários, o seguinte poderá aparecer neste campo:</p> 
    <ul> 
     <li> <p>Adicionar</p> </li> 
     <li> <p>Auditoria</p> </li> 
     <li> <p>Excluir</p> </li> 
     <li> <p>Resumo</p> </li> 
     <li> <p>Editar</p> </li> 
     <li> <p>Restaurar</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td><strong>Código de Objeto Superior</strong> </td> 
   <td> <p>O objeto pai mais alto na hierarquia.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>Escopo</strong> </td> 
   <td> <p>O tipo de objeto que foi alterado.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>Data de Entrada</strong> </td> 
   <td> <p>A data em que o campo foi alterado.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>Editado por nome</strong> </td> 
   <td> <p>O usuário que alterou o campo.</p> </td> 
  </tr> 
 </tbody> 
</table>

Para organizar as informações neste relatório, você pode usar o Projeto de agrupamento incorporado. O agrupamento Project fornece um agrupamento principal de Nome do Projeto e um agrupamento secundário de Data de Entrada. É possível aplicar esse agrupamento existente durante a criação do relatório ou aplicá-lo durante a visualização do relatório.

Para saber como configurar as exibições, filtros e agrupamentos desejados para o relatório, consulte a seção relevante:

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: from&nbsp;Luke: Take this for what it's worth, but part of me wonders if all of these subsections should be separate articles.</p>
<p>The biggest reason for breaking these up would be searchability, in my mind. For example, as a user, I might want to know how to see if the owner of a project changed. If I search the help site for that, I would be a lot more likely to find a separate article called "See if the owner of a project changed" vs an article titled "Create a Journal Entry report" because "Journal Entry" might mean nothing to me.) </p>
</div>
-->

* [Veja quais alterações de status ocorreram](#see-what-status-changes-occurred)
* [Ver quando uma tarefa ou problema foi excluído](#see-when-a-task-or-issue-was-deleted)
* [Veja como os campos personalizados foram alterados durante o ciclo de vida de um projeto](#see-how-custom-fields-changed-over-the-course-of-a-project-s-life-cycle)
* [Veja como a Data de Conclusão Planejada mudou ao longo do ciclo de vida de um projeto](#see-how-the-planned-completion-date-changed-over-the-course-of-a-project-s-life-cycle)
* [Veja se o proprietário de um projeto foi alterado](#see-if-the-owner-of-a-project-changed)

## Veja quais alterações de status ocorreram {#see-what-status-changes-occurred}

Você pode configurar o relatório de Lançamento para mostrar:

* Quantas alterações de status foram feitas em um projeto, tarefa ou problema

* O status anterior antes da alteração
* Quem alterou o status
* Quando a alteração de status ocorreu

Se você quiser ver a integridade de um projeto, também poderá configurar o relatório para mostrar essas mesmas informações usando o projeto **Condição** campo.

Essas informações podem ser usadas para ajudar com a auditoria e para ilustrar o desempenho do planejamento de você e de sua organização.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;for tip below: When analytics adds the status option, update this note to say "these entries (status or condition changes)")</p>
-->

>[!TIP]
>
>Se quiser comparar a diferença em dias entre as alterações de condição, use a Análise aprimorada.\
>Para saber mais sobre a Análise aprimorada, consulte [Visão geral da análise aprimorada](../../../enhanced-analytics/enhanced-analytics-overview.md).

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront, em seguida, clique em **Relatórios**.
1. Clique em **Novo relatório**, em seguida selecione **Entrada de Diário**.

   ![](assets/nwe-select-journal-entry-350x273.png)

   O construtor de relatórios é carregado.

1. No **Colunas (Exibir)** adicione as seguintes colunas:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>Coluna</th> 
      <th>Explicação</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td> <p style="font-weight: bold;">Nome do Campo</p> </td> 
      <td> <p>O nome do campo afetado. Nesse caso, <strong>status</strong> deve ser exibido nesta coluna.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Trocar Tipo</p> </td> 
      <td> <p>O tipo de alteração feita no campo afetado, como <strong>Adicionar</strong>, <strong>Excluir</strong>ou <strong>Editar</strong>.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Editado por nome</p> </td> 
      <td> <p>O nome do usuário que atualizou o status.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Data de Entrada</p> </td> 
      <td> <p>A data em que o status foi alterado.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Valor Velho de Texto</p> </td> 
      <td> <p>A chave do status anterior. Estas são as chaves de status para os status padrão do projeto:</p> 
       <ul> 
        <li> <p> <strong>CUR</strong>: Atual</p> </li> 
        <li> <p><strong>ADICIONADO</strong>: Morto</p> </li> 
        <li> <p><strong>ONH</strong>: Em Espera</p> </li> 
        <li> <p><strong>PLN</strong>: Planejamento</p> </li> 
        <li> <p><strong>CPL</strong>: Concluído</p> </li> 
        <li> <p><strong>REQ</strong>: Solicitado</p> </li> 
        <li> <p><strong>APR</strong>: Aprovado</p> </li> 
        <li> <p><strong>REJ</strong>: Rejeitada</p> </li> 
        <li> <p><strong>IDA</strong>: Ideia</p> </li> 
       </ul> <p>Se sua organização tiver configurado status personalizados, outras chaves de status poderão aparecer nessa coluna. Para saber qual status personalizado está relacionado a uma chave de status, entre em contato com o administrador do Workfront ou o administrador do grupo.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Novo Valor de Texto</p> </td> 
      <td> <p>A chave para o status atualizado.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Código de Objeto Superior</p> </td> 
      <td> <p>O objeto pai mais alto do campo que teve a alteração de status.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Escopo</p> </td> 
      <td> <p>O tipo de objeto que teve a alteração de status.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Nome do problema<br>(Opcional)</p> </td> 
      <td> <p>O nome do problema que teve uma alteração de status.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Nome da tarefa<br>(Opcional)</p> </td> 
      <td> <p>O nome da tarefa que teve uma alteração de status.</p> </td> 
     </tr> 
    </tbody> 
   </table>

   Para obter mais informações sobre como adicionar colunas, consulte [Visão geral das exibições no Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

1. No **Filtros** clique em **Adicionar regra de filtro**, em seguida, adicione a regra de filtro **Nome do campo** > **Igual** > **status**.

   ![](assets/nwe-journal-entry-status-filter-rules-350x90.png)

   >[!TIP]
   >
   >Para criar relatórios sobre alterações de condição, é possível adicionar a regra de filtro **Nome do campo** > **Igual** > **Condição**.

   Para obter mais informações sobre como adicionar filtros, consulte [Visão geral dos filtros no Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. (Opcional) Para restringir o foco do relatório e reduzir o tempo de carregamento, adicione um prompt.

   Ou

   Crie regras de filtro adicionais para incluir projetos, tarefas ou problemas específicos.

   >[!IMPORTANT]
   >
   >Criando uma regra de filtro que usa o modificador **Contém** na verdade, pode aumentar o tempo de carga. Por isso, recomendamos usar um modificador diferente como **Igual** quando possível, filtrar para um projeto específico ou ID de objeto de nível superior.

   Para saber como adicionar um prompt, consulte [Adicionar um prompt a um relatório](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

1. No **Agrupamentos** clique em **Aplicar um agrupamento existente**, em seguida selecione **Projeto**.

   Para obter mais informações sobre como adicionar agrupamentos, consulte [Visão geral dos agrupamentos no Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

1. Clique em **Salvar + Fechar**.

   O novo relatório é carregado.

## Ver quando uma tarefa ou problema foi excluído {#see-when-a-task-or-issue-was-deleted}

Você pode configurar o relatório de Lançamento para mostrar:

* Quais tarefas ou problemas foram excluídos
* Quem excluiu uma tarefa ou problema

Para ver quando uma tarefa ou problema foi excluído:

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront, em seguida, clique em **Relatórios**.
1. Clique em **Novo relatório**, em seguida selecione **Entrada de Diário**.

   ![](assets/nwe-select-journal-entry-350x273.png)

   O construtor de relatórios é carregado.

1. No **Colunas (Exibir)** adicione as seguintes colunas:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>Coluna</th> 
      <th>Explicação</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td> <p style="font-weight: bold;">Escopo</p> </td> 
      <td> <p>O tipo de objeto que foi excluído.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Trocar Tipo</p> </td> 
      <td> <p>O tipo de mudança que aconteceu. O <strong>Excluir</strong> alterar é exibido nesta coluna.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Data de Entrada</p> </td> 
      <td> <p>A data em que a tarefa ou problema foi excluído.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Editado por nome</p> </td> 
      <td> <p>O nome do usuário que excluiu a tarefa ou problema.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Nome do Projeto</p> </td> 
      <td> <p>O nome do projeto que teve tarefas ou problemas excluídos.</p> </td> 
     </tr> 
    </tbody> 
   </table>

   Para obter mais informações sobre como adicionar colunas, consulte [Visão geral das exibições no Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

1. No **Filtros** clique em **Adicionar regra de filtro** e, em seguida, adicione o seguinte:

   * **Alterar tipo** > **Igual** > **Excluir**
   * **ID do projeto** > **Igual** > **`<project>`**

      <!--WRITER check link; this png file has spaces
     [![](assets/classic-task-or-issue-deleted-350x90.png)](../../../Resources/Images/Reports/Creating and Managing Reports/QS_Task or issue deleted.png)-->
   Para obter mais informações sobre como adicionar filtros, consulte [Visão geral dos filtros no Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. (Opcional) Para restringir o foco do relatório e reduzir o tempo de carregamento, adicione um prompt.

   Ou

   Crie regras de filtro adicionais para incluir projetos, tarefas ou problemas específicos.

   >[!IMPORTANT]
   >
   >Criando uma regra de filtro que usa o modificador **Contém** na verdade, pode aumentar o tempo de carga. Por isso, recomendamos usar um modificador diferente como **Igual** quando possível, filtrar para um projeto específico ou ID de objeto de nível superior.

   Para saber como adicionar um prompt, consulte [Adicionar um prompt a um relatório](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

1. (Opcional) Na seção **Agrupamentos** clique em **Aplicar um agrupamento existente**, em seguida selecione **Projeto**.

   Para obter mais informações sobre como adicionar agrupamentos, consulte [Visão geral dos agrupamentos no Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

1. Clique em **Salvar + Fechar**.

   O novo relatório é carregado.

## Veja como os campos personalizados foram alterados durante o ciclo de vida de um projeto {#see-how-custom-fields-changed-over-the-course-of-a-project-s-life-cycle}

É possível rastrear alterações importantes no campo ao longo do projeto. Para fazer isso, você pode configurar o Lançamento para rastrear:

* Se determinados campos personalizados foram adicionados, atualizados ou editados
* Quando essas alterações ocorreram
* Quem fez as mudanças

Para ver como os campos personalizados foram alterados durante o ciclo de vida de um projeto:

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront, em seguida, clique em **Relatórios**.
1. Clique em **Novo relatório**, em seguida selecione **Entrada de Diário**.

   ![](assets/nwe-select-journal-entry-350x273.png)

   O construtor de relatórios é carregado.

1. No **Colunas (Exibir)** adicione as seguintes colunas:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>Coluna</th> 
      <th>Explicação</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td> <p style="font-weight: bold;">Nome do Campo</p> </td> 
      <td> <p>O nome do campo personalizado afetado.</p> <p><span style="font-weight: normal;">When</span> <strong>DE</strong>:<span style="font-weight: normal;"> é exibido nessa coluna, indica que o campo listado é um campo personalizado.</span></p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Trocar Tipo</p> </td> 
      <td> <p>O tipo de alteração feita no campo afetado, como <strong>Adicionar</strong>, <strong>Excluir</strong>ou <strong>Editar</strong>.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Editado por nome</p> </td> 
      <td> <p>O nome do usuário que atualizou o campo personalizado.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Data de Entrada</p> </td> 
      <td> <p>A data em que o valor no campo personalizado foi alterado.</p> <p>Você deve classificar por este campo em ordem decrescente.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Valor Velho de Número</p> </td> 
      <td> <p>O valor do número anterior no campo personalizado.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Novo Valor de Número</p> </td> 
      <td> <p>O valor do número atual no campo personalizado.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Valor Velho de Data</p> </td> 
      <td> <p>O valor da data anterior no campo personalizado.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Novo Valor de Data</p> </td> 
      <td> <p>O valor da data atual no campo personalizado.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Valor Velho de Texto</p> </td> 
      <td> <p>O valor de texto anterior no campo personalizado.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Novo Valor de Texto</p> </td> 
      <td> <p>O valor de texto atual no campo personalizado.</p> <p>Se o campo personalizado for um campo do tipo , a variável <strong>Novo valor de texto</strong> exibe a ID do objeto.</p> </td> 
     </tr> 
    </tbody> 
   </table>

   Para obter mais informações sobre como adicionar colunas, consulte [Visão geral das exibições no Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

1. No **Filtros** clique em **Adicionar regra de filtro** e, em seguida, adicione o seguinte:

   * **Nome do campo de entrada do diário** > **Contém** > **DE**

      >[!TIP]
      >
      >Para limitar esse relatório a campos personalizados específicos, adicione a regra de filtro **Nome do campo de entrada do diário** > **Igual** > **`<custom field>`**.

   * **ID do projeto** > **Igual** > **`<project>`**

      ![](assets/qs-custom-form-changes-filter-350x92.png)
   Para obter mais informações sobre como adicionar filtros, consulte [Visão geral dos filtros no Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. (Opcional) Para restringir o foco do relatório e reduzir o tempo de carregamento, adicione um prompt.

   Ou

   Crie regras de filtro adicionais para incluir projetos, tarefas ou problemas específicos.

   >[!IMPORTANT]
   >
   >Criando uma regra de filtro que usa o modificador **Contém** na verdade, pode aumentar o tempo de carga. Por isso, recomendamos usar um modificador diferente como **Igual** quando possível, filtrar para um projeto específico ou ID de objeto de nível superior.

   Para saber como adicionar um prompt, consulte [Adicionar um prompt a um relatório](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

1. No **Agrupamentos** clique em **Aplicar um agrupamento existente**, em seguida selecione **Projeto**.

   Para obter mais informações sobre como adicionar agrupamentos, consulte [Visão geral dos agrupamentos no Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

1. Clique em **Salvar + Fechar**.

   O novo relatório é carregado.

## Veja como a Data de Conclusão Planejada mudou ao longo do ciclo de vida de um projeto {#see-how-the-planned-completion-date-changed-over-the-course-of-a-project-s-life-cycle}

Você pode configurar o relatório de Lançamento para mostrar a frequência de alteração da Data de Conclusão Planejada ao longo da vida de um projeto.

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront, em seguida, clique em **Relatórios**.
1. Clique em **Novo relatório**, em seguida selecione **Entrada de Diário**.

   ![](assets/nwe-select-journal-entry-350x273.png)

   O construtor de relatórios é carregado.

1. No **Colunas (Exibir)** adicione as seguintes colunas:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>Coluna</th> 
      <th>Explicação</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td> <p style="font-weight: bold;">Nome do Campo</p> </td> 
      <td> <p>O nome do campo afetado.</p> <p><span style="font-weight: normal;">When</span> <strong>DE</strong>:<span style="font-weight: normal;"> é exibido nessa coluna, indica que o campo listado é um campo personalizado.</span></p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Trocar Tipo</p> </td> 
      <td>O tipo de mudança que ocorreu, como <strong>Adicionar</strong>, <strong>Excluir</strong>ou <strong>Editar</strong>.</td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Editado por nome</p> </td> 
      <td> <p>O nome do usuário que atualizou a Data de conclusão planejada do projeto.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Data de Entrada</p> </td> 
      <td> <p>A data em que a Data de Conclusão Planejada do projeto foi alterada.</p> <p>Você deve classificar por este campo em ordem decrescente.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Código de Objeto Superior</p> </td> 
      <td> <p>O objeto pai mais alto do campo que teve a alteração da Data de Conclusão Planejada.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Escopo</p> </td> 
      <td> <p>O objeto com a alteração da Data de conclusão planejada.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Valor Velho de Data</p> </td> 
      <td> <p>O valor anterior da Data de Conclusão Planejada.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Novo Valor de Data</p> </td> 
      <td> <p>O valor atual da Data de Conclusão Planejada.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Nome do Projeto</p> <p>(Opcional)</p> </td> 
      <td> <p>O nome do projeto que teve a alteração da Data de Conclusão Planejada.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Nome da tarefa</p> <p>(Opcional)</p> </td> 
      <td> <p>O nome das tarefas do projeto que tiveram a alteração da Data de Conclusão Planejada.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Nome do Problema</p> <p>(Opcional)</p> </td> 
      <td>O nome dos problemas do projeto que têm a Data de Conclusão Planejada alterada.</td> 
     </tr> 
    </tbody> 
   </table>

   Para obter mais informações sobre como adicionar colunas, consulte [Visão geral das exibições no Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

1. No **Filtros** clique em **Adicionar regra de filtro** e, em seguida, adicione o seguinte:

   * **Nome do campo** > **Igual** > **Data**
   * **ID do projeto** > **Igual** > **`<project>`**

   ![](assets/qs-planned-completion-date-change-filter-350x91.png)

   Para obter mais informações sobre como adicionar filtros, consulte [Visão geral dos filtros no Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. (Opcional) Para restringir o foco do relatório e reduzir o tempo de carregamento, adicione um prompt.

   Ou

   Crie regras de filtro adicionais para incluir projetos, tarefas ou problemas específicos.

   >[!IMPORTANT]
   >
   >Criando uma regra de filtro que usa o modificador **Contém** na verdade, pode aumentar o tempo de carga. Por isso, recomendamos usar um modificador diferente como **Igual** quando possível, filtrar para um projeto específico ou ID de objeto de nível superior.

   Para saber como adicionar um prompt, consulte [Adicionar um prompt a um relatório](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

1. No **Agrupamentos** clique em **Aplicar um agrupamento existente**, em seguida selecione **Projeto**.

   Para obter mais informações sobre como adicionar agrupamentos, consulte [Visão geral dos agrupamentos no Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

1. Clique em **Salvar + Fechar**.

   O novo relatório é carregado.

## Veja se o proprietário de um projeto foi alterado {#see-if-the-owner-of-a-project-changed}

Você pode configurar o relatório de Lançamento para mostrar quantas vezes o proprietário do projeto, ou o gerente do projeto, muda ao longo da vida de um projeto.

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront, em seguida, clique em **Relatórios**.
1. Clique em **Novo relatório**, em seguida selecione **Entrada de Diário**.

   ![](assets/nwe-select-journal-entry-350x273.png)

   O construtor de relatórios é carregado.

1. No **Colunas (Exibir)** adicione as seguintes colunas:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>Coluna</th> 
      <th>Explicação</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td> <p style="font-weight: bold;">Nome do Campo</p> </td> 
      <td>O nome do campo afetado. O <strong>ownerID</strong> é exibido nesta coluna.</td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Trocar Tipo</p> </td> 
      <td> <p>O tipo de mudança que ocorreu, como <strong>Adicionar</strong>, <strong>Excluir</strong>ou <strong>Editar</strong>.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Código de Objeto Superior</p> </td> 
      <td> <p>O objeto pai mais alto do projeto que teve o proprietário do projeto atualizado.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Data de Entrada</p> </td> 
      <td>A data em que o proprietário do projeto foi alterado.<br>Você deve classificar por este campo em ordem decrescente.</td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Editado por nome</p> </td> 
      <td> <p>O nome do usuário que atualizou o proprietário do projeto.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Informação Adicional 1</p> </td> 
      <td> <p>O proprietário do projeto atual no projeto.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Informação Adicional 2</p> </td> 
      <td> <p>O proprietário do projeto anterior no projeto.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Nome do Projeto</p> </td> 
      <td> <p>O projeto que tinha o campo Proprietário do projeto atualizado.</p> </td> 
     </tr> 
    </tbody> 
   </table>

   Para obter mais informações sobre como adicionar colunas, consulte [Visão geral das exibições no Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

1. No **Filtros** clique em **Adicionar regra de filtro** e, em seguida, adicione o seguinte:

   * **Nome do campo** > **Igual** > **ownerID**
   * **ID do projeto** > **Igual** > **`<project name>`**

      ![](assets/qs-owner-changes-filter-350x94.png)
   Para obter mais informações sobre como adicionar filtros, consulte [Visão geral dos filtros no Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. (Opcional) Para restringir o foco do relatório e reduzir o tempo de carregamento, adicione um prompt.

   Ou

   Crie regras de filtro adicionais para incluir projetos, tarefas ou problemas específicos.

   >[!IMPORTANT]
   >
   >Criando uma regra de filtro que usa o modificador **Contém** na verdade, pode aumentar o tempo de carga. Por isso, recomendamos usar um modificador diferente como **Igual** quando possível, filtrar para um projeto específico ou ID de objeto de nível superior.

   Para saber como adicionar um prompt, consulte [Adicionar um prompt a um relatório](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

1. (Opcional) Na seção **Agrupamentos** clique em **Aplicar um agrupamento existente**, em seguida selecione **Projeto**.

   Para obter mais informações sobre como adicionar agrupamentos, consulte [Visão geral dos agrupamentos no Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

1. Clique em **Salvar + Fechar**.

   O novo relatório é carregado.
