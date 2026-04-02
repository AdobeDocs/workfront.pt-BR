---
content-type: overview
product-area: projects
navigation-topic: financials
title: Definir uma taxa de horas extras
description: Você pode definir um índice de horas extras em uma tarefa para ajustar o cálculo de Receita Planejada para as atribuições da tarefa.
author: Lisa
feature: Work Management
source-git-commit: bf8dcc9dfa9697c8d212072bb511c57aa01e7529
workflow-type: tm+mt
source-wordcount: '348'
ht-degree: 11%

---

# Definir uma taxa de horas extras

{{highlighted-preview-article-level}}

Quando um índice de horas extras é adicionado a uma tarefa, ele é aplicado a todas as atribuições na tarefa. Ele multiplica todas as Horas Planejadas para essa tarefa e afeta os cálculos da Receita Planejada.

A taxa de horas extras não pode variar para atribuições na mesma tarefa. Se forem necessários multiplicadores de horas extras diferentes, você deverá criar subtarefas separadas em uma tarefa pai.

>[!NOTE]
>
>Não há validação que impeça a taxa de horas extras de ser adicionada a uma tarefa que não seja de horas extras.

## Cálculo de horas extras na receita planejada

Primeiro, o sistema determina a taxa de faturamento usando a hierarquia de taxa de faturamento padrão. Para obter mais informações, consulte [Visão geral da hierarquia de receita e custo](/help/quicksilver/manage-work/projects/project-finances/overview-revenue-cost-hierarchy.md).

Se a proporção de horas extras existir na tarefa, o cálculo será:
Receita Planejada = Taxa de Cobrança × Proporção de Horas Extras × Horas Planejadas

Se o índice de horas extras estiver em branco, o cálculo será:
Receita Planejada = Taxa de Faturamento × Horas Planejadas

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Pacote do Adobe Workfront</td> 
   <td>Workflow Ultimate</td> 
  </tr> 
  <tr> 
   <td>Licença do Adobe Workfront</td> 
   <td>Padrão</td> 
  </tr> 
  <tr> 
   <td>Configurações de nível de acesso</td> 
   <td>Editar acesso a Tarefas, Projetos e Dados Financeiros</td> 
  </tr> 
  <tr> 
   <td>Permissões de objeto</td> 
   <td><p>Gerenciar permissões para uma tarefa que inclua Editar taxas de cobrança</p>
     <p>Contribute ou tem permissões mais altas para o projeto</p></td> 
  </tr> 
 </tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Pré-requisitos

O tipo de receita da tarefa deve ser Usuário e Função por hora. Para obter mais informações, consulte [Visão geral da hierarquia de receita e custo](/help/quicksilver/manage-work/projects/project-finances/overview-revenue-cost-hierarchy.md).

O campo **Taxa de Horas Extras** deve ser habilitado no modelo de layout.

1. No modelo de layout, clique na seta para baixo em **Personalizar o que os usuários veem** e clique em **Tarefa**.
1. Na seção **Detalhes**, selecione o campo **Taxa de Horas Extras** na área **Finanças**.

   Para obter mais informações, consulte [Personalizar o modo de exibição de Detalhes usando um modelo de layout](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

## Definir a taxa de horas extras em uma tarefa

1. Vá para a tarefa que deseja editar.

   Para obter mais informações, consulte [Gerenciar finanças da tarefa na seção Detalhes da Tarefa](/help/quicksilver/manage-work/tasks/manage-tasks/task-finances-in-details.md).

1. Clique em **Detalhes da tarefa** no painel esquerdo.
1. Na área **Finanças**, insira o multiplicador de horas extras no campo **Taxa de horas extras**.
1. Clique em **Salvar alterações**.

