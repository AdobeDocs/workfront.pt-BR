---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: organization-setup
title: Criar e gerenciar funções de trabalho
description: Como administrador [!DNL Adobe Workfront] ou usuário com acesso administrativo a Funções de Trabalho, você pode criar funções de trabalho que podem ser atribuídas a usuários e excluir funções de trabalho padrão que não são relevantes para sua organização.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 664fb2fe-ff7e-4807-9a43-b37e7d5d57eb
source-git-commit: df1d844346d7ed26dcb004ba1a10ec9e8d07422a
workflow-type: tm+mt
source-wordcount: '1219'
ht-degree: 2%

---

# Criar e gerenciar funções de trabalho

<!-- Audited: 1/2024 -->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

>[!IMPORTANT]
>
>Com a versão 25.11, a opção Substituir moeda para funções de trabalho foi descontinuada na Produção. (A desativação ocorreu em 30 de outubro no ambiente de Pré-visualização.) Em vez de ter uma moeda base e moedas de substituição, uma moeda agora está disponível para funções de trabalho e as taxas de custo e cobrança são definidas usando essa moeda.

Como administrador do [!DNL Adobe Workfront] ou usuário do Standard com acesso de Edição a Funções de Trabalho, você pode criar funções de trabalho que possam ser atribuídas a usuários e excluir funções de trabalho padrão que não sejam relevantes para sua organização. Para obter informações sobre acesso administrativo no [!DNL Workfront], consulte [Conceder aos usuários acesso administrativo a determinadas áreas](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

>[!TIP]
>
>As funções de trabalho são parte integral do gerenciamento de recursos. Para usar as ferramentas de planejamento de recursos, as funções de trabalho precisam de um custo e uma taxa de faturamento associados a elas. Para obter informações, consulte [Introdução ao Gerenciamento de recursos](../../../resource-mgmt/resource-mgmt-overview/get-started-resource-management.md).

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] pacote</td> 
   <td><p>Para criar ou editar uma função de trabalho: qualquer pacote de Workfront ou Workflow</p>
   <p>Para aplicar atributos de taxa e adicionar formulários personalizados à função de trabalho: Ultimate do Workflow</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] licença</td> 
   <td><p>[!UICONTROL Padrão]</p>
       <p>[!UICONTROL Plan]</p></td>
  </tr> 
  <tr> 
   <td>Configurações de nível de acesso</td> 
   <td>Acesso administrativo a Funções de trabalho</td>
  </tr> 
 </tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Criar uma função de trabalho

Para criar uma função de trabalho:

{{step-1-to-setup}}

1. No painel esquerdo, clique em **[!UICONTROL Funções de trabalho]**.
1. Clique em **[!UICONTROL Nova Função] > Criar nova função de trabalho**.
1. Especifique informações nos seguintes campos:

   * **Nome**: indique um nome para a função de trabalho. Esse é o nome exibido em qualquer lugar do Workfront em que o campo Função de trabalho é exibido.

     >[!TIP]
     >
     >O nome de uma função de trabalho pode conter até 255 caracteres. No entanto, nomes mais longos podem estar truncados em determinadas áreas do Workfront.

   * **Descrição**: insira uma descrição para a função que indique o que é exclusivo sobre ela.
   * **Está ativo**: selecione **Sim** se desejar que a função fique ativa e disponível em qualquer lugar do Workfront para ser associada a usuários, itens de trabalho, etc. Selecione **Não** se desejar que a função seja desativada e não esteja disponível para atribuir a usuários, itens de trabalho, etc.

     Para obter informações sobre como desativar funções de trabalho, consulte [Desativar funções de trabalho](/help/quicksilver/administration-and-setup/set-up-workfront/organizational-setup/deactivate-job-roles.md).

1. Clique em **[!UICONTROL Criar Função]**. A função de trabalho agora está disponível para ser atribuída a tarefas, problemas, aprovações ou você pode compartilhar modelos de layout ou outros objetos com ela. Para obter informações sobre todos os usos de funções de trabalho em [!DNL Workfront], consulte [Visão geral da função de trabalho](../../../administration-and-setup/set-up-workfront/organizational-setup/job-role-overview.md). Para obter informações sobre como excluir uma função de trabalho, consulte [Excluir funções de trabalho](../../../administration-and-setup/set-up-workfront/organizational-setup/delete-job-roles.md).

## Adicionar taxas e atributos a uma função de trabalho

As taxas de faturamento e de custo em uma função de trabalho são usadas em cálculos financeiros.

Os atributos de taxa são suportados em áreas do Workfront onde existem taxas, como funções de trabalho e usuários. Quando atributos são aplicados em uma função de trabalho, suas atribuições são resolvidas automaticamente para as taxas corretas.

Para obter mais informações, consulte [Definir atributos de taxa](/help/quicksilver/administration-and-setup/manage-enterprise-operations/define-rate-attributes.md).

{{step-1-to-setup}}

1. No painel esquerdo, clique em **[!UICONTROL Funções de trabalho]**.
1. Clique no nome de uma função de trabalho existente para editá-la.
1. Para atualizar os detalhes da função de trabalho, clique em **Detalhes** no painel esquerdo.
1. (Opcional) Para anexar um formulário personalizado à função de trabalho, clique no campo **Adicionar formulário personalizado** no canto superior direito da página Detalhes e selecione um formulário personalizado na lista exibida.

   Para obter mais informações sobre como anexar um formulário personalizado, consulte [Adicionar um formulário personalizado a um objeto](/help/quicksilver/workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

1. Clique em [!UICONTROL **Taxas**] no painel esquerdo.
1. Clique em [!UICONTROL **Faturamento**] ou [!UICONTROL **Custo**] para selecionar o tipo de taxa.
1. Clique em [!UICONTROL **Adicionar Taxas**] para adicionar uma nova taxa.

   Ou

   Selecione uma taxa existente e clique no **ícone Editar** ![ícone Editar](assets/edit-icon.png) para atualizá-la.

   >[!NOTE]
   >
   >Como cada taxa está associada à combinação da função e dos atributos para criar uma taxa exclusiva, os atributos não podem ser alterados quando você edita uma taxa.

1. Na caixa **Nova Taxa**, selecione atributos para a taxa, como Agência, Local ou Centro de Custos.

   >[!NOTE]
   >
   >Esses atributos são definidos separadamente e podem afetar os cálculos de receita e custo. Para obter mais informações, consulte [Definir atributos de taxa](/help/quicksilver/administration-and-setup/manage-enterprise-operations/define-rate-attributes.md).

1. Selecione a **Moeda** para a taxa. O administrador do Workfront adiciona a Moeda base na área Configuração. Você pode alterar a seleção para outra moeda disponível e alterar a moeda em faixas de datas efetivas.

   >[!TIP]
   >
   >Somente as moedas disponíveis na área Taxas de Câmbio do sistema estão disponíveis neste campo. Se você tiver apenas uma moeda configurada, somente essa moeda estará disponível.

   Para obter informações sobre como configurar a Moeda Base no Workfront, consulte [Configurar taxas de câmbio](/help/quicksilver/administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md).

   Para obter informações sobre como alterar a moeda de um projeto, consulte [Alterar a moeda do projeto](/help/quicksilver/manage-work/projects/project-finances/change-project-currency.md).

1. (Condicional) Para uma taxa de cobrança, insira a **Taxa de Cobrança** para esta função de trabalho.

   Esta é a taxa de cobrança por hora da função de trabalho. Esse valor calcula as receitas planejadas e reais de tarefas e problemas associados à função e, por fim, as receitas planejadas e reais dos projetos. Insira a taxa usando a moeda selecionada.

   Se você usar atributos, eles e a função de trabalho serão combinados para definir uma taxa exclusiva. Por exemplo, uma função Designer em Nova York para a Agência A pode ter uma taxa separada de uma função Designer em Paris para a Agência B.

   Para taxas de cobrança efetivas por data, clique em **Adicionar taxa**. Informe o valor do faturamento/hora para o período e atribua uma Data Inicial e uma Data Final conforme necessário. A primeira taxa de cobrança não terá uma data inicial e a última taxa de cobrança não terá uma data final.

   <!-- Some dates are added automatically. For example, if the first billing rate does not have an end date, and you add a second with a start date of May 1, an end date of April 30 is added to the first billing rate so that no gaps exist.-->

   O Workfront permite que você deixe intervalos entre intervalos de datas, mas você receberá um aviso para confirmar que isso é intencional.

   Para obter informações sobre como a Workfront calcula a receita, consulte [Visão geral de faturamento e receita](/help/quicksilver/manage-work/projects/project-finances/billing-and-revenue-overview.md).

   >[!TIP]
   >
   >Ao editar uma função de trabalho existente, você pode classificar a lista para ver a data de início mais recente na parte superior da lista de taxas.

1. (Condicional) Para uma taxa de custo, insira a **Taxa de Custo** para esta função de trabalho.

   Esta é a taxa de custo por hora da função de trabalho. Esse valor calcula os custos planejados e reais de tarefas e problemas associados à função e, por fim, os custos planejados e reais dos projetos. Insira a taxa usando a moeda selecionada.

   Se você usar atributos, eles e a função de trabalho serão combinados para definir uma taxa exclusiva. Por exemplo, uma função Designer em Nova York para a Agência A pode ter uma taxa separada de uma função Designer em Paris para a Agência B.

   Para taxas de custo atuais, clique em **Adicionar taxa**. Informe o valor do custo/hora para o período e atribua uma Data Inicial e uma Data Final, conforme necessário. A primeira taxa de custo não terá uma data inicial e a última taxa de custo não terá uma data final.

   Algumas datas são adicionadas automaticamente. Por exemplo, se a primeira taxa de custo não tiver uma data final e você adicionar uma segunda taxa de custo com uma data inicial de 1º de maio, uma data final de 30 de abril será adicionada à primeira taxa de custo para que não haja lacunas.

   Para obter informações sobre como a Workfront calcula custos, consulte [Rastrear custos](/help/quicksilver/manage-work/projects/project-finances/track-costs.md).

   >[!TIP]
   >
   >Ao editar uma função de trabalho existente, você pode classificar a lista para ver a data de início mais recente na parte superior da lista de taxas.

1. Clique em [!UICONTROL **Salvar**].

<!--
   * **Override Currency Cost Rate**: This is the cost per hour rate of the job role using the selected Override Currency. Workfront uses this value to calculate the planned and the actual costs of tasks and issues associated with the job role.

     Enter the rate in the Override Currency specified above. This also updates the Cost Rate for this job role when using the Base Currency.

     For information about how Workfront calculates cost, see [Track costs](/help/quicksilver/manage-work/projects/project-finances/track-costs.md).

     >[!TIP]
     >
     >When updating an existing job role that already has a cost rate associated with it, Workfront calculates the Override Currency rate based on the conversion rate in your system. If you update the Override Currency Cost Rate, the cost rate of the job role also updates automatically.

   * **Override Currency Billing Rate**: This is the billing per hour rate of the job role using the selected Override Currency. Workfront uses this value to calculate the planned and the actual revenue of tasks and issues associated with the job role.

      Enter the rate in the Override Currency specified above. This also updates the Billing Rate for this job role when using the Base Currency.

      For information about how Workfront calculates revenue, see [Overview of Billing and Revenue](/help/quicksilver/manage-work/projects/project-finances/billing-and-revenue-overview.md).

     >[!TIP]
     >
     >When updating an existing job role that already has a billing rate associated with it, Workfront calculates the Override Currency rate based on the conversion rate in your system. If you update the Override Currency Billing Rate, the billing rate of the job role also updates automatically.

-->


<!--

   * **Currency**: The Base Currency is shown by default. The Workfront administrator adds the Base Currency in the Setup area. You can change the selection to another available currency, and you can change the currency on effective dated time ranges.

      >[!TIP]
      >
      >Only currencies available in the Exchange Rates area in your system are available in this field. If you only have one currency set up, only that currency is available.

      For information about setting up the Base Currency in Workfront, see [Set up exchange rates](/help/quicksilver/administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md).

      For information about changing the currency of a project, see [Change the project currency](/help/quicksilver/manage-work/projects/project-finances/change-project-currency.md).
   
   * **Cost Rate**: This is the cost per hour rate of the job role. This value calculates the planned and the actual costs of tasks and issues associated with the role, and ultimately the planned and actual costs of the projects. Enter the rate using the selected currency.

      For date effective cost rates, click **Add Rate**. Enter the value of the cost/hour for the time period, and assign a Start Date and End Date as needed. The first cost rate will not have a start date and the last cost rate will not have an end date.

      Some dates are added automatically. For example, if the first cost rate does not have an end date, and you add a second cost rate with a start date of May 1, 2025, an end date of April 30, 2025 is added to the first cost rate so that no gaps exist.

      For information about how Workfront calculates cost, see [Track costs](/help/quicksilver/manage-work/projects/project-finances/track-costs.md).

      >[!TIP]
      >
      >When editing an existing job role, you can sort the list to see the most recent start date at the top of the rate list.

   * **Billing Rate**: This is the billing per hour rate of the job role. This value calculates the planned and actual revenues of tasks and issues associated with the role, and ultimately the planned and actual revenues of the projects. Enter the rate using the selected currency.

      For date effective billing rates, click **Add Rate**. Enter the value of the billing/hour for the time period, and assign a Start Date and End Date as needed. The first billing rate will not have a start date and the last billing rate will not have an end date.

      Some dates are added automatically. For example, if the first billing rate does not have an end date, and you add a second with a start date of May 1, 2025, an end date of April 30, 2025 is added to the first billing rate so that no gaps exist.

      For information about how Workfront calculates revenue, see [Overview of Billing and Revenue](/help/quicksilver/manage-work/projects/project-finances/billing-and-revenue-overview.md).

      >[!TIP]
      >
      >When editing an existing job role, you can sort the list to see the most recent start date at the top of the rate list.

-->



