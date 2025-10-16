---
product-area: portfolios;projects
navigation-topic: portfolio-optimizer
title: Otimizar projetos no Portfolio Otimizer
description: Você pode usar o [!UICONTROL Portfolio Otimizer] para priorizar seus projetos com base em suas pontuações e outros valores. O Otimizer leva em consideração informações importantes do projeto, como custo, alinhamento, risco e ROI, para priorizar os projetos de acordo com o que é mais importante para você.
author: Alina
feature: Work Management, Strategic Planning
exl-id: 25debc5b-5d7d-453f-ab0a-9bf3fba05693
source-git-commit: d7600a55b3dffb242957234de9d85a0deb1ad2e3
workflow-type: tm+mt
source-wordcount: '468'
ht-degree: 0%

---

# Otimizar projetos no [!UICONTROL Portfolio Otimizer]

Você pode usar o [!UICONTROL Portfolio Otimizer] para priorizar seus projetos com base em suas pontuações e outros valores. O [!UICONTROL Otimizer] leva em consideração informações importantes do projeto, como custo, alinhamento, risco e ROI, para priorizar os projetos de acordo com o que é mais importante para você.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo. 

Você deve ter o seguinte acesso para executar as etapas deste artigo:

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

<!--Old
<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td> Any</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront licenses*</td> 
   <td> <p>New: [!UICONTROL Standard] </p>
   <p>Current: [!UICONTROL Plan] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>[!UICONTROL Edit] access to Projects and Portfolios</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>[!UICONTROL Manage] permissions to the portfolio</p> <p>Contribute or higher permissions to the projects</p> 
   <p>You must have Manage permissions to all the projects in the list to be able to use <b>Set project priority</b>.</p>
    </td> 
  </tr> 
 </tbody> 
</table>-->

## Otimizar projetos no Portfolio Otimizer

1. Abra uma Portfolio e clique em **[!UICONTROL Otimização do Portfolio]** no painel esquerdo.

   O [!UICONTROL Portfolio Otimizer] é exibido.

1. Clique no ícone **[!UICONTROL Otimizar]**.

   ![Ícone Otimizar](assets/optimize-icon-portfolio-optimizer.png)

   As categorias pelas quais um projeto pode ser pontuado são exibidas à esquerda do ícone [!UICONTROL Otimizar].

1. Usando o círculo deslizante, modifique a otimização de qualquer uma das seguintes categorias:

   * **[!UICONTROL Baixo Custo]**: mova o controle deslizante para a direita para visualizar projetos com o [!UICONTROL Custo Planejado] mais baixo.
   * **[!UICONTROL Alto alinhamento]**: mova o controle deslizante para a direita para visualizar os projetos com o maior alinhamento com base no [!UICONTROL Scorecard].
   * **[!UICONTROL Valor Alto]**: mova o controle deslizante para a direita para ver projetos com uma pontuação de [!UICONTROL Valor Líquido] mais alta.
   * **[!UICONTROL Baixo Risco para Benefícios]**: mova o controle deslizante para a direita para visualizar projetos com a menor taxa de risco para benefício.
   * **[!UICONTROL ROI alto]**: mova o controle deslizante para a direita para visualizar projetos com ROI (Return On Investment, retorno sobre o investimento) mais alto.

1. Clique no ícone **x** para fechar as categorias de otimização.

   Isso atualiza os valores de [!UICONTROL Pontuação] para cada projeto na coluna **[!UICONTROL Pontuação]**.

   Para obter informações sobre a [!UICONTROL Pontuação do Portfolio Otimizer], consulte [Visão geral da [!UICONTROL Pontuação do Portfolio Otimizer]](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-score.md).

1. Depois que os pesos corretos forem definidos para a coluna **[!UICONTROL Score]**, clique no cabeçalho da coluna **[!UICONTROL Score]** para classificar por essa coluna. O projeto com a pontuação mais alta é exibido na parte superior da lista.

1. (Opcional) Arraste e solte projetos na ordem de sua prioridade.
Isso alterará a ordem dos projetos no [!UICONTROL Portfolio Otimizer].
1. (Opcional) Clique em **[!UICONTROL Definir prioridade]** para salvar a nova prioridade dos projetos.

   >[!NOTE]
   >
   >   Você deve ter permissões de Gerenciamento para todos os projetos da lista para poder usar **Definir prioridade de projeto**.

   Para obter mais informações sobre a priorização de projetos no [!UICONTROL Portfolio Otimizer], consulte o artigo [Priorizar projetos no [!UICONTROL Portfolio Otimizer]](../../../manage-work/portfolios/portfolio-optimizer/prioritize-projects-in-portfolio-optimizer.md).

1. Clique em **[!UICONTROL Salvar]** para salvar o [!UICONTROL Portfolio Otimizer].
