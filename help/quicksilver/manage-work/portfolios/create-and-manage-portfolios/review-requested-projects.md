---
product-area: portfolios;projects
navigation-topic: create-and-manage-portfolios
title: Revisar projetos solicitados
description: As solicitações de projeto são exibidas como projetos com status [!UICONTROL Solicitado] no Adobe Workfront. Este artigo descreve como revisar solicitações de projeto.
author: Alina
feature: Work Management, Strategic Planning
exl-id: 1acfb885-0da3-495d-ba66-e80e339e90de
source-git-commit: 7fef704355fad677f2bdf40e630ea0146a9e1d58
workflow-type: tm+mt
source-wordcount: '427'
ht-degree: 0%

---

# Revisar projetos solicitados

<!--Audited: 10/2025-->

Quando várias solicitações de projeto são enviadas para revisão, o escritório de gerenciamento de projetos ou o comitê do portfólio pode se reunir para revisar as solicitações enviadas e determinar as aprovações das solicitações do projeto. As solicitações de projeto são exibidas como projetos com status [!UICONTROL Solicitado] em [!DNL Adobe Workfront].

Você pode submeter uma solicitação de projeto para revisão seguindo um destes procedimentos:

* Alterar o status do projeto para **[!UICONTROL Solicitado]**.
* Conclua o [!UICONTROL Business Case] do projeto e envie-o para aprovação.\
   Para obter mais informações sobre como concluir um Plano de Negócio para um projeto, consulte [Criar um Plano de Negócio para um projeto](../../../manage-work/projects/define-a-business-case/create-business-case.md).

Você pode revisar projetos solicitados nas seguintes áreas do [!DNL Adobe Workfront]:

* Em um relatório de projeto
* Em um portfólio

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] pacote</td> 
   <td><p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licença</td> 
   <td> <p>[!UICONTROL Padrão] </p> 
   <p>[!UICONTROL Plano]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Acesso de [!UICONTROL View] ou superior a Portfólios</p> <p>[!UICONTROL Editar] acesso a Projetos</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Permissões de [!UICONTROL View] ou superiores no portfólio</p> <p>Permissões [!UICONTROL Manage] nos projetos para atualizar seu status</p>  </td> 
  </tr> 
 </tbody> 
</table>

*Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td><p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td> <p>[!UICONTROL Plan] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>[!UICONTROL View] access or higher to Portfolios</p> <p>[!UICONTROL Edit] access to Projects</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>[!UICONTROL View] permissions or higher on the portfolio</p> <p>[!UICONTROL Manage] permissions on the projects to update their status</p>  </td> 
  </tr> 
 </tbody> 
</table>-->

## Revisar projetos solicitados em um relatório de projeto

Você pode criar um relatório para projetos para ver quais projetos têm status de [!UICONTROL Solicitado].

Para obter mais informações sobre como aprovar solicitações de projeto criando um relatório de projeto, consulte a seção [[!UICONTROL Aprovando o Business Case Criando um Relatório de Projeto]](../../../manage-work/projects/define-a-business-case/approve-business-case.md#build-a-report) em [Aprovar um Business Case](../../../manage-work/projects/define-a-business-case/approve-business-case.md).

## Revisar projetos solicitados em um portfólio

1. Vá para o portfólio cujos projetos solicitados você deseja revisar.
1. Clique em **[!UICONTROL Projetos]** no painel esquerdo
1. No menu suspenso **[!UICONTROL Filtro]**, selecione **[!UICONTROL Solicitado]**.

   Somente projetos com status **[!UICONTROL Solicitado]** são exibidos na lista.

   >[!TIP]
   >
   > Além de ter o Status de **[!UICONTROL Solicitado]**, os projetos devem ser associados ao Portfolio selecionado para serem exibidos nesta lista.

1. Clique no nome de um projeto na lista para abri-lo.
1. Clique em **[!UICONTROL Detalhes do projeto]** no painel esquerdo.
1. Siga um destes procedimentos:

   * Clique em **[!UICONTROL Business Case]** e em **[!UICONTROL Aprovar]** ou **[!UICONTROL Rejeitar]** na área [!UICONTROL Resumo de Business Case] para aprovar ou rejeitar o Business Case.

     ![approve_or_reject_business_case.png](assets/approve-or-reject-business-case-350x563.png)

     O status do projeto será alterado para **[!UICONTROL Aprovado]** se o Business Case for aprovado.

     O status do projeto será alterado para **[!UICONTROL Rejeitado]** se o Plano de Negócio for rejeitado.

     >[!NOTE]
     >
     >Não há notificações que alertem o usuário que enviou a aprovação do business case se a solicitação do projeto foi aprovada ou rejeitada.

     Ou

   * Altere o status do projeto para qualquer outro status no menu suspenso **[!UICONTROL Status]**.

     ![Alterar status do projeto da lista suspensa](assets/project-status-change-from-drop-down-in-header-nwe-350x294.png)



