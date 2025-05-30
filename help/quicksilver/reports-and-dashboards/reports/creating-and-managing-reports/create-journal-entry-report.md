---
title: Relatório sobre a Área Atualizações com um Relatório de Lançamento
description: O relatório de Lançamento documentado revela atualizações de sistema da área Atualizações de projetos, tarefas, problemas e outros objetos que antes só estavam disponíveis por meio da API do Adobe Workfront. Embora este seja um relatório avançado destinado a casos de uso específicos, o formato mais simples facilita a criação de relatórios sobre atividades de projeto e atualizações de sistema no Workfront.
author: Nolan
draft: Probably
feature: Reports and Dashboards
exl-id: ecf947ce-54d8-4103-8903-f455b1d86c39
source-git-commit: 577761ff5d1fb59db104df5995af953a0b5e6c0c
workflow-type: tm+mt
source-wordcount: '2771'
ht-degree: 4%

---

# Relatório na área Atualizações com um relatório de Lançamento

<!-- Audited: 11/2024 -->

O relatório de Lançamento documentado revela atualizações de sistema da área Atualizações de projetos, tarefas, problemas e outros objetos que antes só estavam disponíveis por meio da API do Adobe Workfront. Embora este seja um relatório avançado destinado a casos de uso específicos, o formato mais simples facilita a criação de relatórios sobre atividades de projeto e atualizações de sistema no Workfront.

>[!TIP]
>
>O relatório de Lançamento contém somente atualizações de sistema da área Atualizações de objetos. Para relatar comentários deixados na área Atualizações, é necessário usar o relatório de Notas.\
>Para obter mais informações sobre o relatório de Anotações, consulte [Exibir todas as atualizações em um relatório de Anotações](../../../workfront-basics/updating-work-items-and-viewing-updates/view-all-updates-in-a-report.md).‍

O relatório de Lançamento pode mostrar:

* Quantas alterações de status ocorreram
* Quando uma tarefa ou problema é excluído
* Como os valores em campos personalizados importantes foram alterados durante o ciclo de vida de um projeto
* Quais datas importantes mudaram ao longo do ciclo de vida de um projeto
* Se o proprietário de um projeto mudou

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
      <td> 
      <p>Novo:</p>
         <ul>
         <li><p>Padrão</p></li>
         </ul>
      <p>Atual:</p>
         <ul>
         <li><p>Plano</p></li>
         </ul>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Editar acesso a relatórios, painéis, calendários</p> <p>Editar acesso a Filtros, Visualizações, Agrupamentos</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Exibir permissões para os objetos que contêm as entradas do diário exibidas no relatório</p> <p>Você obterá permissões de gerenciamento para o relatório após criá-lo</p> </td> 
  </tr> 
 </tbody> 
</table>

*Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Pré-requisitos

Antes de executar as ações descritas neste artigo, verifique o seguinte:

* Todos os campos (incluindo campos personalizados) que você deseja relatar são rastreados no Workfront. Você só pode criar relatórios sobre dados da área Atualizações que é rastreada.

  Para saber como adicionar campos que você deseja que o Workfront rastreie, consulte [Configurar atualizações do sistema](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md).

## Visão geral do relatório de Lançamento

Como o relatório de Lançamento consulta atualizações do sistema, ele pode retornar um número significativo de resultados. Por esse motivo, recomendamos que você filtre por objetos específicos (como projetos, programas, portfólios, grupos e assim por diante) ao criar o relatório.

Para saber mais sobre os diferentes tipos de objetos no Workfront, consulte [Entender os objetos no Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

>[!NOTE]
>
>Como o relatório de Lançamento retorna muitos dados, a exportação e a entrega programada de relatórios não são suportadas.

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
   <td> <p><span style="font-weight: normal;">O nome do campo afetado. Dependendo de como você configura o relatório, esta coluna pode conter Status, ID do Proprietário, Nome da Tarefa, Data de Conclusão Planejada ou outros campos.</span> </p> <p><span style="font-weight: normal;">Quando</span> <strong>DE</strong>:<span style="font-weight: normal;"> é exibido nesta coluna, indica que o campo listado é um campo personalizado.</span></p> </td> 
  </tr> 
  <tr> 
   <td><strong>Tipo de alteração</strong> </td> 
   <td> <p>O tipo de alteração feita no campo afetado. Dependendo das regras de filtro configuradas e das ações executadas pelos usuários, o seguinte poderá aparecer neste campo:</p> 
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
   <td><strong>Top ObjCode</strong> </td> 
   <td> <p>O objeto pai mais alto na hierarquia.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>Escopo</strong> </td> 
   <td> <p>O tipo de objeto que foi alterado.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>Data de entrada</strong> </td> 
   <td> <p>A data em que o campo foi alterado.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>Editado por Nome</strong> </td> 
   <td> <p>O usuário que alterou o campo.</p> </td> 
  </tr> 
 </tbody> 
</table>

Para organizar as informações neste relatório, você pode usar o agrupamento incorporado chamado Projeto. O agrupamento de Projeto fornece um agrupamento principal de Nome do Projeto e um agrupamento secundário de Data de Entrada. Você pode aplicar esse agrupamento existente durante a criação do relatório ou pode aplicá-lo ao exibir o relatório.

Para saber como configurar as exibições, os filtros e os agrupamentos desejados para o relatório, consulte a seção relevante:

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: from&nbsp;Luke: Take this for what it's worth, but part of me wonders if all of these subsections should be separate articles.</p>
<p>The biggest reason for breaking these up would be searchability, in my mind. For example, as a user, I might want to know how to see if the owner of a project changed. If I search the help site for that, I would be a lot more likely to find a separate article called "See if the owner of a project changed" vs an article titled "Create a Journal Entry report" because "Journal Entry" might mean nothing to me.) </p>
</div>
-->

* [Veja quais alterações de status ocorreram](#see-what-status-changes-occurred)
* [Veja quando uma tarefa ou problema foi excluído](#see-when-a-task-or-issue-was-deleted)
* [Veja como os campos personalizados foram alterados durante o ciclo de vida de um projeto](#see-how-custom-fields-changed-over-the-course-of-a-project-s-life-cycle)
* [Veja como a Data de Conclusão Planejada mudou durante o ciclo de vida de um projeto](#see-how-the-planned-completion-date-changed-over-the-course-of-a-project-s-life-cycle)
* [Veja se o proprietário de um projeto mudou](#see-if-the-owner-of-a-project-changed)

## Ver quais alterações de status ocorreram {#see-what-status-changes-occurred}

Você pode configurar o relatório de Lançamento para mostrar:

* Quantas alterações de status foram feitas em um projeto, tarefa ou problema

* Qual era o status anterior antes da alteração?
* Quem alterou o status
* Quando ocorreu a alteração de status

Se quiser ver a integridade de um projeto, você também pode configurar o relatório para mostrar essas mesmas informações usando o campo **Condição** do projeto.

Essas informações podem ser usadas para ajudar na auditoria e ilustrar o desempenho do planejamento de você e de sua organização.

1. Clique no ícone **[!UICONTROL Menu Principal]** ![Menu Principal](/help/_includes/assets/main-menu-icon.png) no canto superior direito do Adobe Workfront ou (se disponível) clique no ícone **[!UICONTROL Menu Principal]** ![Menu Principal](/help/_includes/assets/main-menu-icon-left-nav.png) no canto superior esquerdo e clique em **Relatórios**.
1. Clique em **Novo Relatório** e selecione **Entrada do Diário**.

   ![Selecionar entrada do diário](assets/nwe-select-journal-entry-350x273.png)

   O Report Builder é carregado.

1. Na guia **Colunas (Modo de Exibição)**, adicione as seguintes colunas:

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
      <td> <p>O nome do campo afetado. Nesse caso, o <strong>status</strong> deve ser exibido nesta coluna.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Trocar Tipo</p> </td> 
      <td> <p>O tipo de alteração feita no campo afetado, como <strong>Adicionar</strong>, <strong>Excluir</strong> ou <strong>Editar</strong>.</p> </td> 
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
      <td> <p>A chave para o status anterior. A seguir estão as chaves de status para os status padrão do projeto:</p> 
       <ul> 
        <li> <p> <strong>CUR</strong>: atual</p> </li> 
        <li> <p><strong>DED</strong>: inativo</p> </li> 
        <li> <p><strong>ONH</strong>: Em espera</p> </li> 
        <li> <p><strong>PLN</strong>: Planejamento</p> </li> 
        <li> <p><strong>CPL</strong>: Concluído</p> </li> 
        <li> <p><strong>REQ</strong>: Solicitado</p> </li> 
        <li> <p><strong>ABR</strong>: aprovado</p> </li> 
        <li> <p><strong>REJ</strong>: rejeitado</p> </li> 
        <li> <p><strong>IDA</strong>: ideia</p> </li> 
       </ul> <p>Se sua organização tiver configurado status personalizados, outras chaves de status poderão ser exibidas nessa coluna. Para saber qual status personalizado está relacionado a uma chave de status, entre em contato com o administrador do Workfront ou com o administrador de grupo.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Novo Valor de Texto</p> </td> 
      <td> <p>A chave para o status atualizado.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Código de objeto principal
</p> </td> 
      <td> <p>O objeto pai mais alto do campo que teve a alteração de status.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Escopo</p> </td> 
      <td> <p>O tipo de objeto que teve a alteração de status.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Nome do Problema<br>(Opcional)</p> </td> 
      <td> <p>O nome da ocorrência que teve uma alteração de status.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Nome da Tarefa<br>(Opcional)</p> </td> 
      <td> <p>O nome da tarefa que teve uma alteração de status.</p> </td> 
     </tr> 
    </tbody> 
   </table>

   Para obter mais informações sobre como adicionar colunas, consulte [Visão geral das exibições no Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

1. Na guia **Filtros**, clique em **Adicionar uma Regra de Filtro** e adicione a regra de filtro **Nome do Campo** > **Igual** > **status**.

   ![Filtro de status de entrada do diário](assets/nwe-journal-entry-status-filter-rules-350x90.png)

   >[!TIP]
   >
   >Para relatar alterações de condição, você pode adicionar a regra de filtro **Nome do Campo** > **Igual** > **Condição**.

   Para obter mais informações sobre como adicionar filtros, consulte [Visão geral dos filtros](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. (Opcional) Para restringir o foco do relatório e reduzir os tempos de carregamento, adicione um prompt.

   Ou

   Crie regras de filtro adicionais para incluir projetos, tarefas ou problemas específicos.

   >[!IMPORTANT]
   >
   >Criar uma regra de filtro que use o modificador **Contains** pode realmente aumentar os tempos de carregamento. Por isso, recomendamos usar um modificador diferente como **Equal** quando possível para filtrar por um projeto específico ou ID de objeto de nível superior.

   Para saber como adicionar um prompt, consulte [Adicionar um prompt a um relatório](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

1. Na guia **Agrupamentos**, clique em **Aplicar um Agrupamento Existente** e selecione **Projeto**.

   Para obter mais informações sobre como adicionar agrupamentos, consulte [Visão geral dos agrupamentos no Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

1. Clique em **Salvar + Fechar**.

   O novo relatório é carregado.

## Veja quando uma tarefa ou problema foi excluído {#see-when-a-task-or-issue-was-deleted}

Você pode configurar o relatório de Lançamento para mostrar:

* Quais tarefas ou problemas foram excluídos
* Quem excluiu uma tarefa ou problema

Para ver quando uma tarefa ou problema foi excluído:

1. Clique no ícone **[!UICONTROL Menu Principal]** ![Menu Principal](/help/_includes/assets/main-menu-icon.png) no canto superior direito do Adobe Workfront ou (se disponível) clique no ícone **[!UICONTROL Menu Principal]** ![Menu Principal](/help/_includes/assets/main-menu-icon-left-nav.png) no canto superior esquerdo e clique em **Relatórios**.
1. Clique em **Novo Relatório** e selecione **Entrada do Diário**.

   ![Selecionar entrada do diário](assets/nwe-select-journal-entry-350x273.png)

   O Report Builder é carregado.

1. Na guia **Colunas (Modo de Exibição)**, adicione as seguintes colunas:

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
      <td> <p>O tipo de mudança que ocorreu. A alteração <strong>Excluir</strong> é exibida nesta coluna.</p> </td> 
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

1. Na guia **Filtros**, clique em **Adicionar regra de filtro** e adicione os seguintes filtros:

   * **Tipo de Alteração** > **Igual** > **Excluir**
   * **ID do Projeto** > **Igual** > **&lt; nome do projeto >**

     <!--WRITER check link; this png file has spaces
     [![Task or issue deleted](assets/classic-task-or-issue-deleted-350x90.png)](../../../Resources/Images/Reports/Creating and Managing Reports/QS_Task or issue deleted.png)-->

   Para obter mais informações sobre como adicionar filtros, consulte [Visão geral dos filtros](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. (Opcional) Para restringir o foco do relatório e reduzir os tempos de carregamento, adicione um prompt.

   Ou

   Crie regras de filtro adicionais para incluir projetos, tarefas ou problemas específicos.

   >[!IMPORTANT]
   >
   >Criar uma regra de filtro que use o modificador **Contains** pode realmente aumentar os tempos de carregamento. Por isso, recomendamos usar um modificador diferente como **Equal** quando possível para filtrar por um projeto específico ou ID de objeto de nível superior.

   Para saber como adicionar um prompt, consulte [Adicionar um prompt a um relatório](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

1. (Opcional) Na guia **Agrupamentos**, clique em **Aplicar um Agrupamento Existente** e selecione **Projeto**.

   Para obter mais informações sobre como adicionar agrupamentos, consulte [Visão geral dos agrupamentos no Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

1. Clique em **Salvar + Fechar**.

   O novo relatório é carregado.

## Veja como os campos personalizados foram alterados durante o ciclo de vida de um projeto {#see-how-custom-fields-changed-over-the-course-of-a-project-s-life-cycle}

É possível rastrear alterações importantes de campo ao longo do projeto. Para fazer isso, você pode configurar o Lançamento para rastrear:

* Se determinados campos personalizados foram adicionados, atualizados ou editados
* Quando essas mudanças ocorreram
* Quem fez as alterações

Para ver como os campos personalizados foram alterados durante o ciclo de vida de um projeto:

1. Clique no ícone **[!UICONTROL Menu Principal]** ![Menu Principal](/help/_includes/assets/main-menu-icon.png) no canto superior direito do Adobe Workfront ou (se disponível) clique no ícone **[!UICONTROL Menu Principal]** ![Menu Principal](/help/_includes/assets/main-menu-icon-left-nav.png) no canto superior esquerdo e clique em **Relatórios**.
1. Clique em **Novo Relatório** e selecione **Entrada do Diário**.

   ![Selecionar entrada do diário](assets/nwe-select-journal-entry-350x273.png)

   O Report Builder é carregado.

1. Na guia **Colunas (Exibição)**, verifique se você tem ou clique em **Adicionar Coluna** para adicionar as seguintes colunas:

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
      <td> <p>O nome do campo personalizado afetado.</p> <p><span style="font-weight: normal;">Quando</span> <strong>DE</strong>:<span style="font-weight: normal;"> é exibido nesta coluna, indica que o campo listado é um campo personalizado.</span></p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Trocar Tipo</p> </td> 
      <td> <p>O tipo de alteração feita no campo afetado, como <strong>Adicionar</strong>, <strong>Excluir</strong> ou <strong>Editar</strong>.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Editado por nome</p> </td> 
      <td> <p>O nome do usuário que atualizou o campo personalizado.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Data de Entrada</p> </td> 
      <td> <p>A data em que o valor no campo personalizado foi alterado.</p> <p>Você deve classificar por esse campo em ordem decrescente.</p> </td> 
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
      <td> <p>O valor do texto anterior no campo personalizado.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Novo Valor de Texto</p> </td> 
      <td> <p>O valor do texto atual no campo personalizado.</p> <p>Se o campo personalizado for um campo de digitação antecipada, a coluna <strong>Novo valor de texto</strong> exibirá a ID do objeto.</p> </td> 
     </tr> 
    </tbody> 
   </table>

   Para obter mais informações sobre como adicionar colunas, consulte [Visão geral das exibições no Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

1. Na guia **Filtros**, clique em **Adicionar uma Regra de Filtro** e adicione os seguintes filtros:

   * **Nome do Campo de Entrada do Diário** > **Contém** > **DE**

     >[!TIP]
     >
     >Para limitar este relatório a campos personalizados específicos, adicione a regra de filtro **Nome do Campo de Entrada do Diário** > **Igual** > **&lt; nome do campo personalizado>**.

   * **ID do Projeto** > **Igual** > **&lt; projeto >**.

   ![Filtro de alterações em formulários personalizados](assets/qs-custom-form-changes-filter-350x92.png)

   Para obter mais informações sobre como adicionar filtros, consulte [Visão geral dos filtros](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. (Opcional) Para restringir o foco do relatório e reduzir os tempos de carregamento, adicione um prompt.

   Ou

   Crie regras de filtro adicionais para incluir projetos, tarefas ou problemas específicos.

   >[!IMPORTANT]
   >
   >Criar uma regra de filtro que use o modificador **Contains** pode realmente aumentar os tempos de carregamento. Por isso, recomendamos usar um modificador diferente como **Equal** quando possível para filtrar por um projeto específico ou ID de objeto de nível superior.

   Para saber como adicionar um prompt, consulte [Adicionar um prompt a um relatório](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

1. Na guia **Agrupamentos**, clique em **Aplicar um Agrupamento Existente** e selecione **Projeto**.

   Para obter mais informações sobre como adicionar agrupamentos, consulte [Visão geral dos agrupamentos no Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

1. Clique em **Salvar + Fechar**.

   O novo relatório é carregado.

## Veja como a Data de conclusão planejada mudou ao longo do ciclo de vida de um projeto {#see-how-the-planned-completion-date-changed-over-the-course-of-a-project-s-life-cycle}

Você pode configurar o relatório Lançamento para mostrar a frequência com que a Data de Conclusão Planejada muda ao longo da vida útil de um projeto.

1. Clique no ícone **[!UICONTROL Menu Principal]** ![Menu Principal](/help/_includes/assets/main-menu-icon.png) no canto superior direito do Adobe Workfront ou (se disponível) clique no ícone **[!UICONTROL Menu Principal]** ![Menu Principal](/help/_includes/assets/main-menu-icon-left-nav.png) no canto superior esquerdo e clique em **Relatórios**.
1. Clique em **Novo Relatório** e selecione **Entrada do Diário**.

   ![Selecionar entrada do diário](assets/nwe-select-journal-entry-350x273.png)

   O Report Builder é carregado.

1. Na guia **Colunas (Modo de Exibição)**, adicione as seguintes colunas:

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
      <td> <p>O nome do campo afetado.</p> <p><span style="font-weight: normal;">Quando</span> <strong>DE</strong>:<span style="font-weight: normal;"> é exibido nesta coluna, indica que o campo listado é um campo personalizado.</span></p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Trocar Tipo</p> </td> 
      <td>O tipo de alteração que ocorreu, como <strong>Adicionar</strong>, <strong>Excluir</strong> ou <strong>Editar</strong>.</td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Editado por nome</p> </td> 
      <td> <p>O nome do usuário que atualizou a Data de conclusão planejada do projeto.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Data de Entrada</p> </td> 
      <td> <p>A data em que a Data de conclusão planejada do projeto foi alterada.</p> <p>Você deve classificar por esse campo em ordem decrescente.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Código de objeto principal
</p> </td> 
      <td> <p>O objeto pai mais alto do campo que teve a data de conclusão planejada alterada.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Escopo</p> </td> 
      <td> <p>O objeto com a Data de conclusão planejada foi alterado.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Valor Velho de Data</p> </td> 
      <td> <p>O valor anterior da Data de conclusão planejada.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Novo Valor de Data</p> </td> 
      <td> <p>O valor atual da Data de conclusão planejada.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Nome do Projeto</p> <p>(Opcional)</p> </td> 
      <td> <p>O nome do projeto que teve a data de conclusão planejada alterada.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Nome da tarefa</p> <p>(Opcional)</p> </td> 
      <td> <p>O nome das tarefas no projeto que tiveram a data de conclusão planejada alterada.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Nome do Problema</p> <p>(Opcional)</p> </td> 
      <td>O nome dos problemas no projeto que têm a Alteração da data de conclusão planejada.</td> 
     </tr> 
    </tbody> 
   </table>

   Para obter mais informações sobre como adicionar colunas, consulte [Visão geral das exibições no Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

1. Na guia **Filtros**, clique em **Adicionar uma Regra de Filtro** e adicione o seguinte:

   * **Nome do Campo** > **Igual** > **Data**
   * **ID do Projeto** > **Igual** > **&lt; nome do projeto >**.

   ![Filtro de alteração da data de conclusão planejada](assets/qs-planned-completion-date-change-filter-350x91.png)

   Para obter mais informações sobre como adicionar filtros, consulte [Visão geral dos filtros](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. (Opcional) Para restringir o foco do relatório e reduzir os tempos de carregamento, adicione um prompt.

   Ou

   Crie regras de filtro adicionais para incluir projetos, tarefas ou problemas específicos.

   >[!IMPORTANT]
   >
   >Criar uma regra de filtro que use o modificador **Contains** pode realmente aumentar os tempos de carregamento. Por isso, recomendamos usar um modificador diferente como **Equal** quando possível para filtrar por um projeto específico ou ID de objeto de nível superior.

   Para saber como adicionar um prompt, consulte [Adicionar um prompt a um relatório](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

1. Na guia **Agrupamentos**, clique em **Aplicar um Agrupamento Existente** e selecione **Projeto**.

   Para obter mais informações sobre como adicionar agrupamentos, consulte [Visão geral dos agrupamentos no Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

1. Clique em **Salvar + Fechar**.

   O novo relatório é carregado.

## Veja se o proprietário de um projeto mudou {#see-if-the-owner-of-a-project-changed}

Você pode configurar o relatório Lançamento para mostrar quantas vezes o proprietário do projeto—ou gerente de projeto—muda ao longo da vida útil de um projeto.

1. Clique no ícone **[!UICONTROL Menu Principal]** ![Menu Principal](/help/_includes/assets/main-menu-icon.png) no canto superior direito do Adobe Workfront ou (se disponível) clique no ícone **[!UICONTROL Menu Principal]** ![Menu Principal](/help/_includes/assets/main-menu-icon-left-nav.png) no canto superior esquerdo e clique em **Relatórios**.
1. Clique em **Novo Relatório** e selecione **Entrada do Diário**.

   ![Selecionar entrada do diário](assets/nwe-select-journal-entry-350x273.png)

   O Report Builder é carregado.

1. Na guia **Colunas (Modo de Exibição)**, adicione as seguintes colunas:

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
      <td> <p>O tipo de alteração que ocorreu, como <strong>Adicionar</strong>, <strong>Excluir</strong> ou <strong>Editar</strong>.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Código de objeto principal
</p> </td> 
      <td> <p>O objeto pai mais alto do projeto que teve o proprietário atualizado.</p> </td> 
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
      <td> <p>O proprietário atual do projeto.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Informação Adicional 2</p> </td> 
      <td> <p>O proprietário anterior do projeto.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Nome do Projeto</p> </td> 
      <td> <p>O projeto que teve o campo Proprietário do projeto atualizado.</p> </td> 
     </tr> 
    </tbody> 
   </table>

   Para obter mais informações sobre como adicionar colunas, consulte [Visão geral das exibições no Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

1. Na guia **Filtros**, clique em **Adicionar regra de filtro** e adicione o seguinte:

   * **Nome do Campo** > **Igual** > **IDdoProprietário**
   * **ID do Projeto** > **Igual** > **&lt; nome do projeto >**.

   ![Filtro de alteração de proprietário](assets/qs-owner-changes-filter-350x94.png)

   Para obter mais informações sobre como adicionar filtros, consulte [Visão geral dos filtros](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. (Opcional) Para restringir o foco do relatório e reduzir os tempos de carregamento, adicione um prompt.

   Ou

   Crie regras de filtro adicionais para incluir projetos, tarefas ou problemas específicos.

   >[!IMPORTANT]
   >
   >Criar uma regra de filtro que use o modificador **Contains** pode realmente aumentar os tempos de carregamento. Por isso, recomendamos usar um modificador diferente como **Equal** quando possível para filtrar por um projeto específico ou ID de objeto de nível superior.

   Para saber como adicionar um prompt, consulte [Adicionar um prompt a um relatório](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

1. (Opcional) Na guia **Agrupamentos**, clique em **Aplicar um Agrupamento Existente** e selecione **Projeto**.

   Para obter mais informações sobre como adicionar agrupamentos, consulte [Visão geral dos agrupamentos no Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

1. Clique em **Salvar + Fechar**.

   O novo relatório de lançamento é exibido.
