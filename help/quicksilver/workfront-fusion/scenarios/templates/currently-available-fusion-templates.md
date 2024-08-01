---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Modelos do Adobe Workfront Fusion disponíveis no momento
description: Os seguintes modelos públicos estão disponíveis no Adobe Workfront Fusion.
author: Becky
feature: Workfront Fusion
exl-id: 29d95b93-ab54-416d-b0d5-ff12634951b2
source-git-commit: 3c22860b1a9bdc653a772a48ccfcbb4456b11c8c
workflow-type: tm+mt
source-wordcount: '1257'
ht-degree: 0%

---

# Modelos do Adobe Workfront Fusion disponíveis no momento

Os seguintes modelos públicos estão disponíveis no Adobe Workfront Fusion.

Sua equipe ou organização pode ter outros modelos criados por equipe disponíveis.

Para exibir os modelos disponíveis, clique no ícone ![](assets/fusion-template-icon.png) de **Modelos** no menu de navegação lateral no Fusion.

## Modelos do Workfront

Esses modelos automatizam processos e fluxos de trabalho do Workfront.

### [!BADGE Novo!]{type=Informative}

Este Modelo do Fusion cria uma lista de verificação padrão para todos os cartões que informam uma coluna específica em um determinado quadro de acordo com o tempo.

### [!BADGE Novo!]{type=Informative}

<!--new Aug 1. 2024-->

Este cenário é acionado por um novo projeto que está sendo criado. Com esse cenário, é possível criar um quadro com o nome do projeto, renomear ou criar colunas com base nas suas necessidades, criar tags personalizadas e associar um filtro de coluna de entrada ao projeto de origem.  Milhares de alterações adicionais podem ser feitas, mas a partir daqui você verá as possibilidades de criar um ponto de partida para a padronização do conselho da sua organização.

### Workfront - Criação de projeto a partir do CSV

Essa automação cria novos projetos no Workfront com base no nome, Portfolio, status, data de início planejada e detalhes do modelo especificados em um CSV.

### Workfront - Solicitações de limpeza sem novas observações nos últimos 30 dias

Use esse modelo para impor uma atualização de nota de 30 dias às suas solicitações. As solicitações não atualizadas em 30 dias recebem o status alterado e fechado em 60 dias.

### Workfront - Alterar status do projeto para Concluído em 100% concluído.

Essa automação atualiza os projetos para o status Concluído que têm todas as tarefas em 1005 concluídas. Projetos com problemas em aberto ou tarefas em aberto ou aprovações de projetos receberão uma atualização e, quando resolvidos, os projetos serão movidos para o status Concluído.

### Workfront - Avisar e tentar fechar projetos obsoletos

Use este cenário para ajudar a automatizar o aviso e o encerramento de projetos que atendem à política de projetos obsoletos da organização.

### Workfront - Copiar novas observações e respostas do problema/solicitação de origem para um projeto ou tarefa já convertida

Use este modelo para copiar observações e respostas de um problema ou solicitação para um projeto ou tarefa já convertida.

### Workfront - Copiar Forms e dados de campo personalizados do programa para novos projetos associados

Essa automação observa novos projetos em programas com formulários personalizados. Em seguida, adiciona esses formulários e campos personalizados do programa aos novos projetos.

### Workfront - Copiar dados de campo e Forms personalizados do Portfolio para novos projetos associados

Essa automação observa novos projetos em portfólios com formulários personalizados. Em seguida, ele adiciona esses formulários e campos personalizados do portfólio aos novos projetos.

### Workfront - Converter problema aprovado em projeto

Este modelo converte problemas em projetos. Você pode modificá-la para atender aos padrões de sua organização.

### Workfront - Copiar documentos de problemas/solicitações para projetos ou tarefas já convertidos

Esse cenário flexível copia documentos de problemas ou solicitações para projetos ou tarefas convertidos anteriormente.

### Notificação personalizada com base na alteração do campo

Esse modelo cria atualizações personalizadas (e notificações relacionadas) para indivíduos que trabalham em um projeto do Workfront, com base em algum evento exclusivo, como uma alteração em um valor de campo. O cenário observa o Workfront quando um campo especificado é alterado em uma Tarefa ou Problema. Quando encontrado, o cenário avaliará as informações no projeto relacionado e criará uma atualização personalizada para uma pessoa atribuída a uma função específica no projeto.

### Workfront - Anexação em massa ao nome do projeto com convenção

Esse modelo de atualização em massa renomeia todos os projetos que atendem aos critérios de uma pesquisa (estão em um portfólio) e os renomeia com um formato padrão.

### Workfront - Renomear projetos com convenção

Esse modelo localiza todos os projetos que atendem aos critérios de um filtro (se enquadram em um portfólio) e os renomeia com um formato padrão.

### Workfront - Criar Linha de Base na Alteração de Status

Este modelo captura uma linha de base do projeto após qualquer alteração de status do projeto observada nos módulos de &quot;alternância&quot; e cria uma atualização no fluxo de atualização para registro em log.

### Workfront - Criação semanal da linha de base

Este modelo captura uma linha de base do projeto todas as segundas-feiras às 6h00 ET em projetos filtrados por portfólio e cria uma atualização no fluxo de atualização para registro em log.

### Localizar modelos de projeto não usados no tempo da política e notificar

Uma vez por mês, revise os modelos de projeto usando sua própria política com esse modelo fácil de gerenciar que notifica os usuários apropriados sobre os modelos em violação de sua política.

## Workfront - Modelos do Workfront Proof

Esses modelos automatizam fluxos de trabalho que combinam o Workfront com o Workfront Proof.

### Workfront Proof > Workfront - atualização do projeto na decisão da prova

Quando uma decisão é tomada em uma Prova que é adicionada diretamente a um projeto, essa automação reúne informações sobre a Decisão da prova, como quem tomou a decisão, e reflete esse progresso no projeto do Workfront correspondente como uma atualização.

### Workfront Proof > Workfront - atualização e conclusão da tarefa (se aprovada) na decisão da prova

Quando provas individuais estão vinculadas a tarefas individuais, esse cenário fecha a tarefa associada quando uma decisão de aprovação na prova é tomada. Se aprovada, ela conclui a tarefa e atualiza o projeto.

## HTTP - Modelos do Workfront

Esses modelos recuperam informações de um serviço Web e trazem essas informações para a Workfront.

>[!NOTE]
>
> Você deve ter uma licença do Workfront Fusion for Work Automation and Integration para usar modelos nesta seção.

### Estabelecendo conexão usando JWT (JSON Web Token)

Estabeleça Autorização JWT para uma API do cliente.

### APILayer > Workfront - Atualização da Taxa de Câmbio Diária (EUR)

Esse modelo cria um cenário que automatiza a atualização de uma taxa de câmbio em um ponto definido no tempo. Este cenário extrai a taxa de euros (EUR) para dólares (USD) de uma API APIlayers.com e atualiza a taxa no Workfront.

## Modelos Workfront-Marketo

Esses modelos oferecem suporte à integração Workfront-Marketo.

>[!NOTE]
>
> Você deve ter uma licença do Workfront Fusion for Work Automation and Integration para usar modelos nesta seção.

### Aprovar o rascunho de email do Marketo Engage com os fluxos de trabalho de aprovação do Workfront

Isso faz parte da integração Revisar e aprovar entre o Workfront e o Marketo Engage. Esse modelo detecta se uma Prova de email no Workfront foi aprovada e atualiza o email correspondente no Marketo Engage como aprovado.

### Receber solicitações de campanha de marketing no Workfront e automatizar a criação de campanhas no Marketo Engage

Esse cenário fornece uma maneira programática de criar campanhas de email e webinário no Marketo Engage a partir de uma solicitação feita no Workfront. Usando a automação para criar, organizar e configurar campanhas, as equipes podem melhorar a eficiência.

### Revise uma prova de email do seu rascunho de email do Marketo Engage no Workfront

Esse modelo detecta se uma tarefa do Workfront foi definida como um status pronto para revisão e, em seguida, exporta o rascunho de email do Marketo Engage para salvá-lo como uma Prova no Workfront.

## Modelos Workfront-SharePoint

Esses modelos conectam o Workfront e o SharePoint.

>[!NOTE]
>
> Você deve ter uma licença do Workfront Fusion for Work Automation and Integration para usar modelos nesta seção.

### Observar alterações na pasta do SharePoint

Esse modelo permite ver se há uma alteração em uma pasta do SharePoint.


## Modelos Workfront-Anaplan

Esses modelos suportam a integração Workfront-Anaplan e esperam uma configuração específica em Anaplan no Workfront. Para obter informações sobre esses modelos e as configurações necessárias, consulte os artigos para os modelos individuais.

Para obter mais informações sobre a integração Workfront-Anaplan, consulte [Adobe Workfront com Anaplan](../../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/anaplan-integration.md).

>[!NOTE]
>
> Você deve ter uma licença do Workfront Fusion for Work Automation and Integration para usar modelos nesta seção.

### Workflows de otimização de gastos

* [Enviar  [!DNL Adobe Workfront] atualizações de projeto para um item de lista  [!DNL Anaplan] ](../../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-actual-hours-updates-to-anaplan-list-item.md)
* [Enviar  [!DNL Adobe Workfront] despesas para um [!DNL Anaplan] item de lista](../../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-expenses-to-anaplan-list-item.md)
* [Enviar  [!DNL Adobe Workfront] atualizações de horas reais para um item de lista  [!DNL Anaplan] ](../../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-actual-hours-updates-to-anaplan-list-item.md)

### Fluxos de trabalho para vincular solicitações de orçamento

* [Criar um item de lista  [!DNL Anaplan]  a partir de uma solicitação de orçamento  [!DNL Adobe Workfront] ](../../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-budget-request.md)
* [Aplicar uma alocação de orçamento  [!DNL Anaplan]  a um projeto  [!DNL Adobe Workfront] ](../../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-projects.md)

### Fluxos de trabalho para vincular solicitações de campanha

* [Criar um item de lista  [!DNL Anaplan]  a partir de uma solicitação de campanha  [!DNL Adobe Workfront] ](../../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-campaign-request.md)
* [Aplicar uma  [!DNL Anaplan] alocação de orçamento a uma [!DNL Adobe Workfront] solicitação de campanha ou projeto de campanha](../../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-campaign-requests-and-projects.md)


<!--[!BADGE New!]{type=Informative} -->