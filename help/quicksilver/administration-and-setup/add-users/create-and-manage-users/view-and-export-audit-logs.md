---
title: Exibir e exportar logs de auditoria
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: Você pode exibir todos os logs de auditoria no sistema ou aqueles que atendem a determinados critérios de filtragem. Também é possível exportar logs de auditoria. Os logs de auditoria listam as alterações do usuário acionadas no sistema durante os últimos 90 dias.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: b04e8ba5-c3f2-4838-8df1-35e90de5c7bd
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '322'
ht-degree: 0%

---

# Exibir e exportar logs de auditoria

<!--
**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **
-->

Você pode exibir todos os logs de auditoria no sistema ou aqueles que atendem a determinados critérios de filtragem. Também é possível exportar logs de auditoria.

Os logs de auditoria listam as alterações do usuário acionadas no sistema durante os últimos 90 dias.

Para obter informações sobre todos os tipos de log de auditoria e o que os gera, consulte [Logs de auditoria](../../../administration-and-setup/add-users/create-and-manage-users/audit-logs.md).

## Requisitos de acesso

Você deve ter o seguinte para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plano Adobe Workfront</td> 
   <td>Qualquer Um</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença Adobe Workfront</td> 
   <td> <p>Plano </p> <p>Você deve ser um administrador do Workfront.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Exibir logs de auditoria

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront, em seguida, clique em **Configuração** ![](assets/gear-icon-settings.png).

1. No painel esquerdo, clique em **Sistema > Logs de auditoria**.
1. No **Tipo de log** selecione o tipo de log de auditoria que deseja visualizar.

   **Todos os tipos de log** é selecionada por padrão.

   Para obter uma lista de todos os tipos de log de auditoria que você pode exibir e as informações que eles incluem, consulte [Logs de auditoria](../../../administration-and-setup/add-users/create-and-manage-users/audit-logs.md).

1. (Opcional) Defina qualquer um dos filtros disponíveis.

   >[!NOTE]
   >
   >As opções no menu suspenso Tipo de ação variam de acordo com o log de auditoria selecionado.

   ![](assets/audit-logs.jpg)

1. Clique em **Aplicar**.
1. (Opcional) Clique em **Limpar filtros** para redefinir as alterações feitas nos filtros.

## Exportar logs de auditoria

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront, em seguida, clique em **Configuração** ![](assets/gear-icon-settings.png).

1. No painel esquerdo, clique em **Sistema > Logs de auditoria**.

1. No **Tipo de log** selecione um log de auditoria no menu suspenso.

   **Todos os tipos de log** é selecionada por padrão.

1. Defina qualquer um dos filtros disponíveis e clique em **Aplicar**.

   >[!IMPORTANT]
   >
   >Você não pode exportar mais de 50.000 logs de uma vez. O Workfront exporta logs com base nos filtros definidos, não no número de logs exibidos na página. Você pode visualizar o número total de logs filtrados no canto inferior direito da página.

1. Clique em **Exportar**.
