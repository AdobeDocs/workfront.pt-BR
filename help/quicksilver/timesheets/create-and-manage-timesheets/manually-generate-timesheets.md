---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: Gerar folhas de horas manualmente
description: Para permitir que as alterações feitas nos perfis de folha de horas sejam refletidas nas folhas de horas atuais, primeiro exclua as folhas de horas existentes e gere manualmente as novas. Você pode gerar folhas de horas manualmente na área Folhas de horas ou na área Diagnóstico na Configuração, conforme explicado neste artigo.
author: Alina
feature: Timesheets
exl-id: 316c270a-c64e-4d83-a035-4128abe33f87
source-git-commit: a4bb3582eb476acbefa5d11db1f2c06eafc13cdd
workflow-type: tm+mt
source-wordcount: '453'
ht-degree: 0%

---

# Gerar folhas de horas manualmente

Para permitir que as alterações feitas nos perfis de folha de horas sejam refletidas nas folhas de horas atuais, primeiro exclua as folhas de horas existentes e gere manualmente as novas. Você pode gerar folhas de horas manualmente na área Folhas de horas ou na área Diagnóstico na Configuração, conforme explicado neste artigo.

Para obter instruções sobre como excluir folhas de horas, consulte [Excluir folhas de horas no Adobe Workfront](../../timesheets/create-and-manage-timesheets/delete-timesheets.md).

## Requisitos de acesso

Você deve ter o seguinte para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td> <p>Plano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Você deve ser um administrador do Workfront ou, se estiver trabalhando em perfis de folha de horas para um grupo, você deve ser um administrador de grupo (ou administrador do Workfront). Para obter mais informações, consulte <a href="../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Administradores de grupo</a>.</p> <p>Se você ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qual plano, tipo de licença ou acesso você tem, contate o administrador do Workfront.

## Considerações sobre folhas de horas geradas manualmente

Ao gerar folhas de horas manualmente:

* Eles são gerados de acordo com os perfis de folha de horas associados aos usuários. Os usuários que não têm perfis de folha de horas associados a eles não recebem folhas de horas. 
* Somente a folha de horas atual e a seguinte são geradas. O Workfront não gera duas folhas de horas para o mesmo período. Se você já tiver uma planilha de horas para o período atual, outra não será gerada quando você estiver usando o processo manual para gerar planilhas de horas.

## Gerar folhas de horas manualmente na área Folhas de horas e horas

Você pode gerar manualmente folhas de horas no nível do sistema ou do grupo na área Folhas de horas e horas na Configuração.

1. Clique no ícone **do** Menu Principal![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront e em **Configurar** ![](assets/gear-icon-settings.png).

1. Se você estiver gerando planilhas de horas em uso em todo o sistema, clique em **Planilhas de horas e horas.**

   Ou

   Se você estiver gerando planilhas de horas usadas por um grupo específico, clique em **Grupos** e, em seguida, clique no nome do grupo.

1. Clique em **Perfis de Planilha de Horas**.
1. Clique no ícone **Mais** ![Mais ícone](assets/more-icon.png) e em **Gerar folhas de horas**.

   Novas folhas de horas são criadas para até dois períodos de tempo para usuários associados a perfis de folha de horas.

## Gerar planilhas de horas no nível do sistema manualmente na área Diagnóstico

Você pode gerar manualmente planilhas de horas no nível do sistema a partir da área Diagnóstico na Configuração.

1. Clique no ícone **do** Menu Principal![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront e em **Configurar** ![](assets/gear-icon-settings.png).

1. Expanda **Sistema** e clique em **Diagnósticos**.

1. Clique em **Realizar Diagnóstico**. 
1. Clique em **Gerar Planilha de Horas**.
