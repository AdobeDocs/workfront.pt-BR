---
product-area: reporting
navigation-topic: reporting-elements
title: Usar curingas com base no usuário para generalizar relatórios
description: Você pode generalizar um relatório usando curingas em vez de informações específicas ao criar determinados elementos de relatórios.
author: Nolan
feature: Reports and Dashboards
exl-id: 216e2869-b4f8-4cc7-9497-a12ebe00fe49
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '448'
ht-degree: 2%

---

# Usar curingas com base no usuário para generalizar relatórios

<!-- Audited: 11/2024 -->

Você pode generalizar um relatório usando curingas em vez de informações específicas ao criar determinados elementos de relatórios. Por exemplo, se você deseja criar um relatório que mostre as tarefas atribuídas a um usuário específico, é possível usar o nome do usuário no campo Assigned To do filtro. No entanto, se você quiser criar um relatório que mostre tarefas atribuídas ao usuário conectado, independentemente de quem seja esse usuário, você poderá usar um curinga que indique que, quando alguém exibir o relatório, ele exibirá informações pertencentes a ele. Dessa forma, você cria o relatório uma vez, mas como você usa um curinga no filtro, ele produz resultados diferentes sempre que outra pessoa o lê.

Você pode usar curingas baseados no usuário ao criar os seguintes elementos de relatórios:

* Filtros
* Prompts personalizados
* Exibições ao adicionar regras para colunas

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacote do Adobe Workfront</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</strong></td> 
   <td> 
    <p>Standard</p>
    <p>Plano</p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Editar acesso a Filtros, Visualizações, Agrupamentos</p> <p>Editar acesso a relatórios, painéis e calendários para editar elementos de relatórios em um relatório</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
    <td> <p>Gerenciar permissões para um relatório para editar elementos de relatórios em um relatório</p> <p>Gerenciar permissões em uma exibição ou um filtro para editá-las</p></td> 
   </td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Pré-requisitos

Você deve criar um relatório antes de adicionar uma variável curinga a ele.

Para obter instruções sobre como criar relatórios, consulte [Criar um relatório](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md).

## Etapas passo a passo

Para inserir um curinga baseado no usuário em um relatório:

1. Ir para um relatório para o qual você deseja inserir um curinga baseado em usuário.
1. Clique em **Ações de Relatório** e depois em **Editar**.

1. Clique na guia **Filtros**.
1. Clique em **Adicionar uma Regra de Filtro**.
1. Comece digitando o nome do campo pelo qual deseja filtrar.\
   Você deve digitar campos que façam referência ao objeto do usuário ou informações sobre os usuários.
1. Selecione **Igual** no menu suspenso da variável de filtro.

   >[!TIP]
   >
   >Você sempre deve selecionar a variável de filtro **Igual** ao trabalhar com curingas no Adobe Workfront.

1. Na caixa **Comece a digitar o nome ...**, digite: `$$USER.ID` ou `$$USER.name` se desejar que o relatório exiba informações sobre o usuário que faz logon, com base em seu nome. Você pode inserir outros curingas que se referem a Grupo, Equipe, Empresa ou outras informações do usuário conectado.

   Para obter uma lista completa de curingas baseados no usuário, consulte [Visão geral das variáveis de filtro de curinga](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).

1. Clique em **Salvar + Fechar**.

## Informações adicionais

Consulte também:

<!--outdated: * [Basic Report Creation Program](https://one.workfront.com/s/basic-report-creation-program) -->
* [Visão geral das variáveis de filtro curinga](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md)
* [Criar ou editar filtros no Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/create-filters.md)
* [Visão geral dos Filtros](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)
* [Adicionar um prompt a um relatório](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md)
* [Usar formatação condicional em exibições](../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md)
