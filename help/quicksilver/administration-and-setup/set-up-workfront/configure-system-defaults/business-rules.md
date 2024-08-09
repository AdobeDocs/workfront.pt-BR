---
user-type: administrator
product-area: system-administration
navigation-topic: business rules
title: Criar e Editar Regras de Negócios
description: Uma regra de negócios permite aplicar validação a objetos do Workfront e impede que os usuários criem, editem ou excluam um objeto quando determinadas condições forem atendidas. As regras de negócios ajudam a melhorar a qualidade dos dados e a eficiência operacional, evitando ações que podem comprometer a integridade dos dados.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 780c996c-5cf1-42fe-898d-2cc208bbae7b
source-git-commit: f036fbfc203f942fa5a22070860c3a20035a183b
workflow-type: tm+mt
source-wordcount: '1078'
ht-degree: 0%

---

# Criar e editar regras de negócios

Uma regra de negócios permite aplicar validação a objetos do Workfront e impede que os usuários criem, editem ou excluam um objeto quando determinadas condições forem atendidas. As regras de negócios ajudam a melhorar a qualidade dos dados e a eficiência operacional, evitando ações que podem comprometer a integridade dos dados.

Uma única regra de negócios pode ser atribuída a apenas um objeto. Por exemplo, se você criar uma regra de negócios para não editar projetos sob determinadas condições, não poderá aplicar a mesma regra a tarefas. Seria necessário criar uma regra de negócios separada com as mesmas condições para tarefas.

Os níveis de acesso e o compartilhamento de objetos têm uma prioridade mais alta do que as regras de negócios quando um usuário interage com um objeto. Por exemplo, se um usuário tiver um nível de acesso ou permissão que não permita a edição de um projeto, eles terão precedência sobre uma regra de negócios que permita a edição de um projeto sob determinadas condições.

Quando mais de uma regra de negócios se aplica a um objeto, as regras são todas seguidas, mas não são aplicadas em uma determinada ordem. Por exemplo, você tem duas regras de negócios. Restringe-se a criação de despesas no mês de fevereiro. O segundo impede a edição de um projeto quando o status do projeto é Concluído. Se um usuário tentar adicionar uma despesa a um projeto concluído em junho, a despesa não poderá ser adicionada porque acionou a segunda regra.

As regras de negócios se aplicam à criação, edição e exclusão de objetos por meio da API e da interface do Workfront.

>[!NOTE]
>
>Como as regras de negócios bloqueiam determinadas ações, você sempre deve configurar as regras de negócios primeiro em um ambiente de sandbox ou pré-visualização e testá-las completamente antes de ativá-las na produção.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>plano do Adobe Workfront</td> 
   <td>Ultimate</td> 
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

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Cenários de regras de negócios

O formato de uma regra de negócios é &quot;Se a condição definida for atendida, o usuário será impedido de realizar a ação no objeto e a mensagem será exibida&quot;.

A sintaxe das propriedades e outras funções em uma regra de negócios é igual à sintaxe de um campo calculado em um formulário personalizado. Para obter mais informações sobre a sintaxe, consulte [Adicionar campos calculados com o designer de formulário](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md).

Para obter informações sobre instruções IF, consulte a [ visão geral das instruções &quot;IF&quot;](/help/quicksilver/reports-and-dashboards/reports/calc-cstm-data-reports/if-statements-overview.md) e os [Operadores de condição em campos personalizados calculados](/help/quicksilver/reports-and-dashboards/reports/calc-cstm-data-reports/condition-operators-calculated-custom-expressions.md).

Para obter informações sobre curingas baseados no usuário, consulte [Usar curingas baseados no usuário para generalizar relatórios](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/use-user-based-wildcards-generalize-reports.md).

Para obter informações sobre curingas baseados em data, consulte [Usar curingas baseados em data para generalizar relatórios](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/use-date-based-wildcards-generalize-reports.md).

Um curinga de API também está disponível nas regras de negócios. Você pode usar `$$ISAPI` para acionar a regra somente na interface ou somente na API.

Alguns cenários simples de regras de negócios são:

* Os usuários não podem adicionar novas despesas durante a última semana de fevereiro. Esta fórmula pode ser declarada como: `IF(MONTH($$TODAY) = 2 && DAYOFMONTH($$TODAY) >= 22, "You cannot add new expenses during the last week of February.")`
* Os usuários não podem editar um projeto com o status Concluído. Esta fórmula pode ser declarada como: `IF({status} = "CPL", "You cannot edit this project because it is in Complete status.")`

Um cenário com instruções IF aninhadas é:

Os usuários não podem editar projetos concluídos e não podem editar projetos com uma Data de conclusão planejada para março. Esta fórmula pode ser declarada como:

```
IF(
    {status}="CPL",
    "You cannot edit a completed project",
    IF(
        MONTH({plannedCompletionDate})=3,
        "You cannot edit a project with a planned completion date in March")
)
```

## Adicionar uma nova regra de negócios

{{step-1-to-setup}}

1. Clique em **Regras de Negócios** no painel esquerdo.
1. Clique em **Nova regra de negócio**.
1. Selecione o tipo de objeto ao qual atribuir a regra de negócios e clique em **Continuar**.

   ![Selecione um objeto](assets/object-for-business-rule2.png)

1. Digite o **Nome** da regra de negócios.
1. No campo **Está ativo**, selecione se a regra deve estar ativa ao salvá-lo.

   Se você selecionar **Não**, a regra será salva como inativa e você poderá ativá-la mais tarde.

1. Selecione um **Acionador** para a regra de negócios. As opções são:

   * **Na criação do objeto:** a regra é aplicada quando um usuário tenta criar um objeto.
   * **Na edição do objeto:** a regra é aplicada quando um usuário tenta editar um objeto.
   * **Na exclusão de objeto:** a regra é aplicada quando um usuário tenta excluir um objeto.

1. (Opcional) Insira uma **Descrição** da regra de negócios e o que acontece quando ela é aplicada.
1. Crie a fórmula no editor de fórmulas, no centro da caixa de diálogo de regra de negócios.

   O formato de uma regra de negócios é &quot;Se a condição definida for atendida, o usuário será impedido de realizar a ação no objeto e a mensagem será exibida&quot;.

   Na área da fórmula, as partes da regra de negócios criadas são a condição e a mensagem exibida no Workfront quando a condição é atendida.

   * O &quot;objeto&quot; é o tipo de objeto selecionado ao criar a regra de negócios. Ele é exibido no cabeçalho da caixa de diálogo.
   * A &quot;ação&quot; é o acionador selecionado para a regra: criar, editar ou excluir o objeto.
   * Como o objeto e a ação já estão definidos, você não os inclui na fórmula.
   * A mensagem de erro personalizada é exibida ao usuário quando ele aciona a regra de negócios. Ele deve fornecer instruções claras sobre o que deu errado e como corrigir o problema.

   ![Caixa de diálogo Adicionar regra de negócio](assets/add-business-rule-dialog-no-ai-button.png)

   Este exemplo é uma regra de negócios para despesas. Se o mês atual for junho, os usuários não poderão criar novas despesas e a mensagem explica isso.

   Para obter mais exemplos de regras de negócios, consulte [Cenários para regras de negócios](#scenarios-for-business-rules) neste artigo.

1. (Opcional) Use a fórmula **Expressões** e **Campos** no painel direito para auxiliar na criação da regra.

   Procure por uma expressão ou campo para restringir a lista de itens disponíveis.

   A lista de campos disponíveis é limitada aos campos relacionados ao tipo de objeto da regra de negócios.

1. Clique em **Salvar** quando terminar de criar a regra de negócios.

>[!NOTE]
>
>Após adicionar uma regra de negócios, você deverá testá-la adicionando, editando ou excluindo o objeto associado para garantir que a regra seja aplicada corretamente.

## Ativar uma regra de negócios

Quando uma regra de negócios está inativa, o campo Está Ativo na lista de regras de negócios exibe Falso. Não é possível atualizar o status da regra na exibição em lista.

Para ativar uma regra de negócios:

1. Selecione a regra de negócios na lista de regras e clique no ícone Editar.
1. Selecione **Sim** para **Está ativo** na caixa de diálogo de regra de negócios.
1. Clique em **Salvar**.
