---
content-type: release-notes
navigation-topic: product-releases-archive
title: Atividade da versão 2018.3 do Beta 4
description: Esta página descreve todas as alterações disponíveis mais recentemente no ambiente de Pré-visualização com a versão 2018.3 do Beta 4. A funcionalidade estará disponível no ambiente de Pré-visualização em 30 de agosto de 2018. Ele estará disponível no ambiente de Produção em novembro de 2018.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: b40eda2c-8ad4-4945-a7e3-cb28ed8a14db
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '1126'
ht-degree: 0%

---

# Atividade da versão 2018.3 do Beta 4

Esta página descreve todas as alterações disponíveis mais recentemente no ambiente de Pré-visualização com a versão 2018.3 do Beta 4. A funcionalidade estará disponível no ambiente de Pré-visualização em 30 de agosto de 2018. Ele estará disponível no ambiente de Produção em novembro de 2018.

Para obter uma lista de todas as alterações feitas em 2018.3, consulte  Visão geral da atividade da versão [2018.3](../../../../product-announcements/product-releases/quarterly-release-archive/2018.3-release-activity/2018-3-release-activity-overview.md).

A versão 2018.3 do Beta 4 contém melhorias para administradores do Workfront e outros usuários:

**Para Administradores**

* [Atualizar estrutura de relatórios no Perfil de usuário como administrador de grupo](#update-reporting-structure-in-the-user-profile-as-a-group-administrator) 

**Para Todos Os Usuários**

* [Exportar mais informações do Planejador de recursos](#export-more-information-from-the-resource-planner)
* [Melhorias na Lista de Tarefas](#task-list-improvements) Removidas da Versão
* [Melhorias na Lista de Projetos](#project-list-improvements)
* [A Edição da Lista de Tarefas no Modo de Edição do Gráfico de Gantt](#editing-the-task-list-in-gantt-chart-edit-mode) foi removida da Liberação
* [Cores da Ferramenta de Medida](#measurement-tool-colors)
* [Abrir Provas em uma Nova Guia](#proofs-open-in-a-new-tab) Removida da Versão

* [Melhorias no Resumo de Impressão](#print-summary-enhancements)
* [Registrar tempo em dias no aplicativo móvel do Workfront](#log-time-in-days-in-the-workfront-mobile-app)

## Atualizar estrutura de relatórios no Perfil do usuário como administrador de grupo {#update-reporting-structure-in-the-user-profile-as-a-group-administrator}

Os administradores de grupo agora podem editar os campos Subordinados diretos e Subordinados a para usuários nos grupos que eles administram.

Anteriormente, somente os administradores do Workfront e usuários com acesso administrativo aos usuários tinham essa capacidade.

Para obter informações sobre administradores de grupo, consulte [Administradores de grupo](../../../../administration-and-setup/manage-groups/group-roles/group-administrators.md).

## Exportar mais informações do Planejador de recursos {#export-more-information-from-the-resource-planner}

Agora você pode exportar informações de até 52 semanas, 36 meses ou 12 trimestres no Planejador de recursos. Se a quantidade de informações exportada for muito grande, você receberá um email com o arquivo exportado anexado. O arquivo está disponível para download por até uma semana a partir do momento em que o download foi iniciado.

Anteriormente, só era possível exportar até um máximo de 4 semanas, meses ou trimestres por vez.

Para obter mais informações, consulte [Exportar informações do Planejador de Recursos](../../../../resource-mgmt/resource-planning/export-resource-planner.md).

## Melhorias na lista de tarefas {#task-list-improvements}

>[!NOTE]
>
>* Esse recurso foi removido do ambiente de Pré-visualização e não será incluído na versão 2018.3. Ele será lançado em uma data posterior.

Uma nova experiência agora está disponível ao visualizar uma lista de tarefas. Essa experiência inclui maior desempenho, bem como uma navegação de lista mais suave e rápida.

As seguintes alterações visíveis também estão disponíveis:

* Os agrupamentos são recolhidos por padrão.\
  Antes dessa alteração, os agrupamentos eram expandidos por padrão.
* Filtros rápidos foram adicionados à lista de tarefas.
* O cabeçalho do Projeto permanece visível ao rolar a lista de tarefas para baixo.
* Novos ícones de status estão disponíveis.

A seguinte funcionalidade foi alterada nas listas de tarefas:

* Clique com o botão direito do mouse no recurso e no menu contextual fornecido.\
  Em vez de clicar com o botão direito do mouse nas tarefas para editá-las, faça o seguinte:

   * Ao selecionar uma única tarefa, agora é possível usar o menu Mais com as mesmas opções do menu anterior de clique com o botão direito.
   * Quando você seleciona várias tarefas, pode usar os ícones na parte superior da lista para executar qualquer uma das ações incluídas no menu anterior de clique com o botão direito do mouse.

     Todas as alterações são visíveis nas listas de tarefas dentro dos projetos, bem como na guia Subtarefas em tarefas.

Para obter mais informações sobre como trabalhar em listas, consulte [Introdução a listas no Adobe Workfront](../../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

Para obter mais informações sobre encadeamento de tarefas no gráfico de Gantt, consulte [Criar relações de predecessoras encadeando tarefas](../../../../manage-work/tasks/use-prdcssrs/create-predecessors-by-chaining-tasks.md).

## Melhorias na lista de projetos {#project-list-improvements}

A capacidade de reordenar colunas foi adicionada de volta a uma lista de projetos nas seguintes subguias:

* Projetos dos quais sou proprietário
* Projetos em que estou trabalhando
* Todos os Projetos

Essa funcionalidade foi removida na versão 2018.2 do.

Para obter mais informações sobre como trabalhar em listas, consulte [Introdução a listas no Adobe Workfront](../../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

## Editando a Lista de Tarefas no Modo de Edição do Gráfico de Gantt {#editing-the-task-list-in-gantt-chart-edit-mode}

>[!NOTE]
>
>* Esse recurso foi removido do ambiente de Pré-visualização e não será incluído na versão 2018.3. Ele será lançado em uma data posterior.

Agora é possível executar as seguintes ações nas tarefas de um projeto quando elas são exibidas no modo de edição do Diagrama de Gantt:

* Adicionar tarefas
* Remover tarefas
* Tarefas de edição em linha

Embora você possa ver como as alterações afetam a linha do tempo do projeto, as alterações não são imediatas. Você pode salvá-los para atualizar a linha do tempo do projeto ou pode cancelá-los.

Anteriormente, não era possível executar essas ações em tarefas quando elas eram exibidas no modo de edição do Gráfico de Gantt. Você poderia fazer essas alterações em uma lista de tarefas que não era exibida no gráfico de Gantt, mas elas eram imediatas.

Para obter informações sobre como editar tarefas no Gráfico de Gantt, consulte [Atualizar informações na lista de tarefas Gráfico de Gantt](../../../../manage-work/gantt-chart/use-the-gantt-chart/update-info-task-list-gantt.md).

## Cores da Ferramenta de Medida {#measurement-tool-colors}

Ao usar a ferramenta de medida para medir áreas em uma prova, agora é possível alterar a cor e a opacidade da ferramenta. O Workfront lembra dessas configurações em todas as provas que você abre até esvaziar o cache do navegador.

A cor padrão agora é vermelha.

Anteriormente, a ferramenta de medição era exibida apenas em azul, o que dificultava a visualização de conteúdo de prova com tons de azul semelhantes.

## Abrir provas em uma nova guia {#proofs-open-in-a-new-tab}

>[!NOTE]
>
>* Este recurso foi removido do ambiente de Pré-visualização e não será incluído na versão 2018.3.

Ao abrir uma prova em qualquer lugar no Workfront ou Workfront Proof, o visualizador de provas agora é iniciado em uma nova guia do navegador e o foco muda para essa guia. Você pode trabalhar em várias guias do navegador, revisar provas e continuar seu trabalho em projetos, tarefas e problemas no Workfront ou Workfront Proof.

Anteriormente, o visualizador de provas era iniciado em um quadro na parte superior da guia atual do navegador Workfront ou Workfront Proof, tornando essa guia inacessível até que você fechasse o visualizador de provas.

Para obter mais informações, consulte.

## Melhorias no resumo de impressão {#print-summary-enhancements}

Os seguintes aprimoramentos estão disponíveis na página Resumo de impressão ao imprimir uma prova ou salvá-la como um arquivo PDF ou XLS:

* Você pode classificar os comentários da prova por criador.

  Anteriormente, era possível classificar os comentários na ordem em que eram criados ou na ordem em que apareciam em cada página.

* Você pode filtrar os comentários da prova por Autor, Ação e Status não resolvido.

  Anteriormente, a filtragem de comentários não estava disponível na página de resumo de impressão.

* Estágios agora são incluídos, juntamente com os detalhes sobre cada estágio.

  Anteriormente, os estágios não eram incluídos.

Para obter mais informações, consulte [Imprimir um resumo de prova no Adobe Workfront](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/print-proof-summary-in-wf.md).

## Registrar tempo em dias no aplicativo móvel do Workfront {#log-time-in-days-in-the-workfront-mobile-app}

Agora você pode registrar horas em dias no aplicativo móvel do Workfront. 

Anteriormente, você podia registrar tempo usando apenas horas no aplicativo móvel, mesmo quando sua preferência de perfil estava definida para registrar tempo em dias.

Para obter mais informações sobre o tempo de logon no aplicativo móvel, consulte . 

Esse recurso está imediatamente disponível para teste com o aplicativo Android Beta. 
