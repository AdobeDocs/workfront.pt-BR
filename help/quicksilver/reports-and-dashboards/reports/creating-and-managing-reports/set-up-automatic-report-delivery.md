---
product-area: reporting;setup
navigation-topic: create-and-manage-reports
title: Programar uma entrega automática de relatório
description: Programar uma entrega automática de relatório
author: Nolan
feature: Reports and Dashboards
exl-id: 5b8e382c-bfe8-43aa-aa09-a2aa0c4d56cc
source-git-commit: 70bda5a7186abfa7e8cbd26e25a4c58583a322b4
workflow-type: tm+mt
source-wordcount: '1197'
ht-degree: 2%

---

# Programar uma entrega automática de relatório

<!-- Audited: 11/2024 -->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: If this stays, fix links which now go to the reference article)</p>
-->

Você pode agendar relatórios para serem enviados automaticamente aos usuários em um agendamento definido ou pode enviar relatórios manualmente de uma só vez. Ao enviar um relatório do Adobe Workfront, o usuário recebe um email com o relatório do Workfront em um anexo separado.

Para obter mais informações, incluindo limitações de tamanho que podem afetar a entrega de seus relatórios, consulte [Visão geral da entrega de relatórios](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront*</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
      <td> 
      <p>Novo:</p>
         <ul>
         <li><p>Padrão</p></li>
         </ul>
      <p>Atual:</p>
         <ul>
         <li><p>Plano</p></li>
         </ul>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a relatórios, painéis, calendários</p> <p>Editar acesso a Filtros, Visualizações, Agrupamentos</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões para um relatório</p></td> 
  </tr> 
 </tbody> 
</table>

*Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Pré-requisitos

Antes de começar, você deve criar um relatório. Para saber mais sobre como criar relatórios, consulte [Criar um relatório personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

## Programar uma entrega de relatório

Para agendar um relatório para entrega automática ou editar ou excluir uma entrega de relatório existente:&#x200B;

1. Vá para um relatório que você deseja agendar a entrega.

   >[!NOTE]
   >
   >Os deliveries do relatório não contêm prompts. Se quiser limitar os dados em um delivery de relatório, recomendamos aplicar filtros ao relatório que deseja enviar.

1. Clique em **Ações de Relatório** e em **Enviar Relatório**.

   A caixa de diálogo **Enviar Relatório** é exibida.

   >[!TIP]
   >
   >Para enviar um relatório manualmente a qualquer momento, vá para o relatório e clique em **Ações de Relatório** > **Enviar Relatório** > **Enviar Agora**.

1. Selecione a guia **Entregas repetitivas**.
1. (Condicional) Para modificar uma entrega de relatório repetitivo existente, selecione a entrega de relatório na seção **Entregas repetitivas**.
1. Especifique as seguintes informações:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>Enviar para</p> </td> 
      <td> <p>Comece digitando o nome do usuário, grupo, equipe ou função para o qual deseja enviar o relatório e clique no nome quando ele aparecer na lista suspensa.</p> <p>Ou</p> <p>Especifique o endereço de email de uma pessoa externa ao sistema Workfront que deseja que tenha acesso ao relatório.</p> <p>Repita esse processo para enviar o relatório para vários usuários, grupos, equipes ou funções.</p> <p>Nota:  <p>Considere o seguinte ao adicionar recipients do delivery de relatório:</p> 
        <ul> 
         <li>Se sua organização restringir notificações do Workfront a domínios de email específicos, você só poderá enviar relatórios para os endereços de email listados na inclui na lista de permissões de email.<p>Para obter informações sobre como um administrador do Workfront incluir na lista de permissões incluir na lista de permissões atualiza o arquivo de email, consulte a seção <a href="../../../administration-and-setup/get-started-wf-administration/configure-your-email-allowlist.md#configur" class="MCXref xref">Configurar sua pesquisa de email</a>.</p></li> 
         <li> <p>Adicionar um grande número de usuários como recipients pode causar falha no delivery. Se você tiver falhas de delivery, poderá agendar vários deliveries de relatório com grupos menores de usuários.</p> </li> 
        </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Assunto do email</p> </td> 
      <td> <p>Especifique um assunto para a notificação por email.</p> <p>Por padrão, o assunto do email é:</p> <p><em>Relatório do Workfront: [Nome do relatório] [Data]</em> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Mensagem de email</p> </td> 
      <td> <p>Especifique uma mensagem para incluir no email.</p> <p>Por padrão, a mensagem de email é:</p> <p><em>Anexo é o relatório [Nome do relatório] [frequência] gerado pelo Workfront em [Data].</em> </p> <p>Observação: para relatórios entregues como um arquivo do Excel somente, a seguinte mensagem também é adicionada ao email: "Esteja ciente de que, com os tipos de arquivo do MS Excel (XLS), há um limite (65.530) no número de hiperlinks que esses tipos de arquivo suportam. Se esses limites forem excedidos, o arquivo não será aberto e é recomendável reenviar sem os hiperlinks. Retorne ao agendador de relatórios para remover os hiperlinks e reenviar o relatório." A frase "volte para o agendador de relatórios" é um link para o relatório.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Enviar este relatório com direitos de acesso de</p> </td> 
      <td> <p>Comece digitando o nome de um usuário que tem acesso ao relatório e clique no nome quando ele aparecer na lista suspensa. Os usuários que receberem o relatório receberão o mesmo nível de acesso que o usuário especificado aqui.<br> Para obter mais informações, consulte <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/run-deliver-report-access-rights-another-user.md" class="MCXref xref">Executar e entregar um relatório com direitos de acesso de outro usuário</a>.</p> <p>Observação: este campo não aceita curingas. Por exemplo, o uso do curinga $$User.ID não executa o relatório com os direitos de acesso do usuário que está recebendo o relatório.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Formato</p> </td> 
      <td> <p>Selecione o formato desejado para o relatório entregue:</p> 
       <ul> 
        <li> <p>HTML</p> </li> 
        <li> <p>PDF</p> <p>Se você selecionar esta opção, poderá formatar a saída usando as opções adicionais de <strong>Tamanho do Papel</strong> e <strong>Orientação</strong> exibidas.</p> </li> 
        <li> <p>MS Excel (.xlsx)</p> </li> 
        <li> <p>TSV</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Incluir Links</p> </td> 
      <td> <p>Esta opção está disponível somente quando o <strong>MS Excel</strong> é selecionado no menu suspenso <strong>Formatar</strong>. Quando essa opção estiver habilitada, todos os hiperlinks serão incluídos no documento do Excel exportado.</p> <p>Não é possível abrir documentos com mais de 65.530 links. Se o documento exportado contiver mais de 65.530 links, desmarque essa opção.</p> <p>Essa opção está ativada por padrão.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Resumo</p> </td> 
      <td> <p>Exibe um resumo de quando o delivery se repete.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Repete</p> </td> 
      <td> <p>Selecione se o relatório deve ser entregue diariamente, semanalmente, mensalmente ou anualmente.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Repete a cada</p> </td> 
      <td> <p>Selecione a frequência com que deseja que o delivery se repita. O valor selecionado para esta opção baseia-se na opção selecionada na lista suspensa <strong>Repetições</strong>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Hora</p> </td> 
      <td> <p>Selecione a hora do dia para o envio do delivery.</p> <p>Dica: como as cargas do sistema podem afetar os prazos de entrega do relatório, pode haver um atraso de até 24 horas entre o horário agendado e o horário real de entrega. Se você precisar que um relatório seja entregue em um horário específico, recomendamos agendar o delivery antes do horário necessário. Em geral, recomendamos agendar o delivery pelo menos um dia antes da data em que é necessário.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Repete em</p> </td> 
      <td> <p>Esta opção está disponível quando a opção <strong>Repetições</strong> está definida como <strong>Semanalmente</strong> ou <strong>Mensalmente</strong>:</p> 
       <ul> 
        <li> <p>Quando a opção <strong>Repetições</strong> estiver definida como <strong>Semanalmente</strong>: selecione os dias da semana em que a entrega será enviada.</p> </li> 
        <li> <p>Quando a opção <strong>Repetições</strong> estiver definida como <strong>Mensalmente</strong>: selecione se a entrega será enviada no dia do mês, dia da semana ou último dia do mês (essas opções usam a data selecionada no campo <strong>Começa em</strong>).</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Inicia em</p> </td> 
      <td>Selecione a data de início do delivery agendado.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Termina em</p> </td> 
      <td>Selecione uma data para o término do delivery agendado.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Nunca</p> </td> 
      <td>Selecione <strong>Nunca</strong> se desejar que a entrega agendada dure indefinidamente.</td> 
     </tr> 
    </tbody> 
   </table>

1. Clique em **Salvar** para salvar a entrega do relatório.

   O relatório é exibido na seção **Entregas repetitivas** (na caixa de diálogo **Enviar relatório**) e será enviado no horário agendado.

   Para obter informações sobre limitações de tamanho que podem afetar a entrega de seus relatórios, consulte as seções [Limites de entrega de relatórios](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md#understanding-export-limits) e [Limites de exportação](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md#export).

>[!IMPORTANT]
>
>Os relatórios agendados estão sujeitos a um limite de tempo interno ao serem processados para entrega. Caso um relatório leve mais tempo do que o limite para ser enviado, você receberá uma notificação e o relatório não será mais entregue, independentemente de quaisquer deliveries agendados restantes. Para continuar enviando o relatório, primeiro tente reduzir o tamanho do relatório por meio de filtros e visualizações e, em seguida, crie um novo delivery agendado.
>
>Se você estiver usando uma entrega de relatório agendada para analisar dados do Workfront por meio de uma ferramenta de BI, recomendamos usar o Workfront Data Connect. Para obter mais informações, consulte [visão geral do Workfront Data Connect](/help/quicksilver/reports-and-dashboards/data-lake/data-lake-overview.md).

1. (Opcional) Para excluir um delivery agendado:

   1. No painel **Entregas repetitivas**, clique na entrega agendada e em **Excluir**.
   1. Clique em **Excluir** para confirmar.

<!--## Video walk-through

View the following video to learn how to schedule a report delivery. This video was recorded in Workfront Classic. However, the content also applies to the new Workfront experience.

[ ![Video walkthrough of report delivery](assets/video-walk-through--350x197.png)](https://workfront-video.wistia.com/medias/45jffmll62)


<h2 data-mc-conditions="QuicksilverOrClassic.Draft mode">Additional information</h2>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">See also:</p>
-->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="https://one.workfront.com/s/learningpath2/workfront-reporting-20Y0z000000blhLEAQ" target="_blank">Learning Path for reports and dashboards</a> </li>
  -->

<!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="https://one.workfront.com/s/basic-report-creation-program">Basic Report Creation Program for the new Workfront experience</a> </p>
  -->
