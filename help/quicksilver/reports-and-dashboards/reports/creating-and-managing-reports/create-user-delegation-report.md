---
product-area: reporting
keywords: usuário,delegação,relatório,delegado,aprovação
navigation-topic: create-and-manage-reports
title: Criar um relatório de delegação de usuários
description: Criar um relatório de delegação de usuários
author: Nolan
feature: Reports and Dashboards
exl-id: c860574b-0488-499e-8d36-d0f3f85aac2d
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '383'
ht-degree: 3%

---

# Criar um relatório de delegação de usuários

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: consider moving this to the Custom&nbsp;View, Filter, Grouping Samples section as an example of a report)</p>
-->

No Adobe Workfront, os usuários podem delegar projetos, tarefas e emitir aprovações a outros usuários para garantir que suas aprovações sejam gerenciadas quando estiverem fora do escritório. Os usuários com uma licença de Plano podem criar um relatório de Delegação de Usuário para ver:

* Quem delegou sua tarefa, emissão e aprovações de projeto a outro usuário
* Quais usuários delegaram aprovações de tarefa, emissão e projeto atribuídas a eles

* Datas de início e fim das delegações

Para saber mais sobre a delegação de aprovações, consulte [Delegar solicitação de aprovação](../../../review-and-approve-work/manage-approvals/delegate-approval-requests.md).

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">DRAFTED: To learn more about delegating work, see <a href="../../../workfront-basics/manage-your-account-and-profile/manage-time-off/personal-time-off.md" class="MCXref xref">Log personal time off and delegate your work</a>.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">DRAFTED: To learn how to manage delegated work in Home, see [future link here].</p>
-->

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
   <td> <p>Exibir permissões para os itens cujas aprovações são delegadas e para os usuários envolvidos na delegação</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

## Criar um relatório de delegação de usuário

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront, em seguida, clique em **Relatórios**.

1. Clique em **Novo relatório**, em seguida selecione **Delegação de usuários**.\
   ![](assets/classic-new-report-user-delegation-350x644.png)

   Os seguintes campos são exibidos neste relatório por padrão:

   | Campo | Descrição |
   |---|---|
   | **Do usuário** | Esse é o usuário que está delegando suas aprovações de tarefa, emissão e projeto a outro usuário. |
   | **Para o usuário** | Esse é o usuário que tem aprovações de tarefa, emissão e projeto delegadas a ele. |
   | **Início** | Este é o início do tempo esgotado para o usuário que fez as delegações. |
   | **Fim** | Este é o fim do tempo limite para o usuário que fez as delegações. |

   {style="table-layout:auto"}

1. (Opcional) No Construtor de relatórios, modifique o seguinte:

   * Colunas
   * Agrupamento
   * Filtros
   * Gráfico

   Para saber mais sobre esses recursos, consulte [Criar um relatório personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. Após concluir a criação do relatório, clique em **Salvar + Fechar**.

1. Insira um novo nome no **Nome do relatório** e clique em **Salvar relatório**.

   O relatório é exibido.
