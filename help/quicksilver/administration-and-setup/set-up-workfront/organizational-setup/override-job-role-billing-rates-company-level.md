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
TQID: https://experienceleague.adobe.com/EbnybXqWehstH2ziLqNZfMHtarMvUiugvWioYv9wLds
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 8c08e110aeccdf6d6416fd1070fbcbd40fd46983
workflow-type: tm+mt
source-wordcount: 857
ht-degree: 3%

---

# Substituir taxas de cobrança de função de trabalho no nível da empresa

{{preview-fast-release-general}}

Quando uma função de trabalho é criada, você tem a opção de selecionar uma taxa de cobrança por hora para essa função. Você pode criar várias taxas de faturamento por hora específicas para uma empresa. Cada taxa de faturamento é efetiva para uma faixa de datas específica.

No nível do projeto, você pode ativar uma opção para permitir que as taxas de cobrança no nível da empresa substituam as taxas no nível do projeto. Para obter mais informações, consulte [Substituir taxas de cobrança no nível do projeto por taxas de cobrança no nível da empresa](../../../manage-work/projects/project-finances/override-project-level-with-company-level-billing-rates.md).

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] pacote</td> 
   <td><p>Para adicionar atributos de taxa às taxas de faturamento no nível da empresa: Ultimate do Workflow</p>
       <p>Para criar taxas de faturamento no nível da empresa e editar todas as outras configurações de taxa: Qualquer pacote do Workfront ou Workflow</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] licença</td> 
   <td><p>[!UICONTROL Padrão]</p>
       <p>[!UICONTROL Plan]</p></td>
  </tr> 
  <tr> 
   <td>Configurações de nível de acesso</td> 
   <td> <p>Acesso administrativo a Empresas se você não for um Administrador do sistema</p>
   <p>Editar acesso a Dados Financeiros</p> </td>
  </tr> 
 </tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Substituir ou alterar uma taxa de cobrança estabelecida usada para uma função de trabalho específica

{{step-1-to-setup}}

1. Clique em **[!UICONTROL Empresas]**.
1. Localize a empresa à qual a função de trabalho está atribuída.
1. Clique no nome da empresa na lista.
1. Clique em **[!UICONTROL Taxas de cobrança]** no painel esquerdo.
1. Clique em **[!UICONTROL Adicionar Taxa de Cobrança] > [!UICONTROL Nova Taxa de Cobrança]** ou <span class="preview">**Adicionar Taxa de Cobrança**</span>.
1. Na caixa de diálogo [!UICONTROL Nova taxa de cobrança], selecione uma [!UICONTROL **Função de trabalho**] para definir a taxa de cobrança para.

### No ambiente de produção:

A [!UICONTROL **Taxa de Cobrança Padrão**] exibe a taxa no nível do sistema para esta função de trabalho.

![Caixa de diálogo Nova Taxa de Cobrança](assets/date-effective-billing-rates-for-company.png)

1. No campo [!DNL **Taxas de Cobrança 1**], insira a taxa de cobrança. Em seguida, clique em [!UICONTROL **Salvar**] para substituir a taxa de cobrança uma vez.

   Ou

   Clique em [!UICONTROL **Adicionar taxa**] para adicionar mais taxas de cobrança com datas efetivas.

1. (Condicional) Se você estiver adicionando mais de uma taxa de faturamento, especifique as seguintes informações:

   * **[!UICONTROL Taxas de Cobrança 1], 2, etc.**: o valor da taxa de cobrança para o período de tempo.
   * **[!UICONTROL Data de Início]**: a data quando a taxa se torna efetiva.
   * **[!UICONTROL Data de término]**: a data em que a taxa termina.

     A Taxa de Cobrança 1 não terá uma data inicial e a última taxa de cobrança não terá uma data final. Algumas datas são adicionadas automaticamente. Por exemplo, se a Taxa de cobrança 1 não tiver uma data final e você adicionar a Taxa de cobrança 2 com uma data inicial de 1º de maio de 2023, uma data final de 30 de abril de 2023 será adicionada à Taxa de cobrança 1 para que não haja lacunas.

1. Clique em [!UICONTROL **Salvar**].

   >[!NOTE]
   >
   >As taxas de função de trabalho alteradas no projeto afetarão somente esse projeto. As taxas alteradas no nível da empresa afetarão todos os projetos. Para obter mais informações, consulte [Visão geral da substituição de taxas de cobrança e do cálculo de receita em um projeto](/help/quicksilver/manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).

<div class="preview">

### No ambiente de Pré-visualização:

1. Selecione atributos para a taxa, como Agência, Local ou Centro de Custo.

   Esses atributos são definidos separadamente e podem afetar os cálculos de receita e custo. Para obter mais informações, consulte [Definir atributos de taxa](/help/quicksilver/administration-and-setup/manage-enterprise-operations/define-rate-attributes.md).

   ![Caixa de diálogo Nova Taxa de Cobrança](assets/company-billing-rates-090326.png)

1. Selecione a **Moeda** para a taxa. O administrador do Workfront adiciona a Moeda base na área Configuração. Você pode alterar a seleção para outra moeda disponível e alterar a moeda em faixas de datas efetivas.

   >[!TIP]
   >
   >Somente as moedas disponíveis na área Taxas de Câmbio do sistema estão disponíveis neste campo. Se você tiver apenas uma moeda configurada, somente essa moeda estará disponível.

   Para obter informações sobre como configurar a Moeda Base no Workfront, consulte [Configurar taxas de câmbio](/help/quicksilver/administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md).

   Para obter informações sobre como alterar a moeda de um projeto, consulte [Alterar a moeda do projeto](/help/quicksilver/manage-work/projects/project-finances/change-project-currency.md).

1. No campo [!DNL **Taxa de Cobrança**], insira a taxa de cobrança da função de trabalho.

   Esta é a taxa de cobrança por hora da função de trabalho. Esse valor calcula as receitas planejadas e reais de tarefas e problemas associados à função e, por fim, as receitas planejadas e reais dos projetos. Insira a taxa usando a moeda selecionada.

   Se você usar atributos, eles e a função de trabalho serão combinados para definir uma taxa exclusiva. Por exemplo, uma função Designer em Nova York para a Agência A pode ter uma taxa separada de uma função Designer em Paris para a Agência B.

   Para taxas de cobrança efetivas por data, clique em **Adicionar taxa efetiva por data**. Informe a taxa de faturamento por hora para o período e atribua uma Data Inicial e uma Data Final conforme necessário. A primeira taxa de cobrança não terá uma data inicial e a última taxa de cobrança não terá uma data final.

   O Workfront permite que você deixe intervalos entre intervalos de datas, mas você receberá um aviso para confirmar que isso é intencional.

   Para obter informações sobre como a Workfront calcula a receita, consulte [Visão geral de faturamento e receita](/help/quicksilver/manage-work/projects/project-finances/billing-and-revenue-overview.md).

   >[!TIP]
   >
   >Ao editar uma taxa existente, você pode classificar a lista para ver a data de início mais recente no topo da lista de taxas.

1. Clique em [!UICONTROL **Salvar**].

   >[!NOTE]
   >
   >As taxas de função de trabalho alteradas no projeto afetarão somente esse projeto. As taxas alteradas no nível da empresa afetarão todos os projetos aos quais a empresa está atribuída. Para obter mais informações, consulte [Visão geral da substituição de taxas de cobrança e do cálculo de receita em um projeto](/help/quicksilver/manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).

</div>

