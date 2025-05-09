---
navigation-topic: financials
title: Criar registros de cobrança
description: Além de configurar as despesas de rastreamento e receita, você pode criar registros de cobrança em um projeto para as informações que precisam ser faturadas.
author: Lisa
feature: Work Management
exl-id: 6f17a892-7f64-4712-8ee2-7a1940b99be3
source-git-commit: 485f2985c70b1bb095e31323b7b4698bcb7a04cf
workflow-type: tm+mt
source-wordcount: '1862'
ht-degree: 0%

---

# Criar registros de cobrança

Além de configurar as despesas de rastreamento e receita, você pode criar registros de cobrança em um projeto para as informações que precisam ser faturadas.

Não é possível criar registros de cobrança para tarefas. Você só pode criar registros de cobrança para projetos.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte acesso para executar as etapas deste artigo:

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

Os registros de cobrança são criados como anexos a um projeto e contêm dados financeiros do projeto, bem como algumas informações financeiras para as tarefas em um projeto.

Considere o seguinte ao planejar usar registros de faturamento:

* Você cria um registro de faturamento quando deseja faturar uma quantia de dinheiro relacionada ao projeto para um fornecedor ou parceiro externo. Além de faturar uma quantia fixa para uma origem externa, há momentos em que você precisa faturar a quantia de trabalho no projeto (de horas reportadas) para um contratante externo, bem como as despesas incorridas ou a quantia de receitas fixas. É possível incluir todas essas informações no mesmo registro de cobrança.
* Depois que um registro de cobrança é definido como Faturado, ele não pode ser editado.

  >[!IMPORTANT]
  >
  >Isso é importante quando suas taxas variam e você deseja bloquear as informações de receita e despesa em seu projeto. Adicioná-lo a um registro de cobrança e marcá-lo como Faturado impede que ele seja atualizado quando as taxas são atualizadas em seu sistema.

* Um projeto com registros de cobrança que foram marcados como Faturados não pode ser excluído.

## Criar um registro de cobrança

1. Navegue até um projeto.
1. Clique em **Registros de cobrança** no painel esquerdo.
1. Com **Detalhes do Registro de Cobrança** selecionados no painel esquerdo, clique em **Novo Registro de Cobrança**.
1. Na caixa **Novo Registro de Cobrança** que é exibida, especifique as seguintes informações:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Descrição</td> 
      <td>Este campo é obrigatório. Especifique uma descrição para o registro de cobrança, para refletir a finalidade ou a intenção deste registro.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Status da Cobrança</td> 
      <td> <p>Selecione <strong>Não faturado</strong>, se este registro ainda não tiver sido faturado.</p> <p>Selecione <strong>Faturado</strong> quando o registro de cobrança for faturado.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Data de Cobrança</td> 
      <td>Selecione a data em que este registro de cobrança é faturado clicando no ícone de calendário.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Número do Pedido</td> 
      <td>Se houver um Número da OC associado a esse registro de cobrança, especifique essas informações nesse campo.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">ID da Fatura</td> 
      <td>Se houver uma fatura associada a esse registro de cobrança, especifique essas informações nesse campo.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Valor adicional</td> 
      <td>Insira o valor fixo do seu registro de cobrança. Esta é a quantia que você pretende faturar para um cliente externo, contratante ou parceiro deste projeto. Este valor não pode ser modificado depois que o status do registro de cobrança for alterado para Faturado.</td> 
     </tr> 
    </tbody> 
   </table>

1. (Opcional) Em **Forms Personalizado**, selecione um formulário personalizado de registros de cobrança que você deseja adicionar ao registro de cobrança.

   Você (ou outro usuário com acesso a formulários personalizados) deve criar um formulário personalizado de registros de cobrança antes de selecioná-lo aqui. Somente formulários personalizados ativos são exibidos na lista. Para obter informações sobre como criar formulários personalizados, consulte [Criar um formulário personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

   Você pode repetir essa etapa para adicionar outros formulários personalizados necessários para o registro de cobrança.

1. Clique em **Salvar.**

   O registro de cobrança é criado. Para incluir Horas Faturáveis, Despesas e Receitas Fixas no registro de faturamento, siga as etapas descritas na subseção a seguir.

## Incluir Horas Faturáveis, Despesas e Receitas Fixas em um registro de cobrança

* [Incluir Horas Faturáveis em um registro de cobrança](#include-billable-hours-in-a-billing-record)
* [Incluir despesas faturáveis em um registro de cobrança](#include-billable-expenses-in-a-billing-record)
* [Incluir receitas fixas em um registro de cobrança](#include-fixed-revenues-in-a-billing-record)

### Incluir Horas Faturáveis em um registro de cobrança {#include-billable-hours-in-a-billing-record}

Você pode incluir horas que foram conectadas em tarefas, problemas ou o projeto em seus registros de cobrança.\
Se o usuário que registra as horas ou sua função de trabalho principal estiver associada a uma taxa de cobrança por hora, a receita dessas horas será adicionada ao registro de cobrança.

* [Que horas podem ser adicionadas a um registro de cobrança](#what-hours-can-be-added-to-a-billing-record)
* [Adicionar horas a um registro de cobrança](#add-hours-to-a-billing-record)

#### Que horas podem ser adicionadas a um registro de cobrança {#what-hours-can-be-added-to-a-billing-record}

Você pode adicionar horas a um registro de faturamento quando as seguintes condições forem atendidas:

* Tarefas, problemas ou o projeto têm horas registradas.
* O Tipo de Hora das horas registradas é marcado como Count como Receita.

  Para obter mais informações sobre Tipos de Horas, consulte o artigo [Gerenciar tipos de horas](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/hour-types.md).

* Todas as horas registradas para problemas ou para o projeto podem ser adicionadas a um registro de cobrança se o usuário que registra o tempo tiver uma taxa de Faturamento por hora associada a ele ou a sua Função de trabalho principal.
* Se as horas forem registradas em uma tarefa, a tarefa deverá ter o seguinte Tipo de Receita:

   * O tipo de receita não pode ser definido como não faturável.
   * Se o Tipo de receita estiver definido como Hora do usuário, o usuário que registrar o tempo deverá ter uma taxa de faturamento por hora definida em seu perfil.
   * Se o tipo de receita for definido como função por hora, a função principal do usuário que registra o tempo deverá ter uma taxa de faturamento por hora.

     >[!NOTE]
     >
     >Você pode substituir taxas de faturamento para funções de trabalho no nível do projeto.\
     >Para obter mais informações sobre substituição de taxas de cobrança de função de trabalho, consulte a seção &quot;Substituição de taxas de cobrança de função de trabalho no nível do projeto&quot; no artigo [Visão geral da substituição de taxas de cobrança de função de trabalho e cálculo de Receita em um projeto](../../../manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).

* Se **Solicitar aprovação para este projeto** estiver marcado em Configurações do Projeto, o Proprietário do Projeto deverá aprovar as horas registradas.\
  Para obter mais informações sobre a exigência de aprovação em horas de projeto, consulte o artigo [Exigir que o tempo seja aprovado para um projeto](../../../manage-work/projects/manage-projects/require-time-approval-for-projects.md).

#### Adicionar horas a um registro de cobrança {#add-hours-to-a-billing-record}

Para adicionar horas faturáveis a um registro de faturamento:

1. Vá para o projeto com os registros de cobrança.
1. Clique em **Registros de cobrança** no painel esquerdo.
1. Clique na **Descrição** de um registro de cobrança para abrir a guia **Detalhes do Registro de Cobrança**.
1. Clique em **Horas faturáveis** no painel esquerdo.
1. Se houver horas que possam ser incluídas em um registro de cobrança, clique em **Adicionar horas**.\
   A caixa **Adicionar horas faturáveis** é aberta.

   >[!NOTE]
   >
   >Se não houver horas registradas ou se as horas registradas não atenderem às condições necessárias para serem adicionadas a um registro de cobrança, o botão **Adicionar horas** não será exibido. Para obter mais informações sobre quais horas podem ser registradas em um registro de cobrança, consulte a seção [Quais horas podem ser adicionadas a um registro de cobrança](#what-hours-can-be-added-to-a-billing-record) neste artigo.

1. Selecione as entradas de horas que deseja incluir no registro de cobrança e clique em **Adicionar horas**.\
   O Custo Efetivo das horas é adicionado como o **Valor de Horas Faturáveis** para o **Total de Registros de Cobrança**.

1. (Opcional) Clique em **Detalhes de Registros de Cobrança** para examinar os valores de **Horas Faturáveis** e **Total de Registros de Cobrança**. Você também pode ver o total do registro de cobrança no cabeçalho do registro de cobrança.

### Incluir Despesas Faturáveis em um registro de cobrança {#include-billable-expenses-in-a-billing-record}

Se você estiver adicionando Despesas Faturáveis ao registro de faturamento, certifique-se de que as despesas nas tarefas e no projeto estejam marcadas como Faturáveis. Despesas que não estão marcadas como Faturáveis não estão disponíveis para serem adicionadas em um registro de cobrança. Para obter mais informações sobre como adicionar despesas, consulte o artigo [Gerenciar despesas do projeto](../../../manage-work/projects/project-finances/manage-project-expenses.md).

Para adicionar despesas faturáveis a um registro de faturamento:

1. Vá para o projeto com os registros de cobrança.
1. Clique em **Registros de cobrança** no painel esquerdo.
1. Clique na **Descrição** de um registro de cobrança para abrir a guia **Detalhes do Registro de Cobrança**.
1. Clique em **Despesas faturáveis** no painel esquerdo.
1. (Condicional) Se você tiver adicionado despesas às suas tarefas ou ao projeto e as tiver marcado como Faturáveis, clique em **Adicionar despesas**.

   >[!NOTE]
   >
   >Se você tiver despesas, mas elas não estiverem marcadas como Faturáveis, o botão **Adicionar Despesas** não será exibido. Somente despesas faturáveis com um Valor Efetivo maior que zero são elegíveis para serem incluídas em um registro de cobrança.

1. Selecione as despesas faturáveis disponíveis para serem adicionadas ao registro de cobrança e clique em **Adicionar despesas**.\
   O Valor Efetivo das despesas é adicionado como o valor de **Despesas Faturáveis** para o **Total de Registro de Cobrança**.

1. (Opcional) Clique em **Detalhes de Registros de Cobrança** para examinar os valores de **Despesas Faturáveis** e **Total de Registros de Cobrança**. Você também pode ver o total do registro de cobrança no cabeçalho do registro de cobrança.

### Incluir receitas fixas em um registro de cobrança {#include-fixed-revenues-in-a-billing-record}

Você pode adicionar Receitas Fixas aos seus registros de faturamento se tiver tarefas com Receita Fixa disponível. Nenhum outro tipo de tarefa ou receita de projeto está disponível para ser adicionado em um registro de cobrança. Para obter mais informações sobre tipos de receita, consulte a seção [Visão Geral de Faturamento e Receita](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md) em [Visão Geral de Faturamento e Receita](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

Para adicionar receitas fixas a um registro de faturamento:

1. Vá para o projeto com os registros de cobrança.
1. Clique em **Registros de cobrança** no painel esquerdo.
1. Clique na **Descrição** de um registro de cobrança para abrir a guia **Detalhes do Registro de Cobrança**.
1. Selecione a guia **Receitas fixas**.
1. Se você tiver adicionado receitas fixas às suas tarefas, clique em **Adicionar receitas fixas**.

   >[!NOTE]
   >
   >Se você tiver valores de receita em tarefas que não estão marcadas como &quot;Fixas&quot;, o botão **Adicionar Receita Fixa** não será exibido.

1. Selecione as tarefas cujas receitas fixas você deseja incluir no registro de cobrança e clique em **Adicionar tarefas**.\
   O valor de **Receita Fixa** das tarefas é adicionado como o valor de **Receitas Faturáveis** para o **Total de Registro de Cobrança**.

1. (Opcional) Clique em **Detalhes de Registros de Cobrança** para examinar os valores de **Receitas Faturáveis** e **Total de Registros de Cobrança**. Você também pode ver o total do registro de cobrança no cabeçalho do registro de cobrança.

## Editar um registro de cobrança

Depois de criar um registro de cobrança e incluir horas, despesas e receitas no registro de cobrança, você pode editar algumas informações no registro existente, antes que ele seja marcado como Faturado.

1. Vá para o registro de cobrança.
1. Com **Detalhes do Registro de Cobrança** selecionados no painel esquerdo, edite as informações em todos os campos disponíveis

   Ou

   Clique no **ícone Editar** ![ícone Editar](assets/edit-icon.png) no canto superior direito e edite as informações em todos os campos disponíveis.

   Atualize o seguinte:

   * **Descrição**
   * **Status de Cobrança**

     >[!TIP]
     >
     >Se você selecionar **Faturado** para o Status de Cobrança, o registro de cobrança não poderá ser editado depois que você salvar as alterações.

   * **Data de Cobrança**
   * **Número da OC**
   * **ID da fatura**
   * **Valor adicional**

   Os seguintes campos não estão disponíveis para edição:

   * **Horas Faturáveis:** O total da Receita Efetiva das horas incluídas no registro de cobrança. Para obter mais informações sobre como incluir horas em um registro de cobrança, consulte a seção [Incluir horas faturáveis em um registro de cobrança](#include-billable-hours-in-a-billing-record) neste artigo.

   * **Despesas faturáveis**: o valor total das despesas faturáveis incluídas no registro de cobrança. Para obter mais informações sobre como incluir despesas faturáveis em um registro de cobrança, consulte a seção [Incluir despesas faturáveis em um registro de cobrança](#include-billable-expenses-in-a-billing-record) neste artigo.

   * **Receitas faturáveis**: o total da receita fixa das tarefas incluídas no registro de cobrança. Para obter mais informações sobre como incluir receitas fixas em um registro de cobrança, consulte a seção [Incluir receitas fixas em um registro de cobrança](#include-fixed-revenues-in-a-billing-record) neste artigo.

   * **Total de registros de cobrança**: o total de todos os valores faturáveis. Isso é calculado pela seguinte fórmula:

     ```
     Included Hourly Revenue (Billable Hours) + Included Expenses (Billable Expenses) + Included Fixed Revenue (Billable Revenues) + Fixed Amount for Other Billable Items (Additional Amount)
     ```

1. Clique em **Salvar***Alterações**.
