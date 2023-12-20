---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Editar configurações do relatório
description: É possível editar as configurações de um relatório para definir como ele é exibido para outros usuários ou que tipo de informações os usuários podem solicitar antes de executarem o relatório.
author: Nolan
feature: Reports and Dashboards
exl-id: 6fbbc557-65da-4ffe-968a-9c8db6a45811
source-git-commit: dad054fe52bd7c5ca97144567c80e6d340541a50
workflow-type: tm+mt
source-wordcount: '663'
ht-degree: 6%

---

# Editar configurações do relatório

É possível editar as configurações de um relatório para definir como ele é exibido para outros usuários ou que tipo de informações os usuários podem solicitar antes de executarem o relatório.

## Requisitos de acesso

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
   <td> <p>Plano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a relatórios, painéis, calendários</p> <p>Editar acesso a Filtros, Visualizações, Agrupamentos</p> <p>Observação: se você ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões para um relatório</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir seu plano, tipo de licença ou acesso, entre em contato com o administrador do Workfront.

## Etapas passo a passo

1. Comece a criar um relatório acessando o **Menu principal** > **Relatórios**, em seguida, selecione o objeto do relatório.

   Ou

   Abra um relatório existente e clique em **Ações de Relatório** > **Editar**.

1. Clique em **Configurações do relatório** no canto superior direito do report builder.
1. Defina as seguintes configurações de relatório:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Título do relatório</td> 
      <td>Especifique um título para o relatório.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Descrição</td> 
      <td>Especifique uma declaração que descreva a finalidade e os usos do relatório.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Executar este relatório com direitos de acesso de</td> 
      <td>Selecione o usuário cujos direitos de acesso você deseja que este relatório use ao exibir para outros usuários. Para obter mais informações sobre como executar um relatório com os direitos de acesso de outro usuário, consulte o artigo <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/run-deliver-report-access-rights-another-user.md" class="MCXref xref">Executar e entregar um relatório com direitos de acesso de outro usuário</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Quando o relatório for carregado, mostrar a</td> 
      <td>Selecione a guia padrão exibida para todos os usuários quando o relatório for carregado.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Quando o relatório for carregado em um painel, mostrar ... itens</td> 
      <td>Especifique o número de itens exibidos para todos os usuários quando o relatório é carregado em um painel. O padrão é 15 itens e o número máximo de itens é 200.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Mostrar a exibição Grade de Recursos na guia Detalhes</td> 
      <td> <p>(Somente Relatório do Usuário) Selecione esta opção para exibir a Grade de Recursos na guia Detalhes do relatório.</p> <p>Nota: Ao aplicar a visualização da Grade de Recursos a um relatório do usuário, o relatório mostra apenas os projetos que estão no status Atual. Se quiser ver projetos com qualquer outro status, use a guia Utilização do Usuário na área Pessoas da Barra de Navegação Global e aplique a Exibição da Grade de Recursos lá. <!--
         <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
          For more information about using the Resource Grid, see the article Overview of the Resource Grid . (drafted because this article is drafted also: Article is in draft Feb 1, 2021)
         </MadCap:conditionalText>
        --></p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Mostrar uma exibição especial na guia Detalhes</td> 
      <td>(Somente Relatório de Projeto) Especifique o tipo de visualização que os usuários verão ao acessarem essas informações na guia Detalhes. Por exemplo, você pode selecionar uma visualização de Marco ou Gantt.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Mostra este relatório em um gráfico Gantt por padrão</td> 
      <td>(Somente Relatório de Projeto e Relatório de Tarefa) Selecione esta opção para habilitar automaticamente a exibição de Gantt quando os usuários exibirem a guia Detalhes neste relatório.<br>Para obter mais informações sobre a exibição do Gráfico de Gantt em relatórios de projeto e relatórios de tarefa, consulte a seção "Exibir informações da tarefa no Gráfico de Gantt da lista de projetos" no artigo <a href="../../../manage-work/gantt-chart/use-the-gantt-chart/view-info-in-gantt.md" class="MCXref xref">Exibir informações no Gráfico de Gantt </a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Permitir que a visualização seja alterada no relatório</td> 
      <td>Selecione esta opção para permitir que os usuários alterem a Exibição ao executar o relatório.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Permitir que o grupo seja alterado no relatório</td> 
      <td>Selecione esta opção para permitir que os usuários alterem o Grupo ao executar o relatório.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Permitir que o filtro seja alterado no relatório</td> 
      <td>Selecione esta opção para permitir que os usuários alterem o Filtro ao executar o relatório.</td> 
     </tr> 
    </tbody> 
   </table>

1. Clique em **Prompts do relatório** para configurar qualquer prompt para o relatório.\
   Para obter mais informações sobre como adicionar prompts a um relatório, consulte o artigo [Adicionar um prompt a um relatório](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

1. Clique em **Concluído,** e clique em **Salvar + Fechar**.

## Informações adicionais

Consulte também:

<!--outdated: * [Basic Report Creation Program for the new Workfront experience](https://one.workfront.com/s/basic-report-creation-program) -->
* [Introdução a relatórios](../../../reports-and-dashboards/reports/reporting/get-started-reports-workfront.md)
* [Usar relatórios integrados do Adobe Workfront](../../../reports-and-dashboards/reports/using-built-in-reports/use-workfront-built-in-reports.md)
* [Criar um relatório personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)
