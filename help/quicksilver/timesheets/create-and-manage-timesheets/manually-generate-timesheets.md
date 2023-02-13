---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: Gerar manualmente folhas de ponto
description: Para permitir que as alterações feitas nos perfis da folha de ponto sejam refletidas nas folhas de horas atuais, primeiro você deve excluir as folhas de horas existentes e gerar manualmente novas. Você pode gerar manualmente as folhas de horas a partir da área Folhas de horas ou da área Diagnósticos em Configurar, conforme explicado neste artigo.
author: Alina
feature: Timesheets
exl-id: 316c270a-c64e-4d83-a035-4128abe33f87
source-git-commit: 7786d899841cb82cc4d3832fb083c6e2bda2e197
workflow-type: tm+mt
source-wordcount: '450'
ht-degree: 0%

---

# Gerar manualmente folhas de ponto

Para permitir que as alterações feitas nos perfis da folha de ponto sejam refletidas nas folhas de horas atuais, primeiro você deve excluir as folhas de horas existentes e gerar manualmente novas. Você pode gerar manualmente as folhas de horas a partir da área Folhas de horas ou da área Diagnósticos em Configurar, conforme explicado neste artigo.

Para obter instruções sobre como excluir folhas de ponto, consulte [Excluir folhas de ponto no Adobe Workfront](../../timesheets/create-and-manage-timesheets/delete-timesheets.md).

## Requisitos de acesso

Você deve ter o seguinte para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plano Adobe Workfront</td> 
   <td> <p>Qualquer Um</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença Adobe Workfront</td> 
   <td> <p>Plano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Você deve ser um administrador do Workfront ou, se estiver trabalhando nos perfis da folha de ponto de um grupo, deve ser um administrador de grupo (ou administrador do Workfront). Para obter mais informações, consulte <a href="../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Administradores do grupo</a>.</p> <p>Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

## Considerações sobre as folhas de horas geradas manualmente

Ao gerar folhas de horas manualmente:

* Elas são geradas de acordo com os perfis da folha de ponto associados aos usuários. Os usuários que não têm perfis de folha de ponto associados a eles não recebem folhas de ponto. 
* Somente a folha de ponto atual e a que se segue são geradas. O Workfront não gera duas folhas de ponto para o mesmo período. Se você já tiver uma folha de ponto para um período específico, outra não será gerada quando estiver usando o processo manual para gerar folhas de ponto.

## Gerar manualmente folhas de horas a partir da área Folhas e horas

Você pode gerar manualmente as folhas de ponto no nível do sistema ou no nível do grupo a partir da área Folhas de Horas e Horas em Configurar.

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront, em seguida, clique em **Configuração** ![](assets/gear-icon-settings.png).

1. Se você estiver gerando folhas de horas em uso em todo o sistema, clique em **Folhas de horas e horas.**

   Ou

   Se você estiver gerando folhas de horas usadas por um grupo específico, clique em **Grupos** e clique no nome do grupo.

1. Clique em **Perfis de Folha de Horas**.
1. Clique em **Mais**, em seguida **Gerar Folhas de Horas**.

   Novas folhas de horas são criadas por até dois períodos para usuários associados a perfis de folha de ponto.

## Gerar manualmente folhas de ponto no nível do sistema a partir da área de Diagnóstico

Você pode gerar manualmente as folhas de ponto no nível do sistema a partir da área Diagnósticos em Configurar.

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront, em seguida, clique em **Configuração** ![](assets/gear-icon-settings.png).

1. Expandir **Sistema**, depois clique em **Diagnóstico**.

1. Clique em **Conduzir diagnósticos**. 
1. Clique em **Gerar Folhas de Horas**.
