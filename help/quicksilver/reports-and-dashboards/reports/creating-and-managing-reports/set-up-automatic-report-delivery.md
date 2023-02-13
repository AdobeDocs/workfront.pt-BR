---
product-area: reporting;setup
navigation-topic: create-and-manage-reports
title: Programar um delivery de relatório automático
description: Programar um delivery de relatório automático
author: Nolan
feature: Reports and Dashboards
exl-id: 5b8e382c-bfe8-43aa-aa09-a2aa0c4d56cc
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '1164'
ht-degree: 3%

---

# Programar um delivery de relatório automático

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: If this stays, fix links which now go to the reference article)</p>
-->

Você pode programar relatórios para entregá-los automaticamente aos usuários em uma programação definida ou enviar relatórios manualmente de uma só vez. Quando você envia um relatório do Adobe Workfront, o usuário recebe um email com o relatório do Workfront em um anexo separado.

Para obter mais informações, incluindo limitações de tamanho que podem afetar a entrega de seus relatórios, consulte [Visão geral da entrega de relatórios](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plano Adobe Workfront*</td> 
   <td> <p>Qualquer Um</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Plano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a Relatórios, Painéis, Calendários</p> <p>Editar acesso a filtros, visualizações, agrupamentos</p> <p>Observação: Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões de um relatório</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

## Pré-requisitos

Antes de começar, você deve criar um relatório. Para saber mais sobre como criar relatórios, consulte [Criar um relatório personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

## Programar um delivery de relatório

Para agendar um relatório para entrega automática ou editar ou excluir um delivery de relatório existente: &#x200B;

1. Vá para um relatório que deseja agendar para entrega.

   >[!NOTE]
   >
   >Os deliveries de relatório não contêm prompts. Se você deseja limitar os dados em um delivery de relatório, recomendamos aplicar filtros ao relatório que deseja enviar.

1. Clique em **Ações de Relatório**, em seguida **Enviar relatório**.

   O **Enviar relatório** será exibida.

   >[!TIP]
   >
   >Para enviar um relatório manualmente a qualquer momento, vá para o relatório e clique em **Ações de Relatório** > **Enviar relatório** > **Enviar agora**.

1. Selecione o **Repetição de Deliveries** guia .
1. (Condicional) Para modificar um delivery de relatório repetitivo existente, selecione o delivery de relatório no **Repetição de Deliveries** seção.
1. Especifique as seguintes informações:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>Enviar para</p> </td> 
      <td> <p>Comece digitando o nome do usuário, grupo, equipe ou função para quem deseja enviar o relatório e clique no nome quando ele aparecer na lista suspensa.</p> <p>Ou</p> <p>Especifique o endereço de email de uma pessoa externa ao sistema Workfront que você deseja que tenha acesso ao relatório.</p> <p>Repita esse processo para enviar o relatório a vários usuários, grupos, equipes ou funções.</p> <p>Nota:  <p>Considere o seguinte ao adicionar recipients do delivery do relatório:</p> 
        <ul> 
         <li>Se sua organização restringir as notificações do Workfront a domínios de email específicos, você só poderá enviar relatórios para endereços de email listados na  de lista de permissões de email.<p>Para obter informações sobre como um administrador do Workfront atualiza a  de lista de permissões de email, consulte a seção <a href="../../../administration-and-setup/get-started-wf-administration/configure-your-email-allowlist.md#configur" class="MCXref xref">Configurar sua  de lista de permissões de email</a>.</p></li> 
         <li> <p>Adicionar um grande número de usuários como recipients pode causar falha no delivery. Se você tiver falhas de delivery, poderá agendar vários deliveries de relatório com grupos menores de usuários.</p> </li> 
        </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Assunto do email</p> </td> 
      <td> <p>Especifique um assunto para a notificação por email.</p> <p>Por padrão, o assunto do email é:</p> <p><em>Relatório do Workfront: [Nome do relatório] [Data]</em> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Mensagem de email</p> </td> 
      <td> <p>Especifique uma mensagem para incluir no email.</p> <p>Por padrão, a mensagem de email é:</p> <p><em>Anexado está o relatório [frequência do relatório] [Nome do relatório] gerado pelo Workfront em [Data].</em> </p> <p>Observação: Para relatórios entregues somente como um arquivo Excel, a seguinte mensagem também é adicionada ao email: "Esteja ciente de que, com os tipos de arquivo MS Excel (XLS), há um limite (65.530) no número de hiperlinks suportados por esses tipos de arquivo. Se você exceder esses limites, seu arquivo não será aberto e é recomendável reenviar sem os hiperlinks. Retorne ao agendador do relatório para remover hiperlinks e reenviar o relatório." A frase "volte para o agendador do relatório" é um link para o relatório.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Enviar este relatório com direitos de acesso de</p> </td> 
      <td> <p>Comece digitando o nome de um usuário que tem acesso ao relatório e clique no nome quando ele for exibido na lista suspensa. Os usuários que receberem o relatório terão o mesmo nível de acesso ao relatório que o usuário especificado aqui.<br> Para obter mais informações, consulte <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/run-deliver-report-access-rights-another-user.md" class="MCXref xref">Executar e entregar um relatório com os direitos de acesso de outro usuário</a>.</p> <p>Observação: Este campo não suporta curingas. Por exemplo, o uso do curinga $$User.ID não executa o relatório com os direitos de acesso do usuário que está recebendo o relatório.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Formatar</p> </td> 
      <td> <p>Selecione o formato desejado para o relatório entregue:</p> 
       <ul> 
        <li> <p>HTML</p> </li> 
        <li> <p>PDF</p> <p>Se você selecionar essa opção, será possível formatar a saída usando o <strong>Tamanho do papel</strong> e <strong>Orientação</strong> opções exibidas.</p> </li> 
        <li> <p>MS Excel (.xlsx)</p> </li> 
        <li> <p>TSV</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Incluir Links</p> </td> 
      <td> <p>Essa opção só está disponível quando <strong>MS Excel</strong> é selecionado no <strong>Formato</strong> menu suspenso. Quando essa opção estiver ativada, todos os hiperlinks serão incluídos no documento do Excel exportado.</p> <p>Os documentos que contêm mais de 65.530 links não podem ser abertos. Se o documento exportado contiver mais de 65.530 links, desmarque essa opção.</p> <p>Essa opção é ativada por padrão.</p> </td> 
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
      <td> <p>Selecione a frequência com que deseja que o delivery se repita. O valor selecionado para essa opção é baseado na opção selecionada na variável <strong>Repetir</strong> lista suspensa.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Hora</p> </td> 
      <td> <p>Selecione a hora do dia para o delivery ser enviado.</p> <p>Dica: Como as cargas do sistema podem afetar os tempos de entrega do relatório, pode haver um atraso entre o horário agendado e o tempo de entrega real. Se você precisar de um relatório entregue por um tempo específico, recomendamos agendar o delivery antes do tempo em que ele é necessário. Por exemplo, recomendamos agendar o delivery um dia antes da data em que for necessário.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Repete em</p> </td> 
      <td> <p>Essa opção está disponível quando a variável <strong>Repetir</strong> está definida como <strong>Semanalmente</strong> ou <strong>Mensalmente</strong>:</p> 
       <ul> 
        <li> <p>Quando a variável <strong>Repetir</strong> está definida como <strong>Semanalmente</strong>: Selecione os dias da semana em que o delivery é enviado.</p> </li> 
        <li> <p>Quando a variável <strong>Repetir</strong> está definida como <strong>Mensalmente</strong>: Selecione se o delivery é enviado no dia do mês, no dia da semana ou no último dia do mês (essas opções aproveitam a data selecionada na variável <strong>Começa em</strong> campo ).</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Inicia em</p> </td> 
      <td>Selecione a data de início do delivery agendado.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Termina em</p> </td> 
      <td>Selecione uma data para o delivery agendado terminar.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Nunca</p> </td> 
      <td>Selecionar <strong>Nunca</strong> se desejar que o delivery programado dure indefinidamente.</td> 
     </tr> 
    </tbody> 
   </table>

1. Clique em **Salvar** para salvar o delivery do relatório.

   O relatório é exibido na **Repetição de Deliveries** na seção **Enviar relatório** e será enviada no horário agendado.

   Para obter informações sobre limitações de tamanho que podem afetar a entrega de seus relatórios, consulte as seções [Relatórios de limites de delivery](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md#understanding-export-limits) e [Limites de exportação](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md#export).

1. (Opcional) Para excluir um delivery agendado:

   1. No **Repetição de Deliveries** , clique em entrega agendada e, em seguida, clique em **Excluir**.
   1. Clique em **Excluir** para confirmar.

## Apresentação de vídeo

Assista ao vídeo a seguir para saber como agendar um delivery de relatório. Este vídeo foi gravado no Workfront Classic. No entanto, o conteúdo também se aplica à nova experiência do Workfront.

[ ![](assets/video-walk-through--350x197.png)](https://workfront-video.wistia.com/medias/45jffmll62)

<!--
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
