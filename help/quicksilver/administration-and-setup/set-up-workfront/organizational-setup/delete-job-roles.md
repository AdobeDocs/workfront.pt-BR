---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: organization-setup
title: Excluir funções de trabalho
description: É possível excluir funções de trabalho que sua organização não usa mais. Recomendamos que você não exclua funções de trabalho se elas tiverem sido associadas a itens de trabalho no passado. Para manter todas as suas informações históricas sobre atribuições de trabalho, recomendamos desativar funções, em vez de excluí-las quando elas se tornarem obsoletas. Para obter informações sobre como desativar funções, consulte Desativar funções de trabalho.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: b0e81d76-5227-4fda-9a58-68fbce3f5b94
source-git-commit: b6f6964bb80f172849434c669df2b0ecd735a590
workflow-type: tm+mt
source-wordcount: '398'
ht-degree: 0%

---

# Excluir funções de trabalho

É possível excluir funções de trabalho que sua organização não usa mais. Recomendamos que você não exclua funções de trabalho se elas tiverem sido associadas a itens de trabalho no passado.

Para manter todas as suas informações históricas sobre atribuições de trabalho, recomendamos desativar funções, em vez de excluí-las quando elas se tornarem obsoletas. Para obter informações sobre como desativar funções, consulte [Desativar funções de trabalho](../../../administration-and-setup/set-up-workfront/organizational-setup/deactivate-job-roles.md).

## Requisitos de acesso

Você deve ter o seguinte:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plano*</td> 
   <td> <p>Qualquer </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licença*</td> 
   <td>[!UICONTROL Plano]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Acesso administrativo a funções de trabalho</p> <p><b>OBSERVAÇÃO</b>: se você ainda não tiver acesso, pergunte ao administrador do [!DNL Workfront] se ele definiu restrições adicionais no seu nível de acesso. Para obter informações sobre como um administrador do [!DNL Workfront] pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qual plano, tipo de licença ou acesso você tem, contate o administrador do [!DNL Workfront].

## Excluir uma função de trabalho

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this moved from create and manage job roles)</p>
-->

1. Clique no ícone ![](assets/main-menu-icon.png) do **[!UICONTROL Menu Principal]** no canto superior direito de [!DNL Adobe Workfront] e em **[!UICONTROL Configurar]** ![](assets/gear-icon-settings.png).

1. Clique em **[!UICONTROL Funções de trabalho].**
1. Selecione a função de trabalho que você deseja excluir e clique em **[!UICONTROL Excluir].**
1. Se houver objetos (usuários, tarefas, problemas) atribuídos à função de trabalho, execute um dos seguintes procedimentos:

   * **Substitua a função de trabalho por uma função de trabalho diferente:** Selecione a nova função de trabalho na lista suspensa.

     Quaisquer alocações de recursos atuais e anteriores associadas à função de trabalho excluída são transferidas para a função de trabalho selecionada.

     Os usuários que têm somente uma função de trabalho atribuída a eles são reatribuídos à função de trabalho selecionada; os usuários que têm uma função de trabalho secundária atribuída a eles não são reatribuídos à função de trabalho selecionada.

   * **Excluir a função de trabalho e sua alocação de recursos:** Selecione **[!UICONTROL Nenhum]** na lista suspensa.

     >[!IMPORTANT]
     >
     >A exclusão de uma função de trabalho exclui toda a alocação de recursos atual e passada relacionada a essa função de trabalho para todos os projetos.

     &#x200B;Por exemplo, se uma tarefa ou problema for atribuído somente a essa função de trabalho, a tarefa ou problema será desatribuído após a exclusão da função de trabalho.

1. Clique Em **[!UICONTROL Sim, Exclua-O]**.
