---
content-type: release-notes
navigation-topic: product-releases-archive
title: Atividade da versão 2018.2 do Beta 5
description: Esta página descreve todas as alterações disponíveis mais recentemente no ambiente de Pré-visualização com a versão 2018.2 do Beta 5. A funcionalidade estará disponível no ambiente de Pré-visualização em 1 de junho de 2018. Os aprimoramentos de revisão lançados com o Beta 5 estarão disponíveis no ambiente de Pré-visualização na segunda-feira, 4 de junho. Ele estará disponível no ambiente de Produção em julho de 2018.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 0a8602aa-34c8-44d0-a102-9497d106f806
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '3158'
ht-degree: 1%

---

# Atividade da versão 2018.2 do Beta 5

Esta página descreve todas as alterações disponíveis mais recentemente no ambiente de Pré-visualização com a versão 2018.2 do Beta 5. A funcionalidade estará disponível no ambiente de Pré-visualização em 1 de junho de 2018. Os aprimoramentos de revisão lançados com o Beta 5 estarão disponíveis no ambiente de Pré-visualização na segunda-feira, 4 de junho. Ele estará disponível no ambiente de Produção em julho de 2018.

>[!IMPORTANT]
>
> A funcionalidade descrita nesta página está sujeita a alterações antes da disponibilidade no ambiente de produção.

Para obter uma lista de todas as alterações feitas em 2018.2, consulte  Visão geral da atividade da versão [2018.2](../../../../product-announcements/product-releases/quarterly-release-archive/2018.2-release-activity/2018-2-release-activity-overview.md).

A versão 2018.2 do Beta 5 contém as melhorias para administradores do Workfront e outros usuários:

**Para Administradores**

* [Exibir Alterações Acionadas pelo Usuário com Logs de Auditoria](#view-user-triggered-changes-with-audit-logs)
* [Exibir Informações de Licença como um administrador de grupo](#view-license-information-as-a-group-administrator)

**Para Todos Os Usuários**

* [Exibição de calendário na Área Inicial](#calendar-view-in-the-home-area)
* [Atualizações adicionais para a Lista de Trabalho (Painel esquerdo) na Página Inicial](#additional-updates-to-the-work-list-left-panel-in-home)
* [Configurar os Limites de Função de Trabalho para o Agendamento Automatizado de Recursos](#configure-job-role-limits-for-automated-resource-scheduling)
* [Melhorias na exibição de projetos e funções no Planejador de recursos](#project-and-role-view-improvements-in-the-resource-planner)
* [Redimensionar Larguras de Coluna para Listas de Projetos](#resize-column-widths-for-project-lists)
* [Suporte a Ícones para Novas Listas de Projetos](#icon-support-for-the-new-project-lists)
* [Adicionar o campo &quot;Miniatura grande&quot; nas Exibições de Documento](#add-large-thumbnail-field-in-document-views)
* [Aumentar Limite de Exportação do Excel](#increase-excel-export-limit)
* [Filtros rápidos para listas de projetos](#quick-filters-for-project-lists)
* [Referenciar Coleções de Problemas nos Relatórios de Projeto e de Tarefa](#reference-issue-collections-in-project-and-task-reports)
* [Novo menu de versão mais robusta ao adicionar novas versões de documento no Workfront](#new-more-robust-version-menu-when-adding-new-document-versions-in-workfront)
* [Melhorias na publicação de conteúdo para dispositivos móveis no aplicativo móvel do Android Beta](#mobile-improvements-in-the-android-beta-mobile-app)
* [Aprimoramentos do revisor (Workfront e Workfront Proof)](#proofing-viewer-enhancements-workfront-and-workfront-proof)
* [Aprimoramentos de provas no Workfront](#proofing-enhancements-in-workfront)
* [Aprimoramentos de provas no Workfront Proof](#proofing-enhancements-in-workfront-proof)

## Exibição de Calendário na Área Inicial {#calendar-view-in-the-home-area}

Agora você pode gerenciar suas tarefas de trabalho pessoais e agendamentos usando a exibição do Calendário da página inicial da Workfront. A exibição Calendário da página inicial permite fazer o seguinte:

* Defina sua própria programação para realizar as tarefas do Workfront atribuídas a você
* Veja rapidamente as tarefas que estão vencidas ou vencidas
* Exibir o total de horas alocadas por uma semana
* Fazer atualizações em tarefas atribuídas a você

Se você usar um calendário no Outlook, poderá integrar seu calendário para exibir os eventos do Outlook no modo de exibição Calendário da Página Inicial.

## Atualizações adicionais na Lista de trabalho (painel esquerdo) na Página inicial {#additional-updates-to-the-work-list-left-panel-in-home}

Os seguintes aprimoramentos estão disponíveis para a Lista de trabalho na área Página inicial:

* O número de itens concluídos agora é exibido entre parênteses ao lado da opção Concluído no menu suspenso Filtro.

  Anteriormente, o número de itens concluídos não era exibido no menu Filtro. 

* Os itens concluídos são mostrados para as 2 semanas anteriores.

  Anteriormente, os itens concluídos eram exibidos para os 3 meses anteriores.

  Para obter informações sobre como visualizar o trabalho concluído na área Página Inicial, consulte [Exibir itens na Lista de Trabalho na área Página Inicial](../../../../workfront-basics/using-home/using-the-home-area/display-items-in-home-work-list.md) no artigo [Exibir itens na Lista de Trabalho na área Página Inicial](../../../../workfront-basics/using-home/using-the-home-area/display-items-in-home-work-list.md).

* Adicione os campos Duração e Atribuições para exibir quando os itens forem selecionados na área Página inicial.

  Anteriormente, o campo Atribuições ficava disponível por padrão; no entanto, se ele fosse excluído, não poderia ser adicionado novamente. O campo Duração não estava disponível anteriormente para adição.

  Para obter informações sobre como adicionar campos à área da página inicial, consulte &quot;Criar e gerenciar modelos de layout&quot;.

Para obter mais informações sobre como usar a área da Página Inicial, consulte [Usar a área da Página Inicial](../../../../workfront-basics/using-home/using-the-home-area/use-the-home-area.md).

## Exibir alterações acionadas pelo usuário com logs de auditoria {#view-user-triggered-changes-with-audit-logs}

Criamos os seguintes logs de auditoria para administradores do Workfront para rastrear alterações acionadas pelo usuário:

* Log de auditoria do usuário
* Log de Auditoria de Nível de Acesso
* Logs de auditoria de grupo
* Logs de auditoria de tentativas de logon

Anteriormente, não havia como rastrear alterações no sistema.

Para obter mais informações, consulte [Exibir e exportar logs de auditoria](../../../../administration-and-setup/add-users/create-and-manage-users/view-and-export-audit-logs.md).

## Exibir Informações de Licença como um administrador de grupo {#view-license-information-as-a-group-administrator}

Criamos uma página de licenças somente leitura para administradores de grupo para exibir contagens de licença para os grupos que eles administram.

Antes dessa alteração, os administradores de grupo não podiam exibir informações de licença.

Para obter mais informações, consulte [Administradores de grupo](../../../../administration-and-setup/manage-groups/group-roles/group-administrators.md).

## Configurar limites de funções de trabalho para o Agendamento automatizado de recursos {#configure-job-role-limits-for-automated-resource-scheduling}

>[!NOTE]
>
>As ferramentas de Agendamento de recursos foram substituídas e removidas do Workfront com a versão 23.1. Para obter informações sobre o agendamento de recursos usando o Balanceador de carga de trabalho, consulte [Visão geral do Balanceador de carga de trabalho](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

Nas configurações de Agendamento automatizado de recursos, agora é possível atribuir um limite a uma função de trabalho. Isso permite que você controle o número de recursos, com a mesma função, com trabalho atribuído.

Anteriormente, não era possível especificar quantos usuários em uma determinada função de trabalho podiam ser atribuídos a trabalho.

Para obter mais informações, consulte &quot;Atribuir manualmente tarefas e problemas não atribuídos nas áreas de Agendamento&quot;.

## Melhorias na visualização de projetos e funções no Planejador de recursos {#project-and-role-view-improvements-in-the-resource-planner}

As Visualizações de projeto e função do Planejador de recursos agora contêm as seguintes melhorias:

* Filtros aprimorados que extraem informações de todo o banco de dados, em vez de apenas as informações na tela.
* Modo de tela cheia.
* O desempenho agora é mais rápido e mais eficiente.

   * Novos limites para o número de projetos, funções e usuários que você pode exibir.
   * Carregamento lento, para acelerar o carregamento de projetos e funções.

* Acesso rápido a projetos e usuários diretamente do Planejador de recursos.
* Recurso de arrastar e soltar mais rápido na Exibição de projeto, para priorizar seus projetos.

Antes dessas melhorias, você relatou que o Planejador de recursos estava lento para carregar e que havia notado incongruências nos dados exibidos. Com essas melhorias, elas devem ser eliminadas.

Para obter informações e compreender os novos limites do Planejador de recursos, consulte [Limitações de exibição do Planejador de recursos](../../../../resource-mgmt/resource-planning/resource-planner-display-limitations.md)

<!--
<p dir="ltr" data-mc-conditions="QuicksilverOrClassic.Draft mode">To participate in our current beta program and give us feedback on the functionality of the Resource Planner, see <a href="../../../../product-announcements/betas/resource-planner-performance-beta.md" class="MCXref xref" xrefformat="{para}">Resource Planner performance beta </a></p>
-->

## Redimensionar Larguras de Coluna para Listas de Projetos {#resize-column-widths-for-project-lists}

Como estamos trabalhando para melhorar a funcionalidade de nossas listas, desativamos temporariamente a capacidade de redimensionar as larguras das colunas nas seguintes listas de projetos:

* Projetos dos quais sou proprietário
* Projetos em que estou trabalhando
* Todos os Projetos

Com esta versão, agora podemos redimensionar as colunas de todas as listas de projetos.

Adicionamos melhorias adicionais a essa funcionalidade.

Agora, ao arrastar a borda direita de uma coluna para redimensioná-la, a coluna vizinha à direita retém seu tamanho, tornando a lista mais larga, em vez de também ser modificada. Além disso, é possível arrastar a borda de uma coluna para a direita após as bordas das colunas vizinhas.

Antes dessa melhoria, a coluna vizinha à direita da coluna redimensionada também seria redimensionada proporcionalmente para caber na tela e não seria possível arrastar a borda de uma coluna além da borda direita da coluna vizinha.  

Para obter informações sobre como redimensionar as colunas de reordenação em listas, consulte [Modificar largura e ordem da coluna](../../../../reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md).

Para participar do nosso programa de teste beta para as melhorias da lista atual, consulte [Estudo de novas listas.](https://experienceleaguecommunities.adobe.com/t5/workfront/ct-p/workfront?profile.language=pt) (Login necessário)

## Ícone Suporte para novas listas de projeto {#icon-support-for-the-new-project-lists}

Como estamos trabalhando para melhorar a funcionalidade de nossas listas, desativamos temporariamente a exibição de ícones de status nas seguintes listas de projeto:

* Projetos dos quais sou proprietário
* Projetos em que estou trabalhando
* Todos os Projetos

Com esta versão, os ícones de status podem ser exibidos novamente nas listas de projetos para projetos ou outros objetos em uma lista de projetos.

Para obter informações sobre como trabalhar em listas, consulte [Introdução a listas no Adobe Workfront](../../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

## Adicionar o campo &quot;Miniatura grande&quot; nas Visualizações de documento {#add-large-thumbnail-field-in-document-views}

Estamos adicionando um novo campo chamado Miniatura grande a uma exibição de documento em uma lista ou relatório. Quando selecionado em uma visualização de documento, esse campo exibe uma miniatura de 400 pixels de largura do documento em uma lista ou relatório.

Antes dessa alteração, você só podia adicionar o campo Miniatura a uma visualização de documento, que exibe uma miniatura de 33 a 66 pixels de largura do documento.

Para obter informações sobre campos em listas e relatórios, consulte [Glossário da terminologia do Adobe Workfront](../../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

## Aumentar Limite de Exportação do Excel {#increase-excel-export-limit}

Aumentamos o limite de quantas linhas você pode exportar em um arquivo do Excel. Agora você pode exportar o seguinte:

* 65.000 linhas em um arquivo Excel .xls
* 100.000 linhas em um arquivo Excel .xlsx

Os novos limites se aplicam quando você exporta o seguinte do Workfront:

* Uma lista ou um relatório da interface da Web
* Uma lista ou um relatório usando a API
* Um relatório agendado e entregue

Antes dessa melhoria, você só podia exportar 50.000 linhas em qualquer arquivo do Excel.

Para obter informações sobre como exportar dados do Workfront, consulte [Exportar dados](../../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md).

## Filtros rápidos para listas de projetos {#quick-filters-for-project-lists}

Agora é possível aplicar um filtro rápido a listas.

O objetivo de um filtro rápido é ajudá-lo a navegar diretamente para os itens em suas listas grandes que são importantes para você, para que você possa revisá-los, atualizá-los ou compartilhá-los rapidamente com outras pessoas.

Atualmente, os filtros rápidos estão disponíveis somente para as listas de projeto nas seguintes subguias:

* Projetos em que estou trabalhando
* Projetos dos quais sou proprietário
* Todos os Projetos

Para obter informações sobre filtros rápidos, consulte a seção &quot;Aplicando Filtros Rápidos a Listas&quot; em [Introdução a listas no Adobe Workfront](../../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

## Coleções de problemas de referência nos relatórios de projeto e tarefa {#reference-issue-collections-in-project-and-task-reports}

Agora você pode fazer referência a uma coleção de problemas em uma visualização e um filtro de projeto ou tarefa. Você pode fazer isso somente usando o Modo de texto ao criar um relatório.

Antes dessa melhoria, você podia referenciar apenas uma coleção de tarefas em uma visualização ou filtro de projeto.

Para obter informações sobre como fazer referência a uma coleção em um relatório, consulte [Coleções de referência em um relatório](../../../../reports-and-dashboards/reports/text-mode/reference-collections-report.md).

Para obter informações sobre como usar o modo de texto, consulte  [Visão geral dos usos comuns do Modo de Texto](../../../../reports-and-dashboards/reports/text-mode/understand-common-uses-text-mode.md).

>[!NOTE]
>
>No vídeo a seguir, o modo de texto de amostra para coleções de problemas estava incorreto. O modo de texto de exemplo correto está disponível em [Coleções de referência em um relatório](../../../../reports-and-dashboards/reports/text-mode/reference-collections-report.md).

## Novo menu de versão mais robusta ao adicionar novas versões de documento no Workfront {#new-more-robust-version-menu-when-adding-new-document-versions-in-workfront}

Agora, ao adicionar novas versões a documentos no Workfront, o menu Nova versão contém opções adicionais e agora é consistente em todas as áreas do Workfront, onde você pode adicionar uma nova versão.

Você pode adicionar uma nova versão do documento a partir das seguintes áreas do Workfront:

* No menu suspenso Mais na guia Documentos.
* No menu Ações do documento, na página de detalhes do documento.
* Na guia Todas as versões na página de detalhes do documento.

Antes dessa alteração, somente o menu suspenso Mais na guia Documentos continha todas as opções para adicionar uma nova versão.

As seguintes opções agora estão disponíveis no menu Nova versão para todas as áreas em que você pode adicionar uma nova versão:

* Prova
* Somente Documento
* Opções vinculadas (Do Dropbox, Do Google Drive e assim por diante)
* Colar da área de transferência (esta é uma nova opção ao adicionar versões)

Para obter mais informações, consulte [Adicionar documentos ao Adobe Workfront a partir de seu sistema de arquivos](../../../../documents/adding-documents-to-workfront/add-documents-from-file-system.md) no artigo [Adicionar documentos ao Adobe Workfront a partir de seu sistema de arquivos](../../../../documents/adding-documents-to-workfront/add-documents-from-file-system.md).

## Melhorias na plataforma móvel do Android Beta {#mobile-improvements-in-the-android-beta-mobile-app}

Os seguintes aprimoramentos estarão disponíveis na versão do aplicativo móvel para Android Beta, logo após o dia desta versão:

* Deslizar ações

  Você pode realizar atividades como voluntariar para trabalhar em uma tarefa, concluir uma tarefa, marcar uma notificação como vista ou nova, enviar um texto ou chamar um contato passando vários objetos no aplicativo móvel do Workfront.

  As seguintes áreas foram aprimoradas com essa funcionalidade:

   * Meu Trabalho e Página Inicial
   * Notificações
   * Contatos
   * Aprovações

* Nova aparência ao visualizar a guia Detalhes de um item

  A interface foi alterada ao visualizar um item na versão do aplicativo móvel do Android Beta para facilitar a edição, conclusão ou anexação de um documento a ele.

* Nova experiência ao registrar tempo

  O tempo de registro é mais rápido e fácil do que antes, com um botão Tempo de registro mais fácil de acessar e uma interface mais simplificada para horas de registro.

Com esta versão, essas melhorias estão disponíveis apenas para a versão do Beta para Android do aplicativo móvel Workfront. No momento, eles não estão disponíveis para o iOS.

Para obter mais informações sobre como se inscrever para ser um testador beta e baixar a versão do Android Beta do aplicativo móvel Workfront, consulte .

## Aprimoramentos do revisor de provas (Workfront e Workfront Proof) {#proofing-viewer-enhancements-workfront-and-workfront-proof}

* [Página de Resumo de Impressão Atualizada](#updated-print-summary-page)
* [Adicionar usuários a uma prova diretamente do visualizador de provas](#add-users-to-a-proof-directly-from-the-proofing-viewer)
* [Exibir Todas as Ferramentas de Marcação no visualizador de provas](#display-all-markup-tools-in-the-proofing-viewer)
* [Configurar Opções de Classificação Padrão no visualizador de provas](#configure-default-sorting-options-in-the-proofing-viewer)
* [Exibir aprovações de documentos do Workfront no Visualizador de provas de área de trabalho](#view-workfront-document-approvals-in-the-desktop-proofing-viewer)
* [Configurar links que abrem novas guias e janelas para serem abertos no Visualizador de Revisão de Texto da Área de Trabalho](#configure-links-that-open-new-tabs-and-windows-to-open-within-the-desktop-proofing-viewer)
* [Indicador de Presença no visualizador de provas](#presence-indicator-in-the-proofing-viewer)
* [Filtrar comentários para exibir uma única página para provas de URL interativas no visualizador de provas da área de trabalho](#filter-comments-to-display-a-single-page-for-interactive-url-proofs-in-the-desktop-proofing-viewer)
* [Visualizador de Revisores de Texto para Desktop para Conteúdo Estático e de Vídeo](#desktop-proofing-viewer-for-static-and-video-content)
* [Adicionar dispositivos personalizados ao seu sistema](#add-custom-devices-to-your-system)

### Página de resumo de impressão atualizada {#updated-print-summary-page}

A página Resumo de impressão foi atualizada com uma nova aparência e funcionalidade aprimorada.

Para obter informações, consulte [Imprimir um resumo de prova no Adobe Workfront](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/print-proof-summary-in-wf.md).

### Adicionar usuários a uma prova diretamente do visualizador de provas {#add-users-to-a-proof-directly-from-the-proofing-viewer}

Agora é possível adicionar usuários a uma prova diretamente no Web Proofing Viewer e no Desktop Proofing Viewer. 

Anteriormente, não era possível adicionar usuários individuais a uma prova. Em vez disso, você só poderia copiar o URL público ou o código incorporado.

Para obter mais informações, consulte [Compartilhar uma prova adicionando usuários a ela](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/share-a-proof-in-proofing-viewer.md#sharing-with-individual-users) no artigo  [Compartilhar uma prova do visualizador de provas](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/share-a-proof-in-proofing-viewer.md).

### Exibir todas as ferramentas de marcação no visualizador de provas {#display-all-markup-tools-in-the-proofing-viewer}

Agora é possível configurar a ferramenta de marcação para exibir o tempo todo, em vez de em um menu que você precisa abrir. Isso torna mais rápido alternar entre ferramentas. Quando configuradas dessa forma, as ferramentas de marcação são exibidas horizontalmente na parte superior do Visualizador de provas da Web e do Visualizador de provas da área de trabalho.

Anteriormente, as ferramentas de marcação estavam disponíveis somente em um menu suspenso.

Para obter mais informações sobre como definir essa configuração de marcação, consulte [Definir configurações do revisor de provas](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/configure-proofing-viewer-settings.md).

Para obter mais informações sobre como usar opções de marcação ao revisar uma prova, consulte no artigo .

### Configurar opções de classificação padrão no visualizador de provas {#configure-default-sorting-options-in-the-proofing-viewer}

Agora, ao alterar a opção de classificação na lista de comentários em uma prova, essa opção se tornará a opção de classificação padrão na próxima vez que você abrir qualquer prova no Web Proofing Viewer ou no Desktop Proofing Viewer. 

Para obter mais informações, consulte no artigo .

### Visualizar aprovações de documentos do Workfront no Visualizador de provas de desktop {#view-workfront-document-approvals-in-the-desktop-proofing-viewer}

Agora você pode tomar uma decisão de aprovação de documento Workfront no Visualizador de provas de desktop.

Anteriormente, somente o Visualizador de provas da Web permitia que você tomasse uma decisão de aprovação de documento do Workfront. 

Para obter mais informações, consulte  [Tome uma decisão sobre uma prova no visualizador de provas](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md) no artigo  [Tome uma decisão sobre uma prova no visualizador de provas](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md).

### Configurar links que abrem novas guias e janelas para abrir no Visualizador de provas da área de trabalho {#configure-links-that-open-new-tabs-and-windows-to-open-within-the-desktop-proofing-viewer}

Ao revisar o conteúdo interativo no Visualizador de provas da área de trabalho, você pode configurar os links que abrem em uma nova guia ou janela para serem abertos no Visualizador de provas da área de trabalho para que você possa continuar a revisão.

No visualizador de provas herdadas, os links que abriam em uma nova guia ou nova janela não podiam ser revisados no visualizador de provas.

Para obter mais informações, consulte [Definir configurações do revisor de provas](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/configure-proofing-viewer-settings.md).

### Indicador de presença no visualizador de provas {#presence-indicator-in-the-proofing-viewer}

Agora, ao revisar uma prova no Visualizador de provas da Web ou no Visualizador de provas de desktop, você pode exibir o avatar de cada usuário que está visualizando a prova no momento, exibido no canto superior direito do visualizador de provas.

Para obter mais informações, consulte [Revisar uma prova simultaneamente com vários revisores](../../../../workfront-proof/wp-work-proofsfiles/review-proofs-wpv/review-proof-with-multiple-reviewers.md).

### Filtrar comentários para exibir uma única página para provas de URL interativas no visualizador de provas da área de trabalho {#filter-comments-to-display-a-single-page-for-interactive-url-proofs-in-the-desktop-proofing-viewer}

Ao revisar um URL em uma prova interativa no Desktop Proofing Viewer, agora é possível filtrar comentários para exibir comentários feitos apenas na página atual. 

Antes dessa alteração, essa opção estava disponível somente para provas estáticas.

Para obter mais informações, consulte no artigo .

### Visualizador de provas de desktop para conteúdo estático e de vídeo {#desktop-proofing-viewer-for-static-and-video-content}

O Visualizador de provas de desktop agora suporta conteúdo estático e de vídeo.

Anteriormente, ele só aceitava conteúdo interativo.

Para obter informações sobre como configurar provas estáticas e de vídeo para serem abertas no Visualizador de Revisão de Texto para Desktop, consulte [Definir configurações do visualizador de revisão de texto](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/configure-proofing-viewer-settings.md).

Para obter mais informações sobre o Visualizador de Revisão de Texto para Desktop, consulte [Revisando Provas no Visualizador de Revisão de Texto para Desktop.](https://support.workfront.com/hc/en-us/sections/360000686434)

### Adicionar dispositivos personalizados ao seu sistema {#add-custom-devices-to-your-system}

Agora é possível adicionar qualquer dispositivo personalizado ao sistema, permitindo que os usuários revisem o conteúdo interativo e simulem como ele aparece em um dispositivo específico ao revisar uma prova no Visualizador de provas de desktop.

Antes dessa alteração, os usuários podiam escolher somente em uma lista de dispositivos padrão pré-configurados.

Para obter informações sobre como adicionar dispositivos personalizados, consulte em

Para obter informações sobre como os usuários podem selecionar dispositivos ao revisar conteúdo interativo, consulte [Alterar resolução de prova interativa no visualizador de provas](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/view-interactive-content-as-it-appears-in-device.md).

## Aprimoramentos de provas no Workfront {#proofing-enhancements-in-workfront}

* [Compartilhar o link de prova diretamente do Workfront](#share-the-proof-link-directly-from-workfront)
* [Relatório sobre Dados de Revisão Adicionais no Workfront](#report-on-additional-proofing-data-in-workfront)
* [Visualizar dados históricos para aprovações de provas no Workfront](#view-historical-data-for-proof-approvals-in-workfront)

### Compartilhe o link de prova diretamente do Workfront {#share-the-proof-link-directly-from-workfront}

Agora você pode gerar um link para uma prova no Workfront e compartilhá-lo diretamente do Workfront. Como alternativa, você pode copiar o URL e distribuí-lo usando um método alternativo.

Antes dessa alteração, você só podia copiar o link de prova no Workfront e distribuí-lo usando um método alternativo.

Para obter mais informações, consulte [Compartilhar uma prova no Adobe Workfront](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md) no artigo [Compartilhar uma prova no Adobe Workfront](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md).

>[!NOTE]
>
>O link incorporado que está disponível no momento será removido em uma versão futura. O link incorporado ainda estará acessível por meio da API do Workfront.

### Relatório de dados adicionais de comprovação no Workfront {#report-on-additional-proofing-data-in-workfront}

Em relatórios que contêm o objeto Versão do documento (como um relatório Versão do documento e Aprovação de prova), vários campos agora estão disponíveis para exibir informações de prova adicionais.

* Prazo da prova

  Exibe o dia da semana, a data, a hora do dia e o ano do prazo final de prova.

* Decisão da prova

  Exibe o status de decisão da prova (pendente, alterações necessárias ou aprovada).

* Nome da prova

  Exibe o nome da prova.

* Provas de páginas

  Exibe o número de páginas incluídas na prova.

* Progresso da prova

  Exibe o status do progresso da prova (Enviado, Aberto, Comentado, Decisão Tomada).

Para obter mais informações sobre cada um desses campos, consulte  [Glossário da terminologia do Adobe Workfront](../../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

### Visualizar dados históricos para aprovações de provas no Workfront {#view-historical-data-for-proof-approvals-in-workfront}

No relatório Aprovação de prova, é possível adicionar um campo que permite exibir decisões de aprovação de prova para provas que não estão mais ativas. Você pode fazer isso adicionando o campo Decisão do aprovador ao relatório.

Antes dessa alteração, depois que uma decisão sobre uma prova era tomada, a decisão não podia mais ser exibida em um relatório do Workfront.

Para obter mais informações, consulte  [Glossário da terminologia do Adobe Workfront](../../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

## Aprimoramentos de provas no Workfront Proof {#proofing-enhancements-in-workfront-proof}

* [Criar uma nova versão de uma prova diretamente do revisor de provas (Workfront Proof)](#create-a-new-version-of-a-proof-directly-from-the-proofing-viewer-workfront-proof)
* [Novo link de detalhes da prova no revisor de provas e no Visualizador de provas da área de trabalho (Workfront Proof)](#new-proof-details-link-in-the-proofing-viewer-and-desktop-proofing-viewer-workfront-proof)

### Criar uma nova versão de uma prova diretamente do revisor de provas (Workfront Proof) {#create-a-new-version-of-a-proof-directly-from-the-proofing-viewer-workfront-proof}

Agora é possível criar uma nova versão de uma prova diretamente no novo visualizador de provas e no Visualizador de provas da área de trabalho ao fazer provas no Workfront Proof.

Anteriormente, essa opção estava disponível somente no Flash Viewer herdado.

Para obter mais informações, consulte [Copiando provas no Workfront Proof](../../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/copy-proofs.md) no artigo  [Copiando provas no Workfront Proof](../../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/copy-proofs.md).

### Novo link de detalhes da prova no revisor de provas e no Visualizador de provas da área de trabalho (Workfront Proof) {#new-proof-details-link-in-the-proofing-viewer-and-desktop-proofing-viewer-workfront-proof}

Ao visualizar uma prova no visualizador de provas, os usuários do Workfront Proof agora podem ir rapidamente para a página de detalhes da prova no Workfront Proof.

Para obter mais informações, consulte &quot;Exibindo detalhes da prova&quot;.
