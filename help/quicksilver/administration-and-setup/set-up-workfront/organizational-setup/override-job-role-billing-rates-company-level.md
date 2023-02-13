---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: organization-setup
title: Substituir as taxas de faturamento da função de trabalho no nível da empresa
description: Quando uma função de cargo é criada, você tem a opção de selecionar uma taxa de faturamento por hora para essa função. Você pode criar uma taxa de faturamento por hora específica para uma empresa.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: ee60987e-78b5-4853-9a4f-e44aa7a81c05
source-git-commit: b6f6964bb80f172849434c669df2b0ecd735a590
workflow-type: tm+mt
source-wordcount: '308'
ht-degree: 0%

---

# Substituir as taxas de faturamento da função de trabalho no nível da empresa

Quando uma função de cargo é criada, você tem a opção de selecionar uma taxa de faturamento por hora para essa função. Você pode criar uma taxa de faturamento por hora específica para uma empresa.

No nível do projeto, você pode ativar uma opção para permitir que as taxas de faturamento no nível da empresa substituam as taxas no nível do projeto. Para obter mais informações, consulte [Substituir as taxas de faturamento no nível do projeto por taxas de faturamento no nível da empresa](../../../manage-work/projects/project-finances/override-project-level-with-company-level-billing-rates.md).

## Requisitos de acesso

Você deve ter o seguinte:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plano*</td> 
   <td> <p>Qualquer Um </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licença*</td> 
   <td>Plano</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Acesso administrativo às empresas se você não for um administrador do sistema</p> <p>Acesso à [!UICONTROL Editar] para dados financeiros</p> <p><b>OBSERVAÇÃO</b>: Se ainda não tiver acesso, pergunte ao seu [!DNL Workfront] administrador se eles definirem restrições adicionais em seu nível de acesso. Para obter informações sobre como uma [!DNL Workfront] administrador pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com seu [!DNL Workfront] administrador.

## Substituir ou alterar uma taxa de faturamento estabelecida usada para uma função de cargo específica

1. Clique no botão **[!UICONTROL Menu principal]** ícone ![](assets/main-menu-icon.png) no canto superior direito de [!DNL Adobe] Workfront, em seguida, clique em **[!UICONTROL Configuração]** ![](assets/gear-icon-settings.png).

1. Clique em **[!UICONTROL Empresas]**.
1. Localize a empresa na qual a função de trabalho é atribuída.
1. Clique em **[!UICONTROL Editar empresa]** no canto superior direito.
1. No **[!UICONTROL Taxas de Faturamento]** , selecione a função de trabalho que deseja editar e insira a nova taxa de faturamento para essa função de cargo na **[!UICONTROL Taxa de Faturamento da Empresa]** caixa.

   >[!NOTE]
   >
   >As taxas de função de trabalho alteradas no projeto afetarão somente esse projeto. As taxas alteradas no nível da empresa afetarão todos os projetos. Para obter mais informações, consulte [Visão Geral das Taxas de Faturamento da Função do Trabalho e cálculo da Receita em um projeto](../../../manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).
