---
title: Priorizar projetos no Portfolio Otimizer
product-area: portfolios;projects
navigation-topic: portfolio-optimizer
description: É possível priorizar os projetos no Portfolio Otimizer para estabelecer a ordem em que eles devem ser concluídos.
author: Alina
feature: Work Management, Strategic Planning
exl-id: 54e33746-5995-49de-8e21-bf973f0694a6
source-git-commit: 714e6e09f1429f0382c36d17d3f2aca95edcfbc6
workflow-type: tm+mt
source-wordcount: '491'
ht-degree: 2%

---

# Priorizar projetos no [!UICONTROL Portfolio Otimizer]

É possível priorizar os projetos no [!UICONTROL Portfolio Otimizer] para estabelecer a ordem em que eles devem ser concluídos.

Considere o seguinte ao usar o [!UICONTROL Portfolio Otimizer]:

* Os projetos na parte superior do [!UICONTROL Portfolio Otimizer] são considerados mais importantes do que os listados na parte inferior. Você precisará concluir os projetos na ordem de prioridade no [!UICONTROL Portfolio Otimizer] para que o Portfolio seja otimizado.
* A prioridade de projetos no [!UICONTROL Portfolio Otimizer] não está relacionada ao campo [!UICONTROL Prioridade] localizado na guia [!UICONTROL Detalhes do Projeto] de um projeto.

  O campo [!UICONTROL Prioridade] da guia [!UICONTROL Detalhes do Projeto] é um sinalizador visual especificado manualmente para entender a importância que um projeto deve ter.

* A prioridade de projetos no Portfolio Otimizer fica visível no [!DNL Resource Planner], se ela estiver ativada lá. No [!DNL Resource Planner], os projetos recebem recursos na ordem de prioridade [!UICONTROL Planejador de recursos], e não na [!UICONTROL Prioridade do Portfolio].

  Para obter informações sobre a priorização de projetos no [!UICONTROL Planejador de recursos], consulte o artigo [Priorizar projetos no [!UICONTROL Planejador de recursos]](../../../resource-mgmt/resource-planning/prioritize-projects-resource-planner.md).

* A área **[!UICONTROL Priorização de Projetos]** do [!UICONTROL Portfolio Otimizer] exibe os projetos na ordem de [!UICONTROL Datas de Início Planejadas] e [!UICONTROL Valor Líquido], por padrão.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] pacote</td> 
   <td> <p>Workfront Prime ou superior</p>
      <p>Fluxo de trabalho Prime ou superior</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licença</td> 
   <td> <p>[!UICONTROL Padrão]</p>
   <p>[!UICONTROL Plano]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>[!UICONTROL Editar] acesso a [!UICONTROL Portfólios] e [!UICONTROL Projetos]</p>  </td>
</tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Permissões do [!UICONTROL Manager] para o portfólio</p>  </td> 
  </tr> 
 </tbody> 
</table>

*Para obter informações, consulte [Requisitos de acesso para a documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront licenses*</td> 
   <td> <p>New: Standard</p>
   <p>Current: Plan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>[!UICONTROL Edit] access to Projects and Portfolios</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>[!UICONTROL Manage] permissions to the portfolio</p> <p>Contribute or higher permissions to the projects</p> 
   <p>You must have Manage permissions to all the projects in the list to be able to use <b>Set project priority</b>.</p>
    </td> 
  </tr> 
 </tbody> 
</table>-->

## Alterar a prioridade dos projetos no [!UICONTROL Portfolio Otimizer]

{{step1-to-portfolios}}

1. (Opcional) Selecione o filtro correto no menu suspenso **[!UICONTROL Filtro]** para exibir a lista correta de portfólios.
1. Clique no nome de um portfólio para abri-lo.
1. Clique em **[!UICONTROL Otimização do Portfolio]** no painel esquerdo.
1. Na área [!UICONTROL optização de projeto], altere a prioridade dos projetos arrastando os projetos na ordem de prioridade e soltando-os para a posição de exibição desejada.

   ![Otimizador do Portfolio com projetos](assets/portfolio-optimizer-with-projects-nwe-350x89.png)

   Clique em **[!UICONTROL Definir Prioridade]** na área de otimização do projeto quando você terminar de reorganizar os projetos. Os projetos receberão um novo número com base no novo pedido.

1. Clique em **[!UICONTROL Salvar]** para salvar a nova prioridade de projeto no [!UICONTROL Portfolio Otimizer]. A prioridade está listada como um número na coluna número **#**.

   >[!TIP]
   >
   >Isso não altera necessariamente a ordem dos projetos no [!UICONTROL Portfolio Otimizer], pois a lista de projetos pode ser classificada por uma coluna diferente da coluna **#**. Clique no cabeçalho da coluna **#** para ordenar a lista por prioridade de projeto.

   Você pode ver a prioridade do projeto como ela aparece no [!UICONTROL Portfolio Otimizer] no Planejador de Recursos, habilitando a configuração **[!UICONTROL Exibir Prioridades do Portfolio]** no Planejador de Recursos.

   Para obter informações sobre a priorização de projetos no [!UICONTROL Planejador de recursos], consulte o artigo [Priorizar projetos no [!UICONTROL Planejador de recursos]](../../../resource-mgmt/resource-planning/prioritize-projects-resource-planner.md).
