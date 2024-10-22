---
navigation-topic: business-case-and-scorecards
title: Aprovar um Business Case
description: Depois de concluir e enviar o Business Case para uma solicitação de projeto, o Business Case deve ser aprovado. Depende do workflow em sua organização. Um projeto pode ser iniciado sem a aprovação do Business Case, mas o administrador e os proprietários do projeto do Adobe Workfront podem não considerar ideal.
author: Alina
feature: Work Management
exl-id: 60abb054-5cb0-4dd6-9091-c9dcd635a630
source-git-commit: 2def8297fe606adaeaef6cc079b718531377919d
workflow-type: tm+mt
source-wordcount: '733'
ht-degree: 0%

---

# Aprovar um Business Case

Depois de concluir e enviar o Business Case para uma solicitação de projeto, o Business Case deve ser aprovado. Depende do workflow em sua organização. Um projeto pode ser iniciado sem a aprovação do Business Case, mas o administrador e os proprietários do projeto do Adobe Workfront podem não considerar ideal.

Para obter mais informações sobre como concluir e enviar um Business Case, consulte o artigo [Criar um Business Case para um projeto](../../../manage-work/projects/define-a-business-case/create-business-case.md).

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront*</td> 
   <td> <p>Pro ou superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Plano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a projetos</p> <p>Observação: se você ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões para um projeto</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso aos objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qual plano, tipo de licença ou acesso você tem, contate o administrador do Workfront.

## Visão geral da aprovação do Business Case

Considere o seguinte ao aprovar um Business Case de um projeto:

* Você deve ter permissões de gerenciamento para um projeto para aprovar o Business Case para ele.
* Você não poderá ver os projetos que estão aguardando a aprovação do Business Case no widget Minhas aprovações na Página inicial.
* Você deve ir manualmente para os projetos individuais que precisam de aprovação do Business Case para ver que eles estão pendentes de aprovação. Não há um mecanismo de notificação do Workfront que alerta alguém que deve aprovar o Business Case de um projeto.
* Você pode encontrar os projetos que estão aguardando a aprovação do Business Case criando um relatório de projeto ou acessando o portfólio ao qual estão associados.

  Para obter mais informações sobre Portfolio, consulte o artigo [Visão geral sobre Portfolio no Adobe Workfront](../../../manage-work/portfolios/portfolios-overview/portfolio-overview.md).

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

   para exibir onde você está designado como Gerenciador de Portfolio.

1. Clique em **Salvar+Fechar**.

   Observe que todos os projetos no relatório estão no status de **Solicitado**.

1. Clique no nome de um projeto no relatório para abri-lo.
1. Clique em **Business Case** no painel esquerdo.
1. Clique em **Aprovar** ou **Rejeitar** na área Resumo do Business Case para aprovar ou rejeitar o Business Case.

   ![](assets/business-case-summary-with-rp-information--1-.png)

   O status do projeto será alterado para **Aprovado** se o Business Case for aprovado.

   O status do projeto será alterado para **Rejeitado** se o Plano de Negócio for rejeitado.

   >[!NOTE]
   >
   >Não há notificações que alertem o usuário que enviou a aprovação do business case se a solicitação do projeto foi aprovada ou rejeitada.

## Aprove o business case acessando os projetos solicitados em um portfólio

Para obter mais informações sobre como revisar Projetos solicitados, consulte o artigo [Revisar projetos solicitados](../../../manage-work/portfolios/create-and-manage-portfolios/review-requested-projects.md).
