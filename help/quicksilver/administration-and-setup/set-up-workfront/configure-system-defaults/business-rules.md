---
user-type: administrator
product-area: system-administration
navigation-topic: business rules
title: Criar e Editar Regras de Negócios
description: Uma regra de negócios permite aplicar validação a objetos do Workfront e impede que os usuários criem, editem ou excluam um objeto quando determinadas condições forem atendidas. As regras de negócios ajudam a melhorar a qualidade dos dados e a eficiência operacional, evitando ações que podem comprometer a integridade dos dados.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 780c996c-5cf1-42fe-898d-2cc208bbae7b
source-git-commit: c16d107d8162f77436337d0b08ea5826d5c25d83
workflow-type: tm+mt
source-wordcount: '1417'
ht-degree: 4%

---

# Criar e editar regras de negócios

<!--

<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

-->

Uma regra de negócios permite aplicar validação a objetos do Workfront e impede que os usuários criem, editem ou excluam um objeto quando determinadas condições forem atendidas. A validação da regra de negócios ajuda a melhorar a qualidade dos dados e a eficiência operacional, evitando ações que podem comprometer a integridade dos dados.

<!--

<div class="preview">

Organizations that have the Workflow Ultimate package can also configure business rules to automate actions for the created, edited, or modified object when certain conditions are met. Available actions include sharing the object, notifying a user, or attaching a custom form to the object.  

</div>

-->

Uma única regra de negócios pode ser atribuída a apenas um objeto. Por exemplo, se você criar uma regra de negócios para não editar projetos sob determinadas condições, não poderá aplicar a mesma regra a tarefas. Seria necessário criar uma regra de negócios separada com as mesmas condições para tarefas.

Os níveis de acesso e o compartilhamento de objetos têm uma prioridade mais alta do que as regras de negócios quando um usuário interage com um objeto. Por exemplo, se um usuário tiver um nível de acesso ou permissão que não permita a edição de um projeto, eles terão precedência sobre uma regra de negócios que permita a edição de um projeto sob determinadas condições.

Quando mais de uma regra de negócios se aplica a um objeto, as regras são todas seguidas, mas não são aplicadas em uma determinada ordem. Por exemplo, você tem duas regras de negócios. Restringe-se a criação de despesas no mês de fevereiro. O segundo impede a edição de um projeto quando o status do projeto é Concluído. Se um usuário tentar adicionar uma despesa a um projeto concluído em junho, a despesa não poderá ser adicionada porque acionou a segunda regra.

As regras de negócios se aplicam à criação, edição e exclusão de objetos por meio da API e da interface do Workfront.

>[!NOTE]
>
>Como as regras de negócios bloqueiam determinadas ações, você sempre deve configurar as regras de negócios primeiro em um ambiente de sandbox ou pré-visualização e testá-las completamente antes de ativá-las na produção.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr>
   <td>Pacote do Adobe Workfront
   </td>
   <td> <p>Validação da regra de negócios:<ul><li><p>Ultimate</p></li><li>
    <p>Workflow Ultimate</p></li></ul></p><p>Automação de regra de negócios:<ul><li>
    <p>Workflow Ultimate</p></li><ul></p>
   </td>
  </tr> 
  <tr> 
   <td>Licença do Adobe Workfront</td> 
   <td>Padrão</td> 
  </tr> 
  <tr> 
   <td>Configurações de nível de acesso</td> 
   <td>Administrador do sistema</td> 
  </tr>  
 </tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Cenários de regras de negócios

* [Cenários de validação de regra de negócios](#scenarios-for-business-rule-validation)
* [Cenários para automação de regras de negócios](#scenarios-for-business-rule-automation)

### Cenários de validação de regra de negócios

O formato de uma validação de regra de negócios é &quot;Se a condição definida for atendida, o usuário será impedido de executar a ação no objeto e a mensagem será exibida&quot;.

A sintaxe das propriedades e outras funções em uma regra de negócios é igual à sintaxe de um campo calculado em um formulário personalizado. Para obter mais informações sobre a sintaxe, consulte [Adicionar campos calculados com o designer de formulário](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md).

Para obter informações sobre instruções IF, consulte a [&#x200B; visão geral das instruções &quot;IF&quot;](/help/quicksilver/reports-and-dashboards/reports/calc-cstm-data-reports/if-statements-overview.md) e os [Operadores de condição em campos personalizados calculados](/help/quicksilver/reports-and-dashboards/reports/calc-cstm-data-reports/condition-operators-calculated-custom-expressions.md).

Para obter informações sobre curingas baseados no usuário, consulte [Usar curingas baseados no usuário para generalizar relatórios](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/use-user-based-wildcards-generalize-reports.md).

Para obter informações sobre curingas baseados em data, consulte [Usar curingas baseados em data para generalizar relatórios](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/use-date-based-wildcards-generalize-reports.md).

Um curinga de API também está disponível nas regras de negócios. Use `$$ISAPI` para acionar a regra somente na API. Use `!$$ISAPI` para impor a regra somente na interface do usuário e permitir que os usuários ignorem a regra por meio da API.

* Por exemplo, essa regra proíbe que os usuários editem projetos concluídos por meio da API. Se o curinga não fosse usado, a regra bloquearia a ação na interface do usuário e na API.

  ```
  IF({status} = "CPL" && $$ISAPI, "You cannot edit completed projects through the API.")
  ```

Os curingas `$$BEFORE_STATE` e `$$AFTER_STATE` são usados em expressões para acessar os valores de campo do objeto antes e depois de qualquer edição.

* Esses curingas estão disponíveis para o acionador de edição. O estado padrão do acionador de edição (se nenhum estado for incluído na expressão) é `$$AFTER_STATE`.
* O acionador de criação de objeto permite apenas `$$AFTER_STATE`, pois o estado anterior não existe.
* O gatilho de exclusão de objeto permite apenas `$$BEFORE_STATE`, pois o estado posterior não existe.

Alguns cenários simples de regras de negócios são:

* Os usuários não podem adicionar novas despesas durante a última semana de fevereiro. Esta fórmula pode ser declarada como:

  ```
  IF(MONTH($$TODAY) = 2 && DAYOFMONTH($$TODAY) >= 22, "You cannot add new expenses during the last week of February.")
  ```

* Os usuários não podem editar o nome de um projeto com o status Concluído. Esta fórmula pode ser declarada como:

  ```
  IF({status} = "CPL" && {name} != $$BEFORE_STATE.{name}, "You cannot edit the project name.")
  ```

O sistema permite uma regra de negócios por objeto por acionador. Por exemplo, uma regra de acionador de edição é permitida para ocorrências. No entanto, você pode incluir várias regras em uma fórmula com instruções IF aninhadas.

Um cenário com instruções IF aninhadas é:

Os usuários não podem editar projetos concluídos e não podem editar projetos com uma Data de conclusão planejada para março. Esta fórmula pode ser declarada como:

```
IF(
    $$AFTER_STATE.{status}="CPL",
    "You cannot edit a completed project",
    IF(
        MONTH({plannedCompletionDate})=3,
        "You cannot edit a project with a planned completion date in March")
)
```


<!--

## Scenarios for business rule automation

>[!NOTE]
>
>Your organization must have a Workflow Ultimate package to use business rule automation.

The format of a business rule automation is "IF the defined condition is met, then the selected automation is triggered."

Business rule automation formulas do not require an error message

To ensure that an automation runs whenever the selected object and action occurs, such as when a project is created, use the following formula:

```
IF(true, true)
```

To share a project only if that's project has been approved, use a formula like the following:

```
IF({status} = "APR", true)
```

You can use wildcards in business rule actions, as described in the section [Scenarios for business rule validation](#scenarios-for-business-rule-validation).

-->

## Adicionar uma nova regra de negócios

{{step-1-to-setup}}

1. Clique em **Regras de Negócios** no painel esquerdo.
1. Clique em **Nova regra de negócio**.

1. Digite o **Nome** da regra de negócios na caixa de diálogo do construtor de regras.
1. No campo **Está ativo**, selecione se a regra deve estar ativa ao salvá-lo.

   Se você selecionar **Não**, a regra será salva como inativa e você poderá ativá-la mais tarde.

1. (Opcional) Insira uma **Descrição** da regra de negócios e o que acontece quando ela é aplicada.


1. Selecione o tipo de objeto ao qual atribuir a regra de negócios.

   ![Selecione um objeto](assets/object-for-business-rule4.png)

   Você pode aplicar regras de negócios aos seguintes objetos:

   * Projeto
   * Tarefa
   * Problema / Solicitação
   * Portfólio
   * Documento
   * Programa
   * Despesa
   * Empresa
   * Iteração
   * Registro de cobrança
   * Grupo
   * Recurso não trabalhista
   * Risco
   * Cartão de tarifas
   * Atribuição
   * Usuário
   * Função
   * Hora
   * Modelo
   * Folga
   * Conjunto de Recursos
<!--
   * <span class="preview">Job role</span>
   * <span class="preview">Non-labor resource category</span>
   * <span class="preview">Resource Pool</span>
   * <span class="preview">Time Off</span>
   * <span class="preview">Hour</span>
   * <span class="preview">Staffing Plan</span>
   * <span class="preview">Template</span>
   * <span class="preview">Staffing Plan Resource</span>
   * <span class="preview">Team</span>
-->

1. Digite o **Nome** da regra de negócios na caixa de diálogo do construtor de regras.
1. No campo **Está ativo**, selecione se a regra deve estar ativa ao salvá-lo.

   Se você selecionar **Não**, a regra será salva como inativa e você poderá ativá-la mais tarde.

1. Selecione um **Acionador** para a regra de negócios. As opções são:

   * **Criado** A regra é aplicada quando um usuário tenta criar um objeto.
   * **Editada** A regra é aplicada quando um usuário tenta editar um objeto.
   * **Excluída** A regra é aplicada quando um usuário tenta excluir um objeto.

1. Crie a fórmula no editor de fórmulas, no centro da caixa de diálogo de regra de negócios.

   O formato de uma regra de negócios é &quot;Se a condição definida for atendida, o usuário será impedido de realizar a ação no objeto e a mensagem será exibida&quot;.

   Na área da fórmula, as partes da regra de negócios criadas são a condição e a mensagem exibida no Workfront quando a condição é atendida.

   * O &quot;objeto&quot; é o tipo de objeto selecionado ao criar a regra de negócios. Ele é exibido no cabeçalho da caixa de diálogo.
   * A &quot;ação&quot; é o acionador selecionado para a regra: criar, editar ou excluir o objeto.
   * Como o objeto e a ação já estão definidos, você não os inclui na fórmula.
   * A mensagem de erro personalizada <!--<span class="preview">is included only if the rule is for validation, and </span>--> é exibida ao usuário quando ele aciona a regra de negócios. Ele deve fornecer instruções claras sobre o que deu errado e como corrigir o problema.

     É possível incluir um URL estático na mensagem de erro, um link para a documentação ou outras páginas úteis para orientar o usuário sobre como modificar sua ação dentro da restrição da regra.

     Neste exemplo, &quot;Saiba mais&quot; vinculará ao URL. `"You are not allowed to add a new project in November.[Learn more](http://url)"` A URL deve estar entre parênteses, mas o texto do link entre parênteses não é necessário. Você pode exibir o URL completo e ele será um link clicável.

   ![Adicionar caixa de diálogo de regra de negócios](assets/add-business-rule-dialog-no-ai-button.png) <!--UPDATE ME-->

   Este exemplo é uma regra de negócios para projetos. Se o mês atual for novembro, os usuários não poderão criar novos projetos e a mensagem explica isso.

   Para obter mais exemplos de regras de negócios, consulte [Cenários para regras de negócios](#scenarios-for-business-rules) neste artigo.

1. (Opcional) Use a fórmula **Expressões** e **Campos** no painel direito para auxiliar na criação da regra.

   Procure por uma expressão ou campo para restringir a lista de itens disponíveis.

   A lista de campos disponíveis é limitada aos campos relacionados ao tipo de objeto da regra de negócios.

1. (Condicional) Se você estiver validando a ação, se sua organização estiver no pacote Workfront Ultimate, na área Depois, selecione **Validar o objeto**.

   Para outros pacotes, essa opção é pré-selecionada.

<!--

1. (Conditional) To automate another action,, select the action. 

   For details on these actions, see the section [Business rule automation options](#business-rule-automation-options) in this article.

   >[!NOTE]
   >
   >Your organization must be on the Workflow Ultimate package to use actions besides validation. If you do not see these other options, your organization is not on the Workflow Ultimate package.

   -->

1. Clique em **Salvar** quando terminar de criar a regra de negócios.

>[!NOTE]
>
>Após adicionar uma regra de negócios, você deverá testá-la adicionando, editando ou excluindo o objeto associado para garantir que a regra seja aplicada corretamente.

<!--

<div class="preview">

### Business rule automation options

   >[!NOTE]
   >
   >Your organization must be on the Workflow Ultimate package to use actions besides validation. If you do not see these other options, your organization is not on the Workflow Ultimate package.

You can set these actions to automate when the business rule is triggered. Available actions depend on the selected object type.

|Automation|Further configuration|
|---|---|
|Attach a custom form|Select the custom form that you want to add|
|Share the object|Select the people, roles, groups, companies, or access levels that you want to share the object with.|

-->

## Ativar uma regra de negócios

Quando uma regra de negócios está inativa, o campo Está Ativo na lista de regras de negócios exibe Falso. Não é possível atualizar o status da regra na exibição em lista.

Para ativar uma regra de negócios:

1. Selecione a regra de negócios na lista de regras e clique no ícone Editar.
1. Selecione **Sim** para **Está ativo** na caixa de diálogo de regra de negócios.
1. Clique em **Salvar**.
