---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: Habilitar Trimestre personalizado
description: Para fins de relatórios, você pode criar trimestres personalizados se os trimestres de sua organização forem baseados em critérios específicos diferentes das datas do calendário (como dias úteis ou dias de compras).
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 0f643d36-6235-4fd3-b6d3-54fbd03c9b33
source-git-commit: b27b01e1efacc3fc459cec0a53b2c11cbe5e132b
workflow-type: tm+mt
source-wordcount: '386'
ht-degree: 1%

---

# Habilitar trimestres personalizados

<!--Audited: 11/2024-->

Para fins de relatórios, você pode criar trimestres personalizados se os trimestres de sua organização forem baseados em critérios específicos diferentes das datas do calendário (como dias úteis ou dias de compras).

Dependendo dos produtos comprados por sua empresa, é possível configurar o seguinte número de trimestres na área de configuração do Workfront:

* Os clientes que compraram somente [!DNL Workfront] podem configurar até oito trimestres personalizados para seus sistemas [!DNL Adobe Workfront].
* Os clientes que compraram o [!DNL Workfront] e o [!DNL Workfront Planning] podem configurar até 100 trimestres para seus sistemas [!DNL Workfront], que também estão disponíveis no [!DNL Planning].

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plano</td> 
   <td>Qualquer</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licença</td> 
   <td><p>Novo: [!UICONTROL Padrão]</p>
   Ou
   <p>Atual: [!UICONTROL Plano]</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td>[!UICONTROL Administrador do Sistema]</td>
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Configurar trimestres personalizados para o sistema [!DNL Workfront]

{{step-1-to-setup}}

1. Clique em **[!UICONTROL Preferências do projeto]** > **[!UICONTROL Projetos].**

1. Na seção **[!UICONTROL Linhas do Tempo]**, selecione **[!UICONTROL Habilitar Trimestres Personalizados]**.

1. Digite um nome para o trimestre personalizado, como &quot;T1 fiscal de 2021&quot;.
1. Selecione datas de início e término para o trimestre personalizado.

   ![Trimestres personalizados](assets/custom-quarters-nwe.png)

1. (Opcional) Clique em **[!UICONTROL Adicionar trimestre personalizado]** para adicionar mais trimestres personalizados ao sistema.

   >[!IMPORTANT]
   >
   > Se sua empresa comprou o [!DNL Workfront Planning], você não poderá salvar trimestres personalizados se houver lacunas ou sobreposições entre os trimestres.
   >![Trimestres personalizados com aviso de sobreposição](assets/custom-quarters-with-overlap-warning.png)
   >Intervalos e sobreposições entre os trimestres são permitidos somente para [!DNL Workfront] clientes.

1. (Opcional e condicional) Se sua empresa comprou apenas o [!DNL Workfront], sem o [!DNL Workfront Planning], crie um elemento de relatório que faça referência aos trimestres fiscais.


   **Exemplo:** Crie um filtro para uma lista de [!UICONTROL projetos] e inclua a Data de Conclusão Planejada de um projeto que faça referência aos trimestres personalizados.

   ![Filtro de projeto com trimestres personalizados](assets/example-of-project-filter-with-custom-quarters.png)

   As referências a &quot;Este trimestre&quot;, &quot;Próximo trimestre&quot; e &quot;Último trimestre&quot; são substituídas por novas referências aos trimestres personalizados.

   Para obter informações sobre elementos de relatórios, consulte [Elementos de relatórios: filtros, exibições e agrupamentos](../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md).

   Para obter informações sobre como criar filtros, consulte [Criar ou editar filtros em [!DNL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/create-filters.md).
1. (Opcional e condicional) Se você tiver acesso a [!DNL Workfront Planning], vá para uma página de tipo de registro e abra uma exibição de linha do tempo. A exibição mostra os novos trimestres personalizados.
Para obter informações, consulte [Gerenciar a exibição da linha do tempo](/help/quicksilver/planning/views/manage-the-timeline-view.md).
