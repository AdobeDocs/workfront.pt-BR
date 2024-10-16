---
product-area: reporting
keywords: usuário,delegação,relatório,delegado,aprovação
navigation-topic: create-and-manage-reports
title: Criar um relatório de delegação de usuário
description: Criar um relatório de delegação de usuário
author: Nolan
feature: Reports and Dashboards
exl-id: c860574b-0488-499e-8d36-d0f3f85aac2d
source-git-commit: f7ad56375c20e26b0d45ae0966e2e156b5a200f1
workflow-type: tm+mt
source-wordcount: '383'
ht-degree: 1%

---

# Criar um relatório de delegação de usuário

<!--Audited: 10/2024-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: consider moving this to the Custom&nbsp;View, Filter, Grouping Samples section as an example of a report)</p>
-->

No Adobe Workfront, os usuários podem delegar aprovações de projetos, tarefas e problemas a outros usuários para garantir que suas aprovações sejam gerenciadas quando estiverem fora do escritório. Os usuários com uma licença de Plano podem criar um relatório de Delegação de usuários para ver:

* Quem delegou as aprovações de tarefas, problemas e projetos a outro usuário
* Quais usuários delegaram as aprovações de tarefas, problemas e projetos a eles

* As datas de início e término das delegações

Para saber mais sobre delegação de aprovações, consulte [Delegar solicitação de aprovação](../../../review-and-approve-work/manage-approvals/delegate-approval-requests.md).

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">DRAFTED: To learn more about delegating work, see <a href="../../../workfront-basics/manage-your-account-and-profile/manage-time-off/personal-time-off.md" class="MCXref xref">Log personal time off and delegate your work</a>.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">DRAFTED: To learn how to manage delegated work in Home, see [future link here].</p>
-->

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Novo: Padrão </p>
   <p>Atual: Plano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a relatórios, painéis, calendários</p> <p>Editar acesso a Filtros, Visualizações, Agrupamentos</p> <p>Observação: se você ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Exibir permissões para os itens cujas aprovações são delegadas e para os usuários envolvidos na delegação</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso aos objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Para descobrir que plano, tipo de licença ou acesso você tem, entre em contato com o administrador do Workfront.
+++

## Criar um relatório de delegação de usuário

1. Clique no ícone ![](assets/main-menu-icon.png) do **Menu principal** no canto superior direito do Adobe Workfront e em **Relatórios**.

1. Clique em **Novo relatório** e selecione **Delegação de usuários**.\
   ![](assets/classic-new-report-user-delegation-350x644.png)

   Os seguintes campos são exibidos neste relatório por padrão:

   | Campo | Descrição |
   |---|---|
   | **Do Usuário** | Este é o usuário que está delegando suas aprovações de tarefas, problemas e projetos a outro usuário. |
   | **Para Usuário** | Esse é o usuário que tem as aprovações de tarefas, problemas e projetos delegadas a ele. |
   | **Data de Início** | Este é o início do tempo de ausência temporária do usuário que fez as delegações. |
   | **Data de término** | Esse é o fim do tempo de ausência temporária do usuário que fez as delegações. |

   {style="table-layout:auto"}

1. (Opcional) No Report Builder, modifique o seguinte:

   * Colunas (visualizar)
   * Agrupamento
   * Filtros
   * Gráfico

   Para saber mais sobre esses recursos, consulte [Criar um relatório personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. Depois de terminar de criar o relatório, clique em **Salvar + Fechar**.

   O relatório é exibido.
