---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: Aprovar uma planilha de horas
description: O processo de aprovação de planilhas de horas fornece aos gerentes visibilidade sobre as horas de trabalho de seus subordinados diretos. Os aprovadores podem verificar se todo o tempo registrado foi alocado nas áreas corretas e se um número suficiente de horas foi registrado para o período.
author: Alina
feature: Timesheets
exl-id: b27b3307-f61b-456d-8076-590d1c391b4b
source-git-commit: 1a46fa3a8e87a5f345558cef57a4d66171320c9b
workflow-type: tm+mt
source-wordcount: '540'
ht-degree: 0%

---

# Aprovar uma planilha de horas

<!--Audited: 8/2024-->

O processo de aprovação de planilhas de horas fornece aos gerentes visibilidade sobre as horas de trabalho de seus subordinados diretos. Os aprovadores podem verificar se todo o tempo registrado foi alocado nas áreas corretas e se um número suficiente de horas foi registrado para o período.

O Adobe Workfront oferece a capacidade de configurar aprovações de planilhas de horas para serem suportadas nesta área.

Para obter informações sobre o envio de uma planilha de horas, consulte [Enviar uma planilha de horas para aprovação](../../timesheets/create-and-manage-timesheets/submit-timesheet-for-approval.md).

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><p>plano do Adobe Workfront</p></td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Licença da Adobe Workfront*</p></td> 
   <td> <p>Novo: Padrão</p>
   <p>Atual: Plano </p> 
   <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Acesso administrativo a planilhas de horas e horas </p> </td> 
  </tr>

</td> 
  </tr> 
 </tbody> 
</table>

*Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Designar aprovadores de planilhas de horas

Normalmente, as folhas de horas são aprovadas pelos gerentes funcionais ou pela equipe de recursos humanos. Geralmente, as planilhas de horas não são aprovadas pelos gerentes de projeto. Os gerentes de projeto podem aprovar horas reportadas nos projetos, mas os gerentes de equipe ou de recursos humanos devem aprovar folhas de horas.

Um aprovador de folha de horas é definido ao criar o Perfil de folha de horas. Você deve ter uma licença de Plano para ser designado como um aprovador.

Para obter mais informações sobre como designar aprovadores de folha de horas, consulte a seção [Criar ou editar um perfil de folha de horas](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md#create) no artigo [Criar, editar e atribuir perfis de folha de horas](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).

## Aprovar uma planilha de horas

Você pode aprovar qualquer planilha de horas que tenha sido submetida na qual tenha sido designado como aprovador. Quando uma folha de horas é enviada para aprovação, ela é listada na área **Aprovações** da sua página **Página inicial**. Para obter mais informações, consulte [Aprovando trabalho](../../review-and-approve-work/manage-approvals/approving-work.md).

Se o administrador do Workfront tiver ativado a Aprovação de folha de horas para o usuário e a Rejeição de folha de horas para os manipuladores de eventos do usuário, você será notificado depois que a folha de horas for aprovada ou rejeitada. Para obter informações sobre como habilitar notificações de eventos, consulte [Tipos de notificação de eventos](../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).

Para aprovar uma planilha de horas:

{{step1-to-timesheets}}

A área **Folhas de horas** é aberta.

1. Selecione as **Minhas planilhas de horas aprovadas** no canto superior direito da página para exibir somente as planilhas de horas aprovadas por você

   Ou

   Selecione o filtro **Minhas Aprovações de Planilha de Horas** na parte superior da lista de planilhas de horas.

   ![](assets/my-timesheet-approvals-my-timesheets-pills-on-timesheets-list-nwe-350x58.png)

   >[!NOTE]
   >
   >A opção Minhas aprovações de folha de horas não é exibida na parte superior da lista de folha de horas ou na lista de filtros se o administrador do Workfront ou um administrador de grupo removeu o filtro Minhas aprovações de folha de horas dos Controles de lista na área Configuração ou do Modelo de layout. Para obter mais informações, consulte os seguintes artigos:
   >
   >   
   >   
   >   * [Personalizar Filtros, Modos de Exibição e Agrupamentos usando um modelo de layout](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)
   >   
   >

1. (Opcional) Clique no ícone ![](assets/search-icon.png) da **pesquisa** na parte superior da lista de folhas de horas e digite uma palavra-chave para localizar uma folha de horas específica. Você pode pesquisar um intervalo de tempo ou o nome de um proprietário ou aprovador.
1. Clique no intervalo de tempo da folha de horas que você deseja aprovar. A folha de horas é aberta.

   >[!TIP]
   >
   >As planilhas de horas aguardando aprovação têm status de [!UICONTROL Enviadas].


1. Clique em **Aprovar**

   Ou

   Para rejeitar a folha de horas, clique em **Rejeitar** no canto inferior esquerdo da folha de horas.

   Se aprovado, o status da folha de horas muda para **Fechado**.

   Se rejeitado, o status da folha de horas muda para **Rejected**.
