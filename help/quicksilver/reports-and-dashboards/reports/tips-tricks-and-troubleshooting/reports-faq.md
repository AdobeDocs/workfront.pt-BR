---
content-type: faq
product-area: reporting
navigation-topic: tips-tricks-and-troubleshooting-reports
title: Perguntas frequentes sobre relatórios
description: Perguntas frequentes sobre relatórios
author: Nolan
feature: Reports and Dashboards
exl-id: 5e267d45-7922-4c0f-8530-59a8c152f625
source-git-commit: 04818bc054c3bab6e6208b6678365549664d1594
workflow-type: tm+mt
source-wordcount: '1500'
ht-degree: 0%

---

# Perguntas frequentes sobre relatórios

<!--Audited: 05/2025-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina: ***This is the ONE anchor article for all FAQs about Reporting. Add a new FAQ in the TOC at the top first, then add the answer as a section at the bottom.)</p>
-->

A seguir, perguntas frequentes sobre relatórios.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso.

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td><p>Novo: Padrão</p> 
   <p>Atual: trabalho ou superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Editar acesso a relatórios, painéis, calendários</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões para um relatório</p>  </td> 
  </tr> 
 </tbody> 
</table>

*Para obter mais informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Por que meu cálculo personalizado de uma diferença de hora não mostra o resultado correto em uma coluna?

<!--this section is linked from the Actual Hours article for Tasks in the Task Information folder; edit the links or do not delete or change this section-->

Em um relatório de projeto, tenho um cálculo que subtrai as Horas efetivas herdadas das Horas planejadas.

O resultado que estou obtendo está incorreto.

<!--this changed with this issue in May 2025; Actual Hours changed from actualWorkRequired to actualWorkRequiredDouble: https://experience.adobe.com/#/@adobeinternalworkfront/so:hub-Hub/workfront/task/68108e860000120e90a79cb82e5811c2/updates : On a project report I have a calculation that subtracts Actual Hours (2) from Planned Hours (4). The result I am getting is 120 when it should be 2.  -->

Meu cálculo é:

`valueexpression=SUB(workRequired,actualWorkRequired)`

### Responder

A maioria dos campos que usam horas no Workfront é armazenada em minutos. Ao usar esses campos em um cálculo, o resultado será, na maioria das vezes, em minutos. Para obter o resultado em horas, é necessário dividir o resultado do cálculo ou o campo ao qual você está fazendo referência por 60.

O cálculo correto é:

`valueexpression=SUB(workRequired,actualWorkRequired)/60`

>[!NOTE]
>
>Se você estiver usando Horas Efetivas em seu cálculo, use `actualWorkRequiredDouble` para o campo de valor. As horas efetivas são armazenadas em horas. As horas planejadas são armazenadas em minutos.
>
>O cálculo correto para Horas Reais é:
>>`valueexpression=SUB(workRequired/60,actualWorkRequiredDouble)`


## Por que o valor de cada um dos meus elementos de gráfico em um relatório não é exibido no gráfico?

### Responder

Se você tiver mais de 50 elementos de gráfico em um gráfico de relatório, o valor de cada elemento não será exibido no gráfico.

Quando você tem menos de 50 elementos em um gráfico, o valor de cada elemento é exibido no gráfico. Considere adicionar um filtro ou modificar os agrupamentos no relatório para limitar a quantidade de itens exibidos em cada elemento do gráfico.

## Por que meu relatório está retornando muitos resultados para exibir o gráfico?

Quando executo um relatório que tem um gráfico, vejo a mensagem de erro &quot;Olá... Este relatório retornou MUITOS dados, o que torna o gráfico ilegível. Considere restringir seus resultados adicionando um filtro ou alterando os agrupamentos no gráfico.&quot;

### Responder

Esse erro significa que seu gráfico contém até 618 resultados distintos, por exemplo, mais de 618 barras em um gráfico de barras. Para resolver o problema de exibição, você precisa refinar os resultados modificando o filtro atual e agrupando as seleções.

Para obter informações sobre modificação de filtros e agrupamentos, consulte os artigos [Visão geral dos filtros](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md) e [Visão geral dos agrupamentos no Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

## Por que vejo minhas tarefas (ou problemas) quando acesso o mesmo relatório (ou calendário) que meu colega de trabalho e, em vez disso, eles veem suas tarefas?

### Responder

O relatório ou calendário pode ter uma variável de filtro curinga que aponta para o usuário que está conectado. Nesse caso, o relatório mostra informações com base no usuário que está conectado. Ajuste o filtro para remover o curinga que aponta para o usuário conectado.\
![Variável de filtro de ID de usuário](assets/qs--user.id-filter-variable-350x79.png)

Para obter uma lista completa de visão geral das variáveis de filtro Curinga com base no usuário, consulte [Visão geral das variáveis de filtro curinga](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).

## Por que os dados no meu relatório parecem incompletos?

### Responder

Isso pode acontecer na maioria dos casos se você tiver um acesso limitado que o impeça de ver itens no sistema. Além disso, os itens que você deseja ver não são compartilhados com você.

O criador do relatório pode editá-lo para executá-lo com os direitos de acesso de um administrador do sistema ou de qualquer usuário do Plano que tenha acesso para ver os dados.

Para obter mais informações, consulte [Executar e entregar um relatório com direitos de acesso de outro usuário](../../../reports-and-dashboards/reports/creating-and-managing-reports/run-deliver-report-access-rights-another-user.md).

## Como faço para relatar as tarefas (ou problemas) às quais estou atribuído, independentemente de ser o Proprietário delas ou não?

### Responder

Para ver todas as tarefas ou problemas atribuídos a você, seja você o Proprietário (ou o Designado Principal) ou não, use o filtro a seguir em um relatório de tarefas ou problemas:

1. Acessar um relatório de tarefas ou problemas.
1. Na guia **Filtros**, clique em **Adicionar uma Regra de Filtro**.

1. No campo **Comece a digitar o nome do campo ...**, comece a digitar **Nome de Usuários de Atribuição** e selecione-o quando ele aparecer na lista.

   >[!NOTE]
   >
   >Não use o campo **Atribuído a nome**, pois este filtro filtra somente as tarefas e problemas para os quais você é o Atribuído principal ou Proprietário.

1. Selecione o modificador **Equal**.
1. Comece digitando *$$USER.ID* na caixa de texto e selecione-o na lista suspensa exibida.\
   Isso garante que você veja todas as tarefas e problemas atribuídos ao usuário conectado. É possível substituir o curinga por um nome de usuário específico.\
   ![Tarefas atribuídas a mim](assets/qs-tasks-assigned-to-me-assignment-users-name-filter-350x63.png)

1. Clique em **Salvar + Fechar**.

## Por que os links Adicionar problemas/Adicionar tarefas não aparecem na parte inferior das minhas Listas de problemas e tarefas em um projeto?

### Responder

Primeiro, verifique se você tem o acesso e as permissões corretas para adicionar problemas e tarefas a um projeto. Nesse caso, você deve ver os links **Adicionar Problemas** e **Adicionar Tarefas** na parte inferior das listas **Problemas** e **Tarefas**.

No entanto, há algumas coisas que podem impedir a exibição desses links:

* Se você tiver o filtro rápido aplicado a essas listas, os links não serão exibidos. Remova o filtro rápido e os links devem ser exibidos para que você possa adicionar problemas e tarefas aos seus projetos.\
  Para obter informações sobre o filtro rápido, consulte [Introdução a listas no Adobe Workfront](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

* Se você tiver um **Agrupamento** aplicado a essas listas, os links não serão exibidos. Remova o **Agrupamento** e os links deverão ser exibidos para que você possa adicionar problemas e tarefas aos seus projetos.\
  Para obter informações sobre como criar Agrupamentos, consulte [Visão geral sobre Agrupamentos no Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

* Se você tiver uma **Exibição** aplicada a estas listas que tenha uma moeda selecionada diferente da moeda padrão para o projeto, os links não serão exibidos. Altere a **Exibição** para a **Moeda Original do Projeto** e os links deverão ser exibidos para que você possa adicionar problemas e tarefas aos seus projetos.\
  Para obter mais informações sobre como alterar a moeda na sua Exibição, consulte [Criar relatórios de dados financeiros com taxas de câmbio exclusivas](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-financial-data-reports-unique-exchange-rates.md).

![Moeda do projeto](assets/nwe-project-original-currency-350x229.png)

## As informações no meu relatório ou painel são atualizadas automaticamente?

### Responder

As informações nos relatórios ou painéis não são atualizadas automaticamente.

As informações podem ser atualizadas manualmente em um relatório em cache.\
Para obter mais informações sobre como atualizar um relatório em cache, consulte [Executar um relatório](../../../reports-and-dashboards/reports/creating-and-managing-reports/run-report.md).

As informações podem ser atualizadas manualmente em um painel armazenado em cache.\
Para obter mais informações sobre como atualizar um painel em cache, consulte a seção [Exibir painéis](../../../reports-and-dashboards/dashboards/understanding-dashboards/get-started-dashboards.md#running-dashboards) no artigo [Introdução aos painéis](../../../reports-and-dashboards/dashboards/understanding-dashboards/get-started-dashboards.md).

## Posso alterar o proprietário de um relatório?

### Responder

Você não pode alterar o proprietário de um relatório. No entanto, o usuário que criou o relatório pode permitir que outros usuários editem o relatório. A maneira de permitir que os usuários editem um relatório depende do tipo de usuário que você é.

* Os administradores de sistema podem permitir que usuários com uma licença de Plano editem relatórios configurando a opção Editar na linha Relatórios para incluir o acesso a Criar um relatório.\
  Para obter mais informações, consulte [Conceder acesso a relatórios, painéis e calendários](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md).

* Qualquer usuário final com acesso para criar e compartilhar relatórios pode permitir que outros editem relatórios individuais, compartilhando-os e dando a outros usuários permissões de gerenciamento para eles.\
  Para obter mais informações, consulte [Compartilhar um relatório no Adobe Workfront](../../../reports-and-dashboards/reports/creating-and-managing-reports/share-report.md).

Se você tiver permissões para exibir ou gerenciar um relatório, também poderá fazer uma cópia dele, da qual será o proprietário por padrão. Para saber mais sobre como copiar um relatório, consulte [Criar uma cópia de um relatório](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md).

## Por que não posso acessar um relatório de propriedade de um usuário desativado?

### Responder

Às vezes, o proprietário do relatório também é o usuário especificado no **Executar este relatório com o campo Direitos de Acesso de:** no relatório. Se o **Executar este relatório com os Direitos de Acesso de:** usuário estiver desativado, o relatório não será mais exibido para os usuários que têm o relatório compartilhado com eles. Quando isso acontecer, você poderá tornar o relatório acessível novamente deixando o **Executar este Relatório com os Direitos de Acesso de:** em branco ou inserindo um usuário ativo no campo.

Para saber mais sobre o **Executar este Relatório com o campo Direitos de Acesso de:**, consulte [Executar e entregar um relatório com os direitos de acesso de outro usuário](../../../reports-and-dashboards/reports/creating-and-managing-reports/run-deliver-report-access-rights-another-user.md). Para obter informações sobre como identificar todos os relatórios de propriedade de usuários desativados, consulte [Criar um relatório sobre atividades de relatório](../../../reports-and-dashboards/reports/report-usage/create-report-reporting-activities.md).

## Como faço para acessar um painel que contém um relatório de propriedade de um usuário excluído?

### Responder

Ao excluir um usuário, você ainda pode acessar todos os relatórios criados por ele. No entanto, todos os painéis que incluíram o relatório também são excluídos. Isso significa que não é mais possível acessar o seguinte:

* Um painel que contenha o relatório
* Uma seção personalizada que contém um painel do relatório

Para saber mais sobre as implicações da exclusão de um usuário, consulte [Excluir usuários](../../../administration-and-setup/add-users/create-and-manage-users/delete-a-user.md).

Se você tiver acesso de Visualização ao relatório, poderá fazer o seguinte:

1. Criar uma cópia do relatório.\
   Para saber como criar uma cópia de um relatório, consulte [Criar uma cópia de um relatório](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md).

1. Atualize o painel para incluir o relatório copiado.\
   Para aprender a editar um painel, consulte [Editar um painel](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/edit-dashboard.md).
