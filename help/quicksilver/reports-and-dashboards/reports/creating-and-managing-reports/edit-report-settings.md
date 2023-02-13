---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Editar configurações de relatório
description: É possível editar as configurações de um relatório para definir como ele é exibido para outros usuários ou que tipo de informação os usuários podem solicitar antes de executar o relatório.
author: Nolan
feature: Reports and Dashboards
exl-id: 6fbbc557-65da-4ffe-968a-9c8db6a45811
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '677'
ht-degree: 9%

---

# Editar configurações de relatório

É possível editar as configurações de um relatório para definir como ele é exibido para outros usuários ou que tipo de informação os usuários podem solicitar antes de executar o relatório.

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

## Etapas de instruções

1. Comece a criar um relatório acessando o **Menu principal** > **Relatórios**, em seguida, selecione o objeto do relatório.

   Ou

   Abra um relatório existente e clique em **Ações de Relatório** > **Editar**.

1. Clique em **Configurações do relatório** no canto superior direito do construtor de relatórios.
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
      <td>Especifique uma declaração descrevendo a finalidade e os usos do relatório.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Executar este relatório com direitos de acesso de</td> 
      <td>Selecione o usuário cujos direitos de acesso você deseja que esse relatório use ao exibir para outros usuários. Para obter mais informações sobre como executar um relatório com os direitos de acesso de outro usuário, consulte o artigo <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/run-deliver-report-access-rights-another-user.md" class="MCXref xref">Executar e entregar um relatório com os direitos de acesso de outro usuário</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Quando o relatório for carregado, mostrar</td> 
      <td>Selecione a guia padrão que é exibida para todos os usuários quando o relatório é carregado.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Quando o relatório é carregado em um painel, mostrar ... itens</td> 
      <td>Especifique o número de itens que são exibidos para todos os usuários quando o relatório é carregado em um painel. O padrão é 15 itens e o número máximo de itens é 200.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Mostrar a exibição Grade de Recurso na guia Detalhes</td> 
      <td> <p>(Somente Relatório do Usuário) Selecione esta opção para exibir a Grade de Recurso na guia Detalhes do relatório.</p> <p>Observação: Ao aplicar a exibição Grade de Recurso a um relatório de usuário, o relatório mostra somente os projetos que estão no status Atual. Se quiser ver projetos em qualquer outro status, use a Guia Utilização do Usuário na área Pessoas da Barra de Navegação Global e aplique a Exibição de Grade de Recurso lá. <!--
         <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
          For more information about using the Resource Grid, see the article Overview of the Resource Grid . (drafted because this article is drafted also: Article is in draft Feb 1, 2021)
         </MadCap:conditionalText>
        --></p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Mostrar uma visualização especial na guia Detalhes</td> 
      <td>(Somente Relatório do projeto) Especifique o tipo de exibição que os usuários verão quando acessarem essas informações na guia Detalhes. Por exemplo, é possível selecionar uma visualização de Marco ou Gantt.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Mostra este relatório em um gráfico Gantt por padrão</td> 
      <td>(Somente Relatório de projeto e Relatório de tarefa) Selecione essa opção para que a exibição de Gantt seja ativada automaticamente quando os usuários visualizarem a guia Detalhes neste relatório.<br>Para obter mais informações sobre como visualizar o gráfico de Gantt em relatórios de projeto e relatórios de tarefa, consulte a seção "Exibir informações da tarefa na lista de projetos Gráfico de Gantt" no artigo <a href="../../../manage-work/gantt-chart/use-the-gantt-chart/view-info-in-gantt.md" class="MCXref xref">Exibir informações no Gráfico de Gantt </a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Permitir que a visualização seja alterada no relatório</td> 
      <td>Selecione essa opção para permitir que os usuários alterem a Exibição ao executar o relatório.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Permitir que o grupo seja alterado no relatório</td> 
      <td>Selecione essa opção para permitir que os usuários alterem o Grupo ao executar o relatório.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Permitir que o filtro seja alterado no relatório</td> 
      <td>Selecione essa opção para permitir que os usuários alterem o Filtro ao executar o relatório.</td> 
     </tr> 
    </tbody> 
   </table>

1. Clique em **Avisos de Relatório** para configurar qualquer solicitação para o relatório.\
   Para obter mais informações sobre como adicionar prompts a um relatório, consulte o artigo [Adicionar um prompt a um relatório](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

1. Clique em **Feito,** em seguida, clique em **Salvar + Fechar**.

## Informações adicionais

Consulte também:

* [Programa básico de criação de relatórios para a nova experiência do Workfront](https://one.workfront.com/s/basic-report-creation-program)
* [Introdução a relatórios no Adobe Workfront](../../../reports-and-dashboards/reports/reporting/get-started-reports-workfront.md)
* [Usar relatórios internos do Adobe Workfront](../../../reports-and-dashboards/reports/using-built-in-reports/use-workfront-built-in-reports.md)
* [Criar um relatório personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)
