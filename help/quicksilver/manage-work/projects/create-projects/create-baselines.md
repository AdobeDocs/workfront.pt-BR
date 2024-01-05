---
product-area: projects
navigation-topic: create-projects
title: Criar linhas de base do projeto
description: Uma linha de base é um instantâneo de projeto que representa as informações principais incluídas no plano de projeto inicial ou em um determinado momento durante a vida útil do projeto.
author: Alina
feature: Work Management
exl-id: 422bd7a5-d7a0-4c24-8624-bd0fe6e79d7b
source-git-commit: bec625b70b39fec9f9a6d4f7b48023702de43675
workflow-type: tm+mt
source-wordcount: '759'
ht-degree: 0%

---

# Criar linhas de base do projeto

<!-- Audited: 12/2023 -->

Uma linha de base é um instantâneo de projeto que representa as informações principais incluídas no plano de projeto inicial ou em um determinado momento durante a vida útil do projeto.

Você pode usar a linha de base para comparar essas informações do plano atual com o plano original ou qualquer outro ponto no tempo, para identificar tarefas problemáticas, escopo, rastejamento e outras tendências ao longo do tempo.

## Requisitos de acesso

<!--
drafted for P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Standard </p> 
   Or
   <p>Legacy license: Plan </p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level*</td> 
   <td> <p>Edit access to Projects</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information about access to projects, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md" class="MCXref xref">Grant access to projects</a>. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View permissions to the project or higher to view baselines</p> <p>Manage permissions to the project to create baselines</p> <p> For information about project permissions, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Share a project in Adobe Workfront</a>.</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
    <td><p>Novo: Padrão</p>
        <p>ou</p>
        <p>Atual: Plano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Nível de acesso</td> 
   <td> <p>Editar acesso a projetos</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Exibir permissões para o projeto ou superior para exibir linhas de base</p> <p>Gerenciar permissões do projeto para criar linhas de base</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Considerações para trabalhar com linhas de base

* Você pode capturar um instantâneo do progresso de um projeto várias vezes durante a vida útil do projeto, criando várias linhas de base.
* Você pode visualizar as informações incluídas nas linhas de base de um projeto criando uma linha de base ou criando um relatório de Linha de Base.
* Quando você cria uma linha de base, as informações sobre a tarefa também são capturadas nas tarefas dessa linha de base.
* Você pode exibir as informações das tarefas de linha de base criando um relatório de Tarefa de Linha de Base.

>[!IMPORTANT]
>
>Uma linha de base captura um instantâneo do nome, das datas e das informações financeiras do projeto. A linha de base não inclui os valores de campos personalizados no projeto. Para obter informações sobre informações financeiras incluídas na baseline, consulte [Finanças do projeto incluídas nas linhas de base do projeto](../../../manage-work/projects/project-finances/project-finances-included-in-project-baselines.md).

## Criar uma linha de base

Você pode criar uma linha de base das seguintes maneiras:

* **Automaticamente**: O administrador do Workfront ou um administrador de grupo define a preferência do projeto para o Workfront criar automaticamente uma linha de base quando um projeto se tornar Atual. Quando esta configuração está habilitada, uma linha de base é criada quando o status do projeto se torna Atual. Quando esta configuração não está habilitada, você deve criar linhas de base manualmente.

  Para obter mais informações sobre como configurar as preferências do projeto e configurar a criação automática de linha de base, consulte [Configurar preferências de projeto em todo o sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

  >[!CAUTION]
  >
  >Ativar essa configuração cria automaticamente uma linha de base para um projeto sempre que o status de um projeto muda para Atual. A primeira linha de base criada é a padrão. Você deve criar manualmente todas as outras linhas de base durante a vida do projeto.

* **Manualmente**: Você pode criar novas linhas de base para o projeto, conforme necessário, à medida que o projeto avança. Você pode comparar linhas de base para ver como o projeto progrediu com o tempo.

Para criar uma linha de base:

1. Navegue até um projeto.
1. No painel esquerdo, clique em **Linhas de Base**.

   Ou

   Clique em **Mostrar mais** e, em seguida, clique em **Linhas de Base**.

   ![Seção Linhas de Base no projeto](assets/baselines-section-on-project-with-header.png)

1. Clique em **Nova Linha de Base.**
1. Especifique o nome da linha de base.
1. (Opcional) Se esta for a primeira linha de base, talvez você queira escolhê-la como padrão.
1. Clique em **Salvar**.

   Por default, as seguintes informações são exibidas sobre a linha de base que você criou:

   * Nome da linha de base
   * Data de Entrada da Linha de Base
   * Data de Início Planejada do projeto quando a linha de base foi criada
   * Data de Início Projetada do projeto quando a linha de base foi criada
   * Duração real do projeto quando a linha de base foi criada
   * % Concluída do projeto quando a linha de base foi criada
   * Indicador de Linha de Base Padrão que mostra se uma linha de base é a linha de base Padrão do projeto

     >[!TIP]
     >
     >Não é possível exibir informações de duas linhas de base ao mesmo tempo na mesma exibição ou relatório. Você só pode exibir informações de uma determinada linha de base e da Linha de base Padrão no mesmo relatório. Você pode modificar qual linha de base considera ser a Linha de base Padrão a qualquer momento durante a vida útil do projeto.

1. (Opcional) Clique no link **Exibir** e, em seguida, crie uma nova view ou edite a view atual para adicionar campos à view e comparar informações adicionais entre linhas de base. Para obter informações, consulte [Criar ou editar exibições no Adobe Workfront](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-edit-views.md).

## Criar um relatório de Linha de Base ou de Tarefa de Linha de Base

Para exibir informações sobre linha de base, você também pode criar um relatório de Linha de Base ou de Tarefa de Linha de Base. Isso permite que você exiba qualquer número de campos sobre as linhas de base ou tarefas de linha de base para compará-los em uma exibição.

>[!TIP]
>
>Você deve criar uma linha de base antes de criar um relatório de Linha de Base ou de Tarefa de Linha de Base.

Para obter informações sobre como criar um relatório, consulte [Criar um relatório personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

Recomendamos que você adicione um agrupamento Nome do projeto ao seu relatório de Tarefa de linha de base ou linha de base para facilitar a leitura.

Para obter informações sobre como criar um agrupamento, consulte [Criar agrupamentos no Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/create-groupings.md).
