---
product-area: reporting;setup
navigation-topic: create-and-manage-reports
title: Visão geral da entrega de relatórios
description: Visão geral da entrega de relatórios
author: Nolan
feature: Reports and Dashboards
exl-id: 1637df59-ca1d-4cf6-b83d-2b27936cdb96
source-git-commit: 548e713700fda79070f59f3dc3457410d2c50133
workflow-type: tm+mt
source-wordcount: '1532'
ht-degree: 0%

---

# Visão geral da entrega de relatórios

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: This is linked to the UI in the Send Report box inside the Preview sandbox. If you change title, log bug for Dev to fix the link) </p>
-->

Você pode agendar relatórios para que sejam entregues automaticamente aos usuários em um agendamento definido ou pode enviar relatórios de uma só vez, manualmente. Ao enviar um relatório do Adobe Workfront, o usuário recebe um email com o relatório do Workfront em um anexo separado.

Para obter informações sobre como configurar um relatório para entrega, consulte o artigo [Programar uma entrega automática de relatório](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-automatic-report-delivery.md).

Não é possível agendar relatórios para entrega nem entregá-los manualmente no ambiente Visualização da sandbox. Para obter mais informações sobre a Visualização da sandbox, consulte o artigo [O ambiente de sandbox de visualização do Adobe Workfront](../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md).\
Para obter mais informações sobre como fornecer relatórios no ambiente Visualização da sandbox, consulte o artigo [Enviar um relatório no ambiente Visualização da sandbox](../../../reports-and-dashboards/reports/creating-and-managing-reports/send-report-preview-sandbox-environment.md).

## Limites de entrega de relatório

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: [! This information is shared between "Exporting Data" and "Setting Up Report Deliveries."])</p>
-->

Considere o seguinte ao agendar relatórios para entrega:

* Você pode agendar até 10 entregas de relatório repetitivo para qualquer relatório.
* Você pode programar um relatório para ser entregue somente se for o criador do relatório. Se precisar enviar um relatório que não foi criado, é possível enviá-lo manualmente.

## Exportar limites

Há vários limites de tamanho que afetam como os relatórios são exibidos no Workfront e como são exportados por meio de uma exportação manual, um relatório entregue ou pela API:

* **Tamanho do arquivo de 5 MB:** Limite de tamanho de arquivo para qualquer relatório exportado agendado para entrega. Se um arquivo exportado anexado a um email tiver mais de 5 MB, um link no qual o arquivo pode ser baixado será enviado por email, em vez do relatório exportado anexado. 

  >[!NOTE]
  >
  >Arquivos .xlsx do Excel com mais de 5 MB não geram um email. É possível exportar manualmente o relatório para esse formato. Para obter informações sobre a exportação de relatórios, consulte [Exportar dados](../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md).

* **50.000 linhas:** O número de linhas de dados permitidas em uma exportação de relatório para arquivos .pdf e Delimitados por tabulação.

  Para arquivos .xls do Excel, esse limite é **65.000 linhas**.

  Para arquivos .xlsx do Excel, esse limite é **100.000 linhas**.

  Esses limites excluem os cabeçalhos da coluna, bem como linhas para agrupamentos no relatório. Por exemplo, se você tiver seis agrupamentos em um relatório e 50.000 linhas de dados, o arquivo exportado terá 50.000 linhas.

  Se o seu relatório tiver mais itens do que esses limites, você receberá um erro de que a exportação e a entrega do relatório não foram bem-sucedidas. Reduza o número de itens que você vê na tela para um número menor ou igual a esses limites para poder fornecer os resultados. Se quiser exportar todos os dados, sugerimos que você use filtros para obter cargas menores de dados e, em seguida, execute várias exportações. Para obter mais informações, consulte [Visão geral dos filtros](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

  Estes limites aplicam-se a:

   * Uma exportação manual de um relatório.
   * Um relatório agendado.
   * Uma exportação por meio de uma integração de API.
   * Dados exportados por meio de um início.

     Para obter mais informações sobre como exportar dados por meio de kick-starts, consulte o artigo [Exportar dados do Adobe Workfront via Kick-Starts](../../../administration-and-setup/manage-workfront/using-kick-starts/export-data-from-wf-via-kick-starts.md).

     >[!NOTE]
     >
     Você pode exportar 50.000 linhas em um arquivo de início rápido, mas somente para um arquivo em formato Excel. 

   * Exportando informações de utilização de um projeto.

     Para obter mais informações sobre a exportação de informações de utilização de um projeto, consulte [Visão Geral do relatório de Utilização de Recursos](../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md).

* **65.530 hiperlinks:** Esse é um limite imposto pelo Excel a documentos que contêm mais de 65.530 hiperlinks. Esses documentos não podem ser abertos quando são exportados manualmente ou enviados em um relatório entregue. Observe que um documento do Excel pode ter apenas 200 linhas de dados, mas se houver mais de 65.530 links dentro do documento, ele não abrirá. Esse limite existe apenas em arquivos do Excel e não em outros formatos compatíveis. 
* **256 colunas**: esse é um limite imposto pelo Excel a documentos que contêm mais de 256 colunas. Esses documentos não podem ser exportados manualmente ou enviados em um relatório entregue. Esse limite existe apenas em arquivos do Excel e não em outros formatos compatíveis. 

Se você tentar exportar dados além do limite, talvez não receba todos os dados esperados na exportação. Em vez disso, um relatório modificado é produzido dentro do limite. 

Além disso, os relatórios que levarem mais de 60 minutos para serem executados serão interrompidos.

Se você tiver dúvidas ou problemas relacionados ao seu limite, entre em contato com o Suporte técnico da Workfront.

## Entender os carimbos de data e hora em relatórios entregues

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Note about if this is delivered at a time based on the user's time zone settings?)</p>
-->

Ao receber um relatório em um email, o carimbo de data e hora e o formato de hora no relatório podem não corresponder aos do Workfront, caso você visualize o relatório no Workfront ao mesmo tempo em que foi entregue. 

Considere o seguinte: 

* Ao visualizar um relatório no navegador, o carimbo de data e hora e o formato no relatório correspondem à localidade e ao fuso horário do seu navegador, conforme definido nas configurações do seu navegador.
* Quando o relatório é entregue em um email, ele é entregue com o carimbo de data e hora e o formato que corresponde à localidade do usuário e ao fuso horário conforme especificados no perfil do Workfront.\
  Para obter mais informações sobre a localidade do usuário e o fuso horário no Workfront, consulte o artigo [Editar o perfil de um usuário](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## Relatórios com uma exibição especial {#reports-with-a-special-view}

Quando você aplica uma visualização especial a um relatório, ela é exibida na guia Detalhes do relatório no Workfront.

Ao agendar a entrega de um relatório com uma visualização especial, a guia Detalhes padrão é entregue no anexo do email enviado, em vez da visualização especial.

Estas são as visões especiais:

* Exibição de marcos em um relatório de Projeto
* Exibição de Gantt em um relatório de Projeto ou de Tarefa
* Relatórios com um Gráfico como guia padrão

>[!NOTE]
>
Se também houver uma guia Matrix no relatório, além da guia padrão com uma visualização especial, o relatório será entregue da maneira como é exibido na guia Matrix.

Para obter mais informações sobre como aplicar uma exibição especial a um relatório, consulte o artigo [Criar um relatório personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

## Usar o arquivo entregue

 Ao enviar um relatório do Workfront, o usuário recebe um email com o relatório em um anexo separado. 

* [Linha de assunto, nome do anexo e título do relatório](#subject-line-attachment-name-and-report-title)
* [Carimbos de data e hora](#timestamps)
* [Marcas](#branding)
* [Formatação](#formatting)
* [Links](#links)

### Linha de assunto, nome do anexo e título do relatório {#subject-line-attachment-name-and-report-title}

Para obter mais informações sobre a linha de assunto do email do relatório entregue, consulte [Programar uma entrega automática de relatório](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-automatic-report-delivery.md).

O nome do relatório anexado é: *The_Name_Of_The_Report* seguido pelo formato de arquivo exportado. 

Se você agendar o relatório entregue para ser formatado como um arquivo PDF ou HTML, o título do relatório será:

*O Nome do Relatório.*

Os relatórios agendados para entrega nos formatos do Excel, Excel (.xlsx) ou TSV não têm título.

>[!NOTE]
>
Se o relatório tiver uma descrição, ele será incluído no arquivo exportado, se o arquivo estiver formatado como um arquivo PDF ou HTML.

### Carimbos de data e hora {#timestamps}

Um carimbo de data e hora é exibido no arquivo anexado somente se o formato do arquivo for um .pdf. O carimbo de data e hora está no rodapé do arquivo anexado.

O carimbo de data e hora inclui:

* Data
* Hora
* Fuso horário em que o relatório foi enviado

### Marca {#branding}

Se o administrador do Workfront tiver adicionado a marca personalizada à instância do Workfront, os relatórios enviados no formato .pdf também incluirão o logotipo personalizado.

Relatórios enviados em todos os outros formatos não podem ser personalizados com seu logotipo.

Para obter mais informações sobre como marcar sua instância do Workfront, consulte o artigo [Marque sua instância do Adobe Workfront](../../../administration-and-setup/customize-workfront/brand-workfront/brand-your-workfront-instance.md).

### Formatação {#formatting}

Você sempre recebe a guia padrão de um relatório quando ele é enviado ou agendado para um delivery, a menos que o relatório tenha uma visualização especial.

Se o relatório tiver formatação especial no aplicativo web, ele deverá ser entregue com a formatação especial quando as guias Details e Matrix forem entregues somente para arquivos .pdf e Excel.

O filtro, a visualização ou o agrupamento do relatório não estão incluídos no arquivo entregue. A descrição do relatório é incluída somente quando você envia o relatório como um arquivo PDF.

Para obter mais informações sobre como receber relatórios com uma exibição especial, consulte o artigo [Relatórios com uma exibição especial](#reports-with-a-special-view).\
Para obter mais informações sobre a seleção da guia padrão de um relatório e sobre formatação especial, consulte [Criar um relatório personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

### Links {#links}

Quando você envia um relatório do Workfront para o formato PDF ou Excel, todos os links de trabalho existentes no documento original permanecem ativos no arquivo enviado. Os links podem apontar para qualquer objeto no Workfront que ofereça suporte a links.

O nome do relatório na mensagem de email também é um link.

## Relatório sobre relatórios agendados

Você pode ver se um relatório foi configurado para ser entregue criando o seguinte:

* **Uma Visão** para o objeto Relatório em uma lista ou um relatório para relatórios: crie uma exibição em uma lista de relatórios ou em um relatório para relatórios e adicione a seguinte coluna à exibição:\
  *Nome do relatório agendado.\
  *Os nomes de todos os deliveries agendados para esse relatório estão listados na coluna em uma lista com marcadores.\
  ![scheduled_reports_info_in_view.png](assets/scheduled-reports-info-in-view-350x294.png)

* **Um Filtro** para o objeto Relatório: crie um filtro em uma lista de relatórios ou em um relatório sobre relatórios com a seguinte instrução: *A ID do relatório agendado não está em branco*.\
  Isso exibirá somente os relatórios que foram agendados na lista ou no relatório.\
  ![](assets/qs-scheduled-report-filter-350x101.png)\
  Para obter mais informações sobre a criação de relatórios, consulte [Criar um relatório personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md). Para obter informações sobre como criar um relatório sobre relatórios, consulte [Criar um relatório sobre atividades de relatório](../../../reports-and-dashboards/reports/report-usage/create-report-reporting-activities.md).

<!--
<h2 data-mc-conditions="QuicksilverOrClassic.Draft mode">Scheduling a Repeating&nbsp;Report Delivery</h2>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">You can schedule up to 10 repeating report deliveries for any given report.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">You can schedule a report to be delivered only if you are the creator of the report. If you need to send a report that you did not create, you can send it on a manual basis.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">To schedule&nbsp;a report for automatic delivery or to edit an existing report delivery:&nbsp;​</p>
-->

<!--
   <li value="1" data-mc-conditions="QuicksilverOrClassic.Draft mode">Navigate to and click the name of the report for which you want to schedule delivery.&nbsp;</li>
   -->

<!--
   <li value="2" data-mc-conditions="QuicksilverOrClassic.Draft mode">Click <strong>Report Actions</strong>, then&nbsp;<strong>Send Report</strong>.<br> The <strong>Send Report</strong> dialog box is displayed.</li>
   -->

<!--
   <li value="3" data-mc-conditions="QuicksilverOrClassic.Draft mode">Select the <strong>Repeating Deliveries</strong>&nbsp;tab.<br><img src="assets/report-delivery-schedule-350x169.png" alt="" style="width: 350;height: 169;"></li>
   -->

<!--
   <li value="4" data-mc-conditions="QuicksilverOrClassic.Draft mode">(Conditional)&nbsp;To modify an existing repeating report delivery, select the report delivery in the <strong>Repeating Deliveries</strong>&nbsp;section.</li>
   -->

<!--
   <li value="5" data-mc-conditions="QuicksilverOrClassic.Draft mode">Specify the following information:
   <ul>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>Send to:</strong> Begin typing the name of the user, group, team, or role who you want to send&nbsp;the report to, then click the name when it appears in the drop-down list.<br>Or<br>Specify the email address of a person external to the Workfront system who you want to have access to the report.<br> Repeat this process to send the report to multiple users, groups, teams, or roles.</li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>Email Subject:</strong> Specify a subject for the email notification.<br> By default, the email subject is: <em>Workfront Report: <Name of the report> Date of the Export</em>.<strong></strong></li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>Email Message:</strong> Specify a message to include in the email.<br>By default, the email message is:&nbsp;<em>Attached is the <report frequency> report <Name of the report> generated by Workfront on <Date>.</em><br>
   <note type="note">
   For reports delivered as an Excel file only, the following message is also added to the email: "Please be aware that with MS Excel (XLS) file types, there is a limit (65,530) on the number of hyperlinks these file types support. If you exceed those limits, your file will not open and it is recommended to resend without the hyperlinks.&nbsp;Please go back to the report scheduler&nbsp;to remove hyperlinks and resend the report." The "please go back to the report scheduler" phrase is a link back to the report.&nbsp;
   </note>
   </li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>Deliver this report with the Access Rights of:</strong>&nbsp;Begin typing the name of a user who has access to the report, then click the name when it appears&nbsp;in the drop-down list. Users who receive the report will be granted the same level of access to the report as the user that you specify&nbsp;here.<br> For more information, see <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/run-deliver-report-access-rights-another-user.md" class="MCXref xref">Run and deliver a report with the access rights of another user</a>
   <note type="note">
   This field does not support wildcards. For example, using the wildcard $$User.ID does not run the report with the access rights of the user who is receiving the report.
   </note>
   </li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>Format:</strong> Select in which of the following formats you want the report to be delivered:
   <ul>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> HTML</li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode">PDF</li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode">MS&nbsp;Excel</li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode">MS Excel (.xlsx)</li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode">TSV &nbsp;</li>
   </ul></li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>Include Links:</strong>&nbsp;This option is available&nbsp;only when <strong>MS Excel</strong> is selected in the <strong>Format</strong> drop-down menu. When this option is enabled, any hyperlinks are included in the exported Excel document. <br>Documents that contain more than 65,530 links cannot be opened. If the exported document will contain more than 65,530 links, deselect this option.<br>This option is enabled by default.&nbsp;</li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>Summary:</strong> Displays a summary of when the delivery repeats.</li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>Repeats:</strong> Select whether the report should be delivered daily, weekly, monthly, or yearly.</li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>Repeats Every:</strong> Select the frequency with which you want&nbsp;the delivery to repeat. The value you select for this option is&nbsp;based on the option that is selected in the <strong>Repeats</strong>&nbsp;drop-down list.</li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>Time:</strong> Select the time of day for the delivery to be sent.</li>
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>Repeats On:</strong>&nbsp;This option is available when the <strong>Repeats</strong>&nbsp;option is set to either <strong>Weekly</strong>&nbsp;or <strong>Monthly</strong>.</p>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode">When the <strong>Repeats</strong>&nbsp;option is set to <strong>Weekly</strong>: Select the days of the week that the delivery is sent.</li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode">When the <strong>Repeats</strong>&nbsp;option is set to <strong>Monthly</strong>: Select whether the delivery is sent on the day of the month, day of the week, or last day of the month (these options leverage the date that you select in the <strong>Starts On</strong>&nbsp;field).</li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>Starts On:</strong> Select the date for the scheduled delivery to begin.</li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>Ends On:</strong> Select a date for the scheduled delivery to end. <br>Or</li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Select <strong>Never</strong>&nbsp;if you want the scheduled delivery to last indefinitely.</li>
   -->

<!--
   <li value="6" data-mc-conditions="QuicksilverOrClassic.Draft mode">Click <strong>Save</strong>&nbsp;to save the report delivery.<br> The report is saved in the <strong>Repeating Deliveries</strong>&nbsp;section&nbsp;(in the <strong>Send Report</strong> dialog box).<br> The report will be sent at the schedule time<br>Or<br>To manually send the report, click <strong>Send Now</strong>.<br>For more information about sending the report instantly or manually, see&nbsp;.</li>
   -->

<!--
<h2 data-mc-conditions="QuicksilverOrClassic.Draft mode">Deleting a Scheduled Report Delivery</h2>
-->

<!--
   <li value="1" data-mc-conditions="QuicksilverOrClassic.Draft mode">Go to the report with the delivery you want to delete.</li>
   -->

<!--
   <li value="2" data-mc-conditions="QuicksilverOrClassic.Draft mode">Click <strong>Report Actions</strong>, then <strong>Send Report</strong>.&nbsp;</li>
   -->

<!--
   <li value="3" data-mc-conditions="QuicksilverOrClassic.Draft mode">Click <strong>Repeating Deliveries</strong>.&nbsp;</li>
   -->

<!--
   <li value="4" data-mc-conditions="QuicksilverOrClassic.Draft mode">Click the name of the scheduled delivery you want to delete, then click <strong>Delete</strong>. The report is no longer set up for the scheduled delivery.&nbsp;</li>
   -->

<!--
<h2 data-mc-conditions="QuicksilverOrClassic.Draft mode">Sending a Report Manually, on a One-Time Basis</h2>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">You can manually send a report&nbsp;that has been previously scheduled, or you can create a single-use report delivery.​</p>
-->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a title="Setting Up Report Deliveries" href="#sending-a-scheduled-report-now" class="MCXref xref">Sending a Scheduled Report Now</a> </li>
  -->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a title="Setting Up Report Deliveries" href="#sending-a-report-one-time-only" class="MCXref xref">Sending a Report (One Time Only)</a> </li>
  -->

<!--
<h3 data-mc-conditions="QuicksilverOrClassic.Draft mode" id="sending-a-scheduled-report-now">Sending a Scheduled Report Now</h3>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">After a scheduled report has been set up, you can manually send the report rather than&nbsp;waiting until the scheduled time.</p>
-->

<!--
   <li value="1" data-mc-conditions="QuicksilverOrClassic.Draft mode">Navigate to and click the name of the report that you want to send now.</li>
   -->

<!--
   <li value="2" data-mc-conditions="QuicksilverOrClassic.Draft mode">Click <strong>Report Actions</strong>, then&nbsp;<strong>Send Report</strong>.<br> The Send Report dialog box is displayed.</li>
   -->

<!--
   <li value="3" data-mc-conditions="QuicksilverOrClassic.Draft mode">Click the <strong>Repeating Deliveries</strong> tab.</li>
   -->

<!--
   <li value="4" data-mc-conditions="QuicksilverOrClassic.Draft mode">In the <strong>Repeating Deliveries</strong>&nbsp;section, select the report delivery that was previously created.<br><img src="assets/report-delivery-schedule-send-350x160.png" alt="" style="width: 350;height: 160;"></li>
   -->

<!--
   <li value="5" data-mc-conditions="QuicksilverOrClassic.Draft mode">Click <strong>Send Now</strong>.<br> The report is sent to all users identified in the scheduled delivery.</li>
   -->

<!--
<h3 data-mc-conditions="QuicksilverOrClassic.Draft mode" id="sending-a-report-one-time-only">Sending a Report (One Time Only)</h3>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">You can manually send a report at any time. When you send a report in this way, delivery information (such as&nbsp;the users you are sending to and&nbsp;the email subject) are not saved. If you want to create a report delivery that you can save for later use, create a repeating scheduled report.&nbsp;</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">To send a report to users (one time only):</p>
-->

<!--
   <li value="1" data-mc-conditions="QuicksilverOrClassic.Draft mode">Navigate to and click the name of the report that you want to send now.</li>
   -->

<!--
   <li value="2" data-mc-conditions="QuicksilverOrClassic.Draft mode">Click <strong>Report Actions</strong>, then&nbsp;<strong>Send Report</strong>.<br> The <strong>Send Report</strong> dialog box is displayed.<br><img src="assets/report-delivery-sendnow-350x351.png" alt="" style="width: 350;height: 351;"></li>
   -->

<!--
   <li value="3" data-mc-conditions="QuicksilverOrClassic.Draft mode">On the <strong>Send Now</strong>&nbsp;tab, specify the following information:
   <ul>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>Send to:</strong> Begin typing the name of the user, group, team, or role who you want to send&nbsp;the report to, then click the name when it appears in the drop-down list.&nbsp;Or, specify the email address of a person external to the Workfront system who you want to have access to the report.<br> Repeat this process to send the report to multiple users, groups, teams, or roles.</li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>Email Subject:</strong> Specify a subject for the email notification.<br> By default, the email subject is: <em>Workfront Report: <Name of the report> Date of the Export</em>.</li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>Email Message:</strong> Specify a message to include in the email.<br>By default, the email message is:&nbsp;<em>Attached is the <report frequency> report <Name of the report> generated by Workfront on <Date>.</em><br>
   <note type="note">
   For reports delivered as an Excel file only, the following message is also added to the email: "Please be aware that with MS Excel (XLS) file types, there is a limit (65,530) on the number of hyperlinks these file types support. If you exceed those limits, your file will not open and it is recommended to resend without the hyperlinks.&nbsp;Please go back to the report scheduler&nbsp;to remove hyperlinks and resend the report." The "please go back to the report scheduler" phrase is a link back to the report.&nbsp;
   </note>
   </li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>Deliver this report with the Access Rights of:</strong>&nbsp;Begin typing the name of a user who has access to the report, then click the name when it appears&nbsp;in the drop-down list. Users who receive the report will be granted the same level of access to the report as the user that you specify&nbsp;here.<br> For more information, see <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/run-deliver-report-access-rights-another-user.md" class="MCXref xref">Run and deliver a report with the access rights of another user</a>.
   <note type="note">
   This field does not support wildcards. For example, using the wildcard $$User.ID does not run the report with the access rights of the user who is receiving the report.
   </note>
   </li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>Format:</strong> Select in which of the following formats you want the report to be delivered:
   <ul>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> HTML</li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode">PDF</li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode">MS Excel</li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode">MS&nbsp;Excel (.xlsx)</li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode">TSV</li>
   </ul></li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>Include Links:</strong>&nbsp;This option is available&nbsp;only when <strong>MS Excel</strong> is selected in the <strong>Format</strong> drop-down menu. When this option is enabled, any hyperlinks are included in the exported Excel document. <br>Documents that contain more than 65,000 links cannot be opened. If the exported document will contain more than 65,000 links, deselect this option.<br>This option is enabled by default.</li>
   </ul></li>
   -->

<!--
   <li value="4" data-mc-conditions="QuicksilverOrClassic.Draft mode">Click <strong>Send Now</strong>.<br> The report is sent to all users that you identified.<br> Or<br> Click <strong>Make Repeating Delivery</strong>&nbsp;if you want to set up&nbsp;a scheduled delivery with this same information, then complete the additional information regarding the frequency of when the report is sent.</li>
   -->
