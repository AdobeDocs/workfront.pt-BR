---
content-type: release-notes
navigation-topic: product-releases-archive
title: Final do Beta 2017.2
description: Esta página descreve todas as alterações disponíveis mais recentemente no ambiente de Pré-visualização com a versão 2017.2. A funcionalidade nesta página foi disponibilizada no ambiente de Pré-visualização em 28 de junho de 2017. Ele estará disponível no ambiente de Produção em 26 de julho de 2017.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 768e9aad-d7e7-4a3c-9f93-926cf588ddc7
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '2314'
ht-degree: 0%

---

# Final do Beta 2017.2

Esta página descreve todas as alterações disponíveis mais recentemente no ambiente de Pré-visualização com a versão 2017.2. A funcionalidade nesta página foi disponibilizada no ambiente de Pré-visualização em 28 de junho de 2017. Ele estará disponível no ambiente de Produção em 26 de julho de 2017.

>[!IMPORTANT]
>
>A funcionalidade descrita nesta página está sujeita a alterações antes da disponibilidade no ambiente de produção.

Para obter uma lista de todas as alterações feitas em 2017.2, consulte a [visão geral da atividade da versão 2017.2](../../../../product-announcements/product-releases/quarterly-release-archive/2017.2-release-activity/2017-2-release-activity-overview.md).

A versão final do Beta 2017.2 contém melhorias para administradores do Workfront e outros usuários:

**Para Administradores:**

* [Determine a disponibilidade do visualizador da prova de vídeo do HTML5 (ProofHQ e Workfront)](#determine-the-availability-of-the-html5-video-proofing-viewer-proofhq-and-workfront)
* [Suporte a certificados SHA-256 para SAML 2.0](#support-sha-256-certificates-for-saml-2-0)
* [Digite-Adiante para Mapear Atributos](#type-ahead-for-mapping-attributes)
* [Aprimoramento da API: acessar alocações de usuários](#api-enhancement-access-user-allocations)

**Para Todos Os Usuários:**

* [Planejador de recursos](#resource-planner)
* [Nova Área de Agendamento em um Projeto (Team Builder)](#new-scheduling-area-in-a-project-team-builder)
* [Agendamento de Recursos: Mostrar Menos Itens por Padrão](#resource-scheduling-show-fewer-items-by-default)
* [Agendamento de Recursos: Exibir Indicador de Descarte e Superalocação ao Arrastar Tarefas e Problemas](#resource-scheduling-display-drop-indicator-and-over-allocation-when-dragging-tasks-and-issues)
* [Agendamento De Recursos: As Alocações De Usuários Não São Mais Arredondadas Para A Próxima Meia-Hora](#resource-scheduling-user-allocations-are-no-longer-rounded-to-the-nearest-half-hour)
* [Exportar o Relatório de Utilização em Formatos TSV e PDF](#export-the-utilization-report-in-tsv-and-pdf-formats)
* [Final do Beta 2017.2](#user-calendar-enhancements-in-the-my-work-area%22)
* [Final do Beta 2017.2](#layout-template-determines-whether-the-new-or-legacy-calendar-displays-in-the-my-work-area)
* [A decisão de prova é exibida em Minha área de trabalho (Workfront)](#proof-decision-displays-in-the-my-work-area-workfront)
* [Exibir Provas de Mídia Avançada em Resoluções Predefinidas (ProofHQ e Workfront)](#view-rich-media-proofs-in-preset-resolutions-proofhq-and-workfront)
* [Exibir URL para subpáginas em comentários sobre provas de mídia avançada (ProofHQ e Workfront)](#view-url-to-sub-pages-in-comments-on-rich-media-proofs-proofhq-and-workfront)
* [Criar Modos de Exibição Personalizados com Base em Modos de Exibição Padrão Existentes (ProofHQ)](#create-custom-views-based-on-existing-standard-views-proofhq)
* [Filtrar a Área de Relatório (ProofHQ)](#filter-the-reporting-area-proofhq)
* [Exibir Valores Mínimos e Máximos em Relatórios (ProofHQ)](#display-minimum-and-maximum-values-in-reports-proofhq)
* [Notificação no aplicativo para Aprovação de Prova](#in-app-notification-for-proof-approval)
* [Melhorias em dispositivos móveis](#mobile-improvements)
* [Barra Adicionada às Instruções de Filtro para Valores de Campo que Contêm Vírgulas](#slash-added-to-filter-statements-for-field-values-that-contain-commas)
* [Várias Taxas de Cobrança](#multiple-billing-rates)
* [Novo Campo de Horas Orçadas de Recurso](#new-resource-budgeted-hour-field)
* [Mostrar Função de Trabalho do Usuário na Área &#39;Atribuído a&#39; na Página de Detalhes para Tarefas e Problemas](#show-user-job-role-in-assigned-to-area-on-the-details-page-for-tasks-and-issues)

>[!NOTE]
>
>As ferramentas de Agendamento de recursos foram substituídas e removidas do Workfront com a versão 23.1. Para obter informações sobre o agendamento de recursos usando o Balanceador de carga de trabalho, consulte [Visão geral do Balanceador de carga de trabalho](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

## Nova Área de Agendamento em um Projeto (Team Builder) {#new-scheduling-area-in-a-project-team-builder}

A área de Cronograma em um projeto (anteriormente conhecida como Team Builder) foi reprojetada com uma interface de usuário atualizada e mais intuitiva. A nova funcionalidade de Agendamento agora se aproxima mais da funcionalidade de Agendamento de recursos atualmente disponível em outras áreas do Workfront.

As melhorias incluem:

* Exibir alocações de recursos atuais para membros da equipe do projeto, permitindo que você tome decisões mais informadas ao fazer atribuições
* Representação visual das durações da tarefa na linha do tempo de agendamento
* Filtrar as informações exibidas na linha do tempo de agendamento
* Adicione e remova facilmente usuários da equipe do projeto, diretamente da linha do tempo de agendamento

A seguinte funcionalidade está disponível em outras áreas da ferramenta ao agendar recursos, mas não está disponível ao agendar recursos na área Agendamento de equipe:

* Configurar tarefas pai para exibir na linha do tempo de agendamento
* Configurar os nomes dos projetos a serem exibidos na linha de tempo do cronograma
* Modificar atribuições de usuário usando a ferramenta Trocar
* Filtrar por portfólio, programas e projetos

Para obter mais informações sobre a funcionalidade disponível na área Agendamento de equipe, consulte &quot;Introdução ao Agendamento de recursos&quot;.

## Agendamento de recursos: mostrar menos itens por padrão {#resource-scheduling-show-fewer-items-by-default}

Por padrão, um máximo de 10 itens de trabalho por dia agora são exibidos na linha do tempo de agendamento para um determinado usuário. É possível expandir a lista para visualizar todas as tarefas e problemas atualmente atribuídos a esse usuário.

Isso permite que você navegue mais facilmente pela linha do tempo de agendamento quando forem atribuídas muitas tarefas e problemas aos usuários.

Antes dessa alteração, todas as tarefas e problemas eram sempre exibidas para todos os usuários.

Para obter mais informações sobre atribuição de tarefas e problemas a usuários na linha do tempo do agendamento, consulte &quot;Atribuir manualmente tarefas e problemas não atribuídos nas áreas de Agendamento&quot;.

## Agendamento de Recursos: Exibir Indicador de Soltar e Alocação em Excesso ao Arrastar Tarefas e Problemas {#resource-scheduling-display-drop-indicator-and-over-allocation-when-dragging-tasks-and-issues}

Ao atribuir uma tarefa ou problema a um usuário na linha do tempo de agendamento por meio do arrastar e soltar, as seguintes informações agora são exibidas antes de liberar a tarefa ou problema e concluir a atribuição:

* Um indicador de liberação é exibido na linha do usuário. Isso permite que você veja onde um item está sendo atribuído antes de fazer a atribuição.
* Se as alocações de usuário estiverem ativadas na linha do tempo de programação, os indicadores vermelhos de superalocação serão exibidos se a conclusão da atribuição resultar no excesso de alocação do usuário.

Antes dessas alterações, nenhuma informação era exibida antes do lançamento da tarefa ou problema.

Para obter mais informações sobre atribuição de tarefas e problemas a usuários na linha do tempo do agendamento, consulte &quot;Atribuir manualmente tarefas e problemas não atribuídos nas áreas de Agendamento&quot;.

## Agendamento de Recursos: as alocações de usuários não são mais arredondadas para a meia hora mais próxima {#resource-scheduling-user-allocations-are-no-longer-rounded-to-the-nearest-half-hour}

Quando vários usuários são atribuídos a uma tarefa ou problema, ou quando uma tarefa ou problema abrange vários dias, o Workfront tenta distribuir as horas planejadas de maneira uniforme entre os usuários e dias atribuídos. Por padrão, as horas são arredondadas para a centena mais próxima (por exemplo, 1,33).

Anteriormente, ao modificar manualmente as horas distribuídas, as horas eram ajustadas e arredondadas para a meia hora mais próxima (por exemplo, 1,33 era arredondado para 1,5).

Agora, as horas não são mais ajustadas e arredondadas para a meia hora mais próxima (por exemplo, 1,33 permanece como 1,33).

## Aprimoramento da API: acessar alocações de usuários {#api-enhancement-access-user-allocations}

Agora você pode acessar o sombreamento de alocação de usuários por meio da API do Workfront.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">For more information, see <a href="../../../../wf-api/api/access-proj-allocation-info-api.md" class="MCXref xref" xrefformat="{para}">Access Project Allocation Information via the API</a>.</p>
-->

## Exportar o relatório de utilização em formatos TSV e PDF {#export-the-utilization-report-in-tsv-and-pdf-formats}

Agora é possível exportar o relatório de Utilização de um projeto nos formatos TSV e PDF, além do formato XLSX.

Antes dessa alteração, você poderia exportar o relatório de Utilização somente no formato XLSX.

Para obter mais informações sobre como exportar o relatório de Utilização, consulte [Visão Geral do Relatório de Utilização de Recursos](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md) em [Visão Geral do Relatório de Utilização de Recursos](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md).

## A decisão da prova é exibida na área Meu trabalho (Workfront) {#proof-decision-displays-in-the-my-work-area-workfront}

Agora, ao exibir aprovações de provas na guia Minhas aprovações na área Meu trabalho, a decisão de prova é exibida na área Meu trabalho e permanece até você clicar no novo botão Atualizar no Workfront ou até a próxima vez que atualizar a página do navegador.

Antes dessa alteração, não havia nenhuma indicação de que uma decisão já tinha sido tomada na prova, e a prova permaneceu na guia Minhas aprovações até que você atualizasse o navegador.

Para obter mais informações, consulte [Aprovando trabalho](../../../../review-and-approve-work/manage-approvals/approving-work.md) em [Aprovando trabalho](../../../../review-and-approve-work/manage-approvals/approving-work.md).

## Exibir provas de mídia avançada em resoluções predefinidas (ProofHQ e Workfront) {#view-rich-media-proofs-in-preset-resolutions-proofhq-and-workfront}

Em uma versão anterior do ambiente de Pré-visualização, introduzimos a capacidade de ajustar a resolução de provas de Rich Media especificando uma resolução personalizada ou arrastando a imagem para a resolução desejada.

Agora é possível selecionar entre as opções de resolução predefinidas de vários telefones, tablets, notebooks e desktops.

Para obter mais informações, consulte &quot;Exibindo uma Resolução Predefinida&quot; em [Alterar resolução de prova interativa no visualizador de provas](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/view-interactive-content-as-it-appears-in-device.md).

## Visualizar URL para subpáginas em comentários sobre provas de mídia avançada (ProofHQ e Workfront) {#view-url-to-sub-pages-in-comments-on-rich-media-proofs-proofhq-and-workfront}

>[!NOTE]
>
>No momento, esse recurso está disponível no ambiente de Produção.

Agora, ao comentar em uma subpágina em uma prova de Mídia avançada, o URL para a subpágina é exibido no comentário.

Antes dessa alteração, não estava claro a qual subpágina o comentário se referia.

Para obter mais informações, consulte

## Determine a disponibilidade do visualizador da prova de vídeo do HTML5 (ProofHQ e Workfront) {#determine-the-availability-of-the-html5-video-proofing-viewer-proofhq-and-workfront}

Como administrador do Workfront no ProofHQ, você pode determinar se os usuários em sua organização têm acesso ao novo visualizador do ProofHQ HTML5 para provas em vídeo.

Para obter mais informações sobre como configurar essa opção no Workfront, consulte em .

## Criar exibições personalizadas com base em exibições padrão existentes (ProofHQ) {#create-custom-views-based-on-existing-standard-views-proofhq}

Agora é possível criar uma visualização personalizada com base em uma visualização padrão. As opções Colunas, Classificação e Filtros da exibição padrão são incluídas na nova exibição por padrão.

Antes dessa alteração, para criar uma exibição personalizada, era necessário criar a exibição do zero. 

Para obter mais informações, consulte [Criação de um Modo de Exibição Personalizado](../../../../workfront-proof/wp-work-proofsfiles/manage-your-work/create-and-manage-custom-views.md#creating) em [Criar e Gerenciar Modos de Exibição Personalizados no Workfront Proof Proof](../../../../workfront-proof/wp-work-proofsfiles/manage-your-work/create-and-manage-custom-views.md).

## Filtrar a área de relatórios (ProofHQ) {#filter-the-reporting-area-proofhq}

Por padrão, os dados exibidos na guia Relatórios incluem todas as informações do sistema ProofHQ. Agora você pode usar filtros para mostrar apenas as informações relevantes às suas necessidades. 

Para obter mais informações, consulte [Filtrar relatórios](../../../../workfront-proof/wp-work-proofsfiles/manage-your-work/run-reports.md#filtering-reports) em  [Executar Relatórios no Workfront Proof](../../../../workfront-proof/wp-work-proofsfiles/manage-your-work/run-reports.md).

## Exibir valores mínimo e máximo em relatórios (ProofHQ) {#display-minimum-and-maximum-values-in-reports-proofhq}

Agora é possível configurar se os valores mínimo e máximo serão exibidos no gráfico ao exibir relatórios.

Para obter mais informações, consulte [Exibindo Relatórios](../../../../workfront-proof/wp-work-proofsfiles/manage-your-work/run-reports.md#viewing-reports) em  [Executar Relatórios no Workfront Proof](../../../../workfront-proof/wp-work-proofsfiles/manage-your-work/run-reports.md).

## Suporte a certificados SHA-256 para SAML 2.0 {#support-sha-256-certificates-for-saml-2-0}

Agora oferecemos suporte ao Secure Hash Algorithm 256 (SHA-256) ao configurar o Workfront para SSO com SAML 2.0. Antes desta versão, oferecíamos suporte somente ao Algoritmo de hash seguro 1 (SHA-1).

Para obter mais informações sobre como configurar o Workfront com SAML 2.0, consulte [Configurar o Adobe Workfront com SAML 2.0](../../../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md)

## Digite com antecedência para mapear atributos {#type-ahead-for-mapping-attributes}

O tipo de campo Valor padrão na caixa de diálogo Mapeamento de atributos foi atualizado para um campo de digitação antecipada. Antes dessa alteração, o tipo de campo Default Value era uma lista suspensa.

Essa alteração se aplica aos seguintes protocolos SSO:

* Active Directory
* LDAP
* SAML 2.0

O SAML 1.1 não oferece suporte ao mapeamento de atributos.

## Melhorias na mobilidade {#mobile-improvements}

>[!NOTE]
>
> O aplicativo móvel é lançado independentemente do aplicativo Workfront principal. A funcionalidade descrita nesta seção é lançada no início de agosto.

Você verá a seguinte funcionalidade adicionada nos aplicativos móveis, para as plataformas do Android e do iOS:

* Enviar solicitações do aplicativo móvel
* Nova entrada de folha de horas no aplicativo móvel
* Edição de formulário personalizado no aplicativo móvel
* Solicitações de aprovação de prova no aplicativo móvel

Haverá um programa beta público para alguns desses recursos para a plataforma Android.

Para obter mais informações sobre o próximo programa beta para dispositivos móveis, consulte a  Página [&quot;Betas&quot;](https://support.workfront.com/hc/en-us/sections/115000743248).

Para obter mais informações sobre como usar o aplicativo móvel do Workfront, consulte .  

## Barra adicionada às Instruções de filtro para valores de campo que contêm vírgulas {#slash-added-to-filter-statements-for-field-values-that-contain-commas}

Ao criar um filtro no modo de texto e filtrar valores de campo que contenham vírgulas, você deve adicionar uma barra (&quot;/&quot;) antes das vírgulas que separam os valores, para garantir que o valor seja lido como uma opção de filtro. Isso se aplica somente aos seguintes tipos de campo:

* Menus suspensos
* Botões de seleção
* Caixa de Seleção

Antes dessa alteração, não era possível filtrar por campos que tinham opções que continham vírgulas.

Para obter mais informações sobre esta alteração, consulte [Visão geral dos Filtros](../../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

## Várias taxas de cobrança {#multiple-billing-rates}

Agora é possível adicionar várias sobreposições de taxa de faturamento para a mesma função de trabalho no nível do projeto. Com essa nova funcionalidade, é possível definir intervalos de datas para cada substituição de taxa de faturamento. Durante o período especificado, uma taxa de cobrança diferente é aplicada à função de trabalho atribuída às tarefas em um projeto. As taxas de cobrança são multiplicadas por horas no projeto para calcular a receita. A receita calculada dentro do intervalo de datas de uma taxa de cobrança permanece bloqueada nessa taxa e não é atualizada conforme as taxas das funções de trabalho na atualização do projeto. No caso da Receita Efetiva, nenhuma hora registrada antes de substituir a taxa de cobrança será recalculada para refletir a taxa de cobrança atual. As horas registradas antes da substituição da taxa de cobrança ter sido adicionada ao projeto serão associadas à taxa de cobrança da função de trabalho nesse momento.

Antes dessa alteração, você poderia substituir a taxa de cobrança de uma função de trabalho apenas uma vez, e a Receita Efetiva seria recalculada para refletir a taxa de cobrança atual para todas as horas registradas antes da taxa de cobrança ser alterada.

Para obter mais informações sobre Taxas de Cobrança e Receita, consulte [Visão Geral de Faturamento e Receita](../../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

Para obter mais informações sobre substituição de taxas de cobrança para funções de trabalho no nível do projeto, consulte [Visão geral da substituição de Taxas de cobrança de função de trabalho e cálculo de Receita em um projeto](../../../../manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).

## Planejador de recursos {#resource-planner}

Com esta versão, estamos introduzindo a primeira fase do Planejador de recursos, que faz parte do redesign da nova guia Planejamento na área Pessoas. Ao usar o Planejador de recursos, você pode estimar a quantidade de horas que os usuários em seus Conjuntos de recursos estão alocados em todos os projetos atuais para os quais você é o Gerente de recursos. Você pode ver os seguintes números de alocação por projeto, função de trabalho e por usuário no Planejador de recursos:

* Horas Disponíveis
* Horas planejadas
* Horas orçadas
* Variação de Hora (entre as Horas Orçadas e Planejadas)
* Diferença de Hora Líquida (entre as Horas Disponível e Orçada)

Para obter mais informações sobre como usar o Planejador de recursos, consulte [Visão geral do Planejador de recursos](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

## Novo campo de horas orçadas de recurso {#new-resource-budgeted-hour-field}

Para oferecer suporte à nova funcionalidade do Planning e ao Planejador de Recursos, um novo campo foi adicionado ao Report Builder, que permite relatar as Horas orçadas do recurso. Este campo captura a quantidade de horas para as quais um recurso é orçado em um projeto. Este campo não está disponível ao estimar recursos usando a funcionalidade Planejamento de Recursos Legados.

Para obter mais informações sobre como usar as Horas orçadas no Planejador de recursos, consulte [Visão geral do Planejador de recursos](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

## Notificação no aplicativo para aprovação de prova {#in-app-notification-for-proof-approval}

Quando você é designado como aprovador de uma prova, recebe uma notificação no aplicativo sobre a aprovação da prova aguardando sua decisão. A notificação exibe o seguinte texto: `<User name>` deseja que você aprove esta prova&quot;. Se as informações do usuário não estiverem disponíveis, a notificação será alterada para &quot;Esta prova exige sua aprovação&quot;.

Antes dessa melhoria, a única indicação visual de que você foi designado como aprovador em uma prova era uma nova solicitação de prova na área Meu trabalho.

Para obter mais informações sobre notificações no aplicativo, consulte [Exibir e gerenciar notificações no aplicativo](../../../../workfront-basics/using-notifications/view-and-manage-in-app-notifications.md).

## Mostrar Função de Trabalho do Usuário na Área &#39;Atribuído a&#39; na Página de Detalhes para Tarefas e Problemas {#show-user-job-role-in-assigned-to-area-on-the-details-page-for-tasks-and-issues}

Agora, ao exibir a página de detalhes de uma tarefa ou problema, uma função de trabalho é exibida abaixo do nome do destinatário na área Atribuído a. Esta função de trabalho representa a função de trabalho do usuário que corresponde à atribuição de função de trabalho da tarefa ou problema. Se a tarefa ou problema não for atribuído a uma função de trabalho, a função de trabalho principal do usuário atribuído será exibida.

Antes dessa alteração, somente o título do usuário era exibido abaixo do nome do usuário na área Atribuído a. 
