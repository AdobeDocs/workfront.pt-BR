---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: Habilitar Trimestres e Semanas Personalizados
description: Para fins de relatório, você pode configurar trimestres personalizados se os trimestres de sua organização forem baseados em critérios específicos diferentes das datas do calendário (como dias úteis ou dias de compras). Se sua organização comprar pacotes do Workfront Planning, você também poderá configurar semanas personalizadas.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 0f643d36-6235-4fd3-b6d3-54fbd03c9b33
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: 'https://experienceleague.adobe.com/8kRfZ17zcgN0-hlc16wh328YGRjTlzuI3LAe-Yjj25s'
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
  - id: d5896d07-2812-5418-8b18-8957a0d7f0fb
    internal-label: System Setup and Administration
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
    internal-label: Reporting
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: c7c74fdba29c4c6d28d12447459c5903a34c7856
workflow-type: tm+mt
source-wordcount: '615'
ht-degree: 6%
---
# Habilitar trimestres e semanas personalizados

<!--Audited: 03/2026-->

<!--remove Production and Preview references at release-->

<!--

<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>
-->

Para fins de relatórios, você pode criar trimestres personalizados se os trimestres de sua organização forem baseados em critérios específicos diferentes das datas do calendário (como dias úteis ou dias de compras).

Dependendo dos produtos comprados por sua empresa, é possível configurar o seguinte número de trimestres na área de configuração do Workfront:

* Os clientes que compraram somente [!DNL Workfront] podem configurar até oito trimestres personalizados para seus sistemas [!DNL Adobe Workfront].
* Os clientes que compraram o [!DNL Workfront] e o [!DNL Workfront Planning] podem configurar até 100 trimestres para seus sistemas [!DNL Workfront], que também estão disponíveis no [!DNL Planning].

* Os clientes que compraram [!DNL Workfront] e [!DNL Workfront Planning] podem configurar semanas personalizadas para cada trimestre personalizado. As semanas personalizadas estão visíveis nas [!DNL Planning] exibições da linha do tempo.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] pacote</td> 
   <td><p>Qualquer</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] licença</td> 
   <td><p>Licença do [!UICONTROL Workflow Standard] ou [!UICONTROL Workfront Plan]</p>
       <p></p></td>
  </tr> 
  <tr> 
   <td>Configurações de nível de acesso</td> 
   <td>[!UICONTROL Administrador do Sistema]</td> 
  </tr> 
 </tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--
When we release fiscal weeks, replace the table above with this:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] package</td> 
   <td>
   <ul>
   <li><p>To configure custom quarters:</p>
   <p>Any Workfront or Workflow package</p></li>
   <li>
   <div class="preview">
   <p>To configure custom weeks:</p>
   <p>Any Planning package, including Planning as a standalone product</p>
   </div>
   </li>
   </ul>
   </td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] license</td> 
   <td>
   
   <ul>
   <li><p>To configure custom quarters:</p>
   <p>[!UICONTROL Workflow Standard] or [!UICONTROL Workfront Plan] license</p></li>
   <li>
   <div class="preview">
   <p>To configure custom weeks:</p>
   <p>A [!UICONTROL Planning Standard] license, in addition to a Workfront or a Workflow license</p>
   </div>
   </li>
   </ul>
    </td>
  </tr> 
  <tr> 
   <td>Access level configurations</td> 
   <td>[!UICONTROL System Administrator]</td> 
  </tr> 
 </tbody> 
</table>

-->


## Configurar trimestres personalizados para o sistema [!DNL Workfront]

<!--
Setting up custom quarters differs depending on which environment you use. 

### Set up custom quarters for your [!DNL Workfront] system in the Production environment

{{step-1-to-setup}}

1. Click **[!UICONTROL Custom Quarters]**.

1. Select **[!UICONTROL Enable Custom Quarters]**.

1. Type a name for the custom quarter, such as "Fiscal Q1 2021."
1. Select start and end dates for the custom quarter.

   ![Custom quarters](assets/custom-quarters-nwe.png)

1. (Optional) Click **[!UICONTROL Add Custom Quarter]** to add additional custom quarters to the system.

      >[!IMPORTANT]
      >
      > If your company purchased [!DNL Workfront Planning], you cannot save your custom quarters if there are gaps or overlaps between the quarters. 
      >![Custom quarters with overlap warning](assets/custom-quarters-with-overlap-warning.png)
      >Gaps and overlaps between the quarters are allowed for [!DNL Workfront] only customers. 

1. (Optional and conditional) If your company purchased only [!DNL Workfront], without [!DNL Workfront Planning], create a reporting element that refers to the fiscal quarters.

   **Example:** Create a filter for a [!UICONTROL project] list and include the Planned Completion Date of a project referencing the custom quarters.

   ![Project filter with custom quarters](assets/example-of-project-filter-with-custom-quarters.png)

   The references to "This Quarter", "Next Quarter", and "Last Quarter" are replaced with new references to the custom quarters.

   For information about reporting elements, see [Reporting elements: filters, views, and groupings](../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md).

   For information about creating filters, see [Create or edit filters in [!DNL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/create-filters.md).
1. (Optional and conditional) If your company purchased Workfront Planning and you have access to [!DNL Workfront Planning], go to a record type page and open a timeline view. The view displays the new custom quarters. 
For information, see [Manage the timeline view](/help/quicksilver/planning/views/manage-the-timeline-view.md). 

<div class="preview">

### Set up custom quarters for your [!DNL Workfront] system in the Preview environment

-->

>[!NOTE]
>
>Se sua organização adquiriu um pacote do Planning além de um pacote do Workflow, ou se adquiriu o Workfront Planning como um pacote independente, você pode configurar semanas personalizadas, além de trimestres personalizados.
> 
>Semanas personalizadas não estão disponíveis para relatórios e listas do Workfront.

{{step-1-to-setup}}

1. Clique em **[!UICONTROL Trimestres personalizados]**.

1. Selecione **[!UICONTROL Habilitar Trimestres Personalizados]**.

1. Digite um nome para o trimestre personalizado. Por exemplo, &quot;T1 fiscal de 2021&quot;.
1. Selecione datas de início e término para o trimestre personalizado.

1. (Opcional) Selecione a opção **Inicia uma nova sequência semanal personalizada**.

   Quando selecionada, essa opção define o início do trimestre personalizado como o início da primeira semana personalizada do trimestre no modo de exibição de linha do tempo do Planning.
1. (Opcional) Na área **Formato de rótulo de semana personalizado**, escolha o **Formato** para os rótulos de semana personalizados. Escolha entre as seguintes opções:

   * **W1, W2, W3 ...** . Este é o formato padrão.
   * **FW1, FW2, FW3 ...**
   * **Semana1, Semana 2, Semana 3, ...**
   * **Personalizado**

1. (Condicional) Se você selecionou **Personalizado** para o campo **Formato**, digite um **Rótulo personalizado** para identificar as semanas personalizadas.

   As semanas personalizadas são exibidas nas exibições de linha do tempo do Planning.

   >[!TIP]
   >
   >Ao adicionar um rótulo personalizado, você pode digitar até 100 caracteres.
   >
   >Você pode indicar o nome da primeira semana e as semanas seguintes usarão o mesmo rótulo seguido de um número sequencial.
   >
   >Por exemplo, um **Rótulo personalizado** de &quot;Semana fiscal&quot; adicionará os rótulos de &quot;Semana fiscal 1, Semana fiscal 2, Semana fiscal 3 ...&quot; para o resto das semanas na sequência.

1. (Opcional) Clique em **[!UICONTROL Adicionar trimestre personalizado]** para adicionar mais trimestres personalizados ao sistema.

   >[!IMPORTANT]
   >
   > Se sua empresa comprou o [!DNL Workfront Planning], você não poderá salvar trimestres personalizados se houver lacunas ou sobreposições entre os trimestres.
   >![Trimestres personalizados com aviso de sobreposição](assets/custom-quarters-with-overlap-warning-red-outline.png)
   >Intervalos e sobreposições entre os trimestres são permitidos somente para [!DNL Workfront] clientes.

1. (Opcional e condicional) Para exibir os trimestres personalizados no Workfront, crie um elemento de relatório que faça referência aos trimestres personalizados.

   **Exemplo:** Crie um filtro para uma lista de [!UICONTROL projetos] e inclua a Data de Conclusão Planejada de um projeto que faça referência aos trimestres personalizados.

   ![Filtro de projeto com trimestres personalizados](assets/example-of-project-filter-with-custom-quarters.png)

   As referências a &quot;Este trimestre&quot;, &quot;Próximo trimestre&quot; e &quot;Último trimestre&quot; são substituídas por novas referências aos trimestres personalizados.

   Para obter informações sobre elementos de relatórios, consulte [Elementos de relatórios: filtros, exibições e agrupamentos](../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md).

   Para obter informações sobre como criar filtros, consulte [Criar ou editar filtros em [!DNL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/create-filters.md).
1. (Opcional e condicional) Para exibir trimestres e semanas personalizados no Workfront Planning, vá para uma página de tipo de registro e abra uma exibição de linha do tempo. A exibição mostra os novos trimestres e semanas personalizados.

   Para obter informações, consulte [Gerenciar a exibição da linha do tempo](/help/quicksilver/planning/views/manage-the-timeline-view.md).


