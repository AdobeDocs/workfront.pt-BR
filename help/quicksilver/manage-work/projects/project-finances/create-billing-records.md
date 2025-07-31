---
navigation-topic: financials
title: Criar registros de cobrança
description: Além de configurar as despesas de rastreamento e receita, você pode criar registros de cobrança em um projeto para as informações que precisam ser faturadas.
author: Lisa
feature: Work Management
exl-id: 6f17a892-7f64-4712-8ee2-7a1940b99be3
source-git-commit: ec6ddb50d6b9137837c8031b22f213cd6ada70ff
workflow-type: tm+mt
source-wordcount: '1645'
ht-degree: 1%

---

# Criar registros de cobrança

<!-- Audited: 6/2025 -->

Além de configurar as despesas de rastreamento e receita, você pode criar registros de cobrança em um projeto para as informações que precisam ser faturadas.

Não é possível criar registros de cobrança para tarefas; você só pode criar registros de cobrança para projetos.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront</td> 
   <td>Qualquer</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td>
   <p>Novo: Padrão</p>
   <p>ou</p>
   <p>Atual: Plano</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td>Editar acesso a Projetos e Dados Financeiros</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td>Gerenciar permissões do projeto com permissões para Gerenciar Finanças</td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Visão geral dos registros de cobrança

Os registros de cobrança são criados como anexos a um projeto e contêm dados financeiros do projeto, bem como informações financeiras das tarefas do projeto.

Considere o seguinte ao planejar usar registros de faturamento:

* Você cria um registro de faturamento quando deseja faturar uma quantia de dinheiro relacionada ao projeto para um fornecedor ou parceiro externo. Além de faturar uma quantia fixa para uma origem externa, há momentos em que você precisa faturar a quantia de trabalho no projeto (de horas reportadas) para um contratante externo, bem como as despesas incorridas ou a quantia de receitas fixas. É possível incluir todas essas informações no mesmo registro de cobrança.
* Depois que um registro de cobrança é definido como Faturado, ele não pode ser editado.

  >[!IMPORTANT]
  >
  >Isso é importante quando suas taxas variam e você deseja bloquear as informações de receita e despesa em seu projeto. Adicioná-lo a um registro de cobrança e marcá-lo como Faturado impede que ele seja atualizado quando as taxas são atualizadas em seu sistema.

* Um projeto com registros de cobrança que foram marcados como Faturados não pode ser excluído.

## Criar um registro de cobrança

{{step1-to-projects}}

1. Na página **Projetos**, selecione um projeto.
1. Clique em **Registros de cobrança** no painel esquerdo.
1. Clique em **Novo registro de cobrança**.
1. Na caixa **Novo Registro de Cobrança** que é exibida, especifique as seguintes informações:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Descrição</td> 
      <td>(Obrigatório) Informe uma descrição para o registro de faturamento.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Status da Cobrança</td> 
      <td> <p>Selecione <strong>Não faturado</strong> se este registro ainda não tiver sido faturado.</p> <p>Selecione <strong>Faturado</strong> se o registro de cobrança tiver sido faturado.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Data de Cobrança</td> 
      <td>Selecione a data em que este registro de cobrança foi faturado clicando no ícone de calendário.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Número do Pedido</td> 
      <td>Informe o Número da OC associado a este registro de faturamento.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">ID da Fatura</td> 
      <td>Informe a NFF associada a este registro de faturamento.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Valor adicional</td> 
      <td>Insira o valor fixo do seu registro de cobrança. Esta é a quantia que você pretende faturar para um cliente externo, contratante ou parceiro deste projeto. Este valor não pode ser modificado depois que o status do registro de cobrança é alterado para Faturado.</td> 
     </tr> 
    </tbody> 
   </table>

1. (Opcional) Em **Forms Personalizado**, selecione um formulário personalizado de registros de cobrança que você deseja adicionar ao registro.

   Um formulário personalizado de registros de cobrança deve ser criado antes que você possa selecioná-lo aqui. Somente formulários personalizados ativos são exibidos na lista. Para obter informações, consulte [Criar um formulário personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

1. Clique em **Salvar.** O registro de cobrança foi criado.

## Incluir horas faturáveis, despesas e receitas fixas em um registro de cobrança

### Incluir horas faturáveis em um registro de cobrança {#include-billable-hours-in-a-billing-record}

Você pode incluir horas que foram conectadas em tarefas, problemas ou o projeto em seus registros de cobrança.

Se o usuário que registra as horas ou sua função principal de trabalho estiver associada a uma Taxa por hora de faturamento, a receita dessas horas será adicionada ao registro de faturamento.

* [Que horas podem ser adicionadas a um registro de cobrança](#what-hours-can-be-added-to-a-billing-record)
* [Adicionar horas a um registro de cobrança](#add-hours-to-a-billing-record)

#### Que horas podem ser adicionadas a um registro de cobrança {#what-hours-can-be-added-to-a-billing-record}

Você pode adicionar horas a um registro de faturamento quando as seguintes condições forem atendidas:

* Horas foram registradas para as tarefas, problemas ou projeto.
* O Tipo de Hora das horas registradas é marcado como Count como Receita.

  Para obter mais informações, consulte o artigo [Gerenciar tipos de horas](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/hour-types.md).

* Todas as horas registradas para problemas ou o projeto podem ser adicionadas a um registro de cobrança se o usuário que registra o tempo tiver uma taxa de Faturamento por hora associada a eles ou a sua função de trabalho principal.
* Se as horas forem registradas em uma tarefa, a tarefa deverá ter o seguinte Tipo de Receita:

   * O tipo de receita não pode ser definido como não faturável.
   * Se o Tipo de receita estiver definido como Hora do usuário, o usuário que registrar o tempo deverá ter uma taxa de faturamento por hora definida em seu perfil.
   * Se o tipo de receita for definido como função por hora, a função principal do usuário que registra o tempo deverá ter uma taxa de faturamento por hora.

     >[!NOTE]
     >
     >Você pode substituir taxas de faturamento para funções de trabalho no nível do projeto.\
     >Para obter mais informações, consulte a seção &quot;Substituição das taxas de cobrança da função de trabalho no nível do projeto&quot; no artigo [Visão geral da substituição das taxas de cobrança da função de trabalho e cálculo da Receita em um projeto](../../../manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).

* Se a opção Requer que o tempo seja aprovado para este projeto estiver selecionada em Configurações do projeto, o Proprietário do projeto deve aprovar as horas registradas.\
  Para obter mais informações, consulte [Solicitar tempo para ser aprovado para um projeto](../../../manage-work/projects/manage-projects/require-time-approval-for-projects.md).

#### Adicionar horas a um registro de cobrança {#add-hours-to-a-billing-record}

{{step1-to-projects}}

1. Na página **Projetos**, selecione um projeto.
1. Clique em **Registros de cobrança** no painel esquerdo.
1. Clique na **Descrição** do registro de cobrança para abrir a guia **Detalhes do Registro de Cobrança**.
1. Clique em **Horas faturáveis** no painel esquerdo.
1. Se houver horas que possam ser incluídas em um registro de cobrança, clique em **Adicionar horas**. A caixa **Adicionar horas faturáveis** é aberta.

   >[!NOTE]
   >
   >Se não houver horas registradas ou se as horas registradas não atenderem às condições necessárias para serem adicionadas a um registro de cobrança, o botão **Adicionar horas** não será exibido. Para obter mais informações, consulte a seguinte seção neste artigo: [Que horas podem ser adicionadas a um registro de cobrança](#what-hours-can-be-added-to-a-billing-record).

1. Selecione as entradas de horas que deseja incluir no registro de cobrança e clique em **Adicionar horas**. O Custo Efetivo das horas é adicionado como o **Valor de Horas Faturáveis** para o **Total de Registros de Cobrança**.

1. (Opcional) Clique em **Detalhes de Registros de Cobrança** para revisar os valores de **Horas Faturáveis** e **Total de Registros de Cobrança** e o total de registros de cobrança no cabeçalho de registro de cobrança.

### Incluir despesas faturáveis em um registro de cobrança {#include-billable-expenses-in-a-billing-record}

Se você estiver adicionando despesas faturáveis ao registro de faturamento, verifique se as despesas nas tarefas e o projeto estão marcados como Faturáveis. Despesas que não estão marcadas como Faturáveis não estão disponíveis para serem adicionadas em um registro de cobrança. Para obter mais informações sobre como adicionar despesas, consulte o artigo [Gerenciar despesas do projeto](../../../manage-work/projects/project-finances/manage-project-expenses.md).

Para adicionar despesas faturáveis a um registro de faturamento:

{{step1-to-projects}}

1. Na página **Projetos**, selecione um projeto.
1. Clique em **Registros de cobrança** no painel esquerdo.
1. Clique na **Descrição** do registro de cobrança para abrir a guia **Detalhes do Registro de Cobrança**.
1. Clique em **Despesas faturáveis** no painel esquerdo.
1. (Condicional) Se você tiver adicionado despesas às suas tarefas ou ao projeto e as tiver marcado como Faturáveis, clique em **Adicionar despesas**.

   >[!NOTE]
   >
   >Se você tiver despesas, mas elas não estiverem marcadas como Faturáveis, o botão **Adicionar despesas** não será exibido. Somente despesas faturáveis com um Valor Efetivo maior que zero são elegíveis para serem incluídas em um registro de cobrança.

1. Selecione as despesas faturáveis disponíveis para serem adicionadas ao registro de cobrança e clique em **Adicionar despesas**.  O Valor Efetivo das despesas é adicionado como o valor de **Despesas Faturáveis** para o **Total de Registro de Cobrança**.

1. (Opcional) Clique em **Detalhes de Registros de Cobrança** para examinar os valores de **Despesas Faturáveis** e **Total de Registros de Cobrança**, e o total de registros de cobrança no cabeçalho de registro de cobrança.

### Incluir receitas fixas em um registro de cobrança {#include-fixed-revenues-in-a-billing-record}

Você pode adicionar receitas fixas aos seus registros de cobrança se tiver tarefas com receita fixa disponível. Nenhum outro tipo de tarefa ou receita de projeto está disponível para ser adicionado em um registro de cobrança. Para obter mais informações sobre tipos de receita, consulte a &quot;Visão Geral de Faturamento e Receita&quot; no artigo [Visão Geral de Faturamento e Receita](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

{{step1-to-projects}}

1. Na página **Projetos**, selecione um projeto.
1. Clique em **Registros de cobrança** no painel esquerdo.
1. Clique na **Descrição** do registro de cobrança para abrir a guia **Detalhes do registro de cobrança**.
1. Selecione a guia **Receitas fixas**.
1. Se você tiver adicionado receitas fixas às suas tarefas, clique em **Adicionar receitas fixas**.

   >[!NOTE]
   >
   >Se você tiver valores de receita em tarefas que não estão marcadas como Fixas, o botão **Adicionar receita fixa** não será exibido.

1. Selecione as tarefas cujas receitas fixas você deseja incluir no registro de cobrança e clique em **Adicionar tarefas**.  O valor de **Receita Fixa** das tarefas é adicionado como o valor de **Receitas Faturáveis** para o **Total de Registro de Cobrança**.

1. (Opcional) Clique em **Detalhes de registros de cobrança** para revisar os valores de **Receitas faturáveis** e **Total de registros de cobrança**, e o total de registros de cobrança no cabeçalho de registro de cobrança.

## Editar um registro de cobrança

Depois de criar um registro de cobrança e adicionar horas, despesas e receitas a ele, você pode editar algumas informações no registro existente antes que ele seja marcado como Faturado.

1. Navegue até o registro de faturamento.
1. Selecione **Detalhes do Registro de Cobrança** no painel esquerdo.
1. Edite as informações em todos os campos disponíveis.

   Ou

   Clique no ícone **Editar** ![Editar ícone](assets/edit-icon.png) no canto superior direito e edite as informações em todos os campos disponíveis.

   Atualize o seguinte:

   * **Descrição**
   * **Data de Cobrança**
   * **Status de Cobrança**

     >[!TIP]
     >
     >Se você selecionar **Faturado** para o Status de Cobrança, o registro de cobrança não poderá ser editado depois que você salvar as alterações.

   * **ID da fatura**
   * **Número da OC**
   * **Valor adicional**

   Os seguintes campos não estão disponíveis para edição:

   * **Horas Faturáveis:** O total da Receita Efetiva das horas incluídas no registro de cobrança. Para obter mais informações, consulte a seguinte seção neste artigo: [Incluir horas faturáveis em um registro de cobrança](#include-billable-hours-in-a-billing-record).

   * **Despesas faturáveis**: o valor total das despesas faturáveis incluídas no registro de cobrança. Para obter mais informações, consulte a seguinte seção neste artigo: [Incluir despesas faturáveis em um registro de cobrança](#include-billable-expenses-in-a-billing-record).

   * **Receitas faturáveis**: o total da receita fixa das tarefas incluídas no registro de cobrança. Para obter mais informações, consulte a seguinte seção neste artigo: [Incluir receitas fixas em um registro de cobrança](#include-fixed-revenues-in-a-billing-record).

   * **Total de registros de cobrança**: o total de todos os valores faturáveis. Isso é calculado pela seguinte fórmula:

     ```
     Included Hourly Revenue (Billable Hours) + Included Expenses (Billable Expenses) + Included Fixed Revenue (Billable Revenues) + Fixed Amount for Other Billable Items (Additional Amount)
     ```

1. Clique em **Salvar alterações**.
