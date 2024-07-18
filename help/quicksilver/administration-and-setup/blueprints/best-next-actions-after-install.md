---
user-type: administrator
content-type: reference
product-area: system-administration;workfront-integrations
navigation-topic: best-practices-catalog
title: Ações a serem executadas após a instalação de um blueprint
description: Este artigo descreve o que você deve fazer depois de instalar um blueprint no [!DNL Adobe Workfront]  para implantar totalmente o blueprint nos usuários do sistema.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 6e5da58f-105a-4edf-8fc1-65e8762d43c6
source-git-commit: 1ae65d18419bf4235a7c97614b539811643110cc
workflow-type: tm+mt
source-wordcount: '1138'
ht-degree: 0%

---

# Ações a serem executadas após a instalação de um blueprint

Este artigo descreve o que você deve fazer depois de instalar um blueprint no [!DNL Adobe Workfront] para implantar totalmente o blueprint nos usuários do sistema.

* [Recomendações do modelo de projeto](#project-template-recommendations)
* [Recomendações de estrutura organizacional](#organizational-structure-recommendations)
* [Recomendações do painel](#dashboard-recommendations)

## Recomendações do modelo de projeto {#project-template-recommendations}

Esta seção contém recomendações para os modelos de projeto instalados com seus blueprints.

### Atribuir usuários a funções e equipes recém-criadas {#assign-users-to-newly-created-roles-and-teams}

As funções e/ou equipes criadas durante o processo de instalação do blueprint não têm usuários associados automaticamente a elas. Sem atribuir usuários às funções ou equipes recém-adicionadas, você criará trabalhos para uma função que ninguém atenderá. Em alguns casos, pode ser necessário criar novos usuários para preencher essas funções e equipes. Para obter informações sobre como criar novos usuários, consulte [Adicionar usuários](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

### Aplicar um formulário personalizado ao modelo e às tarefas do modelo {#apply-a-custom-form-to-the-template-and-the-template-tasks}

O processo de instalação não associa o modelo de projeto a nenhum formulário personalizado. Se os projetos ou as tarefas exigirem que formulários ou campos específicos sejam preenchidos para criar a consistência do relatório, ou se o formulário de solicitação digital contiver campos que precisam ser retidos no nível do projeto, recomendamos que você associe o modelo ou as tarefas do modelo a esses formulários. Para obter informações, consulte [Adicionar um formulário personalizado a um objeto](../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

### Atualizar estimativas de esforço e duração da tarefa de modelo {#update-template-task-duration-and-effort-estimates}

Cada tarefa no modelo contém uma duração planejada e uma estimativa de esforço planejada. Essas estimativas servem como ponto de partida para as durações e o tempo gasto com essas atividades. No entanto, os recursos, as habilidades e o ritmo de sua organização são exclusivos. Você deve revisar a duração estimada de cada tarefa e o esforço para ajustá-la para refletir as necessidades da sua organização. Para obter informações, consulte [Gerenciar informações da tarefa na área [!UICONTROL Visão Geral de Detalhes da Tarefa]](../../manage-work/tasks/manage-tasks/task-information-in-overview.md).

### Associar um caminho de etapas e etapas {#associate-a-milestone-path-and-milestones}

O processo de instalação não associa o modelo de projeto a um caminho de etapas. Aplique um caminho de marcos ao modelo e aplique marcos às tarefas principais no modelo para atender às suas necessidades de relatórios de marcos. Para obter informações, consulte [Associar marcos a tarefas](../../manage-work/tasks/manage-tasks/associate-milestones-with-tasks.md).

### Implante o modelo para sua equipe {#roll-out-the-template-to-your-team}

Prepare materiais de treinamento para os gerentes de trabalho que usarão este modelo e para os colaboradores individuais que executarão o trabalho dentro do modelo do projeto.

### Criar ou atualizar relatórios e painéis {#create-or-update-reports-and-dashboards}

Se a solução representar um novo tipo de trabalho que sua organização não realizou anteriormente no [!DNL Workfront], talvez seja necessário criar novos relatórios e painéis para dar suporte ao trabalho. Para obter informações, consulte [Criar um relatório personalizado](../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md) e [Criar um painel](../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md).

Se a solução for semelhante ao trabalho que você já está executando no [!DNL Workfront], verifique se o trabalho é alimentado nos relatórios e painéis existentes, conforme esperado. Se não for alimentado em seus relatórios existentes, tome medidas para atualizar filtros ou criar novos relatórios.

## Recomendações de estrutura organizacional {#organizational-structure-recommendations}

Esta seção contém recomendações para os elementos de estrutura organizacional instalados com seus blueprints.

### Empresas

Depois de instalar um blueprint que inclui uma empresa:

* Adicione um formulário personalizado para aumentar o registro da empresa com detalhes úteis (o formulário e seus detalhes são exclusivos para você). Para obter informações, consulte [Adicionar um formulário personalizado a um objeto](../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).
* Se a empresa representa um cliente, analise as taxas de substituição associadas à empresa. Para obter informações, consulte [Substituir taxas de cobrança de função de trabalho no nível da empresa](../../administration-and-setup/set-up-workfront/organizational-setup/override-job-role-billing-rates-company-level.md).
* Se a empresa representar um cliente e se houver outros modelos de projeto exclusivos para essa organização, primeiro pré-associe os modelos de projeto à empresa recém-adicionada. Para obter informações, consulte [Editar modelos de projeto](../../manage-work/projects/create-and-manage-templates/edit-templates.md).
* Se a empresa representa um cliente ou fornecedor, associe os usuários existentes da organização externa que já podem estar em seu ambiente. Para obter informações, consulte [Criar e editar empresas](../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).
* Se a empresa representa um cliente ou um fornecedor, crie usuários colaboradores adicionais para a organização externa que podem ser necessários em seu ambiente para simplificar a comunicação, a execução do trabalho e as aprovações. Para obter informações sobre como criar novos usuários, consulte [Adicionar usuários](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).
* Atualize os relacionamentos do organograma para qualquer usuário associado à empresa recém-adicionada. Para obter informações, consulte [Criar subordinados diretos](../../administration-and-setup/add-users/create-and-manage-users/create-direct-reports.md) e [Exibir o organograma](../../people-teams-and-groups/work-directly-with-others/view-the-org-chart.md).

Para obter informações adicionais sobre empresas, consulte [Criar e editar empresas](../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

## Recomendações do painel {#dashboard-recommendations}

Esta seção contém recomendações para os painéis e relatórios instalados com um blueprint.

### Atualize os painéis recém-criados para adicionar/remover relatórios

Os painéis adicionados de um blueprint têm um ou mais relatórios, páginas externas ou calendários. É provável que você não precise de todos os relatórios e outros elementos do painel, ou que precise aumentar o painel com relatórios, páginas externas e calendários existentes antes que ele esteja pronto para ser compartilhado com outras pessoas. Para obter informações, consulte [Adicionar um relatório a um painel](/help/quicksilver/reports-and-dashboards/dashboards/creating-and-managing-dashboards/add-report-dashboard.md).

### Atualizar os relatórios recém-criados para adicionar/remover colunas ou critérios de filtro

Os relatórios distribuídos por meio de um blueprint do painel não têm todas as colunas ou critérios de filtro para suportar sua configuração do [!DNL Workfront]. Espera-se que você faça alguns ajustes nos relatórios para que eles se encaixem em seus padrões. Para criar consistência com outros relatórios em seu ambiente, adicione uma coluna incluída em todos os relatórios para o objeto que está sendo listado ou adicione alguns critérios de filtro que limitam os resultados a um tipo de projeto ou grupo de usuários específico. Para obter informações, consulte [Criar ou editar exibições](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-edit-views.md) e [Criar ou editar filtros](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-filters.md).

### Compartilhar os painéis ou relatórios com usuários

Se você não estiver planejando colocar o painel em um modelo de layout, compartilhe o painel com as pessoas que o considerarão útil. Para obter informações, consulte [Compartilhar um painel](/help/quicksilver/reports-and-dashboards/dashboards/creating-and-managing-dashboards/share-dashboard.md) e [Compartilhar um relatório](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/share-report.md).

### Adicionar os painéis aos modelos de layout

A melhor maneira de disponibilizar informações para outras pessoas é adicionar painéis a modelos de layout. Identifique os modelos de layout das pessoas que se beneficiariam mais de revisar o painel regularmente e adicione o painel recém-criado a esses modelos de layout. Para obter informações, consulte [Criar e gerenciar modelos de layout](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

### Atualizar outros painéis e relatórios

A introdução de um novo painel e seus relatórios pode possibilitar a desativação e o ajuste de outros painéis e relatórios existentes. Reserve tempo para revisar seus relatórios existentes e identificar relatórios redundantes e contraditórios.

### Distribuir dados personalizados a formulários relevantes

Alguns relatórios incluídos em um blueprint de painel têm campos de dados personalizados na exibição, no filtro ou no agrupamento do relatório. Em alguns casos, o blueprint também terá um formulário ao qual esses campos estão associados. No entanto, na maioria das vezes, os campos personalizados não são aplicados a um formulário personalizado. Para que as colunas, filtros ou agrupamentos funcionem corretamente, esses campos devem ser associados a formulários que estejam conectados a um registro de usuário, projeto, tarefa ou outro objeto. Para obter informações, consulte [Criar um formulário com o designer de formulário](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).
