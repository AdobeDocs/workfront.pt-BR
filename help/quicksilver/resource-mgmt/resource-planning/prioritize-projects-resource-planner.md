---
product-area: resource-management;projects
navigation-topic: resource-planning
title: Priorizar projetos no Planejador de recursos
description: Os projetos são listados em ordem de prioridade no Planejador de recursos, com o projeto mais importante na parte superior.
author: Lisa
feature: Resource Management
exl-id: fe9c8cf9-f1e0-4cd5-9299-0f04893d71a5
source-git-commit: 8cd6c47acf8de313bab5fe7298125eb63cc10faf
workflow-type: tm+mt
source-wordcount: '1282'
ht-degree: 1%

---

# Priorizar projetos no Planejador de recursos

Os projetos são listados em ordem de prioridade no Planejador de recursos, com o projeto mais importante na parte superior.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Pacote do Adobe Workfront</td> 
   <td><p>Qualquer</p></td>
  </tr> 
  <tr> 
   <td>Licença do Adobe Workfront</td> 
   <td><p>Standard</p>
       <p>Plano</p></td> 
  </tr> 
  <tr> 
   <td>Configurações de nível de acesso</td> 
   <td> <p>Editar acesso ao Gerenciamento de recursos que inclui acesso a Editar prioridades e horas de orçamento no Planejador de recursos</p> <p>Editar acesso a Dados Financeiros, Projetos e Usuários</p></td> 
  </tr> 
  <tr> 
   <td>Permissões de objeto</td> 
   <td> <p>Gerenciar permissões para os projetos para os quais você deseja orçar informações com a capacidade de Gerenciar Finanças</p></td>
  </tr> 
 </tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Ordem padrão dos projetos no Planejador de recursos

Por padrão, os projetos são listados na Visualização de projeto do Planejador de recursos considerando os critérios abaixo.

>[!IMPORTANT]
>
>Os projetos são listados de acordo com os três critérios abaixo somente na primeira vez que você abrir o Planejador de recursos. No entanto, essa prioridade padrão torna-se automaticamente sua prioridade personalizada e não pode ser revertida para a prioridade original sempre que você executar um dos seguintes procedimentos:
>
>* Ao clicar em Salvar a qualquer momento.
>* Ao alterar manualmente a prioridade de planejamento do projeto. Para obter informações sobre como alterar a prioridade de planejamento do projeto manualmente, consulte a seção [Alterar manualmente a Prioridade de Planejamento do Projeto](#manually-change-the-project-planning-priority) neste artigo.
>
>Depois que a prioridade do projeto se tornar sua prioridade personalizada, qualquer alteração nas informações do projeto não afetará mais a ordem dos projetos usando esses critérios. Depois disso, somente será possível priorizar os projetos manualmente.

Os critérios padrão originais para listar os projetos na Visualização de projeto são os seguintes, nesta ordem:

1. Pela pontuação de alinhamento no projeto.\
   Para obter mais informações sobre a Pontuação de Alinhamento do projeto, consulte [Aplicar um scorecard a um projeto e gerar uma Pontuação de Alinhamento](../../manage-work/projects/define-a-business-case/apply-scorecard-to-project-to-generate-alignment-score.md).

1. Pela Data de início planejada do projeto (se o campo Alinhamento for nulo ou igual para vários projetos).
1. Em ordem alfabética (se o campo Alinhamento for nulo ou for o mesmo e a data de início planejada for a mesma para vários projetos).

Leve em consideração o seguinte ao trabalhar com as prioridades de projeto no Planejador de recursos:

* Você pode personalizar manualmente a prioridade do projeto somente ao aplicar a Visualização do projeto. Isso também altera a ordem dos projetos no Planejador de recursos.
* Quando você aplica a função ou as visualizações de usuário no Planejador de recursos, os projetos aparecem na mesma ordem de prioridade estabelecida na visualização do projeto.
* A ordem dos projetos no Planejador de recursos é exclusiva para você. Outros usuários podem exibir os mesmos projetos no Planejador de recursos, mas em uma ordem diferente. Não é possível criar relatórios no campo Prioridade de Planejamento do Projeto. Isso é visível somente no Planejador de recursos e serve como um sinalizador para priorizar seus projetos.

Projetos associados a um portfólio podem ter uma prioridade no nível do portfólio. Você pode habilitar a exibição da prioridade do portfólio de um projeto no Planejador de recursos, além da prioridade do Planejador de recursos. Você também pode ordenar os projetos de acordo com a prioridade do portfólio.

## Alterar manualmente a prioridade de planejamento do projeto {#manually-change-the-project-planning-priority}

Você deve ter acesso para Editar ao Gerenciamento de recursos e Gerenciar permissões para projetos, para reordenar projetos no Planejador de recursos.

Ao atribuir uma nova prioridade aos projetos, você pode classificá-los em ordem de importância.

Para editar a Prioridade de Planejamento do Projeto:

1. Vá para o **Planejador de recursos**.

1. Clique dentro do campo à esquerda do nome do projeto que contém um número, insira um número para alterar a Prioridade de Planejamento e pressione Enter.\
   ![Alterar Prioridade de Planejamento](assets/mceclip4.png)\
   Ou\
   Passe o mouse sobre o nome do projeto, clique no indicador à esquerda do nome do projeto, arraste-o e solte-o no ponto correto para alterar a prioridade.

   ![arrastar_e_soltar_projetos_RP_1_.png](assets/drag-and-drop-projects-rp--1--350x184.png)

   Ao selecionar números para priorizar projetos, selecione números mais baixos para prioridades mais altas (mais importantes) e números mais altos para prioridades mais baixas (menos importantes). Quando você altera o número de prioridade de um projeto para um número menor (prioridade mais alta), todos os outros projetos no Planejador de recursos são deslocados para baixo na lista (tornam-se menos importantes).\
   Quando você altera o número de prioridade de um projeto para um número mais alto (prioridade mais baixa), todos os outros projetos no Planejador de recursos são deslocados para cima na lista (tornam-se mais importantes).

1. Clique em **Salvar**.\
   A ordem dos projetos muda de acordo com suas seleções e essa se torna a sua prioridade de projeto personalizada no Planejador de recursos. Outros usuários não podem ver sua ordem de prioridade para os projetos no Planejador de recursos, embora possam ver os mesmos projetos em seus Planejadores de recursos.

## Encomendar projetos de acordo com as prioridades da Portfolio no Planejador de recursos

>[!IMPORTANT]
>
>Sua empresa deve ter um pacote do Prime ou superior Workfront para priorizar projetos no Portfolio Otimizer.
>
>Para obter mais informações sobre pacotes Workfront, consulte [pacotes e preços do Adobe Workfront](https://business.adobe.com/products/workfront/pricing.html).
>
>Para obter informações sobre a priorização de projetos no Portfolio Otimizer, consulte [Priorizar projetos no Portfolio Otimizer](../../manage-work/portfolios/portfolio-optimizer/prioritize-projects-in-portfolio-optimizer.md).

1. Abra o **Planejador de Recursos** na **Exibição do Projeto**.
1. Clique no ícone **Configurações**.
1. Habilite a configuração **Exibir Prioridades do Portfolio** para exibir as prioridades do projeto de acordo com a Portfolio à qual estão atribuídas. A prioridade dos projetos de acordo com seus portfólios é exibida ao lado da prioridade Planejador de recursos. Essa configuração é desativada por padrão.

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: check screen shot to see if this is accurate still - should say Order, and not Sort:)</p>
   -->

   ![Prioridade do Portfolio](assets/rp-portfolio-priority-unordered-edit-350x180.png)

   As prioridades de portfólio dos projetos são exibidas somente na visualização Projeto do Planejador de recursos.

1. Clique em **Ordenar** para ordenar os projetos de acordo com as prioridades do portfólio.

   Se você tiver projetos que pertencem a mais de um portfólio, poderá ver vários projetos com a mesma prioridade de portfólio no Planejador de recursos. Nesse caso, os projetos com a mesma prioridade de portfólio são listados pelos seguintes critérios, nesta ordem:

   1. Pontuação do Alinhamento
   1. Data de início planejado
   1. Nome do Projeto

   ![Prioridade do Portfolio solicitada](assets/rp-portfolio-priority-ordered-350x198.png)

1. Clique em **Salvar**.

## O efeito da alteração da Prioridade de Planejamento do Projeto nas Horas Disponíveis do Usuário

A Prioridade de Planejamento do Projeto afeta as Horas Disponíveis dos usuários. Os usuários associados ao projeto com a maior prioridade mostram sua disponibilidade máxima para a coluna Horas Disponíveis (AVL) para este projeto, de acordo com seus cronogramas.

Os mesmos usuários associados ao segundo projeto em ordem de prioridade mostrarão um valor de Horas Disponíveis que é a diferença entre seu valor total de Horas Disponíveis e o que já foi orçado para o primeiro projeto na coluna Horas Orçadas, e assim por diante. Para obter informações sobre recursos de orçamento no Planejador de recursos, consulte [Recursos de orçamento no Planejador de recursos usando as exibições de Projeto e Função](../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md).

Se nenhuma hora tiver sido orçada para o primeiro projeto (em ordem de prioridade) para um usuário, mas horas tiverem sido orçadas para o segundo projeto para o mesmo usuário, o usuário mostrará o valor total de horas disponíveis para ambos os projetos.

Recomendamos a atualização da coluna Horas orçadas para seus usuários na ordem dos projetos no Planejador de recursos, para garantir que você possa visualizar com precisão as Horas disponíveis para o usuário o tempo todo.

>[!NOTE]
>
>Como a Prioridade de planejamento do projeto é exclusiva a cada gerente de recursos, o projeto de segunda prioridade pode ser um projeto de primeira prioridade para outro usuário que visualiza os mesmos projetos no Planejador de recursos. Se outro gerente de recursos orçar um recurso para seu primeiro projeto, as Horas Disponíveis diminuirão para esse recurso para seu primeiro projeto com base nessa alteração.
>
>O usuário que faz o orçamento das horas primeiro aloca esse recurso e reduz o número de Horas Disponíveis para esse recurso no sistema. A quantidade de Horas disponíveis deve ser atualizada para todos os usuários assim que as Horas orçadas forem salvas para um recurso no Planejador de recursos.
>
>Para obter mais informações sobre Horas Disponíveis, consulte [Disponibilidade e alocação de recursos](../../resource-mgmt/resource-planning/resource-availability-allocation-resource-planner.md#availability-and-allocation-of-resources).
