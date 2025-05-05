---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Export Data
description: You can export Adobe Workfront data from lists, reports, dashboards, and searches.
author: Nolan
feature: Reports and Dashboards
exl-id: 7fd45fa2-f5d2-411d-849e-cff5be420fbc
source-git-commit: ae3fc73e93474c75fd03144b66af23f7142867c0
workflow-type: tm+mt
source-wordcount: '2264'
ht-degree: 0%

---

# Exportar dados

<!-- Audited: 5/2025 -->

You can export Adobe Workfront data from lists, reports, dashboards, and searches.

Alguns motivos para exportar dados são:

* Você deseja fornecer uma cópia dos dados em papel a alguém fora do Workfront.
* Você deseja enviar os resultados de um relatório como um anexo para um usuário externo.
* Você deseja criar um backup externo dos dados do Workfront.
* Há um limite para exibir apenas 2.000 resultados em uma página dentro do aplicativo web do Workfront. If your report produces more than 2,000, you can export the report to any of the available formats and view all the results in the report in one list.

You can either export a report manually, from the Workfront interface, or you can schedule a delivery for a report and that report will be sent to you at a later time. Para obter mais informações sobre o agendamento de relatórios entregues, consulte [Visão geral da entrega de relatórios](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

As informações deste artigo não se aplicam às seguintes exportações:

* Exportar informações de relatórios de gráficos.

  Para obter mais informações sobre como exportar um relatório de gráfico, consulte [Adicionar um gráfico a um relatório](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md).

* Exportando informações do gráfico de Gantt.

  Para obter mais informações sobre como exportar o Gráfico de Gantt, consulte [Exportar o Gráfico de Gantt para o PDF](../../../manage-work/gantt-chart/use-the-gantt-chart/export-gantt-chart-to-pdf.md).

* Exportando informações do Planejador de recursos.

  Para obter mais informações sobre como exportar as informações do Planejador de recursos, consulte &quot;Opção de exportação&quot; na [Visão geral da navegação do Planejador de recursos](../../../resource-mgmt/resource-planning/resource-planner-navigation.md).

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

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
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td>
    <p>Novo:</p>
      <ul>
      <li>Leve ou superior</li>
      </ul>
    <p>Atual:</p>
      <ul>
      <li>Revisar ou superior</li>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>View or higher access to Reports, Dashboards, and Calendars to export reports</p> <p>View or higher access to the objects you view in a list to export the list</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Visualize ou aumente as permissões de um relatório ou painel para exportar o relatório ou painel</p> <p>Permissões de visualização ou superiores para os objetos que você visualiza em uma lista para exportar a lista</p> </td> 
  </tr> 
 </tbody> 
</table>

*Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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
>Dashboards can either be printed or exported only to a PDF file.

### Export limits {#export-limits}

<!--
NOTE: Alina: [! This information is shared between "Exporting Data" and "Setting Up Report Deliveries."]
-->

There are several limitations around the way reports display in Workfront as well as the way they export through a manual export, a delivered report, or through the API.

* **50.000 células:** o número máximo de células permitidas em uma exportação de relatório para arquivos do Excel.
* **50.000 linhas:** o número de linhas de dados permitidas em uma exportação de relatório para arquivos PDF e Delimitados por tabulação.

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

  For information about using prompts, see [Add a prompt to a report](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

* Estes limites aplicam-se a:

   * A manual export of a report.
   * A scheduled report.
   * An export through an API integration.
   * Dados exportados por meio de um início.

     Para obter mais informações sobre como exportar dados por meio de inícios, consulte [Exportar dados do Adobe Workfront por meio de Inícios](../../../administration-and-setup/manage-workfront/using-kick-starts/export-data-from-wf-via-kick-starts.md).

     >[!NOTE]
     >
     >É possível exportar 50.000 linhas em um arquivo de início rápido, embora seja possível exportar os dados somente para um arquivo em formato Excel.

   * Exportando informações de utilização de um projeto.

     For more information about exporting utilization information for a project, see [Overview of the Resource Utilization report](../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md#exporting-utilization-information-for-a-project).

* **10MB file size:** File size limit for any exported report scheduled for delivery. If an exported file attached to an email is larger than 5MB, a link where the file can be downloaded is emailed instead of the attached exported report.
* **65.530 hiperlinks:** esse é um limite imposto pelo Excel a documentos que contêm mais de 65.530 hiperlinks. Esses documentos não podem ser abertos quando são exportados manualmente ou enviados em um relatório entregue. Observe que um documento do Excel pode ter apenas 200 linhas de dados, mas se houver mais de 65.530 links dentro do documento, ele não abrirá. Esse limite existe apenas em arquivos do Excel e não em outros formatos compatíveis.
* **256 colunas**: esse é um limite imposto pelo Excel a documentos que contêm mais de 256 colunas. Esses documentos não podem ser exportados manualmente ou enviados em um relatório entregue. Esse limite existe apenas em arquivos do Excel e não em outros formatos compatíveis.

  >[!IMPORTANT]
  >
  >A exportação de um relatório que inclui uma coluna Relatórios pode resultar em erro, mesmo que o relatório esteja dentro dos limites de exportação listados.
  >
  >Se você estiver usando o recurso de exportação para compartilhar um relatório contendo uma coluna Relatórios com outras pessoas, considere compartilhar o relatório tornando-o público. Para obter mais informações sobre como tornar um relatório público, consulte [Compartilhar um relatório no Adobe Workfront](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/share-report.md).
  >
  >Se você estiver usando o recurso de exportação para avaliar dados externamente, recomendamos usar o Workfront Data Connect. Para obter mais informações, consulte [visão geral do Workfront Data Connect](/help/quicksilver/reports-and-dashboards/data-lake/data-lake-overview.md).

Se você tentar exportar dados além do limite, talvez não receba todos os dados esperados na exportação. Em vez disso, um relatório modificado é produzido dentro do limite.

Além disso, os relatórios que levarem mais de 60 minutos para serem executados serão interrompidos.

If you have concerns or issues regarding your limit, please contact Workfront Technical Support.

## Exportar dados

### Exportar dados de um relatório ou lista {#export-data-from-a-report-or-list}

1. Vá para o relatório ou lista que deseja exportar.
1. Selecione os itens que deseja exportar. Selecionar itens individuais exporta somente os itens selecionados.

   For example, in a project, select the tasks you want to export.

   Ou

   Leave all items deselected to export the entire list.

1. Click **Export**, then select a format.

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

* [File names](#file-names)
* [Titles](#titles)
* [Timestamps](#timestamps)
* [Formatting](#formatting)
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

   * **The_project_name_the_task_name_Exported_Tasks**(*in PDF, Excel, Excel (.xlsx), or Tab delimited formats)*
   * **The_project_name_the_task_name_Exported_Issues**(*in PDF, Excel, Excel (.xlsx), or Tab delimited formats)*

When you export a list of any other objects from a project to a PDF file, the file name of the exported document indicates the type of objects you exported.\
For example, the file name may be:

* *Usuários_Exportados*, ao exportar a guia Pessoas no projeto(*nos formatos PDF, Excel, Excel (.xlsx) ou delimitado por tabulação)*
* *Exported_Risks*, ao exportar uma lista de Riscos no projeto(*nos formatos PDF, Excel, Excel (.xlsx) ou delimitado por tabulação)*

#### Nomes de arquivos para relatórios exportados {#file-names-for-exported-reports}

Quando você exporta um relatório, o nome do arquivo do relatório exportado é:

*The_report_name*(*nos formatos PDF, Excel, Excel (.xlsx) ou delimitado por tabulação)*

### Titles {#titles}

When you export a list of objects, only the file in the PDF format will have a title. If you export a list or a report to Excel, Excel (.xlsx), or Tab Delimited formats, the file does not have a title.

#### Títulos para listas exportadas {#titles-for-exported-lists}

Quando você exporta listas de tarefas e problemas em um projeto para um arquivo PDF, o título do documento exportado é um dos seguintes:

* *Nome do projeto - Tarefas Exportadas*
* *Nome do projeto - Problemas Exportados*

Quando você exporta listas de tarefas e problemas em uma tarefa para um arquivo PDF, o bloco do documento exportado é um dos seguintes:

* *Nome do projeto - Nome da tarefa - Tarefas exportadas*
* *Nome do projeto - Nome da tarefa - Problemas exportados*

Quando você exporta uma lista de quaisquer outros objetos de um projeto para um arquivo do PDF, o título do documento exportado indica o tipo de objetos que você exportou.\
Por exemplo, o título pode ser:

* *Usuários Exportados*, ao exportar a guia Pessoas no projeto.
* *Riscos Exportados*, ao exportar uma lista de Riscos no projeto.

#### Titles for exported reports {#titles-for-exported-reports}

A report that is exported to a PDF file will have a title.

Se o relatório for exportado para os formatos Excel, Excel (.xlsx) ou Delimitado por tabulação, o relatório exportado não terá um título. O título do arquivo exportado é o nome do relatório como ele aparece no aplicativo web do Workfront.

Se o relatório tiver uma descrição, ela será incluída no arquivo exportado.

### Carimbos de data e hora {#timestamps}

A timestamp is displayed on the exported document from the context of the user who exported the item.

O carimbo de data e hora inclui:

* Data
* Hora
* Fuso horário quando o item foi exportado

Dependendo do tipo de documento exportado, os carimbos de data e hora são exibidos em vários locais:

* **PDF:** Os carimbos de data e hora são exibidos no rodapé de cada página e no nome do arquivo.
* **Excel:** Os carimbos de data/hora são exibidos no nome do arquivo.

### Formatação {#formatting}

Quando você exporta um projeto para o PDF, todas as subtarefas são exibidas como recuadas para suas tarefas pai. As listas exportadas não recolhem nenhuma tarefa pai.

Você sempre recebe a guia padrão de um relatório quando ele é enviado ou agendado para um delivery, a menos que o relatório tenha uma visualização especial.

Se o relatório tiver formatação especial no aplicativo web, ele deverá ser entregue com a formatação especial quando as guias Details e Matrix forem entregues, somente para arquivos PDF e Excel.

>[!NOTE]
>
>Se os dados exportados contiverem colunas compartilhadas e você exportar para um formato Excel ou Delimitado por tabulação, essas colunas serão separadas no arquivo exportado.

Para obter mais informações sobre como personalizar a formatação em um relatório, consulte [Usar formatação condicional nos modos de exibição](../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md).

### Links {#links}

Os links podem apontar para qualquer objeto no Workfront que ofereça suporte a links. When you export a list in Workfront to PDF, any supported links that exist in the original document remain live in the exported document.

>[!TIP]
>
>If the line `valueformat=HTML` appears in text mode for a custom field column and the link values do not display in an exported PDF file, you need to enter additional lines of code to your column in text mode.
>
>For example, if you have a custom field called Open Q1 Projects that contains links, you would add the following code:
>
>`link.url=customDataLabelsAsString(Open Q1 Projects)`
>`linkedname=direct`

When you export to an Excel format, only links to objects within Workfront are included in the exported file and they are only supported in places where you can select to allow links in exported Excel documents, such as report deliveries.

## Marca {#branding}

>[!IMPORTANT]
>
>Branding applies only to organizations that are not yet onboarded to Adobe Experience Cloud.
>
>Se sua organização foi integrada ao Adobe Experience Cloud, a marca não está disponível.

Se o administrador do Workfront tiver adicionado uma marca personalizada à sua instância do Workfront para a Barra de navegação global, os arquivos exportados do PDF também incluirão seu logotipo personalizado.

Os dados exportados em qualquer outro formato não podem ser personalizados com o logotipo.

Para obter mais informações sobre como marcar sua instância do Workfront e a Barra de Navegação Global, consulte [Marcar sua instância do Adobe Workfront](../../../administration-and-setup/customize-workfront/brand-workfront/brand-your-workfront-instance.md).
