---
content-type: release-notes
navigation-topic: product-releases-archive
title: Atividade da versão 2018.1 do Beta 2
description: Esta página descreve todas as alterações disponíveis mais recentemente no ambiente de Pré-visualização com a versão 2018.1 do Beta 2. A funcionalidade nesta página foi disponibilizada no ambiente de Pré-visualização em 14 de dezembro de 2017. Ele estará disponível no ambiente de Produção em março de 2018.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 22e3836c-c41e-48a6-9926-e832af91e616
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '1327'
ht-degree: 2%

---

# Atividade da versão 2018.1 do Beta 2

Esta página descreve todas as alterações disponíveis mais recentemente no ambiente de Pré-visualização com a versão 2018.1 do Beta 2. A funcionalidade nesta página foi disponibilizada no ambiente de Pré-visualização em 14 de dezembro de 2017. Ele estará disponível no ambiente de Produção em março de 2018.

>[!IMPORTANT]
>
> A funcionalidade descrita nesta página está sujeita a alterações antes da disponibilidade no ambiente de produção.

Para obter uma lista de todas as alterações feitas em 2018.1, consulte  Visão geral da atividade da versão [2018.1](../../../../product-announcements/product-releases/quarterly-release-archive/2018.1-release-activity/2018-1-release-activity-overview.md).

A versão 2018.1 do Beta 2 contém melhorias para administradores do Workfront e outros usuários:

**Para Administradores**

* [Administração de grupo para usuários e modelos de layout](#group-administration-for-users-and-layout-templates)

**Para Todos Os Usuários**

* [Monitor Widescreen em Todo o Sistema](#system-wide-widescreen-display)
* [Redimensionar Instantâneo de Linha do Tempo no Gráfico de Gantt](#resize-timeline-snapshot-on-the-gantt-chart)
* [Planejador de recursos interativos no Business Case](#interactive-resource-planner-in-the-business-case)
* [Visualização no Planejador de Recursos - Gráfico de Alocação de Usuário](#visualization-in-the-resource-planner-user-allocation-chart)
* [Melhorias na área inicial](#improvements-in-the-home-area)
* [Novas melhorias do visualizador de revisões](#new-proofing-viewer-improvements) 

## Administração de grupo para usuários e modelos de layout {#group-administration-for-users-and-layout-templates}

Agora você pode designar administradores de grupo no Workfront. O campo Proprietário do grupo foi renomeado para administrador de grupo, e os usuários designados como administradores de grupo têm permissões adicionais para gerenciar usuários e modelos de layout para os grupos que gerenciam.

* [Gerenciamento de usuários por administrador de grupo](#user-management-by-group-administrator)
* [Gerenciamento de modelos de layout por administradores de grupo](#layout-template-management-by-group-administrators)

### Gerenciamento de usuários por administrador de grupo {#user-management-by-group-administrator}

Estamos introduzindo o novo conceito de **administrador de grupo**. Para oferecer suporte a isso, o campo **Proprietário do grupo** foi renomeado para **administrador de grupo** e os usuários designados como administradores de grupo têm permissões adicionais para gerenciar usuários e grupos.

Além das permissões que o Proprietário do grupo tinha anteriormente para gerenciar usuários, o administrador do grupo agora tem o seguinte acesso adicional ao gerenciar usuários nos grupos em que estão definidos como administradores do grupo:

* Efetue logon como outro usuário que pertence a um grupo que ele gerencia.
* Redefina a senha de outro usuário que pertença a um grupo gerenciado por ele.
* Crie Modelos de layout administrados pelo grupo. 

Antes dessa alteração, somente o administrador do Workfront podia executar essas funções.

Para obter mais informações sobre administradores de grupo, consulte a seção &quot;Noções básicas sobre administradores de grupo&quot; em [Criar um grupo](../../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).

### Gerenciamento de modelos de layout por administradores de grupo {#layout-template-management-by-group-administrators}

Estamos introduzindo o novo conceito de **Grupo com Acesso de Administração** que você pode associar a um Modelo de Layout.

O usuário designado como administrador de grupo neste grupo tem acesso para gerenciar esse Modelo de layout e criar novos Modelos de layout onde os grupos gerenciados são os grupos administrativos dos modelos. 

Antes dessa alteração, somente o administrador do Workfront poderia criar Modelos de layout.

Para obter mais informações sobre como criar Modelos de Layout, consulte &quot;Criando e Gerenciando Modelos de Layout&quot;.

## Monitor widescreen em todo o sistema {#system-wide-widescreen-display}

Ao exibir qualquer página no Workfront, agora toda a janela do navegador é preenchida automaticamente e se ajusta ao tamanho da tela.

Antes dessa alteração, somente as páginas associadas aos seguintes objetos eram exibidas em tela widescreen:

* Projetos
* Tarefas
* Problemas
* Relatórios
* Painéis
* Calendários

## Redimensionar Instantâneo da Linha do Tempo no Gráfico de Gantt {#resize-timeline-snapshot-on-the-gantt-chart}

Agora você pode expandir o instantâneo da linha do tempo para mostrar o projeto inteiro no gráfico de Gantt.

Antes dessa melhoria, você poderia selecionar um ponto específico no instantâneo da linha do tempo para navegar até ele no gráfico de Gantt.

Para obter mais informações sobre como configurar as informações exibidas no gráfico de Gantt, consulte [Configurar como as informações são exibidas no Gráfico de Gantt](../../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md).

## Planejador de recursos interativos no Business Case {#interactive-resource-planner-in-the-business-case}

Como um Gerente de recursos, agora é possível adicionar Conjuntos de recursos na seção Orçamento de recursos do Business Case. Você também pode estimar os recursos do projeto usando o Planejador de recursos no nível do projeto. Orçar seus recursos para um projeto gera o Custo de mão de obra orçado do projeto.

Antes dessa alteração, você poderia exibir as informações de orçamento de recursos no Business Case se o projeto tivesse sido orçado para recursos no Planejador de recursos global.

Para obter mais informações sobre como concluir o orçamento de recursos do projeto no Business Case, consulte [Recursos de orçamento no Business Case](../../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md).

## Visualização no Planejador de recursos - Gráfico de alocação de usuários {#visualization-in-the-resource-planner-user-allocation-chart}

Agora você pode exibir a Alocação planejada geral de todos os usuários em relação à sua disponibilidade em um gráfico no Planejador de recursos. O gráfico estará disponível quando você selecionar **Exibir por Usuário** no Planejador de Recursos.

O gráfico exibe as seguintes informações:

* % de disponibilidade sem excesso de alocação de todos os usuários
* % de excesso de alocação de todos os usuários
* % de subutilização de todos os usuários
* Há um excesso de alocações para, pelo menos, um usuário durante este período de tempo

Antes dessa alteração, você poderia visualizar a alocação e a disponibilidade de usuários individuais somente no formato de tabela.

Para obter mais informações sobre o gráfico de alocação de usuários no Planejador de recursos, consulte [Visão geral do Planejador de recursos](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

## Melhorias na área inicial {#improvements-in-the-home-area}

Várias melhorias estão disponíveis na área da Página inicial, incluindo:

* Melhorias na aparência

   * O painel direito agora é maior, permitindo mais espaço para informações de tarefas e problemas.
   * Os itens atrasados agora são exibidos em um tom mais claro de vermelho quando selecionados no painel esquerdo.
   * Agora é possível ver mais facilmente a relação entre o painel esquerdo e o painel direito. O documento selecionado no painel esquerdo aponta para o painel direito.

* Os campos padrão são exibidos para os itens selecionados. 

  Para obter mais informações sobre os campos padrão, consulte &quot;Criação e gerenciamento de modelos de layout&quot;.

* Depois de clicar em &quot;Trabalhar nisso&quot; em uma solicitação, os campos associados ao problema são exibidos no painel direito.

  Para obter mais informações sobre como trabalhar nas solicitações da Área inicial, consulte [Gerenciar solicitações de trabalho e de equipe na Área inicial](../../../../workfront-basics/using-home/using-the-home-area/manage-work-and-team-requests-home.md) em [Gerenciar solicitações de trabalho e de equipe na Área inicial](../../../../workfront-basics/using-home/using-the-home-area/manage-work-and-team-requests-home.md).

* Aponte para um avatar do usuário em um item de trabalho no painel esquerdo para exibir o nome do usuário.
* Expanda a área &quot;Atrasado&quot; no painel esquerdo para exibir todos os itens atrasados (quando essa área for recolhida, somente os primeiros 5 itens serão exibidos).
* Depois de marcar um item como Concluído, ele permanece no painel esquerdo até que você selecione outro item.\
  Para obter informações sobre como mostrar itens concluídos, consulte [Exibir itens na Lista de Trabalho na área Página Inicial](../../../../workfront-basics/using-home/using-the-home-area/display-items-in-home-work-list.md) em [Exibir itens na Lista de Trabalho na área Página Inicial](../../../../workfront-basics/using-home/using-the-home-area/display-items-in-home-work-list.md).

Para obter mais informações sobre como usar a nova área Página inicial, bem como informações que descrevem as diferenças de funcionalidade entre Meu Trabalho e Página Inicial, consulte [Usar a área Página Inicial](../../../../workfront-basics/using-home/using-the-home-area/use-the-home-area.md).

## Novas melhorias do visualizador de provas  {#new-proofing-viewer-improvements}

* [Layout e Design Aprimorados](#improved-layout-and-design)
* [Pesquisar comentários por número de comentário](#search-comments-by-comment-number)
* [Opção para Editar Comentário ao lado do Indicador de Marcação](#option-to-edit-comment-next-to-the-markup-indicator)
* [Marcar todos os comentários como lidos](#mark-all-comments-as-read)
* [Melhorias no menu esquerdo](#left-menu-improvements)

### Layout e design aprimorados {#improved-layout-and-design}

O revisor de provas tem uma aparência atualizada. A variável  as seguintes áreas do revisor de provas foram atualizadas:

* Área de miniaturas

  Para obter mais informações sobre o uso da área de miniaturas, consulte em .

* Área de comentários\
  Para obter mais informações sobre a área de comentários, consulte .
* Área do menu esquerdo

### Pesquisar comentários por número do comentário {#search-comments-by-comment-number}

Agora, ao pesquisar a lista de comentários no visualizador de provas, você pode inserir o número do comentário no campo de pesquisa. A lista de comentários é então filtrada para exibir o comentário pesquisado. 

Para obter mais informações, consulte em .

### Opção para editar comentário ao lado do indicador de marcação {#option-to-edit-comment-next-to-the-markup-indicator}

Agora é possível editar mais facilmente um comentário existente. Depois de clicar em um indicador de comentário na prova, um ícone de edição é exibido ao lado do balão. 

Antes dessa alteração, você tinha que clicar no ícone de edição na área Comentário.  

Para obter mais informações, consulte.

### Marcar todos os comentários como lidos {#mark-all-comments-as-read}

Ao visualizar um documento no visualizador de provas, agora é possível marcar todos os comentários como Lidos.

### Melhorias no menu esquerdo {#left-menu-improvements}

O menu no lado esquerdo do revisor de provas contém as seguintes melhorias:

* Aparência e comportamento atualizados
* Ícone na parte superior do menu para mostrar ou ocultar o menu

  ![proof_viewer_menu_hide.png](assets/proof-viewer-menu-hide.png)

* Passe o mouse sobre o menu para expandir automaticamente o menu e exibir rótulos, além de ícones. (Ou ative a opção para manter o menu sempre na exibição recolhida.)
