---
navigation-topic: financials
title: Criar registros de faturamento
description: Além de configurar a receita e as despesas de rastreamento, você pode criar registros de faturamento em um projeto para obter informações que precisam ser faturadas.
author: Alina
feature: Work Management
exl-id: 6f17a892-7f64-4712-8ee2-7a1940b99be3
source-git-commit: a849ecaf6097dcdc924aaab2867f37bf57d5bc09
workflow-type: tm+mt
source-wordcount: '1934'
ht-degree: 1%

---

# Criar registros de faturamento

Além de configurar a receita e as despesas de rastreamento, você pode criar registros de faturamento em um projeto para obter informações que precisam ser faturadas.

Não é possível criar registros de faturamento para tarefas. Você só pode criar registros de faturamento para projetos.

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plano Adobe Workfront*</td> 
   <td> <p>Qualquer Um</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Plano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a Projetos e Dados Financeiros</p> <p>Observação: Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerencie permissões do projeto com permissões para Gerenciar finanças</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

## Visão geral dos registros de cobrança

Os registros de faturamento são criados como anexos a um projeto e contêm dados financeiros do projeto, bem como algumas informações financeiras para as tarefas em um projeto.

Considere o seguinte ao planejar o uso de registros de faturamento:

* Você cria um registro de faturamento quando deseja faturar uma quantia relacionada ao projeto para um fornecedor ou parceiro externo. Além de faturar uma quantia fixa a uma fonte externa, há ocasiões em que você precisa faturar a quantia de trabalho no projeto (de horas registradas) para um contratante externo, bem como as despesas incorridas ou a quantia de receita fixa. Você pode incluir todas essas informações no mesmo registro de faturamento.
* Depois que um registro de faturamento é definido como Faturado, ele não pode ser editado.

   >[!IMPORTANT]
   >
   >Isso é importante quando suas taxas variam e você deseja bloquear as informações de receita e despesa do seu projeto. Adicioná-lo a um registro de faturamento e marcá-lo como Faturado impede que seja atualizado quando as taxas forem atualizadas em seu sistema.

* Um projeto com registros de faturamento que foram marcados como Faturado não pode ser excluído.

## Criar um registro de faturamento

1. Navegue até um projeto.
1. Clique em **Registros de cobrança** no painel esquerdo.

   Esta seção pode estar localizada em **Mostrar mais**.

1. Com **Detalhes do Registro de Faturamento** selecionado no painel esquerdo, clique em **Novo Registro de Faturamento**.
1. No **Novo Registro de Faturamento** , especifique as seguintes informações:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Descrição</td> 
      <td>Este campo é obrigatório. Especifique uma descrição para o registro de faturamento, para refletir a finalidade ou a intenção deste registro.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Status da Cobrança</td> 
      <td> <p>Selecionar <strong>Não Faturado</strong>, se esse registro ainda não tiver sido cobrado.</p> <p>Selecionar <strong>Faturado</strong> quando o registro de faturamento é cobrado.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Data de Cobrança</td> 
      <td>Selecione a data de faturamento deste registro clicando no ícone de calendário.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Número do Pedido</td> 
      <td>Se houver um Número da OC associado a este registro de faturamento, especifique essas informações neste campo.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">ID da Fatura</td> 
      <td>Se houver uma NFF associada a esse registro de faturamento, especifique essas informações neste campo.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Valor adicional</td> 
      <td>Informe a quantia fixa do seu registro de faturamento. Esse é o valor que você pretende faturar um cliente externo, contratante ou parceiro para esse projeto. Esse valor não pode ser modificado após o status do registro de faturamento ser alterado para Faturado.</td> 
     </tr> 
    </tbody> 
   </table>

1. (Opcional) Em **Forms personalizada**, selecione um formulário personalizado de registros de faturamento que deseja adicionar ao registro de faturamento.

   Você (ou outro usuário com acesso a formulários personalizados) deve criar um formulário personalizado de registros de faturamento antes de selecioná-lo aqui. Somente os formulários personalizados ativos são exibidos na lista. Para obter informações sobre como criar formulários personalizados, consulte [Criar ou editar um formulário personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

   É possível repetir essa etapa para adicionar outros formulários personalizados necessários para o registro de faturamento.

1. Clique em **Salvar.**

   O registro de faturamento é criado. Para incluir Horas Faturáveis, Despesas e Receitas Fixas no registro de faturamento, siga as etapas descritas na subseção a seguir.

## Incluir Horas Faturáveis, Despesas e Receitas Fixas em um registro de faturamento

* [Incluir Horas Faturáveis em um registro de faturamento](#include-billable-hours-in-a-billing-record)
* [Incluir Despesas Faturáveis em um registro de faturamento](#include-billable-expenses-in-a-billing-record)
* [Incluir receitas fixas em um registro de faturamento](#include-fixed-revenues-in-a-billing-record)

### Incluir Horas Faturáveis em um registro de faturamento {#include-billable-hours-in-a-billing-record}

Você pode incluir horas que foram conectadas em tarefas, problemas ou o projeto em seus registros de faturamento.\
Se o usuário que registra as horas ou sua Função de Trabalho Principal estiver associada a uma Taxa de Faturamento por Hora, a receita dessas horas será adicionada ao registro de faturamento.

* [Quais horas podem ser adicionadas a um registro de faturamento](#what-hours-can-be-added-to-a-billing-record)
* [Adicionar horas a um registro de faturamento](#add-hours-to-a-billing-record)

#### Quais horas podem ser adicionadas a um registro de faturamento {#what-hours-can-be-added-to-a-billing-record}

Você pode adicionar horas a um registro de faturamento quando as seguintes condições forem atendidas:

* Tarefas, problemas ou o projeto tem horas registradas.
* O Tipo de hora das horas registradas é marcado como Contagem como Receita.

   Para obter mais informações sobre Tipos de hora, consulte o artigo [Gerenciar tipos de hora](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/hour-types.md).

* Todas as horas registradas para problemas ou para o projeto podem ser adicionadas a um registro de faturamento se o usuário que registra a hora tiver uma taxa de Faturamento por hora associada a eles ou sua Função de trabalho principal.
* Se as horas estiverem conectadas em uma tarefa, a tarefa deverá ter o seguinte Tipo de Receita:

   * O Tipo de Receita não pode ser definido como Não Faturável.
   * Se o Tipo de receita for definido como Usuário por hora, o usuário que faz logon na hora deverá ter uma taxa de Faturamento por hora definida em seu perfil.
   * Se o Tipo de receita estiver definido como Função por hora, a Função principal do usuário que registra a hora deverá ter uma taxa de Faturamento por hora.

      >[!NOTE]
      >
      >Você pode substituir as taxas de faturamento das funções de cargo no nível do projeto.\
      >Para obter mais informações sobre a sobreposição de taxas de faturamento de função de cargo, consulte a seção &quot;Sobreposição de Taxas de Faturamento de Função de Cargo no Nível do Projeto&quot; no artigo [Visão Geral das Taxas de Faturamento da Função do Trabalho e cálculo da Receita em um projeto](../../../manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).

* If **Exigir tempo para ser aprovado para este projeto** estiver marcada em Configurações do projeto, o Proprietário do projeto deverá aprovar as horas registradas.\
   Para obter mais informações sobre como exigir aprovação nas horas do projeto, consulte o artigo [Exigir tempo para ser aprovado para um projeto](../../../manage-work/projects/manage-projects/require-time-approval-for-projects.md).

#### Adicionar horas a um registro de faturamento {#add-hours-to-a-billing-record}

Para adicionar horas faturáveis a um registro de faturamento:

1. Vá para o projeto com os registros de cobrança.
1. Clique em **Registros de cobrança** no painel esquerdo.

   Esta seção pode estar localizada em **Mostrar mais**.

1. Clique no botão **Descrição** de um registro de faturamento para abrir o **Detalhes do Registro de Faturamento** guia .

1. Clique em **Horas Faturáveis** no painel esquerdo.
1. Se houver horas que possam ser incluídas em um registro de faturamento, clique em **Adicionar horas**.\
   O **Adicionar Horas Faturáveis** será aberta.

   >[!NOTE]
   >
   >Se não houver horas registradas ou se as horas registradas não atenderem às condições necessárias para serem adicionadas a um registro de faturamento, a variável **Adicionar horas** não é exibido. Para obter mais informações sobre quais horas podem ser registradas em um registro de faturamento, consulte a seção [Quais horas podem ser adicionadas a um registro de faturamento](#what-hours-can-be-added-to-a-billing-record) neste artigo.

1. Selecione as entradas de hora que deseja incluir no registro de faturamento e clique em **Adicionar horas**.\
   O Custo Real das horas é adicionado como o **Horas Faturáveis** do **Total do Registro de Faturamento**.

1. (Opcional) Clique em **Detalhes dos Registros de Faturamento** para revisar a **Horas Faturáveis** e **Total do Registro de Faturamento** montantes. Você também pode ver o total do registro de faturamento no cabeçalho do registro de faturamento.

### Incluir Despesas Faturáveis em um registro de faturamento {#include-billable-expenses-in-a-billing-record}

Se estiver adicionando Despesas Faturáveis ao registro de faturamento, verifique se as despesas das tarefas e do projeto estão marcadas como Faturáveis. As despesas não marcadas como Faturáveis não estão disponíveis para adicionar um registro de cobrança. Para obter mais informações sobre como adicionar despesas, consulte o artigo [Gerenciar despesas do projeto](../../../manage-work/projects/project-finances/manage-project-expenses.md).

Para adicionar despesas faturáveis a um registro de faturamento:

1. Vá para o projeto com os registros de cobrança.
1. Clique em **Registros de cobrança** no painel esquerdo.

   Talvez seja necessário clicar em **Mostrar mais**, em seguida **Registros de cobrança**.

1. Clique no botão **Descrição** de um registro de faturamento para abrir o **Detalhes do Registro de Faturamento** guia .

1. Clique em **Despesas Faturáveis** no painel esquerdo.
1. (Condicional) Se você tiver adicionado despesas às suas tarefas ou ao projeto e as tiver marcado como Faturável, clique em **Adicionar Despesas**.

   >[!NOTE]
   >
   >Se você tiver despesas, mas elas não forem marcadas como Faturáveis, a variável **Adicionar Despesas** não é exibido. Somente as despesas faturáveis com uma Quantia Real maior que zero são elegíveis para serem incluídas em um registro de faturamento.

1. Selecione as despesas faturáveis disponíveis para serem adicionadas ao registro de faturamento e clique em **Adicionar Despesas**.\
   A Quantia Real das despesas é adicionada como a **Despesas Faturáveis** do **Total do Registro de Faturamento**.

1. (Opcional) Clique em **Detalhes dos Registros de Faturamento** para revisar a **Despesas Faturáveis** e **Total do Registro de Faturamento** montantes. Você também pode ver o total do registro de faturamento no cabeçalho do registro de faturamento.

### Incluir receitas fixas em um registro de faturamento {#include-fixed-revenues-in-a-billing-record}

Você pode adicionar Receita Fixa aos seus registros de faturamento se tiver tarefas com Receita Fixa disponíveis. Nenhum outro tipo de tarefa ou receita de projeto está disponível para ser adicionado em um registro de cobrança. Para obter mais informações sobre tipos de receita, consulte [Visão Geral da Faturamento e Receita](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md) seção em [Visão Geral da Faturamento e Receita](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

Para adicionar receitas fixas a um registro de faturamento:

1. Vá para o projeto com os registros de cobrança.
1. Clique em **Registros de cobrança** no painel esquerdo.

   Talvez seja necessário clicar em **Mostrar mais**, em seguida **Registros de cobrança**.

1. Clique no botão **Descrição** de um registro de faturamento para abrir o **Detalhes do Registro de Faturamento** guia .

1. Selecione o **Receitas Fixas** guia .
1. Se você tiver adicionado receitas fixas às suas tarefas, clique em **Adicionar receitas fixas**.

   >[!NOTE]
   >
   >Se você tiver valores de receita em tarefas, mas eles não estiverem marcados como &quot;Fixo&quot;, a variável **Adicionar receita fixa** não é exibido.

1. Selecione as tarefas cujas receitas fixas você deseja incluir no registro de faturamento e clique em **Adicionar Tarefas**.\
   O **Receita fixa** a quantidade de tarefas é adicionada como **Receitas Faturáveis** do **Total do Registro de Faturamento**.

1. (Opcional) Clique em **Detalhes dos Registros de Faturamento** para revisar a **Receitas Faturáveis** e **Total do Registro de Faturamento** montantes. Você também pode ver o total do registro de faturamento no cabeçalho do registro de faturamento.

## Editar um registro de faturamento

Depois de criar um registro de faturamento, incluindo horas, despesas e receitas no registro de faturamento, você pode editar algumas informações no registro existente, antes que sejam marcadas como Faturadas.

1. Vá para o registro de cobrança.
1. Com **Detalhes do Registro de Faturamento** selecionado no painel esquerdo , edite as informações em qualquer campo disponível

   Ou

   Clique no botão **Ícone Editar** ![](assets/edit-icon.png) no canto superior direito, edite as informações em qualquer campo disponível.

   Atualize o seguinte:

   * **Descrição**
   * **Status da Cobrança**

      >[!TIP]
      >
      >Se você selecionar **Faturado** para o Status de Faturamento, o registro de faturamento não pode ser editado depois que você salva as alterações.

   * **Data de Cobrança**
   * **Número do Pedido**
   * **ID da Fatura**
   * **Valor adicional**

   Os seguintes campos não estão disponíveis para edição:

   * **Horas Faturáveis:** O total da Receita Real das horas incluídas no registro de faturamento. Para obter mais informações sobre como incluir horas em um registro de faturamento, consulte a seção [Incluir Horas Faturáveis em um registro de faturamento](#include-billable-hours-in-a-billing-record) neste artigo.

   * **Despesas Faturáveis**: O total da Quantia Real das despesas faturáveis incluídas no registro de faturamento. Para obter mais informações sobre como incluir despesas faturáveis em um registro de faturamento, consulte a seção [Incluir Despesas Faturáveis em um registro de faturamento](#include-billable-expenses-in-a-billing-record) neste artigo.

   * **Receitas Faturáveis**: O total da Receita fixa das tarefas incluídas no registro de faturamento. Para obter mais informações sobre como incluir receitas fixas em um registro de faturamento, consulte a seção [Incluir receitas fixas em um registro de faturamento](#include-fixed-revenues-in-a-billing-record) neste artigo.

   * **Total do Registro de Faturamento**: O total de todos os valores faturáveis. Isso é calculado pela seguinte fórmula:

      ```
      Included Hourly Revenue (Billable Hours) + Included Expenses (Billable Expenses) + Included Fixed Revenue (Billable Revenues) + Fixed Amount for Other Billable Items (Additional Amount)
      ```


1. Clique em **Salvar***Alterações**.
