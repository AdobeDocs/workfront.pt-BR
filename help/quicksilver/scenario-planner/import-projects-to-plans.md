---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Importar projetos para planos no Planejador de cenários
description: Você pode importar projetos existentes para um plano. Os projetos importados são convertidos em iniciativas e você pode gerenciá-los no plano da mesma forma que gerenciaria uma nova iniciativa. O projeto original permanece vinculado à nova iniciativa.
author: Alina
feature: Workfront Scenario Planner
exl-id: 20429bb1-c158-433b-9790-325cd577248e
source-git-commit: 2ff32ba11f9ef214f16b11323386223792b0877e
workflow-type: tm+mt
source-wordcount: '1670'
ht-degree: 0%

---

# Importar projetos para planos no [!DNL Scenario Planner]

Você pode importar projetos existentes para um plano. Os projetos importados são convertidos em iniciativas e você pode gerenciá-los no plano da mesma forma que gerenciaria uma nova iniciativa. O projeto original permanece vinculado à nova iniciativa.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: add information about what happens when you import projects and where the info from projects show up;</p>
<p>- the hours/ FTE come from WorkPerDay</p>
<p>- if a task has a Duration of 0, the FTE should be 0 for that asignee but it should still come across) </p>
</div>
-->

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] plano*</p> </td> 
   <td> <p>Atual: [!UICONTROL Business] ou superior</p>
   <p>Novo: Ultimate </p>
   </td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] licença*</p> </td> 
   <td> <p>Novo: Claro ou superior</p> 
   <p>Atual: [!UICONTROL Review] ou posterior</p> </td> 
  </tr> 
  <tr> 
   <td>Produto* </td> 
   <td> 
   <p>Para os planos atuais do Workfront: </p>
   <p>Você deve comprar uma licença adicional para o [!DNL Adobe Workfront Scenario Planner] acessar a funcionalidade descrita neste artigo.</p> <p>Para obter informações sobre acesso e permissões para o [!DNL Workfront Scenario Planner], consulte <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">Acesso necessário para usar o [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Nível de acesso </td> 
   <td> <p>[!UICONTROL Editar] acesso à [!DNL Scenario Planner]</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>Permissões de objeto </p> </td> 
   <td> <p>[!UICONTROL Gerenciar] permissões para um plano</p> <p>Para obter informações sobre como solicitar acesso adicional a um plano, consulte <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">Solicitar acesso a um plano no [!DNL Scenario Planner]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Para obter informações, consulte [Requisitos de acesso à documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Considerações sobre a importação de projetos para planos como novas iniciativas

* Você deve criar projetos antes de importá-los para um plano como novas iniciativas.

  <!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: no caveats for project statuses yet, mentioned in the import steps as a tip) </p>
  -->

* Você deve ter pelo menos [!UICONTROL permissões de Visualização] para os projetos para poder importá-los para um plano como uma nova iniciativa.
* Você pode importar o mesmo projeto para vários planos.
* Os projetos que você deseja importar devem ter datas incluídas no período do seu plano. Você não pode importar projetos com uma [!UICONTROL Data de conclusão planejada] anterior ao início do plano ou com uma [!UICONTROL Data de início planejada] posterior ao fim do plano.
* Não é possível importar mais de 100 projetos de cada vez.
* Algumas informações do projeto também são importadas para o plano e se tornam informações da iniciativa. Para obter informações sobre quais informações do projeto são importadas para o plano e se tornam informações da iniciativa, consulte a seção [Informações do projeto importadas para o plano](#project-information-imported-into-the-plan) neste artigo.
* As alterações que ocorrem nos projetos vinculados não afetam as iniciativas no plano.
* Alterações que ocorrem nas iniciativas do plano não afetam automaticamente os projetos vinculados Alterações na iniciativa afetam os projetos vinculados somente quando você publica a iniciativa do plano. Para obter informações sobre como as iniciativas de publicação afetam os projetos vinculados, consulte [Atualizar ou criar projetos publicando iniciativas em [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md).
* Excluir uma iniciativa que foi criada com a importação de um projeto não exclui o projeto.
* Excluir um projeto vinculado a uma iniciativa não exclui a iniciativa.

## Informações do projeto importadas para o plano {#project-information-imported-into-the-plan}

Quando você importa um projeto para um plano, algumas informações do projeto também são importadas para o plano e se tornam informações da iniciativa. A tabela a seguir mostra quais informações do projeto se tornam informações da iniciativa quando você importa um projeto para um plano:

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: add what happens if you import a 5 year project to a 1 year plan - how does this display?) </p>
-->

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Informações do projeto</td> 
   <td>Informações da iniciativa </td> 
  </tr> 
  <tr> 
   <td>Nome do Projeto</td> 
   <td>Nome da iniciativa</td> 
  </tr> 
  <tr> 
   <td>Datas Planejadas do Projeto</td> 
   <td> <p>Meses de início e término da iniciativa.</p> <p>Se um projeto começar ou terminar no meio de um mês, as datas de importação são estendidas para abranger um mês inteiro no plano. Por exemplo, se as Datas planejadas do projeto forem de 20 de março a 5 de maio de 2020, as datas da iniciativa importada serão de março a maio de 2020.</p> <p>Se a Data de Início ou Término Planejada estiver além da duração do plano, há uma indicação visual de que a iniciativa importada começa antes ou termina depois do plano. </p> </td> 
  </tr> 
  <tr> 
   <td>Funções de trabalho atribuídas a tarefas e problemas</td> 
   <td> <p>Funções de trabalho da iniciativa. </p> <p>Nota:   <p>Se um usuário alterar funções durante a vida útil do projeto, as funções importadas dependerão do status da atribuição ao importar o projeto. Existem os seguintes cenários:</p> 
     <ul> 
      <li> <p>Se um usuário atribuído a uma tarefa ou problema tiver alterado sua função depois de ter marcado sua atribuição como [!UICONTROL Concluído], o [!DNL Workfront] importará para a iniciativa a função que o usuário atendeu antes de marcar a atribuição como [!UICONTROL Concluído].</p> </li> 
      <li> <p>Se um usuário atribuído a uma tarefa ou problema tiver alterado a função durante a vida do projeto, mas sua atribuição na tarefa ou problema não estiver marcada como [!UICONTROL Concluído] quando você importar o projeto, o [!DNL Workfront] importará somente a função atual do usuário atribuído. </p> </li> 
     </ul> <p>Para obter informações sobre o status de uma atribuição, consulte "Status da Atribuição" no <a href="../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md" class="MCXref xref">Glossário da terminologia do Adobe [!DNL Workfront]</a>. </p> </p> </td> 
  </tr> 
  <tr> 
   <td>Projeto [!UICONTROL Trabalho] associado a funções de trabalho atribuídas a tarefas ou problemas</td> 
   <td> <p><span>Dependendo de o plano estar configurado para usar FTEs ou horas, as [!UICONTROL Horas Planejadas] das tarefas do projeto tornam-se</span> [!UICONTROL FTEs Necessários] <span>ou [!UICONTROL Horas Necessárias] no plano</span>. </p> <p>Para obter informações sobre como configurar um plano para usar FTEs ou horas, consulte <a href="../scenario-planner/create-and-edit-plans.md" class="MCXref xref">Criar e editar planos no [!DNL Scenario Planner]</a>. </p> <p>Considere o seguinte:</p> 
    <ul> 
     <li> <p>[!DNL Workfront] O usa as funções de trabalho atribuídas a tarefas e problemas ou as funções de trabalho que os usuários atribuídos a tarefas ou problemas estão associados no projeto e as transfere para a nova iniciativa como Funções de trabalho obrigatórias. </p> </li> 
     <li> <p>Quando o plano é configurado para usar FTEs, as Horas planejadas associadas às funções de trabalho nas tarefas e problemas do projeto são convertidas primeiro em FTE. Esse FTE é atribuído à função de trabalho da iniciativa. <span>As horas planejadas são igualmente distribuídas em [!DNL Workfront]. Se uma tarefa ou um problema se estender por vários meses, a quantidade de Horas Planejadas para cada mês na duração da iniciativa será convertida em FTE mensal e transferida para cada mês da iniciativa.</span></p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exemplo: </b></span></span><span>Por exemplo, se uma tarefa for atribuída a uma função de trabalho por 80 Horas Planejadas em setembro, a função de trabalho importada exibirá 0,5 FTE para a iniciativa em setembro.</span> </p> </li> 
     <li> <p>[!DNL Workfront] O calcula o FTE das funções de Trabalho Necessárias associadas à iniciativa usando a seguinte fórmula:</p> <p><code>Required Job Role FTE (initiative) = Job Role assignment Planned Hours (</code><code>from tasks and issues on the project)/ 160</code> </p> <p>Dica: o [!DNL Scenario Planner] presume que há 160 horas de trabalho em um mês.</p> <p>Por exemplo, se um projeto tiver uma Duração de 1200 minutos e uma função de trabalho no projeto estiver associada a 600 minutos de Horas planejadas, seu FTE será 0,5. Ao importar o projeto, o FTE de função de trabalho necessário na iniciativa recém-criada é 0,5 para cada mês da iniciativa. </p> </li> 
     <li>Quando uma função de trabalho é atribuída a uma tarefa no projeto com zero Horas planejadas, o FTE necessário para a função de trabalho da iniciativa é zero por padrão. <!--
       <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
         (NOTE: this used to be 1, not zero in Production) 
       </MadCap:conditionalText>
      --></li> 
     <li>Quando uma função de trabalho é atribuída a uma tarefa no projeto com uma [!UICONTROL Duration] zero, o FTE necessário <span>ou horas</span> para a função de trabalho da iniciativa é zero por padrão, mesmo que a tarefa tenha Horas planejadas. </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Importar projetos para um plano

>[!IMPORTANT]
>
>Depois de importar projetos para um plano, eles se tornam iniciativas no plano. Embora os dois itens estejam vinculados, eles existem como entidades independentes e não se afetam automaticamente quando são atualizados.
>
>Ocorrem os seguintes:
>
>* As alterações no projeto nunca afetam a iniciativa após você importar o projeto para o plano. Essas alterações incluem alterações nas alocações de funções de trabalho.
>
>  <!--
>  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this might change if projects will ever affect initiatives automatically) </p>>
>  -->
>
>* As alterações na iniciativa afetam as informações na área [!DNL Scenario Planner] do projeto somente quando você publica a iniciativa no projeto correspondente. Caso contrário, elas não afetarão as informações de [!UICONTROL Horas planejadas] para as tarefas e problemas do projeto.
>
>  Para obter informações sobre como as iniciativas de publicação afetam os projetos vinculados, consulte [Atualizar ou criar projetos publicando iniciativas no Planejador de Cenários](../scenario-planner/publish-scenarios-update-projects.md).
>

{{step1-to-scenario-planner}}

1. Clique no nome de um plano para o qual deseja importar projetos.
1. Clique em **[!UICONTROL Nova iniciativa]** e em **[!UICONTROL Importar projetos]**.

   A caixa [!UICONTROL Importar projetos] é exibida. Os projetos com datas incluídas no período do seu plano são exibidos em uma lista.

   ![](assets/project-import-ui-projects-selected-350x72.png)

   >[!TIP]
   >
   >Os projetos em qualquer status são exibidos na lista.

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: the status of the projects in the import projects UI might change; right now it's ALL statuses)</p>
   -->

1. (Opcional) Clique no **[!UICONTROL ícone de Filtro]** ![](assets/filter-nwepng.png)e selecione um filtro disponível na lista para reduzir a quantidade de projetos na sua lista. Por padrão, a lista de projetos é filtrada pelo filtro de projeto atualmente selecionado pelo usuário em uma lista de projetos.

1. (Opcional) Clique no **[!UICONTROL ícone de Pesquisa]** ![](assets/search-icon.png) e adicione uma palavra-chave exibida em qualquer campo da tela. Os itens que contêm a palavra de pesquisa são exibidos na lista automaticamente e todos os itens ficam ocultos.

1. (Condicional) Clique no **[!UICONTROL ícone X]** para remover a pesquisa e exibir todos os projetos.
1. Selecione até 100 projetos e clique em **[!UICONTROL Importar]**.

   Os projetos são importados como novas iniciativas.

   Observe o seguinte:

   * Um ícone de projeto ![](assets/project-icon-sp.png) é exibido à direita do nome da iniciativa.
   * Se a linha do tempo do projeto exceder a duração do plano, a barra da iniciativa terminará com uma margem apontada para a esquerda (quando a Data Inicial for anterior à data do plano) ou para a direita (quando a Data Final for posterior à data do plano).

     ![](assets/project-bar-earlier-than-the-plan-start-date-350x39.png)

   * O número de meses e funções de trabalho foram atualizados para corresponder ao do projeto.

   >[!TIP]
   >
   >Os custos associados às funções de trabalho são atualizados no nível da iniciativa e não são importados do projeto.

1. Clique na barra que representa a nova iniciativa para abrir o painel de detalhes da iniciativa à direita.

   ![](assets/initiative-duration-with-project-duration-details-panel-350x292.png)

   Na área **[!UICONTROL Duração da Iniciativa]**, analise as seguintes informações:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Duração da Iniciativa]</td> 
      <td>Esta é a duração da iniciativa em meses. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Iniciativa]</td> 
      <td>As datas de início e término da iniciativa. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Projeto]</td> 
      <td> <p>[!UICONTROL Início Planejado] e [!UICONTROL Datas de Término] do projeto vinculado.</p> <p>Dica: se as informações do [!UICONTROL Project] estiverem ausentes, o projeto foi excluído.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Edite o nome da iniciativa. Por padrão, ele corresponde ao nome do projeto.
1. (Opcional) Siga um destes procedimentos:

   * Atualizar funções na seção **[!UICONTROL Funções de Trabalho Necessárias]**
   * Atualizar os **[!UICONTROL Custos Fixos]** na seção **[!UICONTROL Custos]**

   * Clique em **[!UICONTROL Atualizar funções de trabalho disponíveis]** ou **[!UICONTROL Atualizar orçamento disponível]** para resolver conflitos entre a nova iniciativa e outras iniciativas do plano.

1. (Condicional) Clique em **[!UICONTROL Aplicar]** para salvar as alterações na sua iniciativa.
1. Clique em **[!UICONTROL Salvar Plano]** para salvar as alterações em seu plano.
1. (Opcional) Para atualizar as alterações feitas na iniciativa de volta ao projeto do qual foi importada, publique o projeto do plano. Para obter informações sobre planos de publicação, consulte [Atualizar ou criar projetos publicando iniciativas em [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md).
1. (Opcional) Clique no ícone do projeto para acessar o projeto vinculado.

   ![](assets/project-icon-on-initiative-highlighted-350x49.png)
