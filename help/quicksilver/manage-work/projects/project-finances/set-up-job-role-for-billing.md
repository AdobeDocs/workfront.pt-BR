---
content-type: overview
product-area: projects
navigation-topic: financials
title: Configurar uma função de trabalho para faturamento
description: O Workfront permite cobrar de um usuário uma função de trabalho diferente da função de trabalho principal. Isso é útil quando uma pessoa executa temporariamente um trabalho que deve ser faturado a uma taxa diferente.
author: Lisa
feature: Work Management
source-git-commit: d92908d358ca53ae9d443fd76556e3e8b273e3cb
workflow-type: tm+mt
source-wordcount: '680'
ht-degree: 5%

---

# Configurar uma função de trabalho para faturamento

{{highlighted-preview-article-level}}

O Workfront permite cobrar de um usuário uma função de trabalho diferente da função de trabalho principal. Isso é útil quando uma pessoa executa temporariamente um trabalho que deve ser faturado a uma taxa diferente.

Você pode atribuir uma Função de trabalho para faturamento de duas maneiras:

* No nível do projeto: use esta opção quando a pessoa precisar ser cobrada na mesma função de trabalho para todo o projeto.
* No nível de atribuição: Use esta opção quando quiser faturar de forma diferente em tarefas específicas.

>[!NOTE]
>
>* Uma Função de trabalho para faturamento se aplica somente a pessoas (usuários). Isso não se aplica a funções de trabalho genéricas ou espaços reservados.
>* Adicionar uma função de trabalho para faturamento afeta somente a taxa de faturamento, não o custo.
>* O faturamento no nível da atribuição sempre tem prioridade sobre o faturamento no nível do projeto.

Para obter mais informações, consulte [Visão geral da hierarquia de receita e custo](/help/quicksilver/manage-work/projects/project-finances/overview-revenue-cost-hierarchy.md) e [Criar atribuições avançadas](/help/quicksilver/manage-work/tasks/assign-tasks/create-advanced-assignments.md).

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
   <td> Editar acesso a cartões de taxa</td> 
  </tr> 
  <tr> 
   <td>Permissões de objeto</td> 
   <td>Gerenciar permissões do projeto </td> 
  </tr> 
 </tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Atribuir uma função de trabalho para faturamento no nível do projeto

Quando você cria uma função de trabalho para faturamento em um projeto:

* A função de faturamento se aplica a todas as tarefas e atribuições do projeto para esse usuário.
* O faturamento usa a taxa de faturamento da função de trabalho selecionada, mas o custo ainda segue a função principal do usuário.

Para atribuir uma função de cargo para faturamento no nível do projeto:

1. Abra um projeto.
1. Clique em **Recurso para Faturamento** no painel esquerdo.
1. Selecione a guia **Função de trabalho para faturamento** se ela ainda não estiver sendo exibida.
1. Clique em **Adicionar > Adicionar função de trabalho para cobrança**.
1. Na caixa **Adicionar função de trabalho para cobrança**, selecione o **Usuário**.
1. Selecione a **Função de trabalho** a ser usada como a função de trabalho para cobrança para este usuário neste projeto.
1. (Opcional) Clique em **Adicionar função de trabalho** para definir datas de efetivação para a função de trabalho para cobrança. Insira as datas de **Início** e **Término** para a função de trabalho.

[Adicionar função de trabalho para faturamento no nível do projeto](assets/jrfb-project-level.png)

1. Clique em **Adicionar função de trabalho** novamente para especificar funções de cobrança adicionais para diferentes períodos.
1. Clique em **Salvar**.

### Exemplo no nível do projeto

>[!BEGINSHADEBOX]

A principal função de trabalho de John é a Designer 1. O projeto requer um Designer sênior, e John está preenchendo.

Você definiria a Função de trabalho de Faturamento como **Designer Sênior** no nível do projeto.

Resultado:

* A receita de faturamento é a taxa do Designer sênior
* O custo é a taxa de custo do Designer 1 (taxa de custo real de John)

>[!ENDSHADEBOX]

## Atribuir uma Função de Trabalho para Faturamento no nível de atribuição

Quando você adiciona uma função de trabalho para faturamento em uma atribuição, a configuração substitui uma função de faturamento no nível do projeto somente para essa atribuição específica.

Para atribuir uma função de cargo para faturamento no nível de atribuição:

1. Abra um projeto e localize a tarefa.
1. Vá para as **Atribuições Avançadas** da tarefa.

   Para obter informações, consulte [Criar atribuições avançadas](/help/quicksilver/manage-work/tasks/assign-tasks/create-advanced-assignments.md).

1. Na grade de atribuição de tarefas, localize a coluna **Função de trabalho para cobrança**.
1. Selecione uma função de trabalho para cada atribuição na qual você deseja um faturamento diferente.

   >[!NOTE]
   >
   >Se uma função de trabalho para faturamento foi atribuída no nível do projeto, ela aparece na atribuição. Você pode clicar no campo **Função de trabalho para faturamento** e selecionar outra função de trabalho para usar na atribuição.
   >O ícone de informações notifica se uma função de trabalho para faturamento foi definida no nível do projeto ou da atribuição.

   ![Função de trabalho para cobrança em uma atribuição](assets/jrfb-assignment-level.png)

### Exemplo no nível de atribuição

>[!BEGINSHADEBOX]

A principal função de trabalho de John é a Designer 1. Ele é cobrado como um Designer sênior no nível do projeto, mas há uma tarefa especial que requer uma taxa de cobrança do Designer principal.

Você definiria a Função de trabalho de faturamento como Designer principal somente nessa atribuição.

Resultado:

* Todas as outras tarefas de John são faturadas como Designer sênior
* Esta tarefa é listada como Designer Principal
* O custo permanece com o Designer 1

>[!ENDSHADEBOX]
