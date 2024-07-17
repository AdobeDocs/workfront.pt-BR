---
content-type: release-notes
navigation-topic: product-releases-archive
title: Atividade de versão final do Beta 2017.3
description: Esta página descreve todas as alterações disponíveis mais recentemente no ambiente de Pré-visualização com a versão final do Beta 2017.3. A funcionalidade nesta página foi disponibilizada no ambiente de Pré-visualização em 12 de setembro de 2017. Ele estará disponível no ambiente de Produção no início de novembro de 2017.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 880828f4-3908-4ef0-ab1f-774f8dee72b6
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '3821'
ht-degree: 0%

---

# Atividade de versão final do Beta 2017.3

Esta página descreve todas as alterações disponíveis mais recentemente no ambiente de Pré-visualização com a versão final do Beta 2017.3. A funcionalidade nesta página foi disponibilizada no ambiente de Pré-visualização em 12 de setembro de 2017. Ele estará disponível no ambiente de Produção no início de novembro de 2017.

>[!IMPORTANT]
>
> A funcionalidade descrita nesta página está sujeita a alterações antes da disponibilidade no ambiente de produção.

Para obter uma lista de todas as alterações feitas em 2017.3, consulte  Visão geral da atividade da versão [2017.3](../../../../product-announcements/product-releases/quarterly-release-archive/2017.3-release-activity/2017-3-release-activity-overview.md).

A versão final do Beta 2017.3 contém melhorias para administradores do Workfront e outros usuários:

**Para Administradores**

* [Nova Configuração para Retroceder Solicitações na Área de Configurações de Aprovação](#new-configuration-for-recalling-requests-in-the-approval-settings-area)
* [Configurar Funções De Prova Padrão](#configure-default-proof-roles)

**Para Todos Os Usuários**

* [Área Residencial (Atualizou Minha Área de Trabalho)](#home-area-updated-my-work-area)

* [Modelo de layout atualizado para oferecer suporte à Área Inicial](#updated-layout-template-to-support-the-home-area)

* [Kanban para Agile](#kanban-for-agile)
* [Incluir problemas no Backlog de Scrum de uma Equipe Agile](#include-issues-on-the-scrum-backlog-for-an-agile-team)
* [Incluir problemas no Storyboard Scrum Agile](#include-issues-on-the-scrum-agile-story-board)
* [Aplicar Agrupamentos e Filtros ao Backlog de uma Equipe Agile](#apply-groupings-and-filters-to-the-backlog-for-an-agile-team)
* [A Funcionalidade @Tagging aprimorada retorna no Ambiente de Visualização](#enhanced-tagging-functionality-returns-in-the-preview-environment)
* [As Atualizações do Sistema de Filtro no Fluxo de Atualização Agora São Persistentes entre Objetos](#filter-system-updates-in-the-update-stream-is-now-persistent-across-objects)
* [Visualizar Dados no Relatório de Utilização](#visualize-data-in-the-utilization-report)
* [Melhoria no Desempenho do Relatório de Utilização](#utilization-report-performance-improvement)
* [Melhorias do documento: interface simplificada](#document-enhancements-streamlined-interface)
* [Aprimoramentos de revisões no Workfront](#proofing-enhancements-within-workfront)
* [Aprimoramentos de revisões no Workfront Proof e no Workfront](#proofing-enhancements-within-both-workfront-proof-and-workfront)
* [Formatação de Rich Text para Atualizações e Emails](#rich-text-formatting-for-updates-and-emails)
* [Novo Design do Gráfico de Gantt](#new-gantt-chart-redesign)
* [Relatórios Internos Contêm Descrições Atualizadas](#built-in-reports-contain-updated-descriptions)
* [Identidade Visual em Relatórios, Listas e Painéis Exportados](#branding-in-exported-reports-lists-and-dashboards)
* [Melhorias ao copiar tarefas e mover tarefas ou problemas](#improvements-when-copying-tasks-and-moving-tasks-or-issues)
* [Novo Agrupamento para Relatórios de Horas Orçadas de Recursos: Data de Alocação](#new-grouping-for-resource-budgeted-hour-reports-allocation-date)
* [Melhorias no Planejador de recursos](#resource-planner-improvements)
* [Melhorias em dispositivos móveis](#mobile-improvements)
* [Integração do Workfront com o Slack](#workfront-integration-with-slack)
* [Melhorias do Outlook 365](#outlook-365-improvements)
* [Alterações na API](#api-changes)

## Área da Página Inicial (Minha Área de Trabalho Atualizada) {#home-area-updated-my-work-area}

>[!NOTE]
>
>Essa funcionalidade não será lançada no ambiente de Produção com a versão 17.3; ela permanecerá em Pré-visualização até o início de 2018.

A nova área da página inicial oferece uma visualização alternativa e aprimorada dos mesmos dados que estão disponíveis na área Meu trabalho. A área Página inicial oferece os seguintes benefícios na área Meu trabalho:

* Uma interface mais simples e intuitiva
* Desempenho aprimorado

A seguinte funcionalidade está disponível na área Meu trabalho, mas ainda não está implementada na área Página inicial:

* Exibir seu calendário pessoal
* Atualizar tarefas e problemas com formatação de rich text
* Aprovar provas
* Exibir uma lista de trabalhos enviados para aprovação
* Criar um problema ad hoc em um projeto
* Exibir somente as aprovações que foram delegadas a você

Para obter mais informações sobre como usar a nova área da página inicial, consulte [Usar a área da página inicial](../../../../workfront-basics/using-home/using-the-home-area/use-the-home-area.md).

## Modelo de layout atualizado para oferecer suporte à área inicial {#updated-layout-template-to-support-the-home-area}

>[!NOTE]
>
>Essa funcionalidade não será lançada no ambiente de Produção com a versão 17.3; ela permanecerá em Pré-visualização até o início de 2018.

Como administrador do Workfront, você pode determinar se os usuários da sua organização têm acesso à área Página inicial configurando o modelo de layout ao qual estão atribuídos. Os usuários aos quais não é atribuído um modelo de layout podem sempre acessar a área Início.

Para obter mais informações, consulte &quot;Personalizando a página inicial&quot; em &quot;Criando e gerenciando modelos de layout&quot;.

## Kanban para Agile  {#kanban-for-agile}

As equipes Agile agora podem usar uma metodologia Kanban no Workfront, além da metodologia ágil Scrum já compatível.

As metodologias ágeis de Scrum e Kanban no Workfront diferem das seguintes maneiras:

**Benefícios do uso do Kanban no Workfront**

* Exiba o backlog no storyboard ágil de Kanban.

  Para obter mais informações, consulte em .

* Configurar itens no backlog para serem adicionados automaticamente ao storyboard ágil de Kanban quando outros itens forem movidos para um status que equivale a Concluído.

  Para obter mais informações, consulte [Configurar matérias a serem adicionadas automaticamente da lista de pendências](../../../../agile/get-started-with-agile-in-workfront/configure-kanban.md#configur5) em [Configurar Kanban](../../../../agile/get-started-with-agile-in-workfront/configure-kanban.md).

* Configure um limite de Trabalho em andamento (WIP) a ser exibido no storyboard ágil de Kanban.

  Para obter mais informações, consulte [Configurar o limite do trabalho em andamento (WIP)](../../../../agile/get-started-with-agile-in-workfront/configure-kanban.md#configur4) em [Configurar Kanban](../../../../agile/get-started-with-agile-in-workfront/configure-kanban.md).

**Vantagens de Usar Scrum no Workfront**

* Adicione um conjunto de histórias a uma iteração ágil e crie um storyboard para essa iteração.
* Inclua problemas no storyboard Scrum.
* Incluir problemas na lista de pendências de uma equipe ágil.

  Para obter mais informações, consulte [Configurar como as datas são aplicadas ao adicionar itens de trabalho a uma iteração](../../../../agile/get-started-with-agile-in-workfront/configure-scrum.md#configur5) em [Configurar Scrum](../../../../agile/get-started-with-agile-in-workfront/configure-scrum.md).

* As subtarefas podem ser exibidas no storyboard Scrum.
* Visualize um gráfico de burndown para ver o progresso em relação às histórias durante a iteração.

  Para obter mais informações, consulte [Visão geral do gráfico de burndown ágil](../../../../agile/use-scrum-in-an-agile-team/burndown/burndown-chart-overview.md).

Para obter mais informações sobre como habilitar e configurar o Kanban para uma Equipe Ágil, consulte [Decidir sobre uma metodologia Ágil](../../../../agile/get-started-with-agile-in-workfront/create-an-agile-team.md#deciding) em [Criar uma Equipe Ágil](../../../../agile/get-started-with-agile-in-workfront/create-an-agile-team.md).

## Incluir problemas no backlog de Scrum de uma Equipe Agile {#include-issues-on-the-scrum-backlog-for-an-agile-team}

>[!NOTE]
>
>Essa funcionalidade foi removida do ambiente de Produção do em 14 de novembro de 2017. Está planejado para ser reintroduzido no ambiente de Pré-visualização no início de 2018, com um design aprimorado e maior estabilidade. Ele estará disponível no ambiente de Produção com a versão 2018.1.

Agora é possível incluir problemas no backlog de sua equipe ágil ao usar a metodologia ágil de Scrum (os problemas não são exibidos no backlog de uma equipe ágil ao usar a metodologia Kanban). As equipes ágeis do Scrum existentes devem habilitar essa funcionalidade para que os problemas sejam incluídos. Os problemas são incluídos automaticamente no backlog de equipes ágeis do Scrum criadas após a versão 2017.3.

Antes dessa alteração, somente tarefas podiam ser adicionadas ao backlog. Se você quiser adicionar um problema, primeiro é necessário converter o problema em uma tarefa antes que ele possa ser adicionado.

Como agora você tem acesso a mais do que apenas tarefas no backlog, qualquer exibição de tarefa personalizada anteriormente disponível no backlog é copiada e adicionada ao backlog como exibições de Item de Trabalho do Backlog personalizadas.

Para obter informações sobre problemas no backlog, consulte  [Gerenciar o backlog ágil](../../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md).

Para obter informações sobre como ativar problemas para que fiquem disponíveis no backlog de uma equipe ágil de Scrum, consulte  [Configure como as datas são aplicadas ao adicionar itens de trabalho a uma iteração](../../../../agile/get-started-with-agile-in-workfront/configure-scrum.md#configur5) em [Configurar Scrum](../../../../agile/get-started-with-agile-in-workfront/configure-scrum.md).

## Incluir problemas no Storyboard Scrum Agile {#include-issues-on-the-scrum-agile-story-board}

>[!NOTE]
>
>Essa funcionalidade foi removida do ambiente de Produção do em 14 de novembro de 2017. Está planejado para ser reintroduzido no ambiente de Pré-visualização no início de 2018, com um design aprimorado e maior estabilidade. Ele estará disponível no ambiente de Produção com a versão 2018.1.

Agora é possível incluir problemas no storyboard ao usar a metodologia ágil de Scrum.

Para obter mais informações, consulte [Configurar colunas de status no storyboard Agile](../../../../agile/get-started-with-agile-in-workfront/configure-scrum.md#configur2) em [Configurar Scrum](../../../../agile/get-started-with-agile-in-workfront/configure-scrum.md).

## Aplicar agrupamentos e filtros ao backlog de uma equipe Agile {#apply-groupings-and-filters-to-the-backlog-for-an-agile-team}

>[!NOTE]
>
>Essa funcionalidade foi removida do ambiente de Produção do em 14 de novembro de 2017. Está planejado para ser reintroduzido no ambiente de Pré-visualização no início de 2018, com um design aprimorado e maior estabilidade. Ele estará disponível no ambiente de Produção com a versão 2018.1.

As opções de Agrupamento e Filtro agora estão disponíveis no backlog ágil, permitindo organizar o backlog por agrupamentos, bem como filtrar tarefas e problemas específicos.

Antes dessa alteração, você poderia aplicar em exibições ao backlog ágil.

Para obter mais informações, consulte  [Gerenciar a lista de pendências ágil](../../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md) no  [Gerenciar o backlog ágil](../../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md).

## Formatação de Rich Text para atualizações e emails {#rich-text-formatting-for-updates-and-emails}

>[!NOTE]
>
>As alterações de formatação feitas no ambiente de Visualização podem ser revertidas para o estado não formatado.

Agora é possível enfatizar informações importantes formatando os comentários e as atualizações feitas nos objetos do Workfront. 

Usando as ferramentas de Rich Text, você pode aplicar atributos de formatação ao texto, criar listas com marcadores e numeradas e adicionar hiperlinks a recursos adicionais.

A formatação aplicada aos comentários no fluxo de atualização também é exibida nas notificações por email de atualização. Para saber mais sobre como formatar seus comentários, consulte [Trabalho de atualização](../../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

## A funcionalidade @Tagging aprimorada retorna no ambiente de visualização {#enhanced-tagging-functionality-returns-in-the-preview-environment}

Você pode usar novamente o símbolo @ para marcar outros usuários no fluxo de atualização de todos os objetos no ambiente de Pré-visualização. Anteriormente, @tagging colocava o nome e sobrenome do usuário marcado no Fluxo de atualização. Agora, a funcionalidade @tagging aprimorada exibe somente o nome do usuário. Para saber mais sobre como marcar usuários em atualizações, consulte [Marcar outros usuários em atualizações](../../../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md).

## Filtrar atualizações do sistema no fluxo de atualização agora é persistente entre objetos {#filter-system-updates-in-the-update-stream-is-now-persistent-across-objects}

A opção Filtrar atualizações do sistema agora é persistente entre objetos no site do Workfront. Isso permite ocultar atualizações do sistema e exibir somente comentários do usuário no fluxo de atualização em um objeto, e fazer com que essa configuração permaneça conforme você navega para outros objetos.

Antes dessa alteração, você tinha que optar por filtrar as atualizações do sistema para cada objeto à medida que navegava pelo site do Workfront.

Para obter mais informações, consulte [Atualizar trabalho](../../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

## Visualizar Dados no Relatório de Utilização {#visualize-data-in-the-utilization-report}

 Agora é possível exibir as informações de Utilização em uma exibição de gráfico. 

Para obter mais informações, consulte [Visão Geral do Relatório de Utilização de Recursos](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md) em [Visão Geral do Relatório de Utilização de Recursos](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md).

## Melhoria no Desempenho do Relatório de Utilização {#utilization-report-performance-improvement}

>[!NOTE]
>
>Esse recurso foi lançado em um patch após o lançamento final do Beta.

Agora, ao executar um relatório de Utilização, você é solicitado a aplicar um filtro antes da execução do relatório. Essa alteração garante que as informações mais pertinentes sejam geradas no relatório de Utilização o mais rápido possível.

Para obter mais informações sobre como executar um relatório de Utilização, consulte [Visão Geral do Relatório de Utilização de Recursos](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md) em [Visão Geral do Relatório de Utilização de Recursos](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md).

## Melhorias no documento: interface simplificada {#document-enhancements-streamlined-interface}

A experiência do usuário para adicionar documentos ao Workfront agora é mais simplificada e intuitiva. Agora é possível carregar um documento do seu sistema de arquivos, solicitar um documento ou vincular um arquivo de um aplicativo de terceiros (como Google ou Dropbox), tudo a partir de um menu suspenso simples. 

Anteriormente, essas opções estavam disponíveis ao iniciar a caixa de diálogo Adicionar documentos. 

Para obter mais informações, consulte as seguintes informações:

* [Adicionar documentos ao Adobe Workfront a partir do seu sistema de arquivos](../../../../documents/adding-documents-to-workfront/add-documents-from-file-system.md)
* [Solicitar um documento](../../../../documents/adding-documents-to-workfront/request-a-document.md)
* [Vincular documentos de aplicativos externos](../../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md) 

>[!NOTE]
>
>Com essa alteração, a opção para colar uma imagem ou documento da área de transferência não está mais disponível.

## Aprimoramentos de provas no Workfront {#proofing-enhancements-within-workfront}

* [Experiência do usuário aprimorada e funcionalidade adicional](#improved-user-experience-and-additional-functionality)
* [Compartilhar Diretamente do visualizador de revisões](#share-directly-from-the-proofing-viewer)
* [Configurar Funções De Prova Padrão](#configure-default-proof-roles)

### Experiência do usuário aprimorada e funcionalidade adicional {#improved-user-experience-and-additional-functionality}

Além de uma experiência do usuário aprimorada ao criar provas no Workfront, a seguinte funcionalidade adicional está disponível:

* Mescle várias imagens em uma única prova.
* Sites de prova em várias resoluções (várias resoluções podem ser criadas como provas individuais ou combinadas em uma única prova).
* Edite o nome do arquivo durante o processo de upload.
* Inclua campos personalizados no formulário de criação de prova.
* Adicione uma mensagem personalizada para revisar as notificações por email.
* Configurações de prova adicionais 
* Validação de erro em tempo real ao revisar um URL (anteriormente, você tinha que aguardar vários minutos antes de um erro ser exibido)

Para obter mais informações, consulte.

>[!NOTE]
>
> Ao criar uma nova prova com fluxo de trabalho automatizado, arrastar e soltar não é compatível com a movimentação de usuários de um estágio para outro. Em vez disso, remova o usuário de uma etapa e adicione-o a outra.

*A opção de mover usuários de uma etapa para outra usando a função arrastar e soltar será reintroduzida com a versão 2018.1.*

### Compartilhar diretamente do visualizador de provas {#share-directly-from-the-proofing-viewer}

Agora é possível compartilhar com usuários específicos do Workfront diretamente no visualizador de provas.

>[!NOTE]
>
>Essa funcionalidade está disponível somente para novas provas (provas criadas após a versão 2017.3) e somente para instâncias do Workfront que estão integradas a uma conta do Workfront Proof Premium.

Antes dessa alteração, você só podia compartilhar o criando um link e, em seguida, compartilhando esse link com um usuário. 

Para obter mais informações, consulte [Compartilhar uma prova no Adobe Workfront](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md) em [Compartilhar uma prova no Adobe Workfront](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md).

### Configurar Funções De Prova Padrão {#configure-default-proof-roles}

Agora você pode configurar as funções de prova padrão que novos usuários e usuários convidados têm para novas provas no sistema do Workfront. 

Essa é a função padrão à qual os usuários são atribuídos em uma prova quando a prova é compartilhada com eles. 

## Aprimoramentos de provas no Workfront Proof e no Workfront {#proofing-enhancements-within-both-workfront-proof-and-workfront}

* [Reiniciar e ignorar o visualizador de prova de vídeo do HTML5 (Atalhos de Teclado)](#restart-and-skip-in-html5-video-proofing-viewer-keyboard-shortcuts)
* [Atualizações do visualizador de provas HTML5](#html5-proofing-viewer-updates)

### Reiniciar e ignorar no visualizador de prova de vídeo do HTML5 (atalhos de teclado) {#restart-and-skip-in-html5-video-proofing-viewer-keyboard-shortcuts}

Agora, há atalhos de teclado no HTML5 revisor para vídeo que permitem reiniciar o vídeo do início e pular para o final do vídeo.

Para obter mais informações sobre os atalhos de teclado disponíveis, consulte [Atalhos de teclado no visualizador de provas do Workfront Proof](../../../../workfront-proof/wp-work-proofsfiles/review-proofs-wpv/keyboard-shortcuts.md).

### Atualizações do visualizador de provas HTML5 {#html5-proofing-viewer-updates}

O visualizador HTML5 agora é compatível com provas estáticas.

Antes dessa alteração, o visualizador do HTML5 era compatível apenas com provas de vídeo. 

O visualizador de HTML inclui a seguinte nova funcionalidade ao revisar conteúdo estático:

* Fazer um único comentário com marcações em várias páginas em uma única exibição

  Isso era possível anteriormente somente quando se estava na exibição Contínua ou na exibição Revista

* Navegar pelas provas através das miniaturas de prova

   * Identifique facilmente a parte da prova que está sendo revisada. Isso é importante, especialmente quando os usuários trabalham com provas de formato maior e páginas da Web longas ou sempre que o  é necessário um nível de zoom maior para ver os detalhes.
   * Alterar o nível de zoom
   * Deslocar o conteúdo

* Especificar valores personalizados na ferramenta Medição
* Ao anotar texto em uma prova no visualizador de provas do Workfront Proof, você pode incluir opções para indicar que o texto deve estar em negrito, itálico e sublinhado.

O visualizador de HTML5 ainda não suporta todas as funcionalidades atualmente disponíveis no visualizador de Flashes existente. A seguinte funcionalidade não está disponível no momento, mas será incluída em uma versão futura:

* Suporte a arquivos de mídia avançada
* Modo de comparação (vídeo e estático)
* Filtrar comentários (vídeo e estático)
* Revisar hiperlinks em documentos (estático)
* Traduções (vídeo e estáticas)
* Indicador de presença que mostra os usuários que estão trabalhando na prova
* Compartilhar provas

Para obter mais informações sobre provas estáticas de revisão no visualizador de HTML5, consulte .

Como administrador do Workfront no Workfront Proof, você pode determinar se os usuários em sua organização têm acesso ao novo visualizador de provas de HTML 5 para provas em vídeo.

## Novo redesign do gráfico de Gantt {#new-gantt-chart-redesign}

O novo Gráfico de Gantt inclui as seguintes melhorias:

* Novos ícones e marcadores
* Nova opção para ampliar e reduzir um período específico
* Células de tarefas menores na parte da lista do gráfico
* Opções reprojetadas para configurações, impressão e alternância para Datas projetadas.

Para obter mais informações sobre a configuração de opções no Gráfico de Gantt, consulte [Configurar como as informações são exibidas no Gráfico de Gantt](../../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md). 

## Relatórios Internos Contêm Descrições Atualizadas {#built-in-reports-contain-updated-descriptions}

Atualizamos as descrições de nossos relatórios de sistema no Workfront para incluir informações sobre o tipo de relatório e os campos incluídos.  

Antes dessa alteração, a maioria de nossos relatórios internos não tinha descrições ou tinham uma descrição muito limitada.

Para obter mais informações sobre relatórios internos, consulte [Usar relatórios internos do Adobe Workfront](../../../../reports-and-dashboards/reports/using-built-in-reports/use-workfront-built-in-reports.md).

## Marcas em relatórios, listas e painéis exportados {#branding-in-exported-reports-lists-and-dashboards}

>[!NOTE]
>
>No momento, esse recurso não está disponível em todos os clusters no ambiente de Pré-visualização.

Se você estiver usando a marca no Workfront, o logotipo usado na Barra de navegação global agora será incluído nos arquivos .pdf exportados do Workfront.

Os seguintes arquivos .pdf incluirão o logotipo da sua organização no documento exportado:

* Listas exportadas
* Relatórios exportados e entregues
* Painéis impressos

Para obter mais informações sobre como exportar dados do Workfront, consulte [Exportar dados](../../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md).

## Melhorias ao Copiar Tarefas e Mover Tarefas ou Problemas {#improvements-when-copying-tasks-and-moving-tasks-or-issues}

Melhoramos a maneira como você copia uma tarefa ou move uma tarefa ou um problema para facilitar a seleção de um pai para a tarefa ou problema copiado ou movido. Ao selecionar um pai ao copiar uma tarefa, por exemplo, agora é possível ver uma hierarquia de tarefas, com seu relacionamento pai-filho, bem como pesquisar um pai em projetos com muitas tarefas.

Antes dessa alteração, não havia nenhum campo de Pesquisa na etapa **Selecionar pai**, e a hierarquia de tarefas não estava visível na lista de tarefas.

Para obter mais informações sobre como copiar tarefas, consulte [Copiar e duplicar tarefas](../../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md).

Para obter mais informações sobre como mover problemas, consulte [Mover problemas](../../../../manage-work/issues/manage-issues/move-issues.md).

## Nova configuração para Retroceder solicitações na área de configurações de aprovação {#new-configuration-for-recalling-requests-in-the-approval-settings-area}

Introduzimos uma nova configuração na área Configurações de aprovação no nível do sistema, para permitir que os administradores do Workfront decidam se devem permitir que os usuários evoquem um problema ou solicitem um status cujo primeiro status esteja pendente de aprovação. Se a recuperação for permitida, o problema será excluído; se a recuperação não for permitida, os usuários não poderão ver um botão Cancelar quando o primeiro status de um problema estiver pendente de aprovação.

Antes dessa alteração, sempre era permitido o recall do problema. Quando a aprovação era cancelada, a aprovação era completamente ignorada, colocando o problema em seu primeiro status, sem aprovação anexada.

Para obter mais informações sobre configurações de aprovação, consulte [Definir configurações de aprovação globais](../../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md). 

>[!NOTE]
>
>Essa opção estará desativada por padrão quando esse recurso for lançado. Atualmente, a chamada de problemas está ativada por padrão para todas as organizações. Quando esse recurso é lançado, o administrador do Workfront deve habilitar manualmente essa configuração para manter a funcionalidade como está no Workfront.

## Novo Agrupamento para Relatórios de Horas Orçadas de Recursos: Data de Alocação {#new-grouping-for-resource-budgeted-hour-reports-allocation-date}

Adicionamos a capacidade de agrupar seus resultados por Data de Alocação quando você está criando um relatório de Horas Orçadas de Recurso.

Antes dessa alteração, você podia exibir a Data de alocação na exibição do relatório, bem como usá-la em um filtro, mas não podia usar esse campo em um agrupamento.

Para obter mais informações sobre a Data de Alocação, consulte [Glossário da terminologia do Adobe Workfront](../../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

Para obter mais informações sobre a criação de um relatório, consulte [Criar um relatório personalizado](../../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

## Melhorias no planejamento de recursos {#resource-planner-improvements}

* [Planejador de recursos: Mostrar dados por FTE](#resource-planner-show-data-by-fte)
* [Planejador de recursos: mostrar dados por semana e trimestre](#resource-planner-show-data-by-week-and-quarter)
* [Planejador de recursos: ver por usuário](#resource-planner-view-by-user)
* [Planejador de recursos: arrastar e soltar projetos para estabelecer prioridade](#resource-planner-drag-and-drop-projects-to-establish-priority)
* [Planejador de recursos: exporte os dados do Planejador de recursos para o Excel](#resource-planner-export-the-data-in-the-resource-planner-to-excel)

### Planejador de recursos: Mostrar dados por FTE {#resource-planner-show-data-by-fte}

Agora você pode exibir a alocação e a disponibilidade de seus recursos por FTE no Planejador de recursos. Antes dessa alteração, você só poderia exibir os valores em horas.

Para obter mais informações sobre como usar o Planejador de recursos, consulte [Visão geral do Planejador de recursos](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

### Planejador de recursos: mostrar dados por semana e trimestre {#resource-planner-show-data-by-week-and-quarter}

Agora, você pode alterar o intervalo de intervalo de tempo do Planejador de recursos para exibi-lo por semana ou trimestre. Antes dessa alteração, você poderia visualizar a alocação e a disponibilidade de seus recursos e orçá-los apenas por mês.

Para obter mais informações sobre como usar o Planejador de recursos, consulte [Visão geral do Planejador de recursos](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

### Planejador de recursos: Exibir por usuário {#resource-planner-view-by-user}

Agora você pode exibir as informações no Planejador de recursos por usuário, primeiro, e depois por projetos, funções e tarefas. Você também pode exibir uma diferença entre as Horas Planejadas e Disponíveis ou FTE para os usuários. Antes dessa alteração, você poderia exibir as informações no Planejador de recursos por projetos e funções.

Para obter mais informações sobre como usar o Planejador de recursos, consulte [Visão geral do Planejador de recursos](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

### Planejador de recursos: arraste e solte projetos para estabelecer prioridade {#resource-planner-drag-and-drop-projects-to-establish-priority}

Agora é possível arrastar e soltar projetos na ordem de prioridade desejada. Antes dessa alteração, você pode estabelecer a prioridade dos projetos somente atribuindo manualmente um número a eles.

Para obter mais informações sobre como usar o Planejador de recursos, consulte [Visão geral do Planejador de recursos](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

### Planejador de recursos: exporte os dados do Planejador de recursos para o Excel {#resource-planner-export-the-data-in-the-resource-planner-to-excel}

Agora você pode exportar as informações do Planejador de recursos para um arquivo do Excel.

Para obter mais informações sobre como usar o Planejador de recursos, consulte [Visão geral do Planejador de recursos](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

## Melhorias na mobilidade {#mobile-improvements}

Adicionamos a capacidade de acessar e gerenciar seus projetos por meio do aplicativo móvel do Workfront. Agora você pode fazer o seguinte usando o aplicativo móvel do Workfront:

* Acessar uma lista de projetos
* Acessar uma lista de tarefas e subtarefas em um projeto
* Acessar uma lista de problemas em um projeto
* Registrar um novo problema em um projeto

É possível instalar essa funcionalidade ao atualizar o aplicativo móvel do Workfront. A atualização estará disponível nas lojas de dispositivos móveis Apple e Android em novembro de 2017.

## Integração do Workfront com o Slack {#workfront-integration-with-slack}

>[!NOTE]
>
>A integração de Slack não está disponível no momento. Ele estará disponível para uso com seu ambiente de produção em novembro de 2017.

Estamos lançando uma nova integração entre o Workfront e o Slack. Se a sua organização já estiver usando o Slack para a comunicação, agora é possível integrá-lo ao Workfront e executar ações comuns do Workfront sem deixar os canais de comunicação no Slack. Agora você pode executar as seguintes ações a partir da sua conta Slack:

* Pesquisar um item no Workfront
* Acessar suas listas de trabalho e aprovações
* Criar uma tarefa
* Criar um problema
* Inscreva-se em qualquer item a partir de um link compartilhado com você para esse item
* Atribuir tarefas e problemas de um link compartilhado com você a eles
* Aprove seu trabalho
* Acessar seus Favoritos e suas listas de Itens Recentes

Para obter mais informações sobre como acessar o Workfront pelo Slack, consulte [Usar o Workfront com o Slack.](https://support.workfront.com/hc/en-us/sections/115000458033)

## Melhorias no Outlook 365 {#outlook-365-improvements}

Fizemos as seguintes melhorias no complemento Workfront para o  Outlook 365:

* Adicionar uma tarefa ou um problema a um projeto no Workfront: agora é possível converter um email em uma tarefa ou um problema no Workfront, usando o suplemento do Outlook 365. Nesse processo, você pode especificar um projeto ao qual deseja que a tarefa ou o problema seja adicionado, bem como um destinatário e uma data de vencimento. Antes desse aprimoramento, você só poderia enviar uma solicitação para uma fila de solicitações ou adicionar uma tarefa pessoal à sua lista de Trabalho no Outlook 365. 
* Preservar um link para objetos do Workfront no email original convertido em tarefas, problemas ou solicitações: Quando você converte um email do Outlook 365 em uma tarefa, um problema ou uma solicitação, o Outlook 365 preserva um link para a tarefa ou problema que foi convertido desse email dentro do email original. Antes dessa alteração, não havia nenhuma indicação no Outlook se um email havia sido convertido em uma tarefa ou enviado como uma solicitação. 

  Para obter mais informações sobre como converter um email em uma tarefa ou um problema do Outlook 365, consulte [Adicionar um email do Outlook a um projeto como uma tarefa ou um problema](../../../../workfront-integrations-and-apps/using-workfront-with-outlook/add-outlook-email-to-project-as-task-or-issue.md).

## Alterações na API {#api-changes}

* [API 8 agora disponível](#api-8-now-available)
* [Versões removidas e obsoletas da API](#removed-and-deprecated-versions-of-the-api)
* [Atividade de versão final do Beta 2017.3](#updated-message-format-for-event-subscriptions)
* [Tentativas de assinatura de evento para mensagens que não podem ser entregues](#event-subscription-retries-for-undeliverable-messages)

### API 8 agora disponível {#api-8-now-available}

A API do Workfront versão 8 já está disponível e oferece recursos novos e atualizados para suas integrações com o Workfront.

Para obter uma lista das alterações feitas na API do Workfront, consulte [Atualizações para a API versão 8](../../../../wf-api/api/new-api-version-8-updates.md).

### Versões removidas e obsoletas da API {#removed-and-deprecated-versions-of-the-api}

### Formato de mensagem atualizado para assinaturas de evento

Para fornecer mais informações úteis para suas integrações que incluem a API de assinaturas de evento do Workfront, alteramos o formato da mensagem de saída dos recursos compatíveis ao incluir os valores antigos e novos associados a esses recursos. Para evitar falhas, todas as integrações que você tiver usando a API de Assinaturas de Eventos da Workfront precisarão ser atualizadas no novo formato, conforme descrito em [API de Assinatura de Eventos](../../../../wf-api/general/event-subs-api.md).

### Tentativas de assinatura de evento para mensagens que não podem ser entregues {#event-subscription-retries-for-undeliverable-messages}

A estrutura de Assinatura de eventos do Workfront agora fornece um mecanismo para lidar com mensagens de saída acionadas por eventos que não são entregues aos endpoints do cliente. Para garantir a entrega contínua de mensagens, os clientes devem garantir que todos os endpoints que consomem mensagens de saída de assinaturas de evento estejam configurados corretamente. Para obter mais informações, consulte [Tentativas de assinatura de evento](../../../../wf-api/api/event-sub-retries.md).
