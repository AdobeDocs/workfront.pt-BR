---
navigation-topic: business-case-and-scorecards
title: Aprovar um caso comercial
description: Depois de concluir e enviar o Caso de negócios para uma solicitação de projeto, o Caso de negócios deve ser aprovado. Isso depende do fluxo de trabalho na organização. Um projeto pode ser iniciado sem que o Caso de negócios precise ser aprovado, mas o administrador do Adobe Workfront e os proprietários do projeto podem não considerar ideal fazê-lo.
author: Alina
feature: Work Management
exl-id: 60abb054-5cb0-4dd6-9091-c9dcd635a630
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '733'
ht-degree: 0%

---

# Aprovar um caso comercial

Depois de concluir e enviar o Caso de negócios para uma solicitação de projeto, o Caso de negócios deve ser aprovado. Isso depende do fluxo de trabalho na organização. Um projeto pode ser iniciado sem que o Caso de negócios precise ser aprovado, mas o administrador do Adobe Workfront e os proprietários do projeto podem não considerar ideal fazê-lo. 

Para obter mais informações sobre como concluir e enviar um Caso de Negócios, consulte o artigo [Criar um caso de negócios para um projeto](../../../manage-work/projects/define-a-business-case/create-business-case.md).

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plano Adobe Workfront*</td> 
   <td> <p>Pro ou superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Plano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a Projetos</p> <p>Observação: Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões de um projeto</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

## Visão geral da aprovação do Business Case

Considere o seguinte ao aprovar um Caso de negócios de um projeto:

* Você deve ter permissões de gerenciamento para um projeto para aprovar o Caso de negócios para ele. 
* Você não poderá ver os projetos que estão esperando que o Caso de negócios seja aprovado em suas Aprovações em Início.
* Você deve acessar manualmente os projetos individuais que precisam de aprovação de Caso de negócios para ver se estão pendentes de aprovação. Não há um mecanismo de notificação do Workfront que alerta alguém de que ele deve aprovar o Caso de negócios de um projeto.
* Você pode encontrar os projetos aguardando a aprovação do Caso de negócios criando um relatório de projeto ou acessando o portfólio ao qual eles estão associados. 

   Para obter mais informações sobre o Portfolio, consulte o artigo [Visão geral do Portfolio no Adobe Workfront](../../../manage-work/portfolios/portfolios-overview/portfolio-overview.md).

## Aprovar o caso de negócios criando um relatório de projeto

Você pode criar um relatório para projetos para ver quais projetos precisam que seu Caso de negócios seja aprovado. 

Para criar um relatório para projetos que estão aguardando aprovação de seus Casos de negócios:

1. Crie um relatório para projetos.

   Para obter mais informações sobre como criar relatórios, consulte o artigo [Criar um relatório personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. Selecione o **Exibir** do relatório e clique em **Adicionar coluna**.

1. Comece a digitar &quot;Status&quot; no **Mostrar nesta coluna** e selecione esse campo quando ele aparecer na lista.

    Essa coluna exibirá o status dos projetos.

1. Selecione o **Filtros** do relatório e clique em **Adicionar uma regra de filtro**.

1. Comece a digitar &quot;Status&quot; no **Mostrar somente projetos nos quais...** e selecione-o quando aparecer na lista.
1. Selecionar **Igual** para o modificador de filtro.
1. Comece digitando &quot;Requested&quot; no campo disponível. 

   Isso garante que o relatório inclua apenas projetos que estejam no status Solicitado.

     ![requested_projects_filter.png](assets/requested-projects-filter-350x14.png)

1. (Opcional) Clique em **Adicionar outra regra de filtro**.

   Você pode adicionar filtros adicionais, para mostrar apenas projetos em que você é o Proprietário do projeto, o Patrocinador do projeto ou o Proprietário do Portfolio.

   Por exemplo, você pode usar as seguintes instruções de filtro: 

   ```
   Project Sponsor ID Equals $$USER.ID
   ```

   para exibir projetos nos quais você é designado como Patrocinador do Projeto

   ```
   Project Owner ID Equals $$USER.ID
   ```

   para exibir projetos nos quais você é designado como proprietário do projeto

   ```
   Project Portfolio Owner ID Equals $$USER. ID
   ```

   para exibir onde você é designado como o Portfolio Manager. 

1. Clique em **Salvar+Fechar**.

   Observe que todos os projetos do relatório estão no status de **Solicitado**.

1. Clique no nome de um projeto no relatório para abri-lo.
1. Clique em **Caso de negócios** no painel esquerdo.
1. Clique em **Aprovar** ou **Rejeitar** na área Resumo do caso comercial para aprovar ou rejeitar o caso comercial. 

   ![](assets/business-case-summary-with-rp-information--1-.png)

   O status do projeto é alterado para **Aprovado** se o Caso de negócios for aprovado.

   O status do projeto é alterado para **Rejeitada** se o caso comercial for rejeitado.

   >[!NOTE]
   >
   >Não há notificações que alertem o usuário que enviou a aprovação do caso comercial se a solicitação de projeto foi aprovada ou rejeitada.

## Aprove o caso de negócios acessando projetos solicitados em um portfólio

Para obter mais informações sobre como revisar projetos solicitados, consulte o artigo [Revisar projetos solicitados](../../../manage-work/portfolios/create-and-manage-portfolios/review-requested-projects.md).
