---
navigation-topic: use-lists
title: Introdução a listas em  [!DNL Adobe Workfront]
description: Você pode exibir listas de objetos em  [!DNL Adobe Workfront]  para obter informações sobre eles, como suas datas de início e vencimento, usuários atribuídos a eles e outros objetos associados a eles.
feature: Get Started with Workfront
author: Nolan
exl-id: d4262b8e-bbe0-4ac2-8f1f-5d32541311c8
source-git-commit: f0b3b8aa64fa0b03a196bbcc2bdd037eeeb0f89e
workflow-type: tm+mt
source-wordcount: '2275'
ht-degree: 1%

---

# Introdução a listas em [!DNL Adobe Workfront]

<!--Audited: 11/2024-->

Você pode exibir listas de objetos em [!DNL Adobe Workfront] para obter informações sobre eles, como suas datas de início e vencimento, usuários atribuídos a eles e outros objetos associados a eles.

Estas são algumas características das listas em [!DNL Workfront]:

* As listas são atualizadas automaticamente a cada cinco minutos para atualizar as informações que outros usuários no sistema estão atualizando em outro lugar.
* Algumas áreas no [!DNL Workfront] são pré-configuradas com listas de objetos padrão.

  Você pode personalizar a maioria dessas listas pré-configuradas.

* Um administrador do [!DNL Workfront] pode criar listas personalizadas para serem aplicadas a várias áreas do [!DNL Workfront].

  Para obter mais informações sobre como criar listas no nível do sistema, consulte o artigo [Criar, editar e compartilhar filtros, exibições e agrupamentos padrão](../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-and-share-default-fvgs.md).

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacote do Adobe Workfront</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td> 
   <p>Colaborador ou superior</p>
   <p>Solicitação ou superior</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Editar acesso a Filtros, Visualizações, Agrupamentos </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Exibir permissões ou permissões mais altas para um filtro, exibição ou agrupamento com acesso para compartilhar </p>  </td> 
  </tr> 
 </tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old access: 

You must have the following access to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] plan*</strong></td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] license*</strong></td> 
   <td> <p>[!UICONTROL Request] or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Access level configurations*</strong></td> 
   <td> <p>[!UICONTROL View] or higher access to filters, views, groupings</p> <P>For items in the [!UICONTROL Setup] area, you need administrative access for the item or the [!UICONTROL System Administrator] access level.</P> <p>Note: If you still don't have access, ask your [!DNL Workfront] administrator if they set additional restrictions in your access level.<br>For information on how a [!DNL Workfront] administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Object permissions</strong></td> 
   <td> <p>[!UICONTROL View] or higher permissions with access to share</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td>
  </tr> 
 </tbody> 
</table>

To find out what plan, license type, or access you have, contact your [!DNL Workfront] administrator.
-->

## Listas de objetos

Abaixo estão alguns tipos de listas de objetos que você pode encontrar em [!DNL Workfront] e algumas das áreas onde eles são exibidos por padrão quando você tem direitos para visualizar um objeto.

>[!NOTE]
>
>* Esta lista não é abrangente. Cada uma dessas listas de objetos também pode aparecer em um relatório ou painel. Por exemplo, um relatório de Projeto ou um painel que contém um relatório de Projeto também exibe uma lista de projetos.
>* Nesta lista, &quot;selecionar&quot; significa que você precisa clicar no nome do item, não na caixa de seleção à esquerda do nome.


<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>[!DNL Workfront] list</strong></th> 
   <th><strong>Local da lista de objetos</strong></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Lista de portfólos</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Portfólio]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Lista de programas</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Portfólios] &gt;[!UICONTROL selecionar um portfólio] &gt;[!UICONTROL Programas]</p> </li> 
     <li data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <p>[!UICONTROL Programas]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Lista de projetos</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Projetos]</p> </li> 
     <li> <p>[!UICONTROL Portfólios] &gt;[!UICONTROL selecionar um portfólio] &gt;[!UICONTROL Projetos]</p> </li> 
     <li> <p>[!UICONTROL Portfólios] &gt;[!UICONTROL selecionar um portfólio] &gt;[!UICONTROL Programas] &gt;[!UICONTROL selecionar um programa] &gt;[!UICONTROL Projetos]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Lista de tarefas</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Projetos] &gt;[!UICONTROL selecionar um projeto] &gt; [!UICONTROL Tarefas]</p> </li> 
     <li> <p>[!UICONTROL Projetos] &gt;[!UICONTROL selecionar um projeto] &gt;[!UICONTROL Tarefas] &gt;[!UICONTROL selecionar uma tarefa] &gt;[!UICONTROL Subtarefas]</p> </li> 
     <li> <p>[!UICONTROL Projetos] &gt;[!UICONTROL selecionar um projeto] &gt;[!UICONTROL Tarefas] &gt;[!UICONTROL selecionar uma tarefa] &gt; [!UICONTROL Predecessoras*]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Lista de problemas</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Projetos] &gt; [!UICONTROL selecionar] um projeto &gt; [!UICONTROL Problemas]</p> </li> 
     <li> <p>[!UICONTROL Projetos] &gt;[!UICONTROL selecionar um projeto] &gt;[!UICONTROL Tarefas] &gt;[!UICONTROL selecionar uma tarefa] &gt; [!UICONTROL Problemas]</p> </li> 
     <li> <p>[!UICONTROL Projetos] &gt;[!UICONTROL selecionar um projeto] &gt;[!UICONTROL Tarefas] &gt;[!UICONTROL selecionar uma tarefa] &gt;[!UICONTROL Subtarefas] &gt;[!UICONTROL selecionar uma tarefa] &gt; [!UICONTROL Problemas]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Lista de relatórios</td> 
   <td> 
    <ul> 
     <li> <p>  [!UICONTROL Relatórios]  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Lista de painéis</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Painéis]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Lista de iterações</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Equipes] &gt; [!UICONTROL Iterações]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Lista de usuários</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Usuários]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Lista de documentos</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Documentos]</p> </li> 
     <li> <p>[!UICONTROL Portfólios] &gt;[!UICONTROL selecionar um portfólio] &gt; [!UICONTROL Documentos]</p> </li> 
     <li> <p>[!UICONTROL Portfólios] &gt; [!UICONTROL selecionar um portfólio] &gt;[!UICONTROL Programas] &gt;[!UICONTROL selecionar um programa] &gt;[!UICONTROL Documentos]</p> </li> 
     <li> <p>[!UICONTROL Projetos] &gt;[!UICONTROL selecionar um projeto] &gt;[!UICONTROL Documentos]</p> </li> 
     <li> <p>[!UICONTROL Projetos] &gt;[!UICONTROL selecionar um projeto] &gt;[!UICONTROL Tarefas] &gt;[!UICONTROL selecionar uma tarefa] &gt; [!UICONTROL Documentos]</p> </li> 
     <li> <p>[!UICONTROL Projetos] &gt; [!UICONTROL selecionar] um projeto &gt; [!UICONTROL Problemas] &gt; [!UICONTROL selecionar um problema] &gt; [!UICONTROL Documentos]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Lista de planilhas de horas</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Planilha de Horas] s &gt; [!UICONTROL Todas as Planilhas de Horas]*</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Lista de taxas de cobrança</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Projetos] &gt;[!UICONTROL selecionar um projeto] &gt;[!UICONTROL Taxas de Cobrança*]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Lista de registros de cobrança</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Projetos] &gt; [!UICONTROL selecionar um projeto] &gt; [!UICONTROL Registros de Cobrança]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Lista de riscos</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Projetos] &gt;[!UICONTROL selecionar um projeto] &gt;[!UICONTROL Riscos]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Lista de despesas</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Projetos] &gt;[!UICONTROL selecionar] um projeto &gt;[!UICONTROL Despesas]</p> </li> 
     <li> <p>[!UICONTROL Projetos] &gt; [!UICONTROL selecionar um projeto] &gt;[!UICONTROL Tarefas] &gt;[!UICONTROL selecionar uma tarefa] &gt;[!UICONTROL Despesas]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Lista de entradas de horas</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Projetos] &gt;[!UICONTROL selecionar] um projeto</p> </li> 
     <li> <p>[!UICONTROL Projetos] &gt;[!UICONTROL selecionar um projeto] &gt;[!UICONTROL Tarefas] &gt;[!UICONTROL selecionar uma tarefa] &gt;[!UICONTROL Horas]</p> </li> 
     <li> <p>[!UICONTROL Projetos] &gt;[!UICONTROL selecionar] um projeto &gt;[!UICONTROL Problemas] &gt;[!UICONTROL selecionar] um problema &gt;[!UICONTROL Horas]</p> </li>
    </ul> </td> 
  </tr>
  <tr> 
   <td>Lista de formulários personalizados</td> 
   <td> 
    <ul> 
     <li>[!UICONTROL Configuração] &gt;[!UICONTROL Forms Personalizado] </li> 
    </ul> </td> 
  </tr> 
  <tr> 
    <td>Lista de grupos ou subgrupos</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Configuração] &gt;[!UICONTROL Grupos]</p> </li>
     <li> <p>[!UICONTROL Configuração] &gt;[!UICONTROL Grupos] &gt;[!UICONTROL selecionar o grupo pai] &gt;[!UICONTROL Subgrupos] </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Lista de equipes</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Configuração] &gt;[!UICONTROL Equipes]</p> </li> 
    </ul> </td> 
  </tr>
  <tr> 
   <td>Lista de empresas</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Configuração] &gt;[!UICONTROL Empresas]</p> </li> 
    </ul> </td> 
  </tr>
  <tr> 
   <td>Lista de agendamentos</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Configuração] &gt;[!UICONTROL Agendamentos]</p> </li> 
    </ul> </td> 
  </tr>
  <tr> 
   <td>Lista de modelos de layout</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Configuração] &gt;[!UICONTROL Modelos de Layout]</p> </li> 
    </ul> </td> 
  </tr>
 </tbody> 
</table>

Não é possível personalizar a lista na área especificada. Um administrador do [!DNL Workfront] pode criar uma lista personalizada no nível do sistema, ou você pode criar um relatório para este objeto se seu nível de acesso permitir que você edite relatórios.

## Listar elementos

Uma lista contém determinados elementos que definem seu formato e as informações exibidas. Você pode encontrar vários elementos da lista de sistemas disponíveis por padrão. Você também pode criar elementos personalizados para atender às suas necessidades.

>[!NOTE]
>
>Quando você seleciona um novo filtro, exibição ou agrupamento em uma lista, essa seleção é mantida mesmo se você sair do [!DNL Workfront] ou fechar o navegador.

A seguir estão os elementos de uma lista:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Elemento</strong></th> 
   <th><strong>Explicação</strong></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td><strong>[!UICONTROL Filtro]</strong></td> 
   <td> <p>Os filtros mantêm as informações desnecessárias fora de uma lista, com base nos critérios especificados. </p> <p>Para obter mais informações, consulte <a href="../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md" class="MCXref xref">Visão geral dos filtros</a>.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>[!UICONTROL Exibir]</strong></td> 
   <td> <p>As exibições definem quais campos (colunas) são exibidos na tela.</p> <p>Para obter mais informações, consulte Visão geral das <a href="../../../reports-and-dashboards/reports/reporting-elements/views-overview.md" class="MCXref xref">Exibições em [!DNL Adobe Workfront]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>[!UICONTROL Agrupamento]</strong></td> 
   <td> <p>Agrupamentos separam os objetos na lista em áreas com base nos critérios que você especifica.</p> <p>Por exemplo, os problemas em uma lista podem ser exibidos em seções por status ou prioridade.</p> <p>É possível ter até três camadas de agrupamentos em um agrupamento padrão e adicionar uma quarta camada ao configurar um agrupamento no modo de texto.</p> <p>Para obter mais informações sobre agrupamentos, consulte <a href="../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md" class="MCXref xref">Visão geral dos agrupamentos em [!DNL Adobe Workfront]</a>.</p> <p>Para obter mais informações sobre o modo de texto, consulte <a href="../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md" class="MCXref xref">Visão geral do Modo de Texto</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

Esses elementos são exibidos na parte superior de cada lista por padrão. Eles são fixos e não se movem à medida que você percorre a lista. Passe o mouse sobre o ícone de cada elemento para identificá-los.

![Listar elementos](assets/nwe-list-elements.png)

Você pode personalizar elementos de lista nas seguintes áreas e compartilhá-los com outros usuários:

* Qualquer lista padrão do sistema encontrada na seção [Introdução às listas em [!DNL Adobe Workfront]](#default-workfront-lists) neste artigo
* Qualquer relatório compartilhado com você

Os elementos de construção para listas são os mesmos que os elementos de construção para relatórios.

Para obter mais informações sobre como criar e personalizar os elementos de criação de listas e relatórios, consulte [Elementos de relatório: filtros, exibições e agrupamentos](../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md).

## Listar ações

Você pode concluir as seguintes ações em uma lista:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Ação</strong></th> 
   <th><strong>Informações</strong></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td><strong>Edição integrada</strong> </td> 
   <td> <p>Editar objetos e suas informações diretamente na lista.</p> <p>Para obter mais informações, consulte <a href="../../../workfront-basics/navigate-workfront/use-lists/inline-edit-objects.md" class="MCXref xref">itens de edição em linha em uma lista em [!DNL Adobe Workfront]</a>.</p> 
   <p><b>NOTA:</b></p>
   <p>A edição em linha não é possível em um agrupamento.</p>

</td> 
  </tr> 
  <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td><strong>Atualizar com o [!UICONTROL Resumo]</strong> </td> 
   <td> <p>Atualizar tarefas e problemas no nível do projeto usando o painel [!UICONTROL Resumo].</p> <p><b>DICA:</b></p> <p>O Resumo não está disponível para todos os objetos e não está disponível nos relatórios de Tarefa ou Problema.</p> <p>Para obter mais informações, consulte <a href="../../../workfront-basics/the-new-workfront-experience/summary-overview.md" class="MCXref xref">Resumo geral</a>.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>Personalizar exibição de lista</strong> </td> 
   <td> <p>Personalize a aparência de uma lista, a organização da coluna, a ordem de classificação dos itens ou o número de itens exibidos.</p> <p><b>NOTA:</b></p> <p>As alterações feitas no número de itens a serem exibidos em uma página são revertidas quando você sai do [!DNL Workfront] ou fecha o navegador. As alterações também podem ser revertidas após um período de 8 horas.</p> <p>Para obter mais informações, consulte <a href="../../../workfront-basics/navigate-workfront/use-lists/modify-list-display.md" class="MCXref xref">Modificar como uma lista é exibida</a>.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>Filtro rápido</strong> </td> 
   <td> <p>Aplique um filtro rápido para localizar apenas itens importantes para você, para que você possa revisá-los, atualizá-los ou compartilhá-los rapidamente com outras pessoas.</p> <p><b>IMPORTANTE:</b></p> <p> Você pode localizar itens que contenham uma palavra de pesquisa usando o filtro rápido, seja esse item visível na tela ou que será exibido depois de rolar a tela para a parte inferior da página. Ao usar os recursos de pesquisa do seu navegador, você pode encontrar somente itens que já estejam visíveis na tela. Se sua lista tem várias páginas, os filtros rápidos localizam apenas os itens na página atual.</p> <p>Para obter mais informações, consulte <a href="../../../workfront-basics/navigate-workfront/use-lists/apply-quick-filter-list.md" class="MCXref xref">Aplicar o filtro rápido a uma lista</a>.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>Exportar</strong> </td> 
   <td> <p>Exportar uma lista de objetos de [!DNL Workfront]. Quando uma lista contém mais de 2000 itens, exportar a lista é a única maneira de revisar todos os itens em uma página.</p> <p>Para obter mais informações sobre como exportar uma lista, consulte <a href="../../../workfront-basics/navigate-workfront/use-lists/export-lists.md" class="MCXref xref">Exportar uma lista</a>. Para obter mais informações sobre formatos e limites de exportação, consulte <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md" class="MCXref xref">Exportar dados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Barra de ferramentas Lista

A tabela a seguir lista muitos dos ícones disponíveis na barra de ferramentas e indica o que acontece quando você clica neles:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>Ícone</strong></td> 
   <td><strong>Descrição</strong></td> 
   <td><strong>Ao clicar</strong></td> 
  </tr> 
  <tr> 
   <td> <img src="assets/add-icon-plus-in-circle.png"> </td> 
   <td>[!UICONTROL Adicionar item ou usuário]</td> 
   <td>Abra mais opções, incluindo a adição de um novo item ou usuário.</td> 
  </tr> 
  <tr> 
   <td> <img src="assets/qs-insert-task-above-icon-in-new-toolbar.png"> </td> 
   <td>[!UICONTROL Inserir tarefa acima]</td> 
   <td> <p>Insira uma tarefa acima da tarefa selecionada.</p> <p>Isso está disponível somente para tarefas. </p> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/qs-insert-task-below-icon-in-new-toolbar.png"> </td> 
   <td>[!UICONTROL Inserir tarefa abaixo]</td> 
   <td> <p>Insira uma tarefa abaixo da tarefa selecionada.</p> <p>Isso está disponível somente para tarefas. </p> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/edit-icon.png"> </td> 
   <td>[!UICONTROL Editar]</td> 
   <td>Editar o item selecionado.</td> 
  </tr> 
  <tr> 
   <td> <img src="assets/copy-icon.png"> </td> 
   <td>[!UICONTROL Copiar]</td> 
   <td>Copiar o item selecionado.</td> 
  </tr> 
  <tr> 
   <td> <img src="assets/delete.png"> </td> 
   <td>[!UICONTROL Excluir]</td> 
   <td>Excluir o item selecionado.</td> 
  </tr> 
  <tr> 
   <td> <img src="assets/qs-add-to-iteration-icon-in-new-toolbar-for-issues.png"> </td> 
   <td>[!UICONTROL Adicionar a]</td> 
   <td> <p>Abra a caixa de diálogo para adicionar o problema selecionado a uma iteração.</p> <p>Isso está disponível somente para problemas.</p> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/share-icon.png"> </td> 
   <td>[!UICONTROL Compartilhar]</td> 
   <td>Compartilhar o item selecionado.</td> 
  </tr> 
  <tr> 
   <td> <img src="assets/qs-indent-outdent-tasks-icon-in-new-toolbar.png"> </td> 
   <td>[!UICONTROL Recuar e recuar para a esquerda tarefas] </td> 
   <td> <p>Recuar ou recuar para a esquerda a tarefa selecionada. </p> <p>Isso está disponível somente para tarefas. </p> </td> 
  </tr> 
  <tr> 
   <td><img src="assets/more-icon.png"></a> </td> 
   <td>[!UICONTROL Mais]</td> 
   <td>Abrir opções adicionais para o item selecionado.</td> 
  </tr> 
  <tr> 
   <td> <p> <img src="assets/search-icon.png"> </p> </td> 
   <td> <p>[!UICONTROL Filtro rápido] </p> </td> 
   <td> <p>Abra a caixa de pesquisa de filtro rápido para localizar itens na lista exibida.</p> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/export.png"> </td> 
   <td>[!UICONTROL Exportar]</td> 
   <td>Exporte a lista para PDF, Excel ou arquivos delimitados por tabulação.</td> 
  </tr> 
  <tr> 
   <td> <img src="assets/qs-agile-icon-in-new-toolbar-task-list.png"> </td> 
   <td>[!UICONTROL Modo de Exibição Agile]</td> 
   <td>Exiba a lista na exibição Agile.<br>Isso está disponível somente para tarefas.</td> 
  </tr> 
  <tr> 
   <td> <img src="assets/qs-gantt-chart-icon-in-new-toolbar.png"> </td> 
   <td>[!UICONTROL Gráfico de Gantt]</td> 
   <td> <p>Exibir a lista na exibição de Gráfico de Gantt [!UICONTROL].</p> <p>Isso está disponível somente para projetos e tarefas.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <img src="assets/qs-filter-in-new-toolbar-with-name.png"> <p> <img src="assets/qs-filter-in-new-toolbar-with-blue-dot---small.png"> </p> </td> 
   <td>Menu suspenso [!UICONTROL Filtro]</td> 
   <td> <p>Exiba uma lista de filtros e opções adicionais para gerenciar filtros, incluindo a criação de um. </p> <p>Em uma tela pequena, o nome do Filtro é substituído pelo ícone de filtro. Um ponto azul é exibido no ícone Filtro quando você aplica qualquer filtro diferente de "[!UICONTROL Tudo]".</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <img src="assets/qs-view-in-new-toolbar-with-name.png"> <p> <img src="assets/qs-view-in-new-toolbar-with-blue-dot.png"> </p> </td> 
   <td>Menu suspenso [!UICONTROL View]</td> 
   <td> <p>Exibir uma lista de exibições e opções adicionais para gerenciar exibições, incluindo a criação de uma. </p> <p>Em uma tela pequena, o nome da Exibição é substituído pelo ícone [!UICONTROL view]. Um ponto azul é exibido no ícone da [!UICONTROL View] quando você aplica qualquer exibição diferente de "[!UICONTROL Standard]".</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <img src="assets/qs-grouping-in-new-toolbar-with-name.png"> <p> <img src="assets/qs-grouping-in-new-toolbar-with-blue-dot.png"> </p> </td> 
   <td>Menu suspenso [!UICONTROL Grouping]</td> 
   <td> <p>Exibir uma lista de agrupamentos e opções adicionais para gerenciar agrupamentos, incluindo a criação de um. </p> <p>Em uma tela pequena, o nome do agrupamento é substituído pelo ícone [!UICONTROL grouping]. Um ponto azul é exibido no ícone [!UICONTROL Agrupamento] quando você aplica qualquer agrupamento diferente de "[!UICONTROL Nada]".</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <img src="assets/qs-autosave-icon-in-new-toolbar-for-tasks.png"> </td> 
   <td> <p>[!UICONTROL Modo de plano]</p> </td> 
   <td> <p>Escolha se deseja salvar as alterações feitas em uma lista de tarefas automática ou manualmente. </p> <p>Para obter informações sobre como editar tarefas em uma lista, consulte <a href="/help/quicksilver/manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md" class="MCXref xref">Editar tarefas em uma lista</a>. </p> <p>Isso está disponível somente para tarefas.</p> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/summary-panel-icon.png"> </td> 
   <td>[!UICONTROL Resumo]</td> 
   <td> <p>Exibir ou ocultar a caixa [!UICONTROL Resumo] do item selecionado.</p> <p>Isso está disponível somente para tarefas e problemas.</p> <p>Para obter informações sobre o painel [!UICONTROL Summary], consulte <a href="/help/quicksilver/workfront-basics/the-new-workfront-experience/summary-overview.md" class="MCXref xref">Visão geral do Summary</a>.</p> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/remove-icon---x-in-circle.png"> </td> 
   <td>[!UICONTROL Remover]</td> 
   <td>Remover algo da lista. Por exemplo, como um administrador de grupo gerenciando associações de grupo ou subgrupo, remova um membro do grupo conforme explicado em <a href="/help/quicksilver/administration-and-setup/manage-groups/create-and-manage-groups/view-and-manage-a-groups-memberships.md" class="MCXref xref">Exibir e gerenciar as associações de um grupo</a>.</td> 
  </tr> 
  <tr> 
   <td> <img src="assets/comment-icon.png"> </td> 
   <td>[!UICONTROL Comentário] /[!UICONTROL Atualização]</td> 
   <td> <p>Digite um comentário ou uma atualização.</p> </td> 
  </tr> 
 </tbody> 
</table>

## A diferença entre listas e relatórios

Listas e relatórios são grades que contêm informações sobre um tipo de objeto.

A tabela a seguir descreve as semelhanças e diferenças entre listas e relatórios:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Funcionalidade</strong> </th> 
   <th><strong>Lista</strong> </th> 
   <th><strong>Relatório</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Qualquer pessoa pode criá-los</p> </td> 
   <td><span>⌘*</span> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Somente um administrador [!DNL Workfront] e usuários com uma licença de [!UICONTROL Plan] podem criá-los</p> </td> 
   <td> </td> 
   <td>✓**</td> 
  </tr> 
  <tr> 
   <td> <p>Um conjunto padrão está disponível em [!DNL Workfront]</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>Personalizável no modo padrão</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>Personalizável no modo de texto</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>Você pode compartilhá-los com outros usuários</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>Você pode compartilhá-los em todo o sistema</p> </td> 
   <td>✓</td> 
   <td> ✓ </td> 
  </tr> 
  <tr> 
   <td> <p>Você pode compartilhá-los fora do sistema</p> </td> 
   <td> </td> 
   <td>✓ </td> 
  </tr> 
  <tr> 
   <td> <p>É possível exportar para formatos .pdf, [!DNL Excel] e Delimitado por tabulação</p> </td> 
   <td>✓</td> 
   <td> ✓ </td> 
  </tr> 
  <tr> 
   <td> <p>Você pode agendá-los para entrega em um email</p> </td> 
   <td> </td> 
   <td>✓ </td> 
  </tr> 
  <tr> 
   <td> <p>Você pode adicionar a um modelo de layout</p> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>É possível adicioná-los a seções personalizadas </p> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>Você pode adicioná-los a um painel</p> </td> 
   <td> ✓*** </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>Você pode usar prompts para personalizar o que eles exibem</p> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>É possível exibi-los em um gráfico</p> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>É possível editar objetos em linha neles</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

É necessário ter acesso a filtros, visualizações e agrupamentos para poder criá-los. Para obter mais informações, consulte [Conceder acesso a filtros, visualizações e agrupamentos](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-fvg.md).

Você deve ter acesso a filtros, visualizações e agrupamentos, bem como relatórios, painéis e calendários para poder criá-los. Para obter mais informações, consulte [Conceder acesso a relatórios, painéis e calendários](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md).

Você pode personalizar listas para relatórios que são colocados em um painel somente se o criador do relatório tiver configurado os elementos da lista para serem visíveis no painel.

>[!NOTE]
>
>Não é possível adicionar uma lista a um painel sem criar um relatório e adicioná-lo ao painel primeiro.

Para obter mais informações sobre a criação de um relatório, consulte [Criar um relatório personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md). Para obter informações sobre como criar seções personalizadas, consulte [Criar guias ou seções personalizadas](../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/create-custom-tabs.md).

## A diferença entre as listas atualizadas e herdadas

Há dois tipos de listas em [!DNL Workfront]:

* Listas herdadas

  ![Agrupamentos azuis](assets/legacy-list-screen-shot-blue-groupings-350x101.png)

* Listas atualizadas

  ![Agrupamentos cinza](assets/updated-list-screen-shot-gray-groupings-350x71.png)

A tabela a seguir mostra algumas das diferenças entre as listas herdadas e atualizadas em [!DNL Workfront]:

<!--
<span style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode"> [Legacy does not equal Classic. Legacy lists appear in NWE and Classic. Updated lists appear in NWE and Classic.]</span>
-->

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><b>Listas herdadas</b></td> 
   <td><b>Listas atualizadas</b></td> 
  </tr> 
  <td> <p>Exibir <strong>100</strong> itens por padrão</p> </td> 
   <td> <p>Exibir <strong>Todos</strong> ou até <strong>2000</strong> itens por padrão</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Use CTRL+F para localizar itens em uma lista</p> </td> 
   <td> <p>Use filtros rápidos para localizar informações rapidamente em uma lista grande</p> <p>Para obter informações sobre como usar filtros rápidos em listas, consulte <a href="../../../workfront-basics/navigate-workfront/use-lists/apply-quick-filter-list.md" class="MCXref xref">Aplicar o filtro rápido a uma lista</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Não é possível editar campos personalizados em linha com formatação de rich text.</td> 
   <td> <p>O texto em campos personalizados com formatação pode ser configurado para permitir negrito, itálico, sublinhado, marcadores, numeração, hiperlinks e aspas de bloco.</p> <p>Para obter mais informações, consulte <a href="/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md">Criar um formulário personalizado</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>A formatação condicional pode alterar a cor do texto dos links em uma lista</td> 
   <td>Não é possível aplicar alterações de cor de texto aos links em uma lista</td> 
  </tr> 
 </tbody> 
</table>
