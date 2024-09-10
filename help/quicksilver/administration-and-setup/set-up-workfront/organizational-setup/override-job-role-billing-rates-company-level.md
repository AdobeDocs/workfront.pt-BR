---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: organization-setup
title: Substituir taxas de cobrança de função de trabalho no nível da empresa
description: Quando uma função de trabalho é criada, você tem a opção de selecionar uma taxa de cobrança por hora para essa função. Você pode criar uma taxa de cobrança por hora específica para uma empresa.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: ee60987e-78b5-4853-9a4f-e44aa7a81c05
source-git-commit: 439303273239549bb326c171be44eea321f5bb5f
workflow-type: tm+mt
source-wordcount: '461'
ht-degree: 1%

---

# Substituir taxas de cobrança de função de trabalho no nível da empresa

Quando uma função de trabalho é criada, você tem a opção de selecionar uma taxa de cobrança por hora para essa função. Você pode criar várias taxas de faturamento por hora específicas para uma empresa. Cada taxa de faturamento é efetiva para uma faixa de datas específica.

No nível do projeto, você pode ativar uma opção para permitir que as taxas de cobrança no nível da empresa substituam as taxas no nível do projeto. Para obter mais informações, consulte [Substituir taxas de cobrança no nível do projeto por taxas de cobrança no nível da empresa](../../../manage-work/projects/project-finances/override-project-level-with-company-level-billing-rates.md).

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plano</td> 
   <td> <p>Qualquer </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licença</td> 
   <td>
   <p>Novo: [!UICONTROL Padrão]</p>
   <p>Ou</p>
   <p>Atual: [!UICONTROL Plano]</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Acesso administrativo a Empresas se você não for um Administrador do sistema</p>
   <p>Editar acesso a Dados Financeiros</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Substituir ou alterar uma taxa de cobrança estabelecida usada para uma função de trabalho específica

{{step-1-to-setup}}

1. Clique em **[!UICONTROL Empresas]**.
1. Localize a empresa à qual a função de trabalho está atribuída.
1. Clique no nome da empresa na lista.
1. Clique em **[!UICONTROL Taxas de cobrança]** no painel esquerdo.
1. Clique em **[!UICONTROL Adicionar Taxa de Cobrança] > [!UICONTROL Nova Taxa de Cobrança]** ou escolha uma taxa existente para editar.
1. Na caixa de diálogo [!UICONTROL Nova taxa de cobrança], selecione uma [!UICONTROL **Função de trabalho**] para definir a taxa de cobrança para.

   A [!UICONTROL **Taxa de Cobrança Padrão**] exibe a taxa no nível do sistema para esta função de trabalho.

   ![Caixa de diálogo Nova Taxa de Cobrança](assets/date-effective-billing-rates-for-company.png)

1. No campo [!DNL **Taxas de Cobrança 1**], insira a taxa de cobrança. Em seguida, clique em [!UICONTROL **Salvar**] para substituir a taxa de cobrança uma vez.

   Ou

   Clique em [!UICONTROL **Adicionar taxa**] para adicionar mais taxas de cobrança com datas efetivas.

1. (Condicional) Se você estiver adicionando mais de uma taxa de faturamento, especifique as seguintes informações:

   * **[!UICONTROL Taxas de Cobrança 1], 2, etc.**: O valor da taxa de cobrança para o período.
   * **[!UICONTROL Data de Início]**: a data quando a taxa se torna efetiva.
   * **[!UICONTROL Data de término]**: a data em que a taxa termina.

     A Taxa de Cobrança 1 não terá uma data inicial e a última taxa de cobrança não terá uma data final. Algumas datas são adicionadas automaticamente. Por exemplo, se a Taxa de cobrança 1 não tiver uma data final e você adicionar a Taxa de cobrança 2 com uma data inicial de 1º de maio de 2023, uma data final de 30 de abril de 2023 será adicionada à Taxa de cobrança 1 para que não haja lacunas.

1. Clique em [!UICONTROL **Salvar**].

   >[!NOTE]
   >
   >As taxas de função de trabalho alteradas no projeto afetarão somente esse projeto. As taxas alteradas no nível da empresa afetarão todos os projetos. Para obter mais informações, consulte [Visão geral da substituição de Taxas de cobrança de função de trabalho e do cálculo de Receita em um projeto](../../../manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).
