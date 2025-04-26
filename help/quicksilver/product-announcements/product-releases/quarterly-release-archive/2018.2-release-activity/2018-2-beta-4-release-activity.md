---
content-type: release-notes
navigation-topic: product-releases-archive
title: Atividade da versão 2018.2 do Beta 4
description: Esta página descreve todas as alterações disponíveis mais recentemente no ambiente de Pré-visualização com a versão 2018.2 do Beta 4. A funcionalidade estará disponível no ambiente de Pré-visualização em 17 de maio de 2018. Ele estará disponível no ambiente de Produção em julho de 2018.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 4b54b9e6-d1bf-4802-9d6c-9c3d3b6a6583
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '1705'
ht-degree: 0%

---

# Atividade da versão 2018.2 do Beta 4

Esta página descreve todas as alterações disponíveis mais recentemente no ambiente de Pré-visualização com a versão 2018.2 do Beta 4. A funcionalidade estará disponível no ambiente de Pré-visualização em 17 de maio de 2018. Ele estará disponível no ambiente de Produção em julho de 2018.

>[!IMPORTANT]
>
> A funcionalidade descrita nesta página está sujeita a alterações antes da disponibilidade no ambiente de produção.

Para obter uma lista de todas as alterações feitas em 2018.2, consulte  Visão geral da atividade da versão [2018.2](../../../../product-announcements/product-releases/quarterly-release-archive/2018.2-release-activity/2018-2-release-activity-overview.md).

A versão 2018.2 do Beta 4 contém as melhorias para administradores do Workfront e outros usuários:

**Para Administradores**

* [Configuração do Sistema: Informações da Sessão em Páginas Externas](#system-setting-session-information-in-external-pages)

**Para Todos Os Usuários**

* [Melhorias no limite do Trabalho em andamento (WIP) no Quadro Kanban](#work-in-progress-wip-limit-enhancements-on-the-kanban-board)
* [Interface aprimorada para configurar status para uma Equipe Agile](#improved-interface-for-configuring-statuses-for-an-agile-team)
* [Lista de Trabalho Atualizada (Painel Esquerdo) na Área Inicial](#updated-work-list-left-panel-in-the-home-area)
* [Novo Visualizador de Revisores de Texto para Revisão de Conteúdo Interativo (Rich Media)](#new-desktop-proofing-viewer-for-proofing-interactive-rich-media-content) 
* [Exportar o Modo de Exibição de Usuário no Planejador de Recursos](#export-the-user-view-in-the-resource-planner)
* [Suporte para Google Team Drives](#support-for-google-team-drives)
* [Novo limite de exportação para o Gráfico de Gantt](#new-export-limit-for-the-gantt-chart)
* [A Opção Colar da Área de Transferência agora é exibida como esmaecida ao usar o Internet Explorer ou o Safari](#paste-from-clipboard-option-now-displays-as-dimmed-when-using-internet-explorer-or-safari)
* [Novo ambiente do Beta para Android junto com novos recursos](#new-beta-environment-for-android-along-with-new-features)
* [Exemplos de filtros para mensagens de assinaturas de evento](#examples-of-filters-for-event-subscriptions-messages)

## Melhorias do limite de Trabalho em andamento (WIP) no Quadro Kanban {#work-in-progress-wip-limit-enhancements-on-the-kanban-board}

### Configurar Limites de Trabalho em Andamento (WIP) para Cada Coluna no Quadro Kanban

Agora você pode configurar os limites de Trabalho em andamento (WIP) para cada coluna no quadro Kanban. 

Antes dessa alteração, você poderia configurar apenas um limite WIP que se aplicasse a todas as colunas no quadro Kanban. 

Para obter mais informações, consulte a seção  [Configurar o limite do trabalho em andamento (WIP)](../../../../agile/get-started-with-agile-in-workfront/configure-kanban.md#configur4) no artigo  [Configurar Kanban](../../../../agile/get-started-with-agile-in-workfront/configure-kanban.md).

### Atualizar o limite do Trabalho em andamento (WIP) diretamente do Quadro Kanban

Agora, os membros da equipe com direitos de Edição da equipe podem atualizar o limite de WIP diretamente do quadro Kanban.

Antes dessa alteração, você poderia atualizar o limite de WIP somente a partir da área Configurações da equipe.

Para obter mais informações, consulte  no artigo .

## Interface aprimorada para configurar status para uma Equipe Agile {#improved-interface-for-configuring-statuses-for-an-agile-team}

A interface para configurar os status de uma Equipe Ágil foi atualizada com as seguintes melhorias:

* Nova aparência
* Reordenar colunas de status via arrastar e soltar 

Para obter mais informações, consulte os seguintes artigos:

* [Configurar Kanban](../../../../agile/get-started-with-agile-in-workfront/configure-kanban.md)
* [Configurar Scrum](../../../../agile/get-started-with-agile-in-workfront/configure-scrum.md)

## Lista de trabalho atualizada (painel esquerdo) na área da página inicial {#updated-work-list-left-panel-in-the-home-area}

A Lista de trabalho na área Página inicial contém as seguintes melhorias:

* Os itens não lidos agora se destacam com negrito e um ponto azul.

  Os itens exibidos fora da área Página inicial ainda são exibidos como Não lidos na área Página inicial.

  Para obter mais informações, consulte [Exibir itens na Lista de Trabalho na área Página Inicial](../../../../workfront-basics/using-home/using-the-home-area/display-items-in-home-work-list.md).

* Agora, os problemas são exibidos com um ícone de problema ao lado dele.
* As aprovações agora são diferenciadas por tipo de aprovação, com o tipo de aprovação sendo exibido. Os possíveis tipos de aprovação são Tarefa, Projeto, Problema, Acesso, Documento, Planilha de Horas e Prova.

  Antes dessa alteração, as aprovações eram diferenciadas somente pela palavra &quot;Aprovação&quot;.

* Os itens agora são diferenciados pelo fato de estarem prontos para iniciar. As opções possíveis são Ready to Start, Not Ready ou Working On.

  Essas informações não são mostradas para aprovações porque as aprovações estão sempre prontas para começar.

* Um ícone de documento é exibido abaixo do nome do item sempre que um documento é anexado ao item.
* Agora é possível recolher e expandir agrupamentos na Lista de trabalho para controlar melhor quais informações estão visíveis. Os agrupamentos são Atrasado, Projetos, Datas e Concluído.

  Por padrão, a seção Esta semana é expandida e todos os outros agrupamentos são recolhidos.

* Escolha se deseja classificar os itens por Data de Término Planejada ou Data de Compromisso.
* O número de itens em cada agrupamento agora é exibido entre parênteses ao lado do título do agrupamento.

  Este número não está disponível para o agrupamento Concluído.

  Para obter mais informações, consulte [Exibir itens na Lista de Trabalho na área Página Inicial](../../../../workfront-basics/using-home/using-the-home-area/display-items-in-home-work-list.md).

* Redimensionar a Lista de trabalho por meio do arrastar e soltar. É possível redimensionar a Lista de trabalho para consumir até metade da tela. O tamanho definido será mantido na próxima vez que você acessar a Página inicial.

  Antes dessa alteração, não era possível alterar o tamanho da Lista de trabalho.

* Para solicitações de, o avatar do usuário que fez a solicitação agora é exibido, com o texto &quot;[Approver_name] like your approval on.&quot;
* Ao criar uma nova tarefa pessoal, o botão &quot;Tarefas&quot; agora é rotulado como &quot;Pessoal&quot;.

  Para obter mais informações, consulte [Criar itens de trabalho da Área inicial](../../../../workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md) no artigo [Criar itens de trabalho da Área inicial](../../../../workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md).

* Os itens atrasados são indicados como Atrasados somente após uma hora após a Data de conclusão planejada.

Para obter mais informações sobre a área da Página Inicial, consulte [Usar a área da Página Inicial](../../../../workfront-basics/using-home/using-the-home-area/use-the-home-area.md).

## Novo visualizador de provas de desktop para prova de conteúdo interativo (mídia avançada) {#new-desktop-proofing-viewer-for-proofing-interactive-rich-media-content}

O novo Visualizador de provas de desktop permite que você revise o conteúdo interativo. Ao contrário do visualizador de provas herdado existente e do novo visualizador de provas executado no navegador, o Visualizador de provas de desktop é um aplicativo executado na sua estação de trabalho.

Antes do novo Visualizador de provas de desktop, você podia revisar o conteúdo interativo somente no Visualizador de provas herdadas. 

O Visualizador de provas de desktop inclui os seguintes aprimoramentos em relação ao Visualizador de provas herdadas para provas de conteúdo interativo:

* Revisar sites não seguros (HTTP)

  O visualizador de provas herdadas permitia revisar somente sites seguros (HTTPS)

* Revise sites protegidos por iframe (sites protegidos contra visualização em um iframe).

  O visualizador de provas herdadas não oferecia suporte à revisão para sites protegidos contra visualização em um iframe.

* Visualize o conteúdo com resoluções pré-configuradas para vários dispositivos. Por exemplo, você pode ver como o conteúdo é exibido em várias resoluções padrão de desktop ou em dispositivos individuais, como um iPhone 8. 

Para obter mais informações sobre como baixar, instalar e usar o Visualizador de provas de desktop, consulte .

Para obter informações sobre as diferenças de funcionalidade entre o Visualizador de Revisão de Texto para Desktop e os visualizadores de revisão baseada em navegador, consulte [Diferenças entre o Visualizador de Revisão de Texto para Web e a visão geral do Visualizador de Revisão de Texto para Desktop](../../../../review-and-approve-work/proofing/proofing-overview/understand-differences-between-web-viewer.md).

## Exportar a visualização do usuário no Planejador de recursos {#export-the-user-view-in-the-resource-planner}

Desativamos temporariamente a exportação de dados do Planejador de recursos ao exibi-los na Exibição do usuário para resolver algumas preocupações de desempenho. Com esta versão, estamos reativando a exportação de dados ao exibir o Planejador de recursos na Exibição do usuário.

Para obter mais informações sobre como exportar os dados do Planejador de recursos para o Excel, consulte a seção &quot;Opção de Exportação&quot; na [Visão geral da navegação do Planejador de recursos](../../../../resource-mgmt/resource-planning/resource-planner-navigation.md).

Para participar do nosso programa beta atual para o Planejador de recursos, consulte [Beta de desempenho do Planejador de recursos.](https://experienceleaguecommunities.adobe.com/t5/workfront/ct-p/workfront)

## Configuração do Sistema: Informações da Sessão em Páginas Externas {#system-setting-session-information-in-external-pages}

O administrador do Workfront agora pode restringir o uso de informações da sessão (por exemplo, ID de sessão) ao criar uma Página externa.

Antes dessa alteração, os usuários que poderiam criar Páginas externas poderiam usar qualquer informação de sessão ao incorporar outros sites em um painel do Workfront. 

Para obter mais informações sobre como configurar suas Preferências do Sistema no Workfront, consulte [Configurar preferências de segurança do sistema](../../../../administration-and-setup/manage-workfront/security/configure-security-preferences.md).

## Suporte para Google Team Drives {#support-for-google-team-drives}

Agora você pode vincular um documento ou uma pasta localizada em um Google Team Drive da Workfront.

Antes dessa melhoria, você poderia vincular um documento ou uma pasta localizada somente no Google My Drive.

Para obter mais informações sobre como vincular documentos e pastas de vários aplicativos ao Workfront, consulte [Vincular documentos de aplicativos externos](../../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

## Novo limite de exportação para o Gráfico de Gantt {#new-export-limit-for-the-gantt-chart}

Agora é possível exportar até 500 tarefas no gráfico de Gantt.

Anteriormente, só era possível exportar até 250 tarefas.

Para obter mais informações, consulte [Exportar o Gráfico de Gantt para o PDF](../../../../manage-work/gantt-chart/use-the-gantt-chart/export-gantt-chart-to-pdf.md).

## A opção Colar da área de transferência agora é exibida como esmaecida ao usar o Internet Explorer ou o Safari {#paste-from-clipboard-option-now-displays-as-dimmed-when-using-internet-explorer-or-safari}

A opção Colar da área de transferência agora é exibida como esmaecida ao usar os navegadores Internet Explorer ou Safari, com uma dica de ferramenta explicando que somente os navegadores Chrome e Firefox são compatíveis com esse recurso.

Antes dessa alteração, essa opção não era exibida ao usar o Internet Explorer ou o Safari. 

Para obter mais informações sobre como colar imagens da área de transferência, consulte [Colar imagens da Área de Transferência](../../../../documents/managing-documents/paste-image-clipboard.md).

## Novo ambiente do Beta para Android junto com novos recursos {#new-beta-environment-for-android-along-with-new-features}

Agora você pode experimentar os recursos mais recentes em que nossa equipe está trabalhando para o aplicativo móvel antes que eles sejam lançados para o público em geral ao se inscrever para ser um testador beta. No momento, esse ambiente é compatível com o aplicativo móvel Workfront somente para telefones Android.

Para obter mais informações sobre como se inscrever para ser um testador beta do aplicativo móvel do Workfront, consulte .

As seguintes melhorias estão disponíveis na versão beta do aplicativo móvel:

* Página Nova conta

  Agora você pode visualizar as informações da sua conta, gerenciar as configurações móveis, enviar feedback ou sair da nova página Conta.

  Antes dessa melhoria, você não podia visualizar as informações da sua conta no aplicativo móvel e acessar as suas configurações, enviar comentários e sair do menu principal do Workfront.

* Novo painel inferior de navegação

  Uma barra de navegação mais proeminente está disponível na parte inferior da tela e inicia todas as áreas do aplicativo móvel.

  Antes dessa melhoria, as áreas de funcionalidade eram listadas no menu principal do Workfront. O menu principal do Workfront foi removido e substituído pela nova barra de navegação inferior.

  Para obter mais informações sobre como configurar a nova barra de navegação, consulte a seção &quot;Configuração do aplicativo móvel&quot; em .

* Nova Exibição de Lista de Notificações

  Uma aparência aprimorada da lista Notificações permite diferenciar facilmente as notificações na lista, dependendo de que tipo elas são e se foram lidas.

* A caixa de pesquisa foi movida para uma posição mais proeminente.

* Nova experiência de logonHá uma nova experiência de logon mais simplificada.

* Nova experiência de tutorial

  Novos tutoriais agora estão disponíveis para guiar os usuários por meio do aplicativo quando eles fazem logon pela primeira vez. Antes dessa experiência, os tutoriais eram iniciados somente quando os usuários acessavam áreas específicas de funcionalidade.

## Exemplos de filtros para mensagens de assinaturas de evento {#examples-of-filters-for-event-subscriptions-messages}

Para demonstrar como você pode filtrar Assinaturas de eventos para receber apenas as mensagens relevantes para sua organização, exemplos de trechos de código agora estão disponíveis para filtrar o fluxo de eventos que chegam aos seus pontos de extremidade. Para saber mais sobre como exibir os exemplos de filtragem, consulte [Filtrar mensagens de assinatura de evento](../../../../wf-api/api/filter-event-sub-messages.md).
