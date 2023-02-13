---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Importar projetos para planos no Planejador de Cenário
description: Você pode importar projetos existentes para um plano. Os projetos importados são convertidos em iniciativas e você pode gerenciá-los dentro do plano da mesma forma que gerenciaria uma nova iniciativa. O projeto original permanece ligado à nova iniciativa.
author: Alina
feature: Workfront Scenario Planner
exl-id: 20429bb1-c158-433b-9790-325cd577248e
source-git-commit: 844dddec944b6cfb0957eecf09c2980e9d0577cc
workflow-type: tm+mt
source-wordcount: '1699'
ht-degree: 0%

---

# Importar projetos para planos na [!DNL Scenario Planner]

Você pode importar projetos existentes para um plano. Os projetos importados são convertidos em iniciativas e você pode gerenciá-los dentro do plano da mesma forma que gerenciaria uma nova iniciativa. O projeto original permanece ligado à nova iniciativa.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: add information about what happens when you import projects and where the info from projects show up;</p>
<p>- the hours/ FTE come from WorkPerDay</p>
<p>- if a task has a Duration of 0, the FTE should be 0 for that asignee but it should still come across) </p>
</div>
-->

## Requisitos de acesso

Você deve ter o seguinte:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront]<b> plano*</b> </p> </td> 
   <td>[!UICONTROL Business] ou superior</td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront]<b> licença*</b> </p> </td> 
   <td> <p>[!UICONTROL Review] ou superior</p> </td> 
  </tr> 
  <tr> 
   <td><b>Produto</b> </td> 
   <td> <p>Você deve comprar uma licença adicional para a [!DNL Adobe Workfront Scenario Planner] para acessar a funcionalidade descrita neste artigo.</p> <p>Para obter informações sobre como obter o [!DNL Workfront Scenario Planner], consulte <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">O acesso necessário para usar o [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><strong>Configurações de nível de acesso*</strong> </td> 
   <td> <p>Acesso à [!UICONTROL Editar] ou superior à [!DNL Scenario Planner]</p> <p>Observação: Se ainda não tiver acesso, pergunte ao seu [!DNL Workfront] administrador se eles definirem restrições adicionais em seu nível de acesso. Para obter informações sobre como uma [!DNL Workfront] administrador pode alterar seu nível de acesso, consulte <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><strong>Permissões de objeto</strong> </p> </td> 
   <td> <p>Permissões do [!UICONTROL Manager] para um plano</p> <p>Para obter informações sobre como solicitar acesso adicional a um plano, consulte <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">Solicitar acesso a um plano no Planejador de Cenário</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com seu [!DNL Workfront] administrador.

## Considerações sobre a importação de projetos para planos como novas iniciativas

* Você deve criar projetos antes de importá-los para um plano como novas iniciativas.

   <!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: no caveats for project statuses yet, mentioned in the import steps as a tip) </p>
  -->

* Você deve ter pelo menos [!UICONTROL Exibir] Permissões para que os projetos possam importá-los para um plano como nova iniciativa.
* Você pode importar o mesmo projeto em vários planos.
* Os projetos que você deseja importar devem ter datas incluídas no período do plano. Não é possível importar projetos com uma [!UICONTROL Data de Conclusão Planejada] antes do início do plano ou de um [!UICONTROL Data de início planejada] mais tarde do que o fim do plano.
* Não é possível importar mais de 100 projetos por vez.
* Algumas informações do projeto também são importadas para o plano e se tornam informações de iniciativa. Para obter informações sobre quais informações de projeto são importadas para o plano e se tornam informações de iniciativa, consulte o [Informações do projeto importadas no plano](#project-information-imported-into-the-plan) neste artigo.
* As alterações que ocorrem nos projetos vinculados não afetam as iniciativas no plano.
* As alterações que ocorrem nas iniciativas no plano não afetam automaticamente as alterações vinculadas da Iniciativa de projetos afetam os projetos vinculados somente quando você publica a iniciativa do plano. Para obter informações sobre como as iniciativas de publicação afetam os projetos vinculados, consulte [Atualize ou crie projetos publicando iniciativas no [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md).
* A exclusão de uma iniciativa que foi criada importando um projeto não exclui o projeto.
* A exclusão de um projeto vinculado a uma iniciativa não exclui a iniciativa.

## Informações do projeto importadas no plano {#project-information-imported-into-the-plan}

Quando você importa um projeto para um plano, algumas informações do projeto também são importadas para o plano e se tornam informações da iniciativa. A tabela a seguir mostra quais informações do projeto se tornam informações da iniciativa ao importar um projeto para um plano:

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
   <td> <p>A iniciativa começa e termina meses.</p> <p>Se um projeto começar ou terminar no meio de um mês, as datas importadas serão estendidas para abranger um mês inteiro no plano. Por exemplo, se as Datas previstas do projeto forem 20 de março - 5 de maio de 2020, as datas da iniciativa importada serão março - maio de 2020.</p> <p>Se a Data de Início ou Conclusão Planejada estiver além da duração do plano, há uma indicação visual de que a iniciativa importada começa antes ou termina depois do plano. </p> </td> 
  </tr> 
  <tr> 
   <td>Funções de trabalho atribuídas a tarefas e problemas</td> 
   <td> <p>Funções de trabalho da iniciativa. </p> <p>Nota:   <p>Se um usuário alterar funções durante a vida do projeto, as funções importadas dependerão do status da atribuição quando você importar o projeto. Os seguintes cenários existem:</p> 
     <ul> 
      <li> <p>Se um usuário atribuído a uma tarefa ou a um problema alterasse sua função após marcar sua atribuição como [!UICONTROL concluído], [!DNL Workfront] importa para a iniciativa a função que o usuário desempenhou antes de marcar a atribuição como [!UICONTROL concluído].</p> </li> 
      <li> <p>Se um usuário atribuído a uma tarefa ou problema tiver alterado a função durante a vida do projeto, mas sua atribuição na tarefa ou problema não estiver marcada como [!UICONTROL concluído] quando você importar o projeto, [!DNL Workfront] importa somente a função atual do usuário atribuído. </p> </li> 
     </ul> <p>Para obter informações sobre o status de uma atribuição, consulte "Status da Atribuição" em <a href="../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md" class="MCXref xref">Glossário de Adobe [!DNL Workfront] terminologia</a>. </p> </p> </td> 
  </tr> 
  <tr> 
   <td>Projeto [!UICONTROL Horas Planejadas] associado às funções de trabalho atribuídas a tarefas ou problemas</td> 
   <td> <p><span>Dependendo se o plano estiver configurado para usar FTEs ou horas, as [!UICONTROL Horas Planejadas] das tarefas no projeto se tornarão</span> [!UICONTROL FTEs necessários] <span>ou [!UICONTROL Horário necessário] no plano</span>. </p> <p>Para obter informações sobre como configurar um plano para usar FTEs ou horas, consulte <a href="../scenario-planner/create-and-edit-plans.md" class="MCXref xref">Crie e edite planos na [!DNL Scenario Planner]</a>. </p> <p>Considere o seguinte:</p> 
    <ul> 
     <li> <p>[!DNL Workfront] O usa as funções de job atribuídas a tarefas e problemas ou as funções de job às quais os usuários atribuídos a tarefas ou problemas estão associados no projeto e as transfere para a nova iniciativa como Funções de Job Obrigatório. </p> </li> 
     <li> <p>Quando o plano é configurado para usar FTEs, as Horas Planejadas associadas às funções do trabalho nas tarefas e problemas do projeto são convertidas primeiro em FTE. Este ETI é então atribuído à função de trabalho da iniciativa. <span>As Horas Planejadas são igualmente distribuídas em [!DNL Workfront]. Se uma tarefa ou um problema se estender por vários meses, a quantidade de Horas Planejadas para cada mês na duração da iniciativa é convertida em FTE mensal e transferida para cada mês da iniciativa.</span></p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exemplo: </b></span></span><span>Por exemplo, se uma tarefa for atribuída a uma função de trabalho por 80 Horas Planejadas em setembro, a função de trabalho importada exibirá 0,5 FTE para a iniciativa em setembro.</span> </p> </li> 
     <li> <p>[!DNL Workfront] O calcula o FTE das funções de Job Obrigatório associadas à iniciativa usando a seguinte fórmula:</p> <p><code>Required Job Role FTE (initiative) = Job Role assignment Planned Hours (</code><code>from tasks and issues on the project)/ 160</code> </p> <p>Dica: O [!DNL Scenario Planner] parte do princípio de que há 160 horas de trabalho por mês.</p> <p>Por exemplo, se um projeto tiver uma Duração de 1200 minutos e uma função de trabalho no projeto estiver associada a 600 minutos de Horas Planejadas, seu FTE será de 0,5. Ao importar o projeto, o FTE de Função de Trabalho Obrigatório na iniciativa recém-criada será de 0,5 para cada mês da iniciativa. </p> </li> 
     <li>Quando uma função de trabalho é atribuída a uma tarefa no projeto com zero Horas Planejadas, o FTE Necessário para a função de trabalho da iniciativa é zero por padrão. <!--
       <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
         (NOTE: this used to be 1, not zero in Production) 
       </MadCap:conditionalText>
      --></li> 
     <li>Quando uma função de trabalho é atribuída a uma tarefa no projeto com uma [!UICONTROL Duração] zero, o FTE Obrigatório <span>ou horas</span> para o cargo da iniciativa é zero por padrão, mesmo que a tarefa tenha Horas Planejadas. </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>



## Importar projetos para um plano

>[!IMPORTANT]
>
>Depois de importar os projetos em um plano, eles se tornam iniciativas no plano. Embora os dois itens estejam vinculados, eles existem como entidades independentes e não se afetam automaticamente quando são atualizados.
>
>O seguinte ocorre:
>
>* As alterações no projeto nunca afetam a iniciativa após importar o projeto para o plano.Essas alterações incluem alterações nas alocações de função de cargo.
>
>  <!--
>  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this might change if projects will ever affect initiatives automatically) </p>>
>  -->
>
>* As mudanças na iniciativa afetam as informações na [!DNL Scenario Planner] no projeto somente quando você publica a iniciativa no projeto correspondente. Caso contrário, não afetarão a variável [!UICONTROL Horas Planejadas] informações sobre as tarefas e questões do projeto.
>
>  Para obter informações sobre como as iniciativas de publicação afetam os projetos vinculados, consulte  [Atualize ou crie projetos publicando iniciativas no Planejador de Cenários](../scenario-planner/publish-scenarios-update-projects.md).

1. Clique no botão **[!UICONTROL Menu principal]** ![](assets/main-menu-icon.png) no canto superior direito de [!DNL Workfront], depois clique em [!DNL Scenarios] para acessar o [!DNL Scenario Planner].

1. Clique no nome de um plano onde deseja importar projetos.
1. Clique em **[!UICONTROL Nova iniciativa]**, depois clique em **[!UICONTROL Importar projetos]**.

   O [!UICONTROL Importar projetos] será exibida. Os projetos que têm datas incluídas no período do seu plano são exibidos em uma lista.

   ![](assets/project-import-ui-projects-selected-350x72.png)

   >[!TIP]
   >
   >Os projetos em qualquer status são exibidos na lista.

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: the status of the projects in the import projects UI might change; right now it's ALL statuses)</p>
   -->

1. (Opcional) Clique no botão **[!UICONTROL Ícone Filtro]** ![](assets/filter-nwepng.png)e selecione um filtro disponível na lista para reduzir a quantidade de projetos na lista. Por padrão, a lista de projetos é filtrada pelo filtro de projeto atualmente selecionado pelo usuário em uma lista de projetos.

1. (Opcional) Clique no botão **[!UICONTROL Ícone de Pesquisa]** ![](assets/search-icon.png) e adicione uma palavra-chave exibida em qualquer campo da tela. Os itens que contêm a palavra de pesquisa são exibidos automaticamente na lista e todos os itens ficam ocultos.

1. (Condicional) Clique no botão **[!UICONTROL Ícone X]** para remover a pesquisa e exibir todos os projetos.
1. Selecione até 100 projetos e clique em **[!UICONTROL Importar]**.

   Os projetos são importados como novas iniciativas.

   Observe o seguinte:

   * Um ícone de projeto ![](assets/project-icon-sp.png) é exibido à direita do nome da iniciativa.
   * Se a linha do tempo do projeto exceder a duração do plano, a barra da iniciativa terminará com uma margem pontiaguda à esquerda (quando a Data Inicial for anterior à data do plano) ou à direita (quando a Data Final for posterior à data do plano).

      ![](assets/project-bar-earlier-than-the-plan-start-date-350x39.png)

   * O número de meses e funções de trabalho foram atualizados para corresponder aos do projeto.
   >[!TIP]
   >
   >Os custos associados às funções do trabalho são atualizados no nível da iniciativa e não são importados do projeto.

1. Clique na barra que representa a nova iniciativa para abrir o painel de detalhes da iniciativa à direita.

   ![](assets/initiative-duration-with-project-duration-details-panel-350x292.png)

   No **[!UICONTROL Duração da iniciativa]** consulte as seguintes informações:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Initiative Duration]</td> 
      <td>Esta é a duração da iniciativa em meses. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Initiative]</td> 
      <td>As datas de início e término da iniciativa. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Project]</td> 
      <td> <p>As [!UICONTROL Datas de início planejado] e [!UICONTROL Conclusão] do projeto vinculado.</p> <p>Dica: Se as informações do [!UICONTROL Project] estiverem ausentes, o projeto será excluído.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Edite o nome da iniciativa. Por padrão, ele corresponde ao nome do projeto.
1. (Opcional) Siga um destes procedimentos:

   * Atualizar funções de trabalho na **[!UICONTROL Funções de Trabalho Obrigatórias]** seção
   * Atualize o **[!UICONTROL Custos fixos]** no **[!UICONTROL Custos]** seção

   * Clique em **[!UICONTROL Atualizar funções de trabalho disponíveis]** ou **[!UICONTROL Atualizar orçamento disponível]** resolver conflitos entre a nova iniciativa e outras iniciativas sobre o plano.

1. (Condicional) Clique em **[!UICONTROL Aplicar]** para salvar alterações em sua iniciativa.
1. Clique em **[!UICONTROL Salvar plano]** para salvar as alterações no plano.
1. (Opcional) Para atualizar as alterações feitas na iniciativa de volta ao projeto do qual ela foi importada, publique o projeto do plano. Para obter informações sobre planos de publicação, consulte [Atualize ou crie projetos publicando iniciativas no [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md).
1. (Opcional) Clique no ícone do projeto para acessar o projeto vinculado.

   ![](assets/project-icon-on-initiative-highlighted-350x49.png)
