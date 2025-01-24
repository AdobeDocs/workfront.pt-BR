---
content-type: overview;reference
navigation-topic: workfront-navigation
title: Visão geral de [!DNL Adobe Workfront] objetos
description: As informações exibidas em  [!DNL Adobe Workfront]  são representadas por objetos armazenados no banco de dados  [!DNL Workfront] . Os objetos são o que direciona as informações em  [!DNL Workfront]. Saiba mais sobre esses objetos neste artigo.
feature: Get Started with Workfront
author: Alina
exl-id: f324f198-5472-4cf2-a46e-7fc24605ca90
source-git-commit: 158af1f48fba264b98108b5f0a573b7904eb875e
workflow-type: tm+mt
source-wordcount: '2424'
ht-degree: 1%

---

# Visão geral de [!DNL Adobe Workfront] objetos

<!--Audited: 12/2023-->

<!--
<***Linked to several articles, do not remove/ change. 
-->

As informações exibidas em [!DNL Adobe Workfront] são representadas por objetos armazenados no banco de dados [!DNL Workfront]. Os objetos são o que direciona as informações em [!DNL Workfront].

Entender como os objetos são definidos em [!DNL Workfront] é importante para que você possa usar o objeto correto de acordo com as necessidades da sua organização.

Por exemplo, quando você planeja uma grande quantidade de trabalho, precisa usar o objeto [!UICONTROL Projeto] para definir esse trabalho. Para dividir este trabalho em incrementos planejados menores, você pode usar o objeto [!UICONTROL Task]. Para uma quantidade menor de trabalho que não é planejado e pode ocorrer inesperadamente, você pode usar o objeto Problema. Para acompanhar o progresso e a adesão ao orçamento e à linha do tempo de um grupo de projetos, você pode organizá-los em [!UICONTROL Portfolio] e [!UICONTROL Programas]. Para definir outros elementos que ajudam a resolver seu trabalho, você deseja usar outros objetos armazenados em [!UICONTROL Projetos], [!UICONTROL Tarefas], [!UICONTROL Problemas] ou [!UICONTROL Portfolio], como [!UICONTROL Documentos], [!UICONTROL Atualizações], [!UICONTROL Horas], [!UICONTROL Usuários] ou [!UICONTROL Funções de Trabalho].

Os [!UICONTROL Relatórios] e os [!UICONTROL Painéis] são outro exemplo de objetos que podem ajudá-lo a organizar visualmente a quantidade de dados que você tem no [!DNL Workfront], tornando-o facilmente acessível para todos os usuários.

Para obter uma lista completa de objetos em [!DNL Workfront], consulte o [API Explorer](../../../wf-api/general/api-explorer.md).

## Interdependência e hierarquia de objetos

Objetos são vinculados entre si no [!UICONTROL Workfront]. Por exemplo, uma tarefa ou um problema nunca pode existir independentemente fora de um projeto. [!UICONTROL Tarefas] e [!UICONTROL problemas] são exemplos de objetos armazenados no objeto [!UICONTROL projeto]. [!UICONTROL Tarefas] e [!UICONTROL problemas] são considerados objetos filho para projetos.

A seguir estão alguns dos objetos usados com mais frequência em [!DNL Workfront] e seus respectivos objetos pai e filho:

| **Objeto** | **Objetos pai** | **Objetos filho** |
|---|---|---|
| [!UICONTROL Portfólios] |  | [!UICONTROL Programas], [!UICONTROL Projetos], [!UICONTROL Documentos], [!DNL Notes], [!UICONTROL Usuários] |
| [!UICONTROL Programas] | [!UICONTROL Portfólios] | [!UICONTROL Projetos], [!UICONTROL Documentos], [!UICONTROL Notas], [!UICONTROL Usuários] |
| [!UICONTROL Projetos] | [!UICONTROL Portfolio], [!UICONTROL Programas] | [!UICONTROL Tarefas], [!UICONTROL Problemas], [!UICONTROL Documentos], [!UICONTROL Notas], [!UICONTROL Horas], [!UICONTROL Usuários] |
| [!UICONTROL Tarefas] | [!UICONTROL Projetos] | [!UICONTROL Problemas], [!UICONTROL Tarefas Filhas], [!UICONTROL Documentos], [!UICONTROL Notas], [!UICONTROL Horas], [!UICONTROL Usuários] |
| [!UICONTROL Problemas] | [!UICONTROL Tarefas], [!UICONTROL Projetos] | [!UICONTROL Documentos], [!UICONTROL Notas], [!UICONTROL Horas], [!UICONTROL Usuários] |
| [!UICONTROL Painéis] |  | [!UICONTROL Relatórios], Páginas Externas |
| [!UICONTROL Relatórios] | [!UICONTROL Painéis] |  |
| [!UICONTROL Grupos] |  | [!UICONTROL Usuários] |
| [!UICONTROL Equipes] |  | [!UICONTROL Usuários] |
| [!UICONTROL Usuários] | [!UICONTROL Grupos], [!UICONTROL Equipes], [!UICONTROL Empresas] | [!UICONTROL Funções de trabalho] |
| [!UICONTROL Empresas] |  | [!UICONTROL Usuários] |
| [!UICONTROL Documentos] | [!UICONTROL Tarefas], [!UICONTROL Problemas], [!UICONTROL Projetos], [!UICONTROL Portfolio], [!UICONTROL Programas], [!UICONTROL Usuários] |  |
| [!UICONTROL Planos]* |  | [!UICONTROL Iniciativas] |
| [!DNL Goals]* |  | [!UICONTROL Resultados], [!UICONTROL Atividades] |

Para obter uma lista completa de objetos em [!DNL Workfront], consulte o [API Explorer](../../../wf-api/general/api-explorer.md).

*Planos são objetos de [!DNL Adobe Workfront Scenario Planner]. Para obter informações sobre [!DNL Scenario Planner], consulte [A [!UICONTROL visão geral do Planejador de cenários]](../../../scenario-planner/scenario-planner-overview.md).

*[!UICONTROL Metas] são os objetos de [!DNL Adobe Workfront Goals]. Para obter informações sobre [!DNL Workfront Goals], consulte [[!DNL Adobe Workfront Goals] visão geral](../../../workfront-goals/goal-management/wf-goals-overview.md).


## Personalizar nomes de objetos

Como administrador do [!DNL Workfront], você pode personalizar nomes de objetos em [!DNL Workfront] usando um [!UICONTROL Modelo de Layout].

Para obter mais informações sobre como personalizar nomes de objeto usando um [!UICONTROL Modelo de Layout], consulte [Criar e gerenciar modelos de layout](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

Depois de personalizar um modelo de layout e atribuí-lo aos usuários, esses usuários verão os nomes personalizados dos objetos. Os usuários atribuídos ao modelo de layout não verão mais os nomes padrão dos objetos em nenhum lugar no aplicativo web.

Por exemplo, se a maior quantidade de trabalho em sua organização for conhecida como &quot;Envolvimento&quot;, você poderá substituir o nome &quot;[!UICONTROL Projeto]&quot; por &quot;Envolvimento&quot;. A interface [!DNL Workfront] mostra &#39;Envolvimento&#39; em vez de &#39;[!UICONTROL Projeto]&#39; em todos os locais onde o nome &#39;[!UICONTROL Projeto]&#39; apareceria.

>[!NOTE]
>
>Para que os novos nomes dos objetos fiquem visíveis para seus usuários, eles devem fazer logoff e logon novamente em [!DNL Workfront] depois que você salvar o [!UICONTROL Modelo de Layout].

>[!IMPORTANT]
>
>A documentação [!DNL Workfront] sempre se refere aos nomes padrão dos objetos. Como administrador do [!DNL Workfront], notifique os usuários sobre as alterações nos nomes de objetos para que eles possam entender como usar a documentação do [!DNL Workfront], bem como as áreas dos aplicativos que não refletem as alterações nos nomes dos objetos.

* [Nomes de objetos que podem ser personalizados usando um [!UICONTROL Modelo de layout]](#object-names-that-can-be-customized-using-a-layout-template)
* [Áreas de  [!DNL Workfront]  que refletem os nomes de objetos personalizados](#areas-of-workfront-that-reflect-the-customized-object-names)
* [Áreas de  [!DNL Workfront]  que não refletem os nomes de objeto personalizados](#areas-of-workfront-that-do-not-reflect-the-customized-object-names)

### Nomes de objetos que podem ser personalizados usando um [!UICONTROL Modelo de layout]

Como administrador do [!DNL Workfront], você pode personalizar os nomes dos seguintes objetos para corresponder à terminologia na sua organização:

* [!UICONTROL Portfolio]
* [!UICONTROL Programa]
* [!UICONTROL Projeto]
* [!UICONTROL Tarefa]
* [!UICONTROL Problema]
* [!UICONTROL Meta]*
* [!UICONTROL Resultado]*
* [!UICONTROL Atividade]*

  *[!UICONTROL Metas], [!UICONTROL resultados] e [!UICONTROL atividades] só estarão disponíveis se sua empresa tiver comprado o [!DNL Workfront Goals]. Para obter informações sobre [!DNL Workfront Goals], consulte [[!DNL Adobe Workfront Goals] visão geral](../../../workfront-goals/goal-management/wf-goals-overview.md).

* [!UICONTROL Iniciativa]**
* [!UICONTROL Cenário]**
* [!UICONTROL Plano]**

  **[!UICONTROL Iniciativas], [!UICONTROL cenários] e [!UICONTROL planos] só estarão disponíveis se sua empresa tiver comprado o [!DNL Workfront Scenario Planner]. Para obter informações sobre o [!DNL Scenario Planner], consulte [Introdução ao [!DNL Scenario Planner]](../../../scenario-planner/get-started-with-scenario-planning.md).



Para obter mais informações sobre como personalizar nomes de objeto usando [!UICONTROL Modelos de Layout], consulte [Criar e gerenciar modelos de layout](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

Não é possível personalizar os nomes de nenhum outro objeto no Workfront. Para obter uma lista completa de objetos em [!DNL Workfront], consulte o [API Explorer](../../../wf-api/general/api-explorer.md).

Quando você personaliza o nome de um objeto, o novo nome desse objeto aparece na maioria das áreas do aplicativo [!DNL Workfront] em que esse nome de objeto apareceria.

### Áreas de [!DNL Workfront] que refletem os nomes de objetos personalizados

As áreas a seguir mostram o nome atualizado dos objetos:

* Navegação Superior
* Todas as seções na navegação do painel esquerdo
* Todos os menus
* Notificações no aplicativo
* Elementos do Report Builder e de relatórios (exibições, filtros e agrupamentos)
* [!UICONTROL Botões Salvar]
* Arquivos exportados
* Emails
* Aplicativos móveis

### Áreas de [!DNL Workfront] que não refletem os nomes de objetos personalizados

As áreas a seguir não mostram o nome atualizado dos objetos:

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p>Referenced Object Type selection for a Typeahead field in a Custom Form </p> <p>(NOTE: drafting this because I don't think this is true)</p> </li>
  -->

* Suplemento [!DNL Outlook]

### Implicações da personalização de nomes de objetos

Você deve estar ciente do seguinte ao personalizar nomes de objetos em [!DNL Workfront]:

* Você pode encontrar erros estilísticos ou gramaticais em exibições do sistema. Por exemplo, se você renomear &#39;[!UICONTROL Problema]&#39; como &#39;Solicitação&#39; e vir em qualquer lugar do sistema a frase &#39;Uma solicitação&#39;, isso está funcionando como pretendido e não deve ser considerado um erro.
* Os nomes personalizados dos objetos não podem ser traduzidos. Somente os nomes padrão [!DNL Workfront] podem ser traduzidos nos idiomas com suporte. Para obter mais informações sobre idiomas com suporte no [!DNL Workfront], consulte [Idiomas com suporte no [!DNL Adobe Workfront]](../../../workfront-basics/supported-languages-in-workfront.md). Os campos de nome de objeto personalizados oferecem suporte a caracteres estrangeiros para que você possa inserir a terminologia em qualquer idioma.
* Quando você personaliza nomes de objetos usando um [!UICONTROL Modelo de Layout], recomendamos que você atribua seus [!UICONTROL Modelos de Layout] com base nas unidades de negócios (Equipes ou Grupos).\
   Recomendamos que você use nomes claramente compreendidos pelos usuários dessas unidades de negócios para evitar confusão.
* As notificações por email e os relatórios entregues sempre contêm nomes de objetos conforme definidos pelo [!UICONTROL Modelo de layout] do usuário que gera o email. Seus usuários devem estar preparados para ver nomes de objetos em seus emails que não estão relacionados ao seu grupo ou equipe, se eles receberem notificações por email de usuários em outras equipes e grupos.\
   Como administrador do [!DNL Workfront], aconselhe os usuários a notarem os ícones associados a cada objeto. Os ícones permanecem consistentes entre vários nomes de objeto e consistentes com o objeto padrão, conforme ele aparece no banco de dados. Para obter uma lista de todos os ícones [!DNL Workfront] associados a objetos, consulte [Ícones de objeto](#object-icons).

  >[!TIP]
  >
  >Para tarefas comuns em sua organização, considere criar uma documentação personalizada para refletir sua terminologia.

## Ícones de objeto

A documentação [!DNL Workfront] sempre se refere aos nomes padrão de objetos. Se seus objetos tiverem seus nomes personalizados, você poderá confiar no ícone associado a eles para entender qual objeto personalizado corresponde a qual objeto padrão [!DNL Workfront].

Para obter mais informações sobre quais objetos podem ter nomes personalizados em [!DNL Workfront], consulte [Nomes de objetos que podem ser personalizados usando um [!UICONTROL Modelo de Layout]](#object-names-that-can-be-customized-using-a-layout-template).

Veja a seguir uma lista de objetos e seus ícones correspondentes no Workfront.

| **Objeto** | **Ícone** | **Nome de objeto personalizável** |
|---|---|---|
| [!UICONTROL Empresa] | ![](assets/company-icon-nwe.png) , ![](assets/nwe-company-icon-54x54.png) |  |
| [!UICONTROL Painel] | ![](assets/dashboard-icon-nwe.png) , ![](assets/nwe-dashboards-icon.png) |  |
| [!UICONTROL Meta] | ![](assets/nwe-goal-icon.png) | ✔ |
| [!UICONTROL Grupo] | ![](assets/groups-icon-nwe.png) , ![](assets/nwe-group-icon.png) |  |
| [!UICONTROL Problema] | ![](assets/issue-icon-nwe.png) , ![](assets/nwe-issues-icon.png) | ✔ |
| [!UICONTROL Função] | ![ícone_da_função_do_trabalho.png](assets/job-role-icon-52x50.png), ![ícone_da_função_do_trabalho_1_.png](assets/job-role-icon--1--53x44.png), ![](assets/job-role-nwe-no-color.png), ![](assets/job-role-icon-nwe-color.png) |  |
| [!UICONTROL Plano] | ![](assets/plan-icon.png), ![](assets/nwe-plan-icon-60x57.png) |  |
| [!UICONTROL Portfolio] | ![](assets/portfolio-icon-nwe.png) , ![](assets/nwe-portfolios-icon.png) | ✔ |
| [!UICONTROL Programa] | ![](assets/program-icon-nwe.png) , ![](assets/nwe-programs-icon.png) | ✔ |
| [!UICONTROL Projeto] | ![](assets/project-icon-nwe.png) , ![](assets/nwe-projects-icon.png) | ✔ |
| [!UICONTROL Relatório] | ![](assets/report-icon-nwe.png) , ![](assets/nwe-reports-icon.png) |  |
| [!UICONTROL Tarefa] | ![](assets/task-icon-new.png) , ![](assets/nwe-tasks-icon.png) | ✔ |
| [!UICONTROL Equipe] | ![](assets/team-icon-nwe.png), ![](assets/team-icon-nwe-color.png) , ![](assets/nwe-teams-icon.png) |  |
| [!UICONTROL Modelo] | ![](assets/template-icon-nwe.png) , ![](assets/nwe-templates-icon.png) |  |
| [!UICONTROL Usuário] | ![](assets/users-icon-gray.png) , ![](assets/user-icon-blue.png) , ![](assets/user-icon-initials.png) , ![](assets/user-avatar.png) , ![](assets/user-main-menu-area.png) |  |

## Números de referência de objetos

Cada objeto criado em [!DNL Workfront] recebe um número de referência exclusivo. Números de referência são úteis na distinção entre dois objetos semelhantes (como tarefas com o mesmo nome). Você pode pesquisar objetos usando seus números de referência e pode incluir números de referência em relatórios.

Para obter informações sobre como pesquisar objetos por número de referência, consulte [Usar o número de referência de objetos](../../../workfront-basics/navigate-workfront/search/reference-number-of-objects.md).

## Pesquisas específicas por objeto

Você pode pesquisar em todos os objetos que podem ser pesquisados no [!DNL Workfront] ou pode selecionar um objeto específico a ser pesquisado em suas pesquisas básicas e avançadas.

Nem todos os objetos são pesquisáveis em [!DNL Workfront]. Você pode executar pesquisas básicas e avançadas para os seguintes objetos em [!DNL Workfront]:

| **Objeto** | **Pesquisa básica** | **Pesquisa avançada** |
|---|---|---|
| [!UICONTROL Projetos] | ✓ µ | ✓ µ |
| [!UICONTROL Tarefas] | ✓ µ | ✓ µ |
| [!UICONTROL Problemas] | ✓ µ | ✓ µ |
| [!UICONTROL Relatórios] | ✓ µ | ✓ µ |
| [!UICONTROL Usuários] | ✓ µ | ✓ µ |
| [!UICONTROL Modelos] | ✓ µ | ✓ µ |
| [!UICONTROL Documentos] | ✓ µ | ✓ µ |
| [!UICONTROL Portfólios] | ✓ µ | ✓ µ |
| [!UICONTROL Programas] | ✓ µ | ✓ µ |
| [!UICONTROL Painéis] | ✓ µ | ✓ µ |
| [!UICONTROL Empresas] | ✓ µ | ✓ µ |
| [!UICONTROL Notas] (ou [!UICONTROL Atualizações]) | ✓ µ |  |

Para obter mais informações sobre como executar pesquisas básicas e avançadas no [!DNL Workfront], consulte [Pesquisa [!DNL Adobe Workfront]](../../../workfront-basics/navigate-workfront/search/search-workfront.md).


## Acesso restrito a objetos

Quando um usuário não tem acesso a um objeto, o usuário vê &quot;Sem acesso&quot; em qualquer lugar que o nome do objeto seja exibido no Workfront.

O acesso a objetos pode ser restrito no nível de acesso ou nas permissões de um objeto específico.

Isso se aplica a todos os objetos e objetos filho listados na seção [Interdependência e hierarquia de objetos](#interdependency-and-hierarchy-of-objects) deste artigo. Isso não se aplica aos objetos Equipe e Usuário.

## Relatório sobre objetos

Entender a hierarquia e a interdependência de objetos é extremamente importante antes de começar a criar relatórios no [!DNL Workfront]. Os relatórios são específicos de objetos. Você deve selecionar o objeto correto para seu relatório antes de exibir os dados desejados.

>[!IMPORTANT]
>
>Você pode relatar somente o objeto selecionado e os objetos pai no mesmo relatório. Você não pode ter informações sobre os objetos filhos em um relatório de objeto pai. Por exemplo, você pode exibir informações do projeto em um relatório de tarefa, mas não informações da tarefa em um relatório de projeto.

Você pode relatar todos os objetos no banco de dados usando nossa API aberta. Para obter uma lista completa de todos os objetos no banco de dados, consulte [API Explorer](../../../wf-api/general/api-explorer.md).

>[!NOTE]
>
> * Se você tiver personalizado os nomes dos objetos usando um modelo de layout, os nomes do objeto no Report Builder também serão personalizados. Verifique se você sabe quais objetos foram personalizados e procure o nome personalizado no Report Builder. Para obter mais informações sobre quais objetos podem ter nomes personalizados em [!DNL Workfront], consulte [Nomes de objetos que podem ser personalizados usando um [!UICONTROL Modelo de Layout]](#object-names-that-can-be-customized-using-a-layout-template) neste artigo.
> * Ao usar o modo de texto em seus relatórios, os nomes dos objetos em expressões de modo de texto são os nomes padrão em [!DNL Workfront], e não os nomes de objetos personalizados. Para obter mais informações sobre como usar o modo de texto em relatórios, consulte [Visão geral do Modo de Texto](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

Para obter mais informações sobre a criação de um relatório, consulte [Criar um relatório personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).\
Para obter mais informações sobre nossa API, consulte [API Explorer](../../../wf-api/general/api-explorer.md).

### Objetos disponíveis para relatórios

Você pode criar relatórios sobre os seguintes objetos ao usar o construtor de relatórios no aplicativo Web [!DNL Workfront]. Os marcadores recuados fornecem mais informações sobre o objeto e não representam objetos adicionais.

* [!UICONTROL Projeto]
* [!UICONTROL Tarefa]
* [!UICONTROL Hora]
* [!UICONTROL Problema]
* [!UICONTROL Usuário]
* Nível de [!UICONTROL Acesso]
* [!UICONTROL Aprovação]
* [!UICONTROL Processo de aprovação]
* [!UICONTROL Atribuição]
* [!UICONTROL Linha de base]
* [!UICONTROL Tarefa da linha de base]
* [!UICONTROL Registro de Cobrança]
* [!UICONTROL Hora orçada]
   * Estas são as [!UICONTROL Horas orçadas], conforme aparecem nas ferramentas de gerenciamento de recursos obsoletas mais antigas.
   * O &quot;Bud. O campo Horas no relatório [!UICONTROL Horas Orçadas] refere-se às horas orçadas para funções de trabalho no [!UICONTROL Planejador de Recursos]. Para obter mais informações, consulte [Entender [!UICONTROL Custo do Trabalho Orçado] e [!UICONTROL Horas Orçadas] para projetos](../../../manage-work/projects/project-finances/budgeted-labor-cost.md).

* [!UICONTROL Evento de calendário]
* [!UICONTROL Empresa]
* [!UICONTROL Formulário personalizado]
* [!UICONTROL Painel]
* [!UICONTROL Documento]
* [!UICONTROL Aprovação de documento]
* [!UICONTROL Versão do Documento]
   * Você pode exibir informações sobre a versão do documento, o documento ao qual a versão está associada, quem criou a versão e o usuário que criou a prova na versão do documento, se existir (Criador da prova).
* [!UICONTROL Modelo de email]
* [!UICONTROL Despesa]
* [!UICONTROL Tipo de Despesa]
* [!UICONTROL Página Externa]
* [!UICONTROL Favorito]
* [!UICONTROL Filtro]
* [!UICONTROL Meta]
   * Você pode criar um relatório para metas estratégicas ou exibir informações relacionadas a metas em um relatório de projeto quando os projetos são associados a metas como atividades de meta. Você só poderá criar metas estratégicas e conectá-las a projetos se a sua organização tiver comprado uma licença do [!DNL Workfront Goals]. Para obter informações sobre [!DNL Workfront Goals], consulte [[!DNL Workfront Goals] visão geral](../../../workfront-goals/goal-management/wf-goals-overview.md). Para obter informações sobre como conectar projetos a metas estratégicas, consulte [Adicionar projetos a metas nas Metas da Adobe Workfront](../../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md).
*Você não pode relatar metas de projeto associadas a um [!UICONTROL Business Case]. Para obter informações sobre metas do projeto versus metas estratégicas, consulte [Glossário de [!DNL Adobe Workfront] terminologia](../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

* [!UICONTROL Grupo]
* [!UICONTROL Agrupamento]
* [!UICONTROL Tipo de Hora]
* [!UICONTROL Iniciativa]
   * Você pode criar um relatório para iniciativas que são objetos secundários de um plano somente se sua empresa tiver comprado uma licença do [!DNL Workfront Scenario Planner]. Para obter informações sobre iniciativas, consulte [Visão geral das iniciativas no [!DNL Workfront Scenario Planner]](../../../scenario-planner/initiatives-overview.md).

* Função de trabalho da iniciativa
   * Você pode criar um relatório para as funções de trabalho associadas às iniciativas em um plano somente se sua empresa tiver comprado uma licença do [!DNL Workfront Scenario Planner]. Para obter informações sobre como criar iniciativas e associá-las a funções de trabalho, consulte [Criar e editar iniciativas no [!DNL Workfront Scenario Planner]](../../../scenario-planner/create-and-edit-initiatives.md).

* [!UICONTROL Iteração]
* [!UICONTROL Função]
* [!UICONTROL Entrada do diário]
   * Você pode criar relatórios sobre atualizações de sistema rastreadas na área [!UICONTROL Atualizações] de objetos como tarefas, projetos, problemas, etc. Para obter mais informações, consulte [Relatório na área Atualizações com um relatório de Entrada de Diário](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-journal-entry-report.md).

* [!UICONTROL Modelo de layout]
* [!UICONTROL Marco]
* [!UICONTROL Caminho de Etapas]
* [!UICONTROL Observação] ou [!UICONTROL Atualizações]
   * Você pode relatar comentários adicionados por usuários individuais.

* [!UICONTROL Parâmetro] (ou [!UICONTROL Campo Personalizado])
* [!UICONTROL Grupo de Parâmetros] (ou [!UICONTROL Quebra de Seção])
* [!UICONTROL Portfolio]
* [!UICONTROL Programa]
* [!UICONTROL Projeto (Dados Financeiros)]
   * As informações financeiras são populadas nos relatórios do [!UICONTROL Project (Financial Data)] somente quando os dados associados a elas têm menos de 5 anos. Por exemplo, se uma função de trabalho foi alocada para uma tarefa em janeiro de 2015 e hoje é setembro de 2021, um campo financeiro como [!UICONTROL Data de Alocação] para a função de trabalho não será preenchido no relatório [!UICONTROL Projeto (Dados Financeiros)].

  >[!CAUTION]
  >
  >A execução de um relatório de Projeto (Dados Financeiros) executa um recálculo dos dados financeiros, que podem substituir dados financeiros anteriores e levar um tempo significativo. Para obter mais informações sobre as consequências do recálculo de dados financeiros, consulte [Recalcular as finanças do projeto](/help/quicksilver/manage-work/projects/project-finances/recalculate-project-finances.md).

* [!UICONTROL Aprovação da revisão]
   * Permite exibir várias informações sobre a aprovação da prova, incluindo: a prova que foi enviada para aprovação, informações sobre o [!UICONTROL Aprovador], informações sobre o Solicitante (se o Solicitante for um usuário licenciado do [!DNL Workfront]), informações da versão, a ID da prova e a data de criação da prova.\
      Os relatórios de [!UICONTROL Aprovação de prova] incluem somente provas que estão disponíveis nas áreas Meu trabalho dos usuários, onde ainda não foram tomadas decisões.\
   * Aprovações de provas são atribuídas em [!DNL Workfront] conforme descrito [Adicionar usuários a uma prova](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md#add) em [Compartilhar uma prova no [!DNL Adobe Workfront]](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md).

* [!UICONTROL Fila]
* [!UICONTROL Enfileirar tópico]
* [!UICONTROL Taxa] (exibe informações sobre a [!UICONTROL Taxa de Cobrança] da função de trabalho)
* [!UICONTROL Notificação de Lembrete]
* [!UICONTROL Relatório]
* [!UICONTROL Pool de Recursos]
* [!UICONTROL Risco]
* [!UICONTROL Tipo de Risco]
* [!UICONTROL Agendar]
* [!UICONTROL Scorecard]
* [!UICONTROL Equipe]
* [!UICONTROL Modelo]
* [!UICONTROL Modelo de Tarefa]
* [!UICONTROL Folga]
   * Você pode relatar o tempo de folga de um usuário conforme indicado pelo usuário em seu perfil.

* [!UICONTROL Planilha de horas]
* [!UICONTROL Perfil de Planilha de Horas]
* [!UICONTROL Grupo de Tópicos]
* [!UICONTROL Aprovação de usuário]
* [!UICONTROL Delegação de usuários]

   * Você pode relatar usuários que foram delegados a executar tarefas e problemas de outras pessoas enquanto estiverem fora do escritório. Esse relatório exibe o usuário que está fora do escritório, bem como o usuário que cumpre suas obrigações enquanto está fora.

* [!UICONTROL Decisões de Usuários]

   * Você pode relatar quantas decisões os usuários tomaram sobre provas e documentos no mês atual.

* [!UICONTROL Exibir]
* [!UICONTROL Item de trabalho] (isso produz um relatório para tarefas e problemas)
