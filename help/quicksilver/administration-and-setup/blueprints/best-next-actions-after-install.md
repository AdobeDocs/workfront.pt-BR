---
user-type: administrator
content-type: reference
product-area: system-administration;workfront-integrations
navigation-topic: best-practices-catalog
title: Ações a serem tomadas após a instalação de um blueprint
description: Este artigo descreve o que você deve fazer após instalar um blueprint no [!DNL Adobe Workfront] para implantar totalmente o blueprint nos usuários do sistema.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 6e5da58f-105a-4edf-8fc1-65e8762d43c6
source-git-commit: d46eb98c443a421f340b1021972ddb89eda1966b
workflow-type: tm+mt
source-wordcount: '1139'
ht-degree: 0%

---

# Ações a serem tomadas após a instalação de um blueprint

Este artigo descreve o que você deve fazer após instalar um blueprint no [!DNL Adobe Workfront] para implantar totalmente o blueprint nos usuários do sistema.

* [Recomendações do modelo de projeto](#project-template-recommendations)
* [Recomendações sobre a estrutura organizacional](#organizational-structure-recommendations)
* [Recomendações do painel](#dashboard-recommendations)

## Recomendações do modelo de projeto {#project-template-recommendations}

Esta seção contém recomendações para os modelos de projeto instalados com seus blueprints.

### Atribuir usuários a funções e equipes recém-criadas {#assign-users-to-newly-created-roles-and-teams}

As funções e/ou equipes criadas durante o processo de instalação do blueprint não têm usuários associados a elas automaticamente. Sem atribuir usuários às funções ou equipes recém-adicionadas, você criará trabalho para uma função que ninguém selecionará. Em alguns casos, pode ser necessário criar novos usuários para preencher essas funções e equipes. Para obter informações sobre como criar novos usuários, consulte [Adicionar usuários](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

### Aplicar um formulário personalizado ao modelo e às tarefas do modelo {#apply-a-custom-form-to-the-template-and-the-template-tasks}

O processo de instalação não associa o modelo do projeto a nenhum formulário personalizado. Se os projetos ou as tarefas exigirem que formulários ou campos específicos sejam preenchidos para criar consistência de relatórios, ou se o formulário de solicitação digital contiver campos que precisam ser retidos no nível do projeto, recomendamos que você associe o modelo ou as tarefas do modelo a esses formulários. Para obter mais informações, consulte [Adicionar um formulário personalizado a um objeto](../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

### Atualizar a duração da tarefa do modelo e estimativas de esforço {#update-template-task-duration-and-effort-estimates}

Cada tarefa no template contém uma duração planejada e uma estimativa de esforço planejada. Essas estimativas servem como ponto de partida para durações e tempo gasto para essas atividades. No entanto, os recursos, as habilidades e o espaço de sua organização são únicos. Você deve revisar a duração estimada de cada tarefa e o esforço para ajustá-la de modo a refletir as necessidades da organização. Para obter mais informações, consulte [Gerencie informações da tarefa na [!UICONTROL Visão geral dos detalhes da tarefa] area](../../manage-work/tasks/manage-tasks/task-information-in-overview.md).

### Associar um caminho de marco e marcos {#associate-a-milestone-path-and-milestones}

O processo de instalação não associa o modelo do projeto a um caminho de marco. Aplique um caminho de marco ao modelo e aplique marcos às tarefas principais no modelo para dar suporte às suas necessidades de relatórios de marco. Para obter mais informações, consulte [Associar marcos a tarefas](../../manage-work/tasks/manage-tasks/associate-milestones-with-tasks.md).

### Implementar o modelo para sua equipe {#roll-out-the-template-to-your-team}

Prepare materiais de treinamento para os gerentes de trabalho que usarão esse modelo e os contribuidores individuais que executarão o trabalho dentro do modelo do projeto.

### Criar ou atualizar relatórios e painéis {#create-or-update-reports-and-dashboards}

Se a solução representar um novo tipo de trabalho que sua organização não executou anteriormente em [!DNL Workfront], talvez seja necessário criar novos relatórios e painéis para dar suporte ao trabalho. Para obter mais informações, consulte [Criar um relatório personalizado](../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md) e [Criar um painel](../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md).

Se a solução for semelhante ao trabalho que você já executou no [!DNL Workfront], verifique se o trabalho é alimentado em relatórios e painéis existentes, conforme esperado. Se ele não for alimentado em seus relatórios existentes, execute uma ação para atualizar os filtros ou criar novos relatórios.

## Recomendações sobre a estrutura organizacional {#organizational-structure-recommendations}

Esta seção contém recomendações para os elementos da estrutura organizacional instalados com seus blueprints.

### Empresas

Depois de instalar um blueprint que inclui uma empresa:

* Adicione um formulário personalizado para aumentar o registro da empresa com detalhes úteis (o formulário e seus detalhes são exclusivos de você). Para obter mais informações, consulte [Adicionar um formulário personalizado a um objeto](../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).
* Se a empresa representa um cliente, analise as taxas de substituição associadas à empresa. Para obter mais informações, consulte [Substituir as taxas de faturamento da função de trabalho no nível da empresa](../../administration-and-setup/set-up-workfront/organizational-setup/override-job-role-billing-rates-company-level.md).
* Se a empresa representar um cliente e se houver outros modelos de projeto exclusivos para essa organização, primeiro pré-associe os modelos de projeto à empresa recém-adicionada. Para obter mais informações, consulte [Editar modelos de projeto](../../manage-work/projects/create-and-manage-templates/edit-templates.md).
* Se a empresa representar um cliente ou fornecedor, associe usuários existentes da organização externa que já podem estar em seu ambiente. Para obter mais informações, consulte [Criar e editar empresas](../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).
* Se a empresa representa um cliente ou fornecedor, crie usuários colaboradores adicionais para a organização externa que podem ser necessários em seu ambiente para simplificar a comunicação, a execução do trabalho e as aprovações. Para obter informações sobre como criar novos usuários, consulte [Adicionar usuários](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).
* Atualize as relações do organograma para qualquer usuário associado à empresa recém adicionada. Para obter mais informações, consulte [Criar relatórios diretos](../../administration-and-setup/add-users/create-and-manage-users/create-direct-reports.md) e [Exibir o gráfico organizacional](../../people-teams-and-groups/work-directly-with-others/view-the-org-chart.md).

Para obter informações adicionais sobre empresas, consulte [Criar e editar empresas](../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

## Recomendações do painel {#dashboard-recommendations}

Esta seção contém recomendações para os painéis e relatórios instalados com um blueprint.

### Atualizar os painéis recém-criados para adicionar/remover relatórios

Os painéis adicionados de um blueprint têm um ou mais relatórios, páginas externas ou calendários. É provável que você não precise de todos os relatórios e outros elementos do painel ou precisará aumentar o painel com relatórios, páginas externas e calendários existentes antes que ele esteja pronto para compartilhar com outras pessoas. Para obter mais informações, consulte [Adicionar um relatório a um painel](/help/quicksilver/reports-and-dashboards/dashboards/creating-and-managing-dashboards/add-report-dashboard.md).

### Atualizar os relatórios recém-criados para adicionar/remover colunas ou critérios de filtro

Os relatórios distribuídos por meio de um blueprint do painel não têm todas as colunas ou critérios de filtro para suportar sua configuração de [!DNL Workfront]. Espera-se que você faça alguns ajustes nos relatórios para se adequar aos seus padrões. Para criar consistência com outros relatórios em seu ambiente, convém adicionar uma coluna que inclua em todos os relatórios do objeto que está sendo listado ou adicionar alguns critérios de filtro que limitem os resultados a um tipo de projeto ou grupo de usuários específico. Para obter mais informações, consulte [Criar ou editar visualizações](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-edit-views.md) e [Criar ou editar filtros](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-filters.md).

### Compartilhar painéis ou relatórios com usuários

Se não estiver planejando colocar o painel em um modelo de layout, você deve compartilhá-lo com as pessoas que o consideram útil. Para obter mais informações, consulte [Compartilhar um painel](/help/quicksilver/reports-and-dashboards/dashboards/creating-and-managing-dashboards/share-dashboard.md) e [Compartilhar um relatório](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/share-report.md).

### Adicionar painéis aos modelos de layout

A melhor maneira de disponibilizar informações para outras pessoas é adicionar painéis a modelos de layout. Identifique os modelos de layout das pessoas que se beneficiariam mais com a revisão regular do painel e adicione o painel recém-criado a esses modelos de layout. Para obter mais informações, consulte [Criar e gerenciar modelos de layout](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

### Atualizar outros painéis e relatórios

A introdução de um novo painel e seus relatórios pode permitir a desativação e o ajuste de outros painéis e relatórios existentes. Reserve tempo para revisar seus relatórios existentes e identificar quaisquer relatórios redundantes e contraditórios.

### Distribuir dados personalizados para formulários relevantes

Alguns relatórios incluídos em um blueprint do painel têm campos de dados personalizados na exibição, no filtro ou no agrupamento do relatório. Em alguns casos, o blueprint também terá um formulário ao qual esses campos estão associados. No entanto, com mais frequência do que não, os campos personalizados não são aplicados a um formulário personalizado. Para que as colunas, filtros ou agrupamentos funcionem corretamente, esses campos devem ser associados a formulários conectados a um usuário, projeto, tarefa ou outro registro de objeto. Para obter mais informações, consulte [Adicionar um campo personalizado a um formulário personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md).
