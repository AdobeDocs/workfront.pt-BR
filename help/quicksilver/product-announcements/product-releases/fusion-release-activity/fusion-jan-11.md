---
product-previous: workfront-fusion
content-type: release-notes
product-area: workfront-integrations
navigation-topic: fusion-release-activity
title: "Atividade de lançamento do Workfront Fusion: semana de 11 de janeiro de 2021"
description: Esta página descreve todas as melhorias feitas no Adobe Workfront Fusion na semana de 11 de janeiro de 2021.
author: Luke
feature: Product Announcements, Workfront Fusion
recommendations: noDisplay, noCatalog
exl-id: 2439e2a7-9404-433a-bd71-a7776042d8a0
hidefromtoc: true
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '703'
ht-degree: 0%

---

# Atividade de lançamento do Workfront Fusion: semana de 11 de janeiro de 2021

Esta página descreve todas as melhorias feitas no Adobe Workfront Fusion na semana de 11 de janeiro de 2021.

Para obter uma lista de todas as alterações recentes, consulte [atividade de versão do Adobe Workfront Fusion](../../../product-announcements/product-releases/fusion-release-activity/fusion-release-activity.md).

Para obter uma lista de correções de erros recentes no Workfront Fusion, consulte a página [Atualizações de Manutenção do Workfront](https://experienceleague.adobe.com/docs/workfront-known-issues/releases/current-updates.html) e verifique se há atualizações rotuladas como Atualização de Manutenção do Workfront Fusion.

## Ampliar conector e módulos agora disponíveis

Agora você pode usar o Workfront Fusion para se conectar à sua conta do Widen. Com os módulos Ampliar, você pode:

* Adicionar ou remover ativos de uma coleção
* Baixar ou carregar arquivos
* Ler ou atualizar metadados de ativos
* Pesquisar ativos com base nos critérios especificados
* Recuperar uma lista de ativos em uma coleção
* Execute uma chamada de API personalizada.

Para obter mais informações, consulte [Ampliar módulos](../../../workfront-fusion/apps-and-their-modules/widen-modules.md).

## Conector e módulos do Datadog agora disponíveis

Agora você pode usar o Workfront Fusion para se conectar à sua conta do Datadog.

Com os módulos Datadog, é possível:

* Pontos da série temporal Post
* Executar uma chamada de API personalizada

Para obter informações sobre módulos Datadog, consulte [módulos Datadog](../../../workfront-fusion/apps-and-their-modules/datadog-modules.md).

## Conector de evento e módulos agora disponíveis

Agora você pode usar o Workfront Fusion 2.0 para se conectar à sua conta Cvent.

Com os módulos de Evento, você pode:

* Criar uma solicitação de reunião
* Ler registros como contatos, eventos ou convites
* Listar registros com base nos critérios que você especificar
* Registrar ou adicionar convidados a eventos específicos
* Atualizar ou excluir contatos
* Fazer uma chamada de API personalizada

Para obter informações sobre módulos Cvent disponíveis, consulte [Módulos Cvent](../../../workfront-fusion/apps-and-their-modules/cvent-modules.md).

## Conector e módulos do Microsoft Dynamics 365 agora disponíveis

Agora você pode usar o Workfront Fusion 2.0 para se conectar à sua conta do Microsoft Dynamics 365. Com os módulos do Microsoft Dynamics 365, é possível:

* Acione um cenário quando os registros forem adicionados ou atualizados no Microsoft Dynamics 365
* Criar, ler, atualizar ou excluir um registro do Microsoft Dynamics 365
* Executar uma chamada de API personalizada

Para obter informações sobre módulos do Microsoft Dynamics 365 disponíveis, consulte [módulos do Microsoft Dynamics 365](../../../workfront-fusion/apps-and-their-modules/microsoft-dynamics-365-modules.md).

## Conector e módulos do DocuSign agora disponíveis

Agora você pode usar o Workfront Fusion 2.0 para se conectar à sua conta do Docusign. Com os módulos de Documentação, você pode:

* Acionar um cenário quando um envelope alterar seu status
* Criar um envelope
* Ler, enviar ou adicionar um destinatário a um envelope existente
* Adicionar ou modificar campos personalizados em documentos
* Baixar um documento como um campo
* Carregar um arquivo em um envelope
* Executar uma chamada de API personalizada

Para obter mais informações, consulte [módulos do DocuSign](../../../workfront-fusion/apps-and-their-modules/docusign-modules.md).

## Pesquisar o histórico de execução do cenário

Facilitamos a localização de informações específicas de execuções de cenários anteriores. A nova pesquisa de texto completo do Fusion permite pesquisar o histórico de execução de quaisquer dados contidos em um pacote. Por exemplo, para identificar qual execução criou uma tarefa específica, você pode usar a pesquisa de texto completo para procurar essa ID de tarefa.

Anteriormente, a localização de informações de execução específicas exigia a visualização de cada execução individualmente.

Para obter mais informações, consulte [Exibir o histórico de execução de um cenário no Adobe Workfront Fusion](../../../workfront-fusion/scenarios/view-scenario-execution-history.md).

## Atualizações do Armazenamento de Dados Fusion 2.0

Para facilitar a personalização dos armazenamentos de dados, adicionamos algumas novas funcionalidades. Agora, ao visualizar um armazenamento de dados, você pode:

* Arraste e solte para reordenar as colunas
* Editar uma única célula
* Adicionar várias linhas

Para obter mais informações sobre Repositórios de Dados, consulte [Módulos de repositório de dados](../../../workfront-fusion/apps-and-their-modules/data-store-modules.md).

## Fazer uma solicitação de autorização de Chave de API por meio do conector HTTP

Para aumentar a flexibilidade das maneiras de acessar APIs, adicionamos um novo módulo ao conector HTTP. Agora, você pode usar o conector HTTP para fazer uma solicitação quando o serviço Web que você está acessando exigir o uso de uma chave de API.

Para obter mais informações, consulte [Módulos HTTP](../../../workfront-fusion/apps-and-their-modules/http-modules/http-modules-1.md).

## Novas funções disponíveis no painel de mapeamento

Para ajudar você a personalizar e simplificar fórmulas em seus módulos, adicionamos algumas novas funções.

* O

  ```
  omit
  ```

  é uma função geral que omite as chaves fornecidas do objeto e retorna o restante.
* O

  ```
  pick
  ```

  é uma função geral que escolhe somente as chaves fornecidas do objeto.
* O

  ```
  escapeMarkdown
  ```

  é uma função de sequência de caracteres que escapa todas as tags do Markdown em um texto.

Para obter mais informações sobre as funções omitir e escolher, consulte [Funções gerais no Adobe Workfront Fusion](../../../workfront-fusion/functions/general-functions.md).

Para obter mais informações sobre a função escapeMarkdown, consulte [Funções de string no Adobe Workfront Fusion](../../../workfront-fusion/functions/string-functions.md).
