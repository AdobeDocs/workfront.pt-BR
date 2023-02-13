---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: Habilitar trimestres personalizados para projetos
description: Para fins de relatório, você pode criar trimestres personalizados se os trimestres de sua organização se basearem em critérios específicos diferentes das datas do calendário (como dias úteis ou dias de compras).
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 0f643d36-6235-4fd3-b6d3-54fbd03c9b33
source-git-commit: 2fd772ffc667c4f32c6a7b0de9c87676ee6dd65b
workflow-type: tm+mt
source-wordcount: '285'
ht-degree: 0%

---

# Habilitar trimestres personalizados para projetos

Para fins de relatório, você pode criar trimestres personalizados se os trimestres de sua organização se basearem em critérios específicos diferentes das datas do calendário (como dias úteis ou dias de compras).

Você pode configurar até oito trimestres personalizados para sua [!DNL Adobe Workfront] sistema.

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plano</td> 
   <td>Qualquer Um</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licença</td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Você deve ser um [!DNL Workfront] administrador.</p> <p><b>OBSERVAÇÃO</b>: Se ainda não tiver acesso, pergunte ao seu [!DNL Workfront] administrador se eles definirem restrições adicionais em seu nível de acesso. Para obter informações sobre como uma [!DNL Workfront] administrador pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Configure os trimestres personalizados para sua [!DNL Workfront] sistema

1. Clique no botão **[!UICONTROL Menu principal]** ícone ![](assets/main-menu-icon.png) no canto superior direito de [!DNL Adobe Workfront], depois clique em **[!UICONTROL Configuração]** ![](assets/gear-icon-settings.png).

1. Clique em **[!UICONTROL Preferências do projeto]** > **[!UICONTROL Projetos].**

1. No **[!UICONTROL Linhas do tempo]** seção , selecione **[!UICONTROL Ativar Trimestres Personalizados]**.

1. Digite um nome para o trimestre personalizado, como &quot;T1 fiscal 2021.&quot;
1. Selecione datas de início e término para o trimestre personalizado.

   ![](assets/custom-quarters-nwe.png)

1. (Opcional) Clique em **[!UICONTROL Adicionar Trimestre Personalizado]** para adicionar outros trimestres personalizados ao sistema.
1. (Opcional) Crie um elemento de relatório que se refere aos trimestres fiscais.

   **Exemplo:** Criar um filtro para um [!UICONTROL projeto] e incluir a Data de conclusão planejada de um projeto que faça referência aos trimestres personalizados.

   ![](assets/example-of-project-filter-with-custom-quarters.png)

   As referências a &quot;Este Trimestre&quot;, &quot;Próximo Trimestre&quot; e &quot;Último Trimestre&quot; são substituídas por novas referências aos trimestres personalizados.

   Para obter informações sobre elementos de relatório, consulte [Elementos de relatório: filtros, visualizações e agrupamentos](../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md).

   Para obter informações sobre como criar filtros, consulte [Criar ou editar filtros em [!DNL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/create-filters.md).
