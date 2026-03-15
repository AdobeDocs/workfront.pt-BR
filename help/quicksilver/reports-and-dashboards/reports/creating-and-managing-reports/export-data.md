---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Exportar dados
description: Você pode exportar dados do Adobe Workfront de listas, relatórios, painéis e pesquisas.
author: Courtney
feature: Reports and Dashboards
exl-id: 7fd45fa2-f5d2-411d-849e-cff5be420fbc
source-git-commit: 6a6d3d47ed5741e3202c44b7240a2e67b687ea95
workflow-type: tm+mt
source-wordcount: '2252'
ht-degree: 2%

---

# Exportar dados

<!-- Audited: 5/2025 -->

Você pode exportar dados do Adobe Workfront de listas, relatórios, painéis e pesquisas.

Alguns dos motivos para exportar dados são:

* Você deseja fornecer uma cópia impressa dos seus dados para alguém fora do Workfront.
* Você deseja enviar os resultados de um relatório como um anexo para um usuário externo.
* Você deseja criar um backup externo dos dados do Workfront.
* Há um limite para exibir apenas 2.000 resultados em uma página dentro do aplicativo web do Workfront. Se o seu relatório produzir mais de 2.000, você poderá exportá-lo para qualquer um dos formatos disponíveis e exibir todos os resultados em uma lista.

Você pode exportar um relatório manualmente, pela interface do Workfront, ou pode agendar uma entrega para um relatório e ele será enviado a você posteriormente. Para obter mais informações sobre o agendamento de relatórios entregues, consulte [Visão geral da entrega de relatórios](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

As informações neste artigo não se aplicam às seguintes exportações:

* Exportando informações de relatórios de gráficos.

  Para obter mais informações sobre como exportar um relatório de gráfico, consulte [Adicionar um gráfico a um relatório](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md).

* Exportando informações do gráfico de Gantt.

  Para obter mais informações sobre como exportar o Gráfico de Gantt, consulte [Exportar o Gráfico de Gantt para o PDF](../../../manage-work/gantt-chart/use-the-gantt-chart/export-gantt-chart-to-pdf.md).

* Exportando informações do Planejador de Recursos.

  Para obter mais informações sobre como exportar as informações do Planejador de Recursos, consulte “Opção de Exportação” em [Visão geral de navegação do Planejador de Recursos](../../../resource-mgmt/resource-planning/resource-planner-navigation.md).

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacote do Adobe Workfront</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td> 
      <p>Leve</p>
      <p>Revisar</p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Visualize ou acesse mais relatórios, painéis e calendários para exportar relatórios</p> <p>Acesso de visualização ou superior aos objetos exibidos em uma lista para exportar a lista</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Visualize ou aumente as permissões de um relatório ou painel para exportar o relatório ou painel</p> <p>Permissões de visualização ou superiores para os objetos que você visualiza em uma lista para exportar a lista</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações contidas nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Pré-requisitos

O relatório deve ser criado antes que você possa exportar seus dados.

Para obter mais informações sobre como criar relatórios, consulte [Criar um relatório personalizado](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md) ou [Criar uma cópia de um relatório](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md).

## Exportar formatos e limites

### Formatos de exportação {#export-formats}

As informações podem ser exportadas nos seguintes formatos:

* PDF (paisagem ou retrato)
* Excel
* Excel (.xlsx)
* Delimitado por tabulação

>[!NOTE]
>
>Painéis podem ser impressos ou exportados somente para um arquivo do PDF.

### Limites de exportação {#export-limits}

<!--
NOTE: Alina: [! This information is shared between "Exporting Data" and "Setting Up Report Deliveries."]
-->

Há várias limitações em relação à maneira como os relatórios são exibidos no Workfront, bem como à maneira como eles são exportados por meio de uma exportação manual, um relatório entregue ou por meio da API.

* **50.000 células:** o número máximo de células permitidas em uma exportação de relatório para arquivos do Excel.
* **50.000 linhas:** o número de linhas de dados permitidas em uma exportação de relatório para arquivos Delimitados por PDF e Tabulação.

   * Para arquivos do Excel, esse limite é de **65.000 linhas**.
   * Para arquivos do Excel(.xlsx), esse limite é de **100.000 linhas**.
   * Esses limites excluem os cabeçalhos da coluna, bem como linhas para agrupamentos no relatório. Por exemplo, se você tiver seis agrupamentos em um relatório e 50.000 linhas de dados, o arquivo exportado terá 50.000 linhas.

  >[!IMPORTANT]
  >
  >A exportação de um relatório que inclui uma referência de coleção em uma coluna pode resultar em erro, mesmo que o relatório esteja dentro dos limites de exportação listados. Se a coleção referenciada for muito grande, o processo de exportação expirará e resultará em um erro.
  >
  >Para evitar esse erro, exclua as colunas que fazem referência a coleções grandes ou reduza o tamanho das coleções referenciadas antes da exportação.

  Se o relatório tiver mais itens do que esses limites, você receberá um erro de que a exportação não foi bem-sucedida. Reduza o número de itens que você vê na tela para um número menor ou igual a esses limites para poder exportar os resultados.

  Se seu relatório tiver mais de 50.000/ 65.000/ 100.000 linhas e você quiser exportar todos os dados, sugerimos que você use filtros ou prompts para obter cargas menores de dados e executar várias exportações.

  Para obter informações sobre como usar filtros, consulte [Visão geral dos filtros](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

  Para obter informações sobre como usar prompts, consulte [Adicionar um prompt a um relatório](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

* Estes limites aplicam-se a:

   * Uma exportação manual de um relatório.
   * Um relatório agendado.
   * Uma exportação por meio de uma integração de API.
   * Dados exportados por meio de um kick-start.

     Para obter mais informações sobre como exportar dados via inícios, consulte [Exportar dados do Adobe Workfront via inícios de primeiros passos](../../../administration-and-setup/manage-workfront/using-kick-starts/export-data-from-wf-via-kick-starts.md).

     >[!NOTE]
     >
     >Você pode exportar 50.000 linhas em um arquivo de início rápido, embora seja possível exportar os dados somente para um arquivo em formato Excel.

   * Exportando informações de utilização de um projeto.

     Para obter mais informações sobre como exportar informações de utilização de um projeto, consulte [Visão geral do relatório de Utilização de Recursos](../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md#exporting-utilization-information-for-a-project).

* **Tamanho de arquivo de 10 MB:** limite de tamanho de arquivo para qualquer relatório exportado agendado para entrega. Se um arquivo exportado anexado a um email tiver mais de 5 MB, um link no qual o arquivo pode ser baixado será enviado por email em vez do relatório exportado anexado.
* **65.530 hiperlinks:** esse é um limite imposto pelo Excel em documentos que contêm mais de 65.530 hiperlinks. Esses documentos não podem ser abertos quando são exportados manualmente ou enviados em um relatório entregue. Observe que um documento do Excel pode ter apenas 200 linhas de dados, mas se houver mais de 65.530 links dentro do documento, ele não será aberto. Esse limite existe apenas em arquivos do Excel, e não em outros formatos compatíveis.
* **256 colunas**: este é um limite imposto pelo Excel em documentos que contêm mais de 256 colunas. Esses documentos não podem ser exportados manualmente nem enviados em um relatório entregue. Esse limite existe apenas em arquivos do Excel, e não em outros formatos compatíveis.

  >[!IMPORTANT]
  >
  >Exportar um relatório que inclua uma coluna Relatórios pode resultar em um erro, mesmo que o relatório esteja dentro dos limites de exportação listados.
  >
  >Se você estiver usando o recurso de exportação para compartilhar com outras pessoas um relatório contendo uma coluna Relatórios, considere compartilhar o relatório tornando-o público. Para obter mais informações sobre como tornar um relatório público, consulte [Compartilhar um relatório no Adobe Workfront](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/share-report.md).
  >
  >Se você estiver usando o recurso de exportação para avaliar dados externamente, recomendamos usar o Workfront Data Connect. Para obter mais informações, consulte [visão geral do Workfront Data Connect](/help/quicksilver/reports-and-dashboards/data-lake/data-lake-overview.md).

Se você tentar exportar dados além do limite, talvez não receba todos os dados esperados na exportação. Em vez disso, um relatório modificado é produzido dentro do limite.

Além disso, os relatórios que levarem mais de 60 minutos para serem executados serão interrompidos.

Se você tiver dúvidas ou problemas relacionados ao seu limite, entre em contato com o Suporte Técnico da Workfront.

## Exportar dados

### Exportar dados de um relatório ou lista {#export-data-from-a-report-or-list}

1. Vá para o relatório ou lista que deseja exportar.
1. Selecione os itens que deseja exportar. Selecionar itens individuais exporta somente os itens selecionados.

   Por exemplo, em um projeto, selecione as tarefas que deseja exportar.

   Ou

   Deixe todos os itens desmarcados para exportar toda a lista.

1. Clique em **Exportar** e selecione um formato.

   <!--
   This note doesn't seem to be true (I tested with e reviewer and they could export the dashboard and its reports), and there's another article all about exporting dashboards. Lisa 12/23
   >[!NOTE]
   >
   >To export a Dashboard report, you must have a Plan license.  
   >![Export dashboard note](assets/nwe-dashboard-export-note-350x271.png)
   -->

   Ou

   Clique no ícone **Exportar** ![Ícone Exportar](assets/export-icon-nwe.png) e selecione um formato.

   As opções disponíveis para você exportar o PDF dependem das configurações de Local de email nas configurações de usuário do Workfront:

   * América do Norte - Carta - Paisagem, Carta - Retrato, Outros Tamanhos

   * Todos os locais fora da América do Norte - A4 - Paisagem, A4 - Retrato, Outros Tamanhos

1. (Condicional) Dependendo do sistema operacional usado, talvez você tenha a opção de abrir ou salvar o arquivo. Abra o arquivo com o aplicativo associado ou salve-o no disco rígido.
1. Para entender como as informações são exibidas no arquivo exportado, continue lendo a seção [Usar o documento exportado](#use-the-exported-document) neste artigo.

### Exportar dados de um painel {#export-data-from-a-dashboard}

Você pode imprimir as informações de um painel ou exportá-las como um arquivo do PDF.

Para obter mais informações sobre como exportar dados de um painel, consulte [Exportar um painel](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/export-dashboard.md).

## Usar o documento exportado {#use-the-exported-document}

As seções a seguir descrevem como as informações são exibidas em um arquivo exportado:

* [Nomes de arquivos](#file-names)
* [Títulos](#titles)
* [Carimbos de data/hora](#timestamps)
* [Formatação](#formatting)
* [Links](#links)
* [Marca](#branding)

### Nomes de arquivos {#file-names}

Se você exportar uma lista de objetos ou um relatório, seu arquivo exportado terá um nome de arquivo e um título. É possível encontrar o arquivo exportado em seu computador referindo-se ao nome do arquivo. O título do relatório fornecerá aos usuários uma indicação do que o arquivo exportado representa ao compartilhá-lo com eles.

#### Nomes de arquivo para listas exportadas {#file-names-for-exported-lists}

Quando você exporta uma lista de objetos, o tipo do objeto é exibido no arquivo exportado no nome do arquivo e no título da lista.

Quando você exporta uma lista de tarefas ou problemas, o **Nome do Arquivo** pode ser um dos seguintes:

* Ao exportar listas de tarefas e problemas em um projeto:

   * *The_project_name_Exported_Tasks*(*nos formatos PDF, Excel, Excel (.xlsx) ou delimitado por tabulação)*
   * *The_project_name_Exported_Issues*(*nos formatos PDF, Excel, Excel (.xlsx) ou delimitado por tabulação)*

* Ao exportar listas de tarefas e problemas em uma tarefa (subtarefas):

   * **The_project_name_the_task_name_Exported_Tasks**(*nos formatos PDF, Excel, Excel (.xlsx) ou delimitado por tabulação)*
   * **The_project_name_the_task_name_Exported_Issues**(*nos formatos PDF, Excel, Excel (.xlsx) ou delimitado por tabulação)*

Quando você exporta uma lista de quaisquer outros objetos de um projeto para um arquivo PDF, o nome do arquivo do documento exportado indica o tipo de objetos que você exportou.\
Por exemplo, o nome do arquivo pode ser:

* *Usuários_Exportados*, ao exportar a guia Pessoas no projeto(*em formatos delimitados por PDF, Excel, Excel (.xlsx) ou tabulação)*
* *Riscos_Exportados*, ao exportar uma lista de Riscos no projeto(*em formatos delimitados por PDF, Excel, Excel (.xlsx) ou tabulação)*

#### Nomes de arquivos para relatórios exportados {#file-names-for-exported-reports}

Ao exportar um relatório, o nome de arquivo do relatório exportado é:

*The_report_name*(*em formatos delimitados por PDF, Excel, Excel (.xlsx) ou tabulação)*

### Títulos {#titles}

Ao exportar uma lista de objetos, somente o arquivo no formato PDF terá um título. Se você exportar uma lista ou um relatório para os formatos Excel, Excel (.xlsx) ou Tabulação delimitada, o arquivo não tem um título.

#### Títulos para listas exportadas {#titles-for-exported-lists}

Ao exportar listas de tarefas e de ocorrências de um projeto para um arquivo PDF, o título do documento exportado será um dos seguintes:

* *Nome do projeto - Tarefas Exportadas*
* *Nome do projeto - Problemas Exportados*

Quando você exporta listas de tarefas e de ocorrências de uma tarefa para um arquivo PDF, o bloco do documento exportado é um dos seguintes:

* *Nome do projeto - Nome da Tarefa - Tarefas Exportadas*
* *Nome do projeto - Nome da tarefa - Problemas exportados*

Quando você exporta uma lista de quaisquer outros objetos de um projeto para um arquivo do PDF, o título do documento exportado indica o tipo de objetos que você exportou.\
Por exemplo, o título pode ser:

* *Usuários Exportados*, ao exportar a guia Pessoas no projeto.
* *Riscos Exportados*, ao exportar uma lista de Riscos no projeto.

#### Títulos para relatórios exportados {#titles-for-exported-reports}

Um relatório que é exportado para um arquivo PDF terá um título.

Se o relatório for exportado para os formatos Excel, Excel (.xlsx) ou Delimitado por tabulação, o relatório exportado não terá um título. O título do arquivo exportado é o nome do relatório como ele aparece no aplicativo web do Workfront.

Se o relatório tiver uma descrição, ela será incluída no arquivo exportado.

### Carimbos de data e hora {#timestamps}

Um carimbo de data e hora é exibido no documento exportado do contexto do usuário que exportou o item.

O carimbo de data e hora inclui:

* Data
* Hora
* Fuso horário de exportação do item

Dependendo do tipo de documento exportado, as marcas de data/hora são exibidas em vários locais:

* **PDF:** carimbos de data/hora são exibidos no rodapé de cada página e no nome do arquivo.
* **Excel:** Os carimbos de data/hora são exibidos no nome do arquivo.

### Formatação {#formatting}

Quando você exporta um projeto para o PDF, todas as subtarefas são exibidas como recuadas para suas tarefas pai. As listas exportadas não recolhem nenhuma tarefa principal.

Você sempre recebe a guia padrão de um relatório quando um relatório é enviado ou programado para uma entrega, a menos que o relatório tenha uma exibição especial.

Se o relatório tiver uma formatação especial no aplicativo da Web, ele deverá ser entregue com a formatação especial quando as guias Detalhes e Matriz forem fornecidas, somente para arquivos PDF e Excel.

>[!NOTE]
>
>Se os dados que você está exportando contiverem colunas compartilhadas e você exportar para um formato Excel ou Delimitado por tabulação, essas colunas serão separadas no arquivo exportado.

Para obter mais informações sobre como personalizar a formatação em um relatório, consulte [Usar formatação condicional em exibições](../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md).

### Links {#links}

Os links podem apontar para qualquer objeto no Workfront que ofereça suporte a links. Quando você exporta uma lista no Workfront para o PDF, todos os links compatíveis existentes no documento original permanecem ativos no documento exportado.

>[!TIP]
>
>Se a linha `valueformat=HTML` aparecer no modo de texto para uma coluna de campo personalizado e os valores de link não forem exibidos em um arquivo do PDF exportado, você precisará inserir linhas adicionais de código na coluna no modo de texto.
>
>Por exemplo, se você tem um campo personalizado chamado Abrir projetos Q1 que contém links, você adicionaria o seguinte código:
>
>`link.url=customDataLabelsAsString(Open Q1 Projects)`
>`linkedname=direct`

Quando você exporta para um formato do Excel, somente os links para objetos no Workfront são incluídos no arquivo exportado e só são suportados em locais onde você pode selecionar para permitir links em documentos exportados do Excel, como deliveries de relatórios.

## Marca {#branding}

>[!IMPORTANT]
>
>A marca se aplica somente a organizações que ainda não estão integradas ao Adobe Experience Cloud.
>
>Se sua organização foi integrada ao Adobe Experience Cloud, a marca não está disponível.

Se o administrador do Workfront tiver adicionado uma marca personalizada à sua instância do Workfront para a Barra de navegação global, os arquivos exportados do PDF também incluirão seu logotipo personalizado.

Os dados exportados em qualquer outro formato não podem ser personalizados com o logotipo.

Para obter mais informações sobre como marcar sua instância do Workfront e a Barra de Navegação Global, consulte [Marcar sua instância do Adobe Workfront](../../../administration-and-setup/customize-workfront/brand-workfront/brand-your-workfront-instance.md).
