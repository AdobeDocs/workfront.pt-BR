---
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: Exibir todas as atualizações em um relatório de Nota
description: Exibir todas as atualizações em um relatório de Nota
author: Lisa and Alina
feature: Get Started with Workfront
exl-id: fa5b91e4-b88c-42f0-860c-6864105b4652
source-git-commit: 923c9e25fbd73c9d6a6a20436333c6e7969e9538
workflow-type: tm+mt
source-wordcount: '393'
ht-degree: 0%

---

# Exibir todas as atualizações em um relatório de Nota

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina: ***This is a report and it is in the Getting Started/ Updates section because I think it makes more sense to be in this area, where people want to view updates. - added this to this section from Reporting on 7/3/2018 ) </p>
-->

A área Atualizações de um objeto exibe um número máximo de 200 atualizações por padrão. Para visualizar todas as atualizações que qualquer usuário inseriu para um objeto, é possível criar um relatório de Nota que exibe todas as atualizações.

>[!NOTE]
>
>Você pode criar um relatório para exibir atualizações em objetos em Visualizar com o relatório de entrada do diário. Para obter mais informações, consulte [Relatório sobre a área Atualizações](../../reports-and-dashboards/reports/creating-and-managing-reports/create-journal-entry-report.md).

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Plano Adobe Workfront*</strong></td> 
   <td> <p>Qualquer Um</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Licença da Adobe Workfront*</strong></td> 
   <td> <p>Plano</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurações de nível de acesso*</strong></td> 
   <td> <p>Editar acesso a:</p> 
    <ul> 
     <li> <p>Criar relatórios, painéis e calendários</p> </li> 
     <li> <p>Criar filtros, visualizações e agrupamentos</p> </li> 
    </ul> <p>Observação: Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso.<br>Para obter informações sobre como um administrador do Workfront pode alterar seu nível de acesso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Permissões de objeto</strong></td> 
   <td> <p>Exibir</p> <p>Observação: Se você não tiver permissão de Exibição ou superior a um objeto, as informações desse objeto não serão exibidas no relatório.</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

## Criar um relatório de Nota

A criação de um relatório para Notas para qualquer objeto é idêntica, independentemente do objeto.

Por exemplo, para criar um relatório de Nota para todas as notas em um projeto:

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront.

1. Clique em **Relatórios**.
1. Clique em **Novo relatório** e escolha **Observação**.

1. (Opcional) Clique em **Exibições**, em seguida **Adicionar coluna** para adicionar o **Nome** do **Projeto** na exibição do relatório. 

1. (Opcional) Clique em **Agrupamentos**, em seguida **Adicionar agrupamento** para agrupar pela **Nome do projeto**, se estiver relatando vários projetos ao mesmo tempo.\
   Isso garante que as notas sejam agrupadas por seus respectivos projetos, facilitando a leitura do relatório. 

1. (Opcional) Clique em **Filtros,** then **Adicionar uma regra de filtro** para filtrar por apenas um projeto ou projetos específicos.

1. (Condicional e opcional) Defina o **Nome do projeto** as **Igual** para o nome do projeto para o qual você deseja visualizar as atualizações.  

1. Clique em **Salvar + Fechar**.\
   Todas as atualizações inseridas no projeto por todos os usuários com permissões para, pelo menos, Visualizar o projeto são exibidas no relatório.
