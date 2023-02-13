---
content-type: faq
product-area: reporting
navigation-topic: tips-tricks-and-troubleshooting-reports
title: Perguntas frequentes sobre relatórios
description: Perguntas frequentes sobre relatórios
author: Nolan
feature: Reports and Dashboards
exl-id: 5e267d45-7922-4c0f-8530-59a8c152f625
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '1502'
ht-degree: 0%

---

# Perguntas frequentes sobre relatórios

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina: ***This is the ONE anchor article for all FAQs about Reporting. Add a new FAQ in the TOC at the top first, then add the answer as a section at the bottom.)</p>
-->

As perguntas a seguir são frequentes sobre os relatórios.

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plano Adobe Workfront*</td> 
   <td> <p>Qualquer Um</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Plano, Trabalho</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a Relatórios, Painéis, Calendários</p> <p>Observação: Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões de um relatório</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

## Por que meu cálculo personalizado para uma diferença de hora não mostra o resultado correto em uma coluna?

Em um relatório de projeto, tenho um cálculo que subtrai Horas Reais (2) das Horas Planejadas (4). O resultado que estou recebendo é 120, quando deveria ser 2.\
Meu cálculo é:
<pre>valueexpression=SUB(workRequired,atualWorkRequired)</pre>

### Resposta

Os campos que usam horas no Workfront são armazenados em minutos. Ao usar o campo em um cálculo, o resultado será em minutos. Para obter o resultado em horas, você deve dividir o resultado do cálculo por 60.

O cálculo correto é:

<pre>valueexpression=SUB(workRequired,atualWorkRequired)/60</pre>

## Por que o valor de cada um dos meus elementos de gráfico em um relatório não é exibido no gráfico?

### Resposta

Se você tiver mais de 50 elementos de gráfico em um gráfico de relatório, o valor de cada elemento não será exibido no gráfico.

Quando você tem menos de 50 elementos em um gráfico, o valor de cada elemento é exibido no gráfico. Considere adicionar um filtro ou modificar os agrupamentos no relatório para limitar a quantidade de itens exibidos em cada elemento do gráfico.

## Por que meu relatório retorna muitos resultados para exibir o gráfico?

Quando executo um relatório com um gráfico, vejo a mensagem de erro &quot;Opa aí... Este relatório retornou MUITOS dados que tornam o gráfico ilegível. Considere restringir seus resultados adicionando um filtro ou alterando os agrupamentos no gráfico.&quot;

### Resposta

Esse erro significa que seu gráfico contém até 618 resultados distintos, por exemplo, mais de 618 barras em um gráfico de barras. Para resolver o problema de exibição, é necessário refinar os resultados modificando o filtro atual e as seleções de agrupamento.

Para obter informações sobre modificação de filtros e agrupamentos, consulte os artigos [Visão geral dos filtros no Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md) e [Visão geral dos agrupamentos no Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

## Por que vejo minhas tarefas (ou problemas) quando acesso o mesmo relatório (ou calendário) do meu colega de trabalho e elas veem suas tarefas em vez disso?

### Resposta

O relatório ou calendário pode ter uma variável de filtro curinga que aponta para o usuário que está conectado. Nesse caso, o relatório mostra informações com base no usuário que está conectado. Ajuste o filtro para remover o curinga que aponta para o usuário conectado.\
![](assets/qs--user.id-filter-variable-350x79.png)

Para obter uma lista completa de variáveis de filtros curingas baseadas em usuários, consulte [Variáveis de filtro curinga](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).

## Por que razão os dados do meu relatório parecem incompletos?

### Resposta

Isso pode acontecer na maioria dos casos se você tiver um acesso limitado que impede a visualização de itens no sistema. Além disso, os itens que deseja ver não são compartilhados com você.

O criador do relatório pode editar o relatório para executá-lo com os direitos de acesso de um administrador do sistema ou de qualquer usuário do Plano que tenha acesso para ver os dados.

Para obter mais informações, consulte [Executar e entregar um relatório com os direitos de acesso de outro usuário](../../../reports-and-dashboards/reports/creating-and-managing-reports/run-deliver-report-access-rights-another-user.md).

## Como faço para relatar sobre tarefas (ou problemas) às quais estou atribuído, seja Proprietário delas ou não?

### Resposta

Para ver todas as tarefas ou problemas atribuídos a você, seja o Proprietário (ou Destinatário Principal) ou não, use o seguinte filtro em um relatório de tarefa ou ocorrência:

1. Acesse uma tarefa ou um relatório de problemas.
1. No **Filtros** clique em **Adicionar uma regra de filtro**.

1. No **Começar a digitar o nome do campo ...** , comece a digitar **Nome dos usuários da atribuição** e, em seguida, selecione-a quando ela for exibida na lista.

   >[!NOTE]
   >
   >Não utilize o **Atribuído ao nome** , pois isso filtra somente para as tarefas e problemas para os quais você é o Destinatário Principal ou o Proprietário.

1. Selecione o **Igual** modificador.
1. Comece a digitar *$$USER.ID* na caixa de texto e selecione-a na lista suspensa exibida.\
   Isso garante que você veja todas as tarefas e problemas atribuídos ao usuário conectado. Você pode substituir o curinga por um nome de usuário específico.\
   ![](assets/qs-tasks-assigned-to-me-assignment-users-name-filter-350x63.png)

1. Clique em **Salvar + Fechar**.

## Por que os links Adicionar problemas/Adicionar tarefas não estão aparecendo na parte inferior das listas de Problemas e Tarefas em um projeto?

### Resposta

Primeiro, verifique se você tem o acesso e as permissões corretas para adicionar problemas e tarefas a um projeto. Nesse caso, você deve ver a variável **Adicionar problemas** e **Adicionar Tarefas** links na parte inferior da **Problemas** e **Tarefas** listas.

No entanto, há algumas coisas que podem impedir que esses links sejam exibidos:

* Se você tiver o filtro rápido aplicado a essas listas, os links não serão exibidos. Remova o filtro rápido e os links devem ser exibidos para que você possa adicionar problemas e tarefas aos seus projetos.\
   Para obter informações sobre o filtro rápido, consulte [Introdução a listas no Adobe Workfront](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

* Se você tiver uma **Agrupamento** aplicadas a essas listas, os links não são exibidos. Remova o **Agrupamento** e os links devem ser exibidos para que você possa adicionar problemas e tarefas aos seus projetos.\
   Para obter informações sobre como criar Agrupamentos, consulte [Visão geral dos agrupamentos no Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

* Se você tiver uma **Exibir** aplicados a essas listas que têm uma moeda selecionada diferente da moeda padrão do projeto, os links não são exibidos. Altere o **Exibir** para **Moeda original do projeto** e os links devem ser exibidos para que você possa adicionar problemas e tarefas aos seus projetos.\
   Para obter mais informações sobre como alterar a moeda na sua Exibição, consulte [Criar relatórios de dados financeiros com taxas de câmbio exclusivas](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-financial-data-reports-unique-exchange-rates.md).

![](assets/nwe-project-original-currency-350x229.png)

## As informações no meu relatório ou painel são atualizadas automaticamente?

### Resposta

As informações em relatórios ou painéis não são atualizadas automaticamente.

As informações podem ser atualizadas manualmente em um relatório em cache.\
Para obter mais informações sobre como atualizar um relatório em cache, consulte [Executar um relatório](../../../reports-and-dashboards/reports/creating-and-managing-reports/run-report.md).

As informações podem ser atualizadas manualmente em um painel em cache.\
Para obter mais informações sobre como atualizar um painel em cache, consulte a seção [Exibir painéis](../../../reports-and-dashboards/dashboards/understanding-dashboards/get-started-dashboards.md#running-dashboards) no artigo [Introdução aos painéis](../../../reports-and-dashboards/dashboards/understanding-dashboards/get-started-dashboards.md).

## Posso alterar o proprietário de um relatório?

### Resposta

Não é possível alterar o proprietário de um relatório. No entanto, o usuário que criou o relatório pode permitir que outros usuários editem o relatório. A maneira de permitir que os usuários editem um relatório depende do tipo de usuário que você está.

* Os administradores do sistema podem permitir que os usuários com uma licença do Plano editem os relatórios configurando a opção Editar na linha Relatórios para incluir o acesso a Criar um relatório.\
   Para obter mais informações, consulte [Conceder acesso a relatórios, painéis e calendários](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md).

* Qualquer usuário final com acesso para criar e compartilhar relatórios pode permitir que outros editem relatórios individuais ao compartilhá-los e conceder permissões de gerenciamento a outros usuários.\
   Para obter mais informações, consulte [Compartilhar um relatório no Adobe Workfront](../../../reports-and-dashboards/reports/creating-and-managing-reports/share-report.md).

Se você tiver permissões para visualizar ou gerenciar um relatório, também poderá fazer uma cópia do relatório, que será o proprietário por padrão. Para saber mais sobre como copiar um relatório, consulte [Criar uma cópia de um relatório](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md).

## Por que não consigo acessar um relatório de propriedade de um usuário desativado?

### Resposta

Às vezes, o proprietário do relatório também é o usuário especificado na variável **Execute este relatório com os Direitos de acesso de:** no relatório. Se a variável **Execute este relatório com os Direitos de acesso de:** estiver desativado, o relatório não será mais exibido para usuários que tenham o relatório compartilhado com eles. Quando isso acontece, é possível tornar o relatório acessível novamente deixando a variável **Execute este Relatório com os Direitos de Acesso de:** em branco ou inserir um usuário ativo no campo.

Para saber mais sobre o **Execute este Relatório com os Direitos de Acesso de:** , consulte [Executar e entregar um relatório com os direitos de acesso de outro usuário](../../../reports-and-dashboards/reports/creating-and-managing-reports/run-deliver-report-access-rights-another-user.md). Para obter informações sobre como identificar todos os relatórios de propriedade de usuários desativados, consulte [Criar um relatório sobre atividades de relatório](../../../reports-and-dashboards/reports/report-usage/create-report-reporting-activities.md).

## Como faço para acessar um painel que contém um relatório de propriedade de um usuário excluído?

### Resposta

Ao excluir um usuário, você ainda pode acessar qualquer relatório que ele tenha criado, no entanto, os painéis incluídos no relatório também são excluídos. Isso significa que você não pode mais acessar o seguinte:

* Um painel que contém o relatório
* Uma seção personalizada que contém um painel do relatório

Para saber mais sobre as implicações da exclusão de um usuário, consulte [Excluir usuários](../../../administration-and-setup/add-users/create-and-manage-users/delete-a-user.md).

Se você tiver o acesso de Exibição ao relatório, poderá fazer o seguinte:

1. Crie uma cópia do relatório.\
   Para saber como criar uma cópia de um relatório, consulte [Criar uma cópia de um relatório](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md).

1. Atualize o painel para incluir o relatório copiado.\
   Para saber como editar um painel, consulte [Editar um painel](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/edit-dashboard.md).
