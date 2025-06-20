---
navigation-topic: business-case-and-scorecards
title: Aprovar um Business Case
description: Depois de concluir e enviar o Business Case para uma solicitação de projeto, o Business Case deve ser aprovado. Depende do workflow em sua organização. Um projeto pode ser iniciado sem a aprovação do Business Case, mas o administrador e os proprietários do projeto do Adobe Workfront podem não considerar ideal.
author: Alina
feature: Work Management
exl-id: 60abb054-5cb0-4dd6-9091-c9dcd635a630
source-git-commit: f97c989f57d864252adf6e24f8e6b03f56d26901
workflow-type: tm+mt
source-wordcount: '692'
ht-degree: 0%

---

# Aprovar um Business Case

<!--Audit: 6/2025-->

Depois de concluir e enviar o Business Case para uma solicitação de projeto, o Business Case deve ser aprovado. Depende do workflow em sua organização. Um projeto pode ser iniciado sem a aprovação do Business Case, mas o administrador e os proprietários do projeto do Adobe Workfront podem não considerar ideal.

Para obter mais informações sobre como concluir e enviar um Business Case, consulte o artigo [Criar um Business Case para um projeto](../../../manage-work/projects/define-a-business-case/create-business-case.md).

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><p>plano do Adobe Workfront*</p></td> 
   <td> 
   <p>Atual: Prime ou superior</p>
   <p>ou</p>
   <p>Herdados: Business ou superior</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> 
   <p>Atual: Padrão </p> 
   <p>Herdados: plano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Editar acesso a projetos</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Permissões de objeto</p></td> 
   <td> <p>Gerenciar permissões para um projeto</p> <p>Exibir ou aumentar as permissões de um portfólio</p>  </td> 
  </tr> 
 </tbody> 
</table>

*Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Visão geral da aprovação do Business Case

Considere o seguinte ao aprovar um Business Case de um projeto:

* Você deve ter permissões de gerenciamento para um projeto para aprovar o Business Case para ele.
* Você não poderá ver os projetos que estão aguardando a aprovação do Business Case no widget Minhas aprovações na Página inicial.
* Você deve ir manualmente para os projetos individuais que precisam de aprovação do Business Case para ver que eles estão pendentes de aprovação. Não há um mecanismo de notificação do Workfront que alerta alguém que deve aprovar o Business Case de um projeto.
* Você pode encontrar os projetos que estão aguardando a aprovação do Business Case criando um relatório de projeto ou acessando o portfólio ao qual estão associados.

  Para obter mais informações sobre Portfólios, consulte o artigo [Visão geral do Portfolio no Adobe Workfront](../../../manage-work/portfolios/portfolios-overview/portfolio-overview.md).

## Aprove o Business Case criando um relatório de projeto

Você pode criar um relatório para projetos para ver quais projetos precisam de sua Business Case aprovada.

Para criar um relatório para projetos que estão pendentes de aprovação de seus Casos de Negócios:

1. Criar um relatório de projetos.

   Para obter mais informações sobre como criar relatórios, consulte o artigo [Criar um relatório personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. Selecione a guia **Exibir** do relatório e clique em **Adicionar coluna**.

1. Comece digitando &quot;Status&quot; no campo **Mostrar nesta coluna** e selecione este campo quando ele aparecer na lista.

   Essa coluna exibirá o status dos projetos.

1. Selecione a guia **Filtros** do relatório e clique em **Adicionar uma Regra de Filtro**.

1. Comece digitando &quot;Status&quot; em **Mostrar apenas projetos em que o campo ...** está e selecione-o quando ele aparecer na lista.
1. Selecione **Igual** para o modificador de filtro.
1. Comece a digitar &quot;Solicitado&quot; no campo disponível.

   Isso garante que o relatório inclua apenas projetos que estejam no status Solicitado.

   ![requested_projects_filter.png](assets/requested-projects-filter-350x14.png)

1. (Opcional) Clique em **Adicionar outra regra de filtro**.

   É possível adicionar filtros extras, para mostrar apenas os projetos em que você é o Proprietário do projeto, o Patrocinador do projeto ou o Proprietário do Portfolio.

   Por exemplo, você pode usar as seguintes instruções de filtro:

   ```
   Project Sponsor ID Equals $$USER.ID
   ```

   para exibir projetos designados como Patrocinadores do Projeto

   ```
   Project Owner ID Equals $$USER.ID
   ```

   para exibir projetos em que você é designado como proprietário do Projeto

   ```
   Project Portfolio Owner ID Equals $$USER. ID
   ```

   para exibir onde você está designado como o Portfolio Manager.

1. Clique em **Salvar+Fechar**.

   Observe que todos os projetos no relatório estão no status de **Solicitado**.

1. Clique no nome de um projeto no relatório para abri-lo.
1. Clique em **Business Case** no painel esquerdo.
1. Clique em **Aprovar** ou **Rejeitar** na área Resumo do Business Case para aprovar ou rejeitar o Business Case.

   ![Caso de negócios](assets/business-case-summary-with-rp-information--1-.png)

   O status do projeto será alterado para **Aprovado** se o Business Case for aprovado.

   O status do projeto será alterado para **Rejeitado** se o Plano de Negócio for rejeitado.

   >[!NOTE]
   >
   >Não há notificações que alertem o usuário que enviou a aprovação do business case se a solicitação do projeto foi aprovada ou rejeitada.

## Aprove o business case acessando os projetos solicitados em um portfólio

Para obter mais informações sobre como revisar Projetos solicitados, consulte o artigo [Revisar projetos solicitados](../../../manage-work/portfolios/create-and-manage-portfolios/review-requested-projects.md).
