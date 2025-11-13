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
source-git-commit: a30e505aa2061240f92642fda274be66e4947bce
workflow-type: tm+mt
source-wordcount: '864'
ht-degree: 0%

---

# Criar e gerenciar funções de trabalho

<!-- Audited: 1/2024 -->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

>[!IMPORTANT]
>
>Com a versão 25.11, a opção Substituir moeda para funções de trabalho foi descontinuada na Produção. (A desativação ocorreu em 30 de outubro no ambiente de Pré-visualização.) Em vez de ter uma moeda base e moedas de substituição, uma moeda agora está disponível para funções de trabalho e as taxas de custo e cobrança são definidas usando essa moeda.

Como administrador do [!DNL Adobe Workfront] ou usuário com acesso administrativo às Funções de Trabalho, você pode criar funções de trabalho que podem ser atribuídas a usuários e excluir funções de trabalho padrão que não são relevantes para sua organização. Para obter informações sobre acesso administrativo no [!DNL Workfront], consulte [Conceder aos usuários acesso administrativo a determinadas áreas](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

>[!TIP]
>
>As funções de trabalho são parte integral do gerenciamento de recursos. Para usar as ferramentas de planejamento de recursos, as funções de trabalho precisam de um custo e uma taxa de faturamento associados a elas. Para obter informações, consulte [Introdução ao Gerenciamento de recursos](../../../resource-mgmt/resource-mgmt-overview/get-started-resource-management.md).

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

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
   <td><p>[!UICONTROL Padrão]</p>
       <p>[!UICONTROL Plano]</p></td>
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

1. No painel esquerdo, clique em&#x200B; **[!UICONTROL Funções de trabalho].**
1. Clique em **[!UICONTROL Nova Função].**
1. Configure os seguintes campos:

   * **Nome**: indique um nome para a função de trabalho. Esse é o nome exibido em qualquer lugar do Workfront em que o campo Função de trabalho é exibido.

     >[!TIP]
     >
     >O nome de uma função de trabalho pode conter até 255 caracteres. No entanto, nomes mais longos podem estar truncados em determinadas áreas do Workfront.

   * **Descrição**: insira uma descrição para a função que indique o que é exclusivo sobre ela.
   * **Está ativo**: selecione **Sim** se desejar que a função fique ativa e disponível em qualquer lugar do Workfront para ser associada a usuários, itens de trabalho, etc. Selecione **Não** se desejar que a função seja desativada e não esteja disponível para atribuir a usuários, itens de trabalho, etc.

     Para obter informações sobre como desativar funções de trabalho, consulte [Desativar funções de trabalho](/help/quicksilver/administration-and-setup/set-up-workfront/organizational-setup/deactivate-job-roles.md).

   * **Moeda**: a Moeda Base é mostrada por padrão. O administrador do Workfront adiciona a Moeda base na área Configuração. Você pode alterar a seleção para outra moeda disponível e alterar a moeda em faixas de datas efetivas.

     >[!TIP]
     >
     >Somente as moedas disponíveis na área Taxas de Câmbio do sistema estão disponíveis neste campo. Se você tiver apenas uma moeda configurada, somente essa moeda estará disponível.

     Para obter informações sobre como configurar a Moeda Base no Workfront, consulte [Configurar taxas de câmbio](/help/quicksilver/administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md).

     Para obter informações sobre como alterar a moeda de um projeto, consulte [Alterar a moeda do projeto](/help/quicksilver/manage-work/projects/project-finances/change-project-currency.md).

   * **Taxa de Custo**: esta é a taxa de custo por hora da função de trabalho. Esse valor calcula os custos planejados e reais de tarefas e problemas associados à função e, por fim, os custos planejados e reais dos projetos. Insira a taxa usando a moeda selecionada.

     Para taxas de custo atuais, clique em **Adicionar taxa**. Informe o valor do custo/hora para o período e atribua uma Data Inicial e uma Data Final, conforme necessário. A primeira taxa de custo não terá uma data inicial e a última taxa de custo não terá uma data final.

     Algumas datas são adicionadas automaticamente. Por exemplo, se a primeira taxa de custo não tiver uma data final e você adicionar uma segunda taxa de custo com uma data inicial de 1º de maio de 2025, uma data final de 30 de abril de 2025 será adicionada à primeira taxa de custo para que não haja lacunas.

     Para obter informações sobre como a Workfront calcula custos, consulte [Rastrear custos](/help/quicksilver/manage-work/projects/project-finances/track-costs.md).

     >[!TIP]
     >
     >Ao editar uma função de trabalho existente, você pode classificar a lista para ver a data de início mais recente na parte superior da lista de taxas.

   * **Taxa de Cobrança**: esta é a taxa de cobrança por hora da função de trabalho. Esse valor calcula as receitas planejadas e reais de tarefas e problemas associados à função e, por fim, as receitas planejadas e reais dos projetos. Insira a taxa usando a moeda selecionada.

     Para taxas de cobrança efetivas por data, clique em **Adicionar taxa**. Informe o valor do faturamento/hora para o período e atribua uma Data Inicial e uma Data Final conforme necessário. A primeira taxa de cobrança não terá uma data inicial e a última taxa de cobrança não terá uma data final.

     Algumas datas são adicionadas automaticamente. Por exemplo, se a primeira taxa de cobrança não tiver uma data final e você adicionar um segundo com uma data inicial de 1º de maio de 2025, uma data final de 30 de abril de 2025 será adicionada à primeira taxa de cobrança para que não haja lacunas.

     Para obter informações sobre como a Workfront calcula a receita, consulte [Visão geral de faturamento e receita](/help/quicksilver/manage-work/projects/project-finances/billing-and-revenue-overview.md).

     >[!TIP]
     >
     >Ao editar uma função de trabalho existente, você pode classificar a lista para ver a data de início mais recente na parte superior da lista de taxas.

1. Clique em **[!UICONTROL Criar Função]**. A função de trabalho agora está disponível para ser atribuída a tarefas, problemas, aprovações ou você pode compartilhar modelos de layout ou outros objetos com ela. Para obter informações sobre todos os usos de funções de trabalho em [!DNL Workfront], consulte [Visão geral da função de trabalho](../../../administration-and-setup/set-up-workfront/organizational-setup/job-role-overview.md). Para obter informações sobre como excluir uma função de trabalho, consulte [Excluir funções de trabalho](../../../administration-and-setup/set-up-workfront/organizational-setup/delete-job-roles.md).

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


   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Name]</td> 
      <td> <p>Indicate a name for the job role. This is the name that displays everywhere in [!DNL Workfront] where the [!UICONTROL Job Role] field displays. </p> <p>Tip: The name of a job role may contain up to 255 characters. However, longer names might be truncated in certain areas of [!DNL Workfront]. </p> </td> 
     </tr>
     <tr> 
      <td role="rowheader">[!UICONTROL Description]</td> 
      <td>Enter a description for the role that indicates what is unique about it. </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL Is Active]</span> </td> 
      <td> 
       <ul> 
        <li> <p>Select <b>[!UICONTROL Yes]</b> if you want the role to be active and available everywhere in [!DNL Workfront] to be associated with users, work items, etc. </p> </li> 
        <li> <p>Select <b>[!UICONTROL No]</b>, if you want the role to be deactivated and not available to assign to users, work items, etc. </p> </li> 
       </ul> <p><span>For information about deactivating job roles, see</span> <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/deactivate-job-roles.md" class="MCXref xref">Deactivate job roles</a>. </p> </td> 
     </tr>
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL Base Currency]</span> </td> 
      <td> <p><span>This is the [!UICONTROL Base Currency], as set in the [!UICONTROL Setup] area by your Workfront administrator. For information, see</span> <a href="../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md" class="MCXref xref">Set up exchange rates</a> .</p> <p>Tip: <span>You cannot edit the [!UICONTROL Base Currency] at the job role level. This field is dimmed and serves as a reminder for what the base currency is for your system.</span> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Cost Rate]</td> 
      <td><p>This is the cost per hour rate of the job role. This value calculates the planned and the actual costs of tasks and issues associated with the role, and ultimately the planned and actual costs of the projects. Enter the rate using the [!UICONTROL Base Currency].</p> 
      <p>For date effective cost rates, click <strong>[!UICONTROL Add Rate]</strong>. Enter the value of the cost/hour for the time period, and assign a [!UICONTROL Start Date] and [!UICONTROL End Date] as needed. The first cost rate will not have a start date and the last cost rate will not have an end date.</p> <p>Some dates are added automatically. For example, if the first cost rate does not have an end date, and you add a second cost rate with a start date of May 1, 2023, an end date of April 30, 2023 is added to the first cost rate so that no gaps exist.</p> <p>Tip: When editing an existing job role, you can select <strong>Sort by start date</strong> to see the most recent start date at the top of the rate list.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Billing Rate] </td> 
      <td><p>This is the billing per hour rate of the job role. This value calculates the planned and actual revenues of tasks and issues associated with the role, and ultimately the planned and actual revenues of the projects. Enter the rate using the [!UICONTROL Base Currency].</p> <p>For date effective billing rates, click <strong>[!UICONTROL Add Rate]</strong>. Enter the value of the billing/hour for the time period, and assign a [!UICONTROL Start Date] and [!UICONTROL End Date] as needed. The first billing rate will not have a start date and the last billing rate will not have an end date.</p> <p>Some dates are added automatically. For example, if the first billing rate does not have an end date, and you add a second with a start date of May 1, 2023, an end date of April 30, 2023 is added to the first billing rate so that no gaps exist.</p> <p>Tip: When editing an existing job role, you can select <strong>Sort by start date</strong> to see the most recent start date at the top of the rate list.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL Override Currency]</span> </td> 
      <td>
        <p>Select a currency associated with this job role. This is the currency that [!DNL Workfront] uses for calculating costs and revenue associated with this job role. </p> 
        <p><span>This is different than the [!UICONTROL Base Currency] set up by your [!DNL Workfront] administrator in the [!UICONTROL Setup] area, and can be different than the currency associated with a project.</span> </p> 
        <p>Tip: Only currencies available in the [!UICONTROL Exchange Rates] area in your system are available in this field. If you only have one currency set up, this field is does not appear.</p> 
       <p><span>For information about setting up the [!UICONTROL Base Currency] in [!DNL Workfront], see</span> <a href="../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md" class="MCXref xref">Set up exchange rates</a>.</p> <p><span>For information about changing the currency of a project, see</span> <a href="../../../manage-work/projects/project-finances/change-project-currency.md" class="MCXref xref">Change the project currency</a>.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL Override Currency Cost Rate]</span> </td> 
      <td>
        <p>This is the cost per hour rate of the job role using the selected [!UICONTROL Override Currency]. [!DNL Workfront] uses this value to calculate the planned and the actual costs of tasks and issues associated with the job role. </p> 
        <p><span>Enter the rate in the [!UICONTROL Override Currency] specified above. This also updates the Cost Rate for this job role when using the [!UICONTROL Base Currency].</span> </p> 
        <p>For information about how [!DNL Workfront] calculates cost, see <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Track costs</a>.</p> 
       <p>Tip: When updating an existing job role that already has a Cost Rate associated with it, [!DNL Workfront] calculates the [!UICONTROL Override Currency] rate based on the conversion rate in your system. If you update the [!UICONTROL Override Currency Cost Rate], the Cost Rate of the job role also updates automatically.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL Override Currency Billing Rate]</span> </td> 
      <td>
        <p>This is the billing per hour rate of the job role using the selected [!UICONTROL Override Currency]. [!DNL Workfront] uses this value to calculate the planned and the actual revenue of tasks and issues associated with the job role. </p>
        <p><span>Enter the rate in the [!UICONTROL Override Currency] specified above. This also updates the Billing Rateate for this job role when using the [!UICONTROL Base Currency].</span> </p>
        <p>For information about how [!DNL Workfront] calculates revenue, see <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">Overview of Billing and Revenue</a>.</p>
        <p>Tip: When updating an existing job role that already has a Billing Rate associated with it, [!DNL Workfront] calculates the Override Currency rate based on the conversion rate in your system. If you update the Override Currency Billing Rate, the Billing Rate of the job role also updates automatically. </p>
       </td>
     </tr> 
    </tbody> 
   </table>
-->



