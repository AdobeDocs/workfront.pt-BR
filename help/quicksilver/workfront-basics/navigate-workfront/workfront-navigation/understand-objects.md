---
content-type: overview;reference
navigation-topic: workfront-navigation
title: Entender objetos em [!DNL Adobe Workfront]
description: Entender objetos em [!DNL Adobe Workfront]
feature: Get Started with Workfront
exl-id: f324f198-5472-4cf2-a46e-7fc24605ca90
source-git-commit: 9c78d8e08e62c86a4e1340644ed76c61ce7f2674
workflow-type: tm+mt
source-wordcount: '2308'
ht-degree: 6%

---

# Entender objetos em [!DNL Adobe Workfront]

<!--
<***Linked to several articles, do not remove/ change. 
-->

As informações exibidas em [!DNL Adobe Workfront] é representado por objetos armazenados no [!DNL Workfront] banco de dados. Os objetos são o que direciona as informações [!DNL Workfront].

Como entender como os objetos são definidos em [!DNL Workfront] é importante para que você possa usar o objeto correto para as necessidades necessárias em sua organização.

Por exemplo, quando você planeja uma grande quantidade de trabalho, é necessário usar a variável [!UICONTROL Projeto] para definir esse trabalho. Para dividir esse trabalho em incrementos planejados menores, você pode usar a variável [!UICONTROL Tarefa] objeto. Para uma quantidade menor de trabalho não planejado e que pode ocorrer inesperadamente, é possível usar o objeto Issue . Se você quiser acompanhar o progresso e a adesão ao orçamento e à linha do tempo de um grupo de projetos, poderá organizá-los em [!UICONTROL Portfolio] e [!UICONTROL Programas]. Para definir outros elementos que ajudam a resolver seu trabalho, você deseja usar outros objetos armazenados em [!UICONTROL Projetos], [!UICONTROL Tarefas], [!UICONTROL Problemas]ou [!UICONTROL Portfolio], como [!UICONTROL Documentos], [!UICONTROL Notas], [!UICONTROL Horas], [!UICONTROL Usuários]ou [!UICONTROL Funções do Trabalho].

[!UICONTROL Relatórios] e [!UICONTROL Painéis] são outro exemplo de objetos que pode ajudar a organizar a quantidade de dados que você tem em [!DNL Workfront] visualmente, para facilitar o acesso para todos os usuários.

Para obter uma lista completa de objetos em [!DNL Workfront], consulte o [API Explorer](../../../wf-api/general/api-explorer.md).

## Interdependência e hierarquia de objetos

Os objetos são vinculados uns aos outros no [!UICONTROL Workfront]. Por exemplo, uma tarefa ou um problema nunca pode existir independentemente fora de um projeto. [!UICONTROL Tarefas] e [!UICONTROL problemas] são exemplos de objetos armazenados no [!UICONTROL projeto] objeto. [!UICONTROL Tarefas] e [!UICONTROL problemas] são considerados objetos filhos de projetos.

Veja a seguir alguns dos objetos usados com mais frequência em [!DNL Workfront] e seus respectivos objetos pai e filho:

| **Objeto** | **Objetos pai** | **Objetos filho** |
|---|---|---|
| [!UICONTROL Portfólios] |  | [!UICONTROL Programas], [!UICONTROL Projetos], [!UICONTROL Documentos], [!DNL Notes], [!UICONTROL Usuários] |
| [!UICONTROL Programas] | [!UICONTROL Portfólios] | [!UICONTROL Projetos], [!UICONTROL Documentos], [!UICONTROL Notas], [!UICONTROL Usuários] |
| [!UICONTROL Projetos] | [!UICONTROL Portfolio], [!UICONTROL Programas] | [!UICONTROL Tarefas], [!UICONTROL Problemas], [!UICONTROL Documentos], [!UICONTROL Notas], [!UICONTROL Horas], [!UICONTROL Usuários] |
| [!UICONTROL Tarefas] | [!UICONTROL Projetos] | [!UICONTROL Problemas], [!UICONTROL Tarefas Filhas], [!UICONTROL Documentos], [!UICONTROL Notas], [!UICONTROL Horas], [!UICONTROL Usuários] |
| [!UICONTROL Problemas] | [!UICONTROL Tarefas], [!UICONTROL Projetos] | [!UICONTROL Documentos], [!UICONTROL Notas], [!UICONTROL Horas], [!UICONTROL Usuários] |
| [!UICONTROL Painéis] |  | [!UICONTROL Relatórios], Páginas externas |
| [!UICONTROL Relatórios] | [!UICONTROL Painéis] |  |
| [!UICONTROL Grupos] |  | [!UICONTROL Usuários] |
| [!UICONTROL Equipes] |  | [!UICONTROL Usuários] |
| [!UICONTROL Usuários] | [!UICONTROL Grupos], [!UICONTROL Equipes], [!UICONTROL Empresas] | [!UICONTROL Função no trabalho] |
| [!UICONTROL Empresas] |  | [!UICONTROL Usuários] |
| [!UICONTROL Documentos] | [!UICONTROL Tarefas], [!UICONTROL Problemas], [!UICONTROL Projetos], [!UICONTROL Portfolio], [!UICONTROL Programas], [!UICONTROL Usuários] |  |
| [!UICONTROL Planos]* |  | [!UICONTROL Iniciativas] |
| [!DNL Goals]* |  | [!UICONTROL Resultados], [!UICONTROL Atividades] |

Para obter uma lista completa de objetos em [!DNL Workfront], consulte o [API Explorer](../../../wf-api/general/api-explorer.md).

*Os planos são os objetos da variável [!DNL Workfront Scenario Planner]. Para obter informações sobre o [!DNL Scenario Planner], consulte [O [!UICONTROL Planejador de Cenário] visão geral](../../../scenario-planner/scenario-planner-overview.md).

*[!UICONTROL Metas] são objetos de [!DNL Workfront Goals]. Para obter informações sobre [!DNL Workfront Goals], consulte [[!DNL Adobe Workfront Goals] visão geral](../../../workfront-goals/goal-management/wf-goals-overview.md).


## Personalizar nomes de objetos

Como um [!DNL Workfront] administrador, é possível personalizar os nomes de objetos em [!DNL Workfront] usando um  [!UICONTROL Modelo de layout].

Para obter mais informações sobre como personalizar nomes de objetos usando um  [!UICONTROL Modelo de layout], consulte [Criar e gerenciar modelos de layout](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

Após personalizar um modelo de layout e atribuí-lo aos usuários, eles visualizarão os nomes personalizados dos objetos. Os usuários que foram atribuídos ao modelo de layout não veem mais os nomes padrão dos objetos em qualquer lugar no aplicativo Web.

>[!NOTE]
>
>Para que os novos nomes dos objetos fiquem visíveis para os usuários, eles devem fazer logoff e logon novamente no [!DNL Workfront] depois de salvar o  [!UICONTROL Modelo de layout].

>[!IMPORTANT]
>
>O [!DNL Workfront] a documentação sempre se refere aos nomes padrão dos objetos. Como um [!DNL Workfront] administrador, certifique-se de notificar os usuários sobre as alterações nos nomes de objetos, para que eles possam entender como usar a variável [!DNL Workfront] documentação, bem como as áreas dos aplicativos que não refletem as alterações nos nomes dos objetos.

* [Nomes de objetos que podem ser personalizados usando um  [!UICONTROL Modelo de layout]](#object-names-that-can-be-customized-using-a-layout-template)
* [Áreas de [!DNL Workfront] que refletem os nomes de objeto personalizados](#areas-of-workfront-that-reflect-the-customized-object-names)
* [Áreas de [!DNL Workfront] que não refletem os nomes de objetos personalizados](#areas-of-workfront-that-do-not-reflect-the-customized-object-names)

### Nomes de objetos que podem ser personalizados usando um [!UICONTROL Modelo de layout]

Como um [!DNL Workfront] administrador, é possível personalizar os nomes dos seguintes objetos para corresponder à terminologia na organização:

* [!UICONTROL Portfólio]
* [!UICONTROL Programa]
* [!UICONTROL Projeto]
* [!UICONTROL Tarefa]
* [!UICONTROL Problema]
* [!UICONTROL Meta]*
* [!UICONTROL Resultado]*
* [!UICONTROL Atividade]*

   *[!UICONTROL Metas], [!UICONTROL resultados]e [!UICONTROL atividades] só estarão disponíveis se sua empresa tiver comprado [!DNL Workfront Goals]. Para obter informações sobre [!DNL Workfront Goals], consulte [[!DNL Adobe Workfront Goals] visão geral](../../../workfront-goals/goal-management/wf-goals-overview.md).

* [!UICONTROL Iniciativa]**
* [!UICONTROL Cenário]**
* [!UICONTROL Plano]**

   **[!UICONTROL Iniciativas], [!UICONTROL cenários]e [!UICONTROL planos] estão disponíveis somente se sua empresa adquiriu o [!DNL Workfront Scenario Planner]. Para obter informações sobre o [!DNL Scenario Planner], consulte [Introdução ao [!DNL Scenario Planner]](../../../scenario-planner/get-started-with-scenario-planning.md).


Por exemplo, se a quantidade maior de trabalho em sua organização for conhecida como &quot;Envolvimento&quot;, você poderá substituir o nome &quot;[!UICONTROL Projeto]&quot; por &quot;Envolvimento&quot;. Seu [!DNL Workfront] a interface mostra &quot;Envolvimento&quot; em vez de &quot;[!UICONTROL Projeto]&#39; em todos os locais onde o nome &#39;[!UICONTROL Projeto]&#39; apareceria.

Para obter mais informações sobre como personalizar nomes de objetos usando  [!UICONTROL Modelos de layout], consulte [Criar e gerenciar modelos de layout](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

Não é possível personalizar os nomes de nenhum outro objeto no Workfront. Para obter uma lista completa de objetos em [!DNL Workfront], consulte o [API Explorer](../../../wf-api/general/api-explorer.md).

Quando você personaliza o nome de um objeto, o novo nome desse objeto aparece na maioria das áreas da variável [!DNL Workfront] aplicativo onde esse nome de objeto seria exibido.

### Áreas de [!DNL Workfront] que refletem os nomes de objeto personalizados

As seguintes áreas mostram o nome atualizado dos objetos:

* Navegação Superior
* Todas as seções no painel de navegação esquerdo
* Todos os menus
* Notificações no aplicativo
* Construtor de relatórios e elementos de relatório (exibições, filtros e agrupamentos)
* [!UICONTROL Salvar] botões
* Arquivos exportados
* Emails
* Aplicativos móveis

### Áreas de [!DNL Workfront] que não refletem os nomes de objetos personalizados

As seguintes áreas não mostram o nome atualizado dos objetos:

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p>Referenced Object Type selection for a Typeahead field in a Custom Form </p> <p>(NOTE: drafting this because I don't think this is true)</p> </li>
  -->

* [!DNL Outlook] Suplemento

## Implicações da personalização de nomes de objetos

Você deve estar ciente do seguinte ao personalizar nomes de objetos em [!DNL Workfront]:

* Você pode encontrar erros estilísticos ou gramaticais nas exibições do sistema. Por exemplo, se você renomear &#39;[!UICONTROL Problema]&#39; para &#39;Solicitar&#39; e você vê em qualquer lugar do sistema a frase &#39;Uma solicitação&#39;, isso está funcionando como pretendido e não deve ser considerado um erro.
* Os nomes personalizados dos objetos não são traduzíveis. Somente a variável [!DNL Workfront] os nomes padrão podem ser traduzidos nos idiomas suportados. Para obter mais informações sobre idiomas compatíveis com o [!DNL Workfront], consulte [Idiomas suportados em [!DNL Adobe Workfront]](../../../workfront-basics/supported-languages-in-workfront.md). Os campos de nome de objeto personalizado oferecem suporte a caracteres estrangeiros para que você possa inserir a terminologia em qualquer idioma.
* Ao personalizar nomes de objetos usando uma  [!UICONTROL Modelo de layout], recomendamos que você atribua sua  [!UICONTROL Modelos de layout] em torno de suas unidades comerciais (equipes ou grupos).\
   Recomendamos que você use nomes que sejam claramente entendidos pelos usuários dessas unidades de negócios, para evitar confusão.
* As notificações por email e os relatórios entregues sempre contêm nomes de objetos, conforme definido pelo  [!UICONTROL Modelo de layout] do usuário que gera o email. Seus usuários devem estar preparados para ver nomes de objetos em seus emails que não estejam relacionados a seus grupos ou equipes, se receberem notificações por email de usuários em outras equipes e grupos.\
   Como um [!DNL Workfront] administrador, aconselhe os usuários a notarem os ícones associados a cada objeto. Os ícones permanecem consistentes entre vários nomes de objetos e são consistentes com o objeto padrão, como ele aparece no banco de dados. Para uma lista de todos [!DNL Workfront] ícones associados a objetos, consulte [Ícones de objeto](#object-icons).

   >[!TIP]
   >
   >Para tarefas comuns em sua organização, considere criar uma documentação personalizada para refletir sua terminologia.

## Ícones de objeto

O [!DNL Workfront] a documentação sempre se refere aos nomes padrão dos objetos. Se os objetos tiverem seus nomes personalizados, você poderá confiar no ícone associado a eles para entender qual objeto personalizado corresponde ao qual [!DNL Workfront] objeto padrão.

Para obter mais informações sobre quais objetos podem ter nomes personalizados em [!DNL Workfront], consulte [Nomes de objetos que podem ser personalizados usando um  [!UICONTROL Modelo de layout]](#object-names-that-can-be-customized-using-a-layout-template).

Veja a seguir uma lista de objetos e seus ícones correspondentes no Workfront.

| **Objeto** | **Ícone** | **Nome de objeto personalizável** |
|---|---|---|
| [!UICONTROL Empresa] | ![](assets/company-icon-nwe.png)  , ![](assets/nwe-company-icon-54x54.png) |  |
| [!UICONTROL Painel de Controle] | ![](assets/dashboard-icon-nwe.png)  , ![](assets/nwe-dashboards-icon.png) |  |
| [!UICONTROL Meta] | ![](assets/nwe-goal-icon.png) | ✔ |
| [!UICONTROL Grupo] | ![](assets/groups-icon-nwe.png)  , ![](assets/nwe-group-icon.png) |  |
| [!UICONTROL Problema] | ![](assets/issue-icon-nwe.png)  , ![](assets/nwe-issues-icon.png) | ✔ |
| [!UICONTROL Função de trabalho] | ![job_role_icon.png](assets/job-role-icon-52x50.png), ![job_role_icon_1_.png](assets/job-role-icon--1--53x44.png), ![](assets/job-role-nwe-no-color.png), ![](assets/job-role-icon-nwe-color.png) |  |
| [!UICONTROL Plano] | ![](assets/plan-icon.png), ![](assets/nwe-plan-icon-60x57.png) |  |
| [!UICONTROL Portfólio] | ![](assets/portfolio-icon-nwe.png)  , ![](assets/nwe-portfolios-icon.png) | ✔ |
| [!UICONTROL Programa] | ![](assets/program-icon-nwe.png)  , ![](assets/nwe-programs-icon.png) | ✔ |
| [!UICONTROL Projeto] | ![](assets/project-icon-nwe.png)  , ![](assets/nwe-projects-icon.png) | ✔ |
| [!UICONTROL Relatório] | ![](assets/report-icon-nwe.png) , ![](assets/nwe-reports-icon.png) |  |
| [!UICONTROL Tarefa] | ![](assets/task-icon-new.png)  , ![](assets/nwe-tasks-icon.png) | ✔ |
| [!UICONTROL Equipe] | ![](assets/team-icon-nwe.png), ![](assets/team-icon-nwe-color.png) , ![](assets/nwe-teams-icon.png) |  |
| [!UICONTROL Modelo] | ![](assets/template-icon-nwe.png)  , ![](assets/nwe-templates-icon.png) |  |

## Números de referência de objetos

Cada objeto criado em [!DNL Workfront] é atribuído um número de referência exclusivo. Os números de referência são úteis na distinção entre dois objetos similares (como tarefas com o mesmo nome). É possível pesquisar objetos usando seus números de referência e incluir números de referência em relatórios.

Para obter informações sobre como pesquisar objetos por número de referência, consulte [Usar o número de referência de objetos](../../../workfront-basics/navigate-workfront/search/reference-number-of-objects.md).

## Pesquisas específicas por objeto

É possível pesquisar em todos os objetos pesquisáveis no [!DNL Workfront]ou você pode selecionar um objeto específico para procurar em suas pesquisas básicas e avançadas.

Nem todos os objetos podem ser pesquisados no [!DNL Workfront]. Você pode executar pesquisas básicas e avançadas para os seguintes objetos em [!DNL Workfront]:

| **Objeto** | **Pesquisa Básica** | **Busca Avançada** |
|---|---|---|
| [!UICONTROL Projetos] | ✓ | ✓ |
| [!UICONTROL Tarefas] | ✓ | ✓ |
| [!UICONTROL Problemas] | ✓ | ✓ |
| [!UICONTROL Relatórios] | ✓ | ✓ |
| [!UICONTROL Usuários] | ✓ | ✓ |
| [!UICONTROL Modelos] | ✓ | ✓ |
| [!UICONTROL Documentos] | ✓ | ✓ |
| [!UICONTROL Portfólios] | ✓ | ✓ |
| [!UICONTROL Programas] | ✓ | ✓ |
| [!UICONTROL Painéis] | ✓ | ✓ |
| [!UICONTROL Empresas] | ✓ | ✓ |
| [!UICONTROL Notas] | ✓ |  |

Para obter mais informações sobre como executar pesquisas básicas e avançadas no [!DNL Workfront], consulte [Pesquisar [!DNL Adobe Workfront]](../../../workfront-basics/navigate-workfront/search/search-workfront.md).

## Relatório sobre objetos

Compreender a hierarquia e a interdependência de objetos é extremamente importante antes de começar a criar relatórios em [!DNL Workfront]. Os relatórios são específicos do objeto. Você deve selecionar o objeto correto para seu relatório antes de poder exibir os dados desejados.

Dependendo do objeto selecionado para o relatório, é possível acessar apenas os objetos que estão diretamente vinculados ao objeto do relatório.

>[!IMPORTANT]
>
>É possível criar relatórios somente sobre o objeto selecionado e os objetos pai no mesmo relatório. Não é possível ter informações sobre os objetos filhos em um relatório de objeto pai. Por exemplo, você pode exibir informações do projeto em um relatório de tarefa, mas não informações de tarefa em um relatório de projeto.

Você pode criar relatórios sobre todos os objetos no banco de dados usando nossa API aberta. Para obter uma lista completa de todos os objetos no banco de dados, consulte [API Explorer](../../../wf-api/general/api-explorer.md).

>[!NOTE]
>
>Se você personalizou os nomes dos objetos usando um modelo de layout, os nomes dos objetos no construtor de relatórios também foram personalizados. Saiba quais objetos foram personalizados e procure o nome personalizado no construtor de relatórios. Para obter mais informações sobre quais objetos podem ter nomes personalizados em [!DNL Workfront], consulte *[Nomes de objetos que podem ser personalizados usando um  [!UICONTROL Modelo de layout]](#object-names-that-can-be-customized-using-a-layout-template).*
>Ao usar o modo de texto em seus relatórios, os nomes dos objetos em expressões de modo de texto são os nomes padrão em [!DNL Workfront]e não os nomes de objeto personalizados. Para obter mais informações sobre como usar o modo de texto nos relatórios, consulte [Visão geral do modo de texto](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

Para obter mais informações sobre como criar um relatório, consulte [Criar um relatório personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).\
Para obter mais informações sobre nossa API, consulte [API Explorer](../../../wf-api/general/api-explorer.md).

Você pode criar relatórios sobre os seguintes objetos ao usar o construtor de relatórios na [!DNL Workfront] aplicação web:

* [!UICONTROL Projeto]
* [!UICONTROL Tarefa]
* [!UICONTROL Hora]
* [!UICONTROL Problema]
* [!UICONTROL Usuário]
* [!UICONTROL Nível de acesso]
* [!UICONTROL Aprovação]
* [!UICONTROL Processo de aprovação]
* [!UICONTROL Atribuição]
* [!UICONTROL Item de Trabalho do Backlog]\
   Exibe tarefas ou problemas no backlog ágil. Para obter mais informações sobre o backlog ágil, consulte [Gerenciar o backlog ágil](../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md).

* [!UICONTROL Linha de base]
* [!UICONTROL Tarefa da Linha de Base]
* [!UICONTROL Registro de Cobrança]
* [!UICONTROL Hora orçada]

   Este é o [!UICONTROL Horas Orçamentadas], conforme aparecem no nas ferramentas de gerenciamento de recursos mais antigas e obsoletas.

   O &quot;Bud&quot;. Campo &quot;Horas&quot; na [!UICONTROL Hora do Orçamento] relatório refere-se às horas orçadas para funções de cargo na [!UICONTROL Planejador de recursos]. Para obter mais informações, consulte [Entender [!UICONTROL Custo de Mão-de-Obra Orçada] e [!UICONTROL Horas Orçamentadas] para projetos](../../../manage-work/projects/project-finances/budgeted-labor-cost.md).

* [!UICONTROL Evento de calendário]
* [!UICONTROL Categoria] ou [!UICONTROL Formulário personalizado])
* [!UICONTROL Empresa]
* [!UICONTROL Painel de Controle]
* [!UICONTROL Documento]
* [!UICONTROL Aprovação de documento]
* [!UICONTROL Versão do Documento]\
   Permite exibir várias informações sobre a versão do documento, o documento ao qual a versão está associada, quem criou a versão e o usuário que criou a prova na versão do documento, se existir (Criador de prova).
* [!UICONTROL Modelo de email]
* [!UICONTROL Despesa]
* [!UICONTROL Tipo de Despesa]
* [!UICONTROL Página Externa]
* [!UICONTROL Favorito]
* [!UICONTROL Filtro]
* [!UICONTROL Meta]

   Você pode criar um relatório para metas estratégicas ou pode exibir informações relacionadas à meta em um relatório de projeto quando os projetos estão associados a metas como atividades de meta. Você pode criar metas estratégicas e conectar projetos somente se sua organização tiver comprado um [!DNL Workfront Goals] licença. Para obter informações sobre [!DNL Workfront Goals], consulte [[!DNL Workfront Goals] visão geral](https://one.workfront.com/s/document-item?bundleId=the-new-workfront-experience&amp;topicId=Content%2FWorkfront_Goals%2FGoal_management%2Fwf-goals-overview.htm&amp;_LANG=en). Para obter informações sobre como conectar projetos a metas estratégicas, consulte [Adicionar projetos às metas em Metas da Adobe Workfront](https://one.workfront.com/s/document-item?bundleId=the-new-workfront-experience&amp;topicId=Content%2FWorkfront_Goals%2FResults_and_activities%2Fconnect-projects-to-goals-overview.htm&amp;_LANG=en).

   <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  (NOTE: hardcoded links in this paragraph)
  </MadCap:conditionalText>
  -->

   >[!TIP]
   >
   >Não é possível relatar as metas do projeto associadas a um [!UICONTROL Caso de negócios]. Para obter informações sobre metas de projeto versus metas estratégicas, consulte [Glossário de [!DNL Adobe Workfront] terminologia](../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

* [!UICONTROL Grupo]
* [!UICONTROL Agrupamento]
* [!UICONTROL Tipo de hora]
* [!UICONTROL Iniciativa]

   Você pode criar um relatório para iniciativas que são objetos filhos de um plano somente se sua empresa adquiriu um [!DNL Workfront Scenario Planner] licença. Para obter informações sobre iniciativas, consulte [Visão geral das iniciativas na [!DNL Workfront Scenario Planner]](https://one.workfront.com/s/csh?context=2066&amp;pubname=the-new-workfront-experience).

   <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  (NOTE: this link is hardcoded)
  </MadCap:conditionalText>
  -->

* Função de trabalho da iniciativa

   Você pode criar um relatório para as funções de cargo associadas às iniciativas em um plano somente se a empresa adquiriu um [!DNL Workfront Scenario Planner] licença. Para obter informações sobre como criar iniciativas e associá-las a funções de cargo, consulte [Crie e edite iniciativas na [!DNL Workfront Scenario Planner]](https://one.workfront.com/s/csh?context=2061&amp;pubname=the-new-workfront-experience).

   <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  (NOTE: this link is hardcoded)
  </MadCap:conditionalText>
  -->

* [!UICONTROL Iteração]
* [!UICONTROL Função de trabalho]
* [!UICONTROL Entrada no Relatório]

   Você pode criar relatórios sobre atualizações rastreadas do sistema no [!UICONTROL Atualizações] área de objetos como tarefas, projetos, problemas, etc. Para saber mais, consulte [Relatório sobre [!UICONTROL Atualizações] area](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-journal-entry-report.md).

* [!UICONTROL Modelo de Layout]
* [!UICONTROL Etapa]
* [!UICONTROL Caminho de Etapas]
* [!UICONTROL Nota]

   >[!NOTE]
   >
   >É possível criar relatórios sobre comentários adicionados por usuários individuais.

* [!UICONTROL Parâmetro] ou [!UICONTROL Campo personalizado])
* [!UICONTROL Grupo de parâmetros] ou [!UICONTROL Quebra de seção])
* [!UICONTROL Perfil do portal] (isso exibe informações que foram substituídas)
* [!UICONTROL Portfólio]
* [!UICONTROL Programa]
* [!UICONTROL Projeto] ([!UICONTROL Dados financeiros])

   >[!NOTE]
   >
   >As informações financeiras são preenchidas em [!UICONTROL Projeto] ([!UICONTROL Dados financeiros]) relata somente quando os dados associados a ela tiverem menos de 5 anos. Por exemplo, se uma função de trabalho foi alocada para uma tarefa em janeiro de 2015 e hoje é setembro de 2021, um campo financeiro como o [!UICONTROL Data de alocação] para a função de trabalho não é preenchida na variável [!UICONTROL Projeto (Dados Financeiros)] relatório.

* [!UICONTROL Aprovação da revisão]\
   Permite exibir várias informações sobre a aprovação de prova, incluindo: a prova que foi submetida para aprovação, informações sobre a [!UICONTROL Aprovador], informações sobre o Requerente (se o Requerente for um licenciado) [!DNL Workfront] usuário), informações de versão, a ID da prova e a data de criação da prova.\
   [!UICONTROL Aprovação de prova] Os relatórios incluem somente provas que estão disponíveis nas áreas Meu trabalho dos usuários, onde as decisões ainda não foram tomadas.\
   As aprovações de prova são atribuídas em [!DNL Workfront] conforme descrito [Adicionar usuários a uma prova](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md#add) em [Compartilhar uma prova em [!DNL Adobe Workfront]](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md).

* [!UICONTROL Fila]
* [!UICONTROL Enfileirar tópico]
* [!UICONTROL Rate] (isso exibe a função de trabalho [!UICONTROL Taxa de Faturamento] informações)
* [!UICONTROL Lembrete de Notificação]
* [!UICONTROL Relatório]
* [!UICONTROL Conjunto de Recursos]
* [!UICONTROL Risco]
* [!UICONTROL Tipo de Risco]
* [!UICONTROL Cronograma]
* [!UICONTROL Scorecard]
* [!UICONTROL Equipe]
* [!UICONTROL Modelo]
* [!UICONTROL Modelo de Tarefa]
* [!UICONTROL Folga]

   Você pode relatar o tempo de folga de um usuário, conforme indicado pelo usuário em seu perfil.

* [!UICONTROL Planilha de horas]
* [!UICONTROL Perfil da Planilha de Horas]
* [!UICONTROL Grupo de Tópicos]
* [!UICONTROL Delegação de usuários]

   Você pode relatar usuários que foram delegados para executar tarefas e problemas de outras pessoas enquanto estão fora do escritório. Este relatório exibe o usuário que está fora do escritório, bem como o usuário que cumpre suas funções enquanto está fora.

* [!UICONTROL Exibir]
* [!UICONTROL Item de Trabalho] (refere-se a tarefas e questões)
