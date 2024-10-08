---
content-type: release-notes
navigation-topic: product-releases-archive
title: Atividade da versão 2018.2 do Beta 1
description: Esta página descreve todas as alterações disponíveis mais recentemente no ambiente de Pré-visualização com a versão 2018.2 do Beta 1. A funcionalidade foi disponibilizada no ambiente de Pré-visualização em 22 de março de 2018. Ele estará disponível no ambiente de Produção em junho de 2018.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: cbe98ee2-f155-4d31-88c4-7f41b6f91eb2
source-git-commit: 51b8e474cefe63b4db8c42e480990ca0ba431a4d
workflow-type: tm+mt
source-wordcount: '1166'
ht-degree: 0%

---

# Atividade da versão 2018.2 do Beta 1

Esta página descreve todas as alterações disponíveis mais recentemente no ambiente de Pré-visualização com a versão 2018.2 do Beta 1. A funcionalidade foi disponibilizada no ambiente de Pré-visualização em 22 de março de 2018. Ele estará disponível no ambiente de Produção em junho de 2018.

>[!IMPORTANT]
>
>A funcionalidade descrita nesta página está sujeita a alterações antes da disponibilidade no ambiente de produção.

Para obter uma lista de todas as alterações feitas em 2018.2, consulte a [visão geral da atividade da versão 2018.2](../../../../product-announcements/product-releases/quarterly-release-archive/2018.2-release-activity/2018-2-release-activity-overview.md).

A versão 2018.2 do Beta 1 contém as seguintes melhorias:

* [Modificar Datas da Tarefa no Gráfico de Gantt](#modify-task-dates-in-the-gantt-chart)
* [Acesse o Gráfico de Gantt do Projeto da Guia Atualizações](#access-the-project-gantt-chart-from-the-updates-tab) (Removido Temporariamente)

* [Vários Links Reintroduzidos a Documentos na Lista de Documentos](#various-links-re-introduced-to-documents-on-the-document-list)
* [Melhorias na exibição do usuário no Planejador de recursos](#user-view-improvements-in-the-resource-planner)
* [Nova Experiência de Lista de Projetos](#new-project-list-experience)
* [Nova Guia Procurar Atualizações](#new-look-for-updates-tab)
* [Melhorias na mobilidade](#mobile-improvements)

## Modificar Datas da Tarefa no Gráfico de Gantt {#modify-task-dates-in-the-gantt-chart}

Agora você pode arrastar a bolha de tarefas para alterar as Datas de Início Planejadas e de Conclusão Planejada no gráfico de Gantt. Com essa alteração, você pode aplicar cenários hipotéticos ao seu projeto sem afetar a linha do tempo.

Antes dessa alteração, você poderia alterar as datas da tarefa somente na lista de tarefas ou no nível da tarefa.

Para obter mais informações, consulte [Atualizar informações no Gráfico de Gantt da lista de tarefas](../../../../manage-work/gantt-chart/use-the-gantt-chart/update-info-task-list-gantt.md).

## Acesse o Gráfico de Gantt do Projeto na Guia Atualizações {#access-the-project-gantt-chart-from-the-updates-tab}

>[!NOTE]
>
>Essa funcionalidade foi removida temporariamente do ambiente de Pré-visualização.

Agora você pode acessar o novo gráfico de Gantt do projeto na guia Atualizações. Quando um usuário altera a Data de confirmação de uma tarefa de uma forma que afeta a linha do tempo do projeto, você pode visualizar o impacto no gráfico de Gantt do projeto.

Antes dessa alteração, o link Linha do tempo do projeto abria o Gráfico de Gantt herdado.

Para obter mais informações, consulte [Visão geral da Data de Confirmação](../../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md).

Para obter mais informações, consulte [visão geral do Portfolio Otimizer](../../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md).

## Vários links foram reintroduzidos a documentos na lista de documentos {#various-links-re-introduced-to-documents-on-the-document-list}

Na versão 18.1, vários links foram removidos dos documentos na lista de documentos e movidos para outras áreas da interface (alguns como um botão ao lado do nome do documento e outros em um menu suspenso no botão). Os links a seguir estão sendo reintroduzidos abaixo do nome do documento com esta versão e agora estão disponíveis em documentos individuais na lista de documentos:

* Gerar prova (disponível quando uma prova ainda não foi gerada)
* Abrir prova (disponível quando uma prova é gerada)
* Detalhes do documento (disponível quando uma prova ainda não foi gerada)
* Detalhes da prova (disponível quando uma prova é gerada)
* Imprimir Sumário

As seguintes ações não estão sendo reintroduzidas como links no documento na lista de documentos:

* Compartilhar (ainda disponível como um botão no menu)
* Check-out / Check-in (ainda disponível no menu suspenso Mais no menu)

Para obter mais informações, consulte as seguintes seções:

*  in 

## Melhorias na visualização do usuário no Planejador de recursos {#user-view-improvements-in-the-resource-planner}

A visualização Usuário do Planejador de recursos agora contém as seguintes melhorias:

* A Exibição do usuário agora é a padrão, substituindo a Exibição do projeto.
* Filtros aprimorados que extraem informações de todo o banco de dados, em vez de apenas as informações na tela.
* Modo de tela cheia.
* O desempenho agora é mais rápido e mais eficiente.

   * Novos limites para o número de usuários, projetos, funções e tarefas que você pode exibir.
   * Carregamento lento, para carregamento mais rápido de usuários.

A seguinte funcionalidade foi temporariamente desabilitada no Planejador de recursos:

* Exportar os dados do Planejador de recursos ao usar a Exibição de usuário.

Antes dessas melhorias, você relatou que o Planejador de recursos estava lento para carregar e que havia notado incongruências nos dados exibidos. Com essas melhorias, elas devem ser eliminadas.

Para obter mais informações sobre as áreas do Planejador de recursos, consulte [Visão geral da navegação do Planejador de recursos](../../../../resource-mgmt/resource-planning/resource-planner-navigation.md).

<!--
<p dir="ltr" data-mc-conditions="QuicksilverOrClassic.Draft mode">To participate in our current beta program and give us feedback on the functionality of the Resource Planner, see <a href="../../../../product-announcements/betas/resource-planner-performance-beta.md" class="MCXref xref">Resource Planner performance beta </a></p>
-->

## Nova experiência de lista de projetos {#new-project-list-experience}

Uma nova experiência agora está disponível ao visualizar uma lista de projetos. Essa experiência inclui maior desempenho e navegação de lista mais suave e rápida. Somente as listas na guia Projetos da área Projetos do Workfront foram atualizadas para essa nova experiência.

Na maioria das vezes, as mudanças estão na velocidade e eficiência da lista. Foram também introduzidas as seguintes alterações visíveis:

* A lista exibe até 2.000 itens por padrão.

  Antes dessa melhoria, a lista exibia 100 itens.

* Os agrupamentos são recolhidos por padrão.

  Antes dessa alteração, os agrupamentos eram expandidos por padrão.

* A área para selecionar uma linha se expandiu para a linha inteira.

Os seguintes recursos foram temporariamente desabilitados nas listas de projetos especificadas:

* Redimensionamento de colunas (essa funcionalidade foi reintroduzida na versão 2018.2 do Beta 5)
* Reorganização de coluna
* Os campos de ícone de status são exibidos como em branco (essa funcionalidade foi reintroduzida na versão 2018.2 do Beta 5)
* O Gráfico de Gantt não está acessível (essa funcionalidade foi reintroduzida na versão 2018.2 do Beta 3.)

Para obter mais informações sobre como trabalhar em listas, consulte [Introdução a listas no Adobe Workfront](../../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

## Nova Guia Procurar Atualizações {#new-look-for-updates-tab}

>[!NOTE]
>
>Para alguns usuários, a nova guia Atualizações pode não ser exibida no ambiente de Pré-visualização. No momento, nossa equipe de desenvolvimento está solucionando o problema e trabalhando para resolvê-lo o mais rápido possível.

A aparência da guia Atualizações foi alterada para estar mais alinhada com outras áreas da interface. Essa alteração se aplica a projetos, tarefas, problemas e documentos.

A tabela a seguir mostra as atualizações feitas na guia Atualizações:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Tarefa</strong> </p> </th> 
   <th> <p><strong>Ação do usuário anterior</strong> </p> </th> 
   <th> <p><strong>Nova ação de usuário</strong> </p> </th> 
   <th> <p><strong>Para obter mais informações, consulte...</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Registrando horas em uma planilha de horas</p> </td> 
   <td> <p>Clique no link Registro de tempo</p> </td> 
   <td> <p>Clique no botão Registro de tempo</p> </td> 
   <td> <p><a href="../../../../timesheets/create-and-manage-timesheets/log-time.md" class="MCXref xref">Registrar tempo</a> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Filtragem de atualizações do sistema na guia Atualizações</p> </td> 
   <td> <p>Clique no link Filtrar atualizações do sistema</p> </td> 
   <td> <p>Desativar a opção Mostrar registro de atividades</p> </td> 
   <td> <p><a href="../../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md" class="MCXref xref">Atualizar trabalho</a> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Exibição de atualizações do sistema na guia Atualizações</p> </td> 
   <td> <p>Clique em Mostrar todas as atualizações</p> </td> 
   <td> <p>Ativar a opção Mostrar registro de atividades</p> </td> 
   <td> <p><a href="../../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md" class="MCXref xref">Atualizar trabalho</a> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Marcar outros usuários em uma atualização ou comentário</p> </td> 
   <td> <p>Clique no ícone Incluir outros nesta atualização</p> </td> 
   <td> <p>Adicionar usuários e equipes no campo Notificar</p> </td> 
   <td> <p><a href="../../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md" class="MCXref xref">Atualizar trabalho</a> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Permitir que apenas usuários em sua empresa visualizem um objeto</p> </td> 
   <td> <p>Clique no ícone Bloquear</p> </td> 
   <td> <p>Ativar a opção Privado para minha empresa</p> </td> 
   <td> <p><a href="../../../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md" class="MCXref xref">Marcar outros usuários sobre atualizações</a> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Permitir que usuários fora da empresa visualizem um objeto</p> </td> 
   <td> <p>Clique no ícone Bloquear</p> </td> 
   <td> <p>Desativar a alternância de Privado para Minha Empresa</p> </td> 
   <td> <p><a href="../../../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md" class="MCXref xref">Marcar outros usuários sobre atualizações</a> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Adicionar uma resposta ou atualização a um comentário ou atualização</p> </td> 
   <td> <p>Clique no botão Comentário</p> </td> 
   <td> <p>Clique no botão Responder ou Atualizar</p> </td> 
   <td> <p><a href="../../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md" class="MCXref xref">Atualizar trabalho</a> </p> <p><a href="../../../../manage-work/projects/updating-work-in-a-project/update-task-status.md" class="MCXref xref">Atualizar status da tarefa</a> </p> <p><a href="../../../../manage-work/projects/updating-work-in-a-project/update-condition-for-tasks-and-issues.md" class="MCXref xref">Atualizar condição para tarefas e problemas</a> </p> <p> </p> <p><a href="../../../../documents/managing-documents/add-update-documents.md" class="MCXref xref">Adicionar uma atualização a um documento</a> </p> </td> 
  </tr> 
 </tbody> 
</table>

## Melhorias na mobilidade {#mobile-improvements}

O aplicativo móvel contém as seguintes melhorias:

* Os links compartilhados com você em outros aplicativos móveis agora são abertos no aplicativo móvel do Workfront.

  Para obter mais informações sobre compartilhamento de links, consulte .

  Essa atualização será lançada no iOS às vezes nesta semana, e a atualização do Android deve seguir logo depois.

* Atualizamos nossos requisitos de suporte para a plataforma iOS para oferecer suporte ao iPhone X.

  Para obter mais informações sobre dispositivos móveis e sistemas operacionais compatíveis, consulte o .
