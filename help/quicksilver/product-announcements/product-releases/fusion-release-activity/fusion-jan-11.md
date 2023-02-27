---
product-previous: workfront-fusion
content-type: release-notes
product-area: workfront-integrations
navigation-topic: fusion-release-activity
title: "Atividade da versão do Workfront Fusion: Semana de 11 de janeiro de 2021"
description: Esta página descreve todas as melhorias feitas no Adobe Workfront Fusion na semana de 11 de janeiro de 2021.
author: Luke
feature: Product Announcements, Workfront Fusion
exl-id: 2439e2a7-9404-433a-bd71-a7776042d8a0
hidefromtoc: true
source-git-commit: e6995cd57c4210725d49379df5bcd7e93ce4b02a
workflow-type: tm+mt
source-wordcount: '697'
ht-degree: 0%

---

# Atividade de lançamento do Workfront Fusion: semana de 11 de janeiro de 2021

Esta página descreve todas as melhorias feitas no Adobe Workfront Fusion na semana de 11 de janeiro de 2021.

Para obter uma lista de todas as alterações recentes, consulte [Atividade de versão do Adobe Workfront Fusion](../../../product-announcements/product-releases/fusion-release-activity/fusion-release-activity.md).

Para obter uma lista de correções de erros recentes no Workfront Fusion, consulte o [Atualizações de manutenção do Workfront](https://experienceleague.adobe.com/docs/workfront-known-issues/releases/current-updates.html) e verifique se há atualizações rotuladas como Atualização de manutenção do Workfront Fusion.

## Conector e módulos de largura disponíveis

Agora você pode usar o Workfront Fusion para se conectar à sua conta do Widen. Com os módulos de Largura, é possível:

* Adicionar ativos a ou remover ativos de uma coleção
* Baixar ou carregar arquivos
* Ler ou atualizar metadados de ativos
* Pesquisar ativos com base nos critérios que você especificar
* Recuperar uma lista de ativos em uma coleção
* Execute uma chamada de API personalizada.

Para obter mais informações, consulte [Módulos de largura](../../../workfront-fusion/apps-and-their-modules/widen-modules.md).

## O conector e os módulos de registro de dados já estão disponíveis

Agora você pode usar o Workfront Fusion para se conectar à sua conta de Datadog.

Com os módulos de diálogo, é possível:

* Pontos da pós-série
* Executar uma chamada de API personalizada

Para obter informações sobre módulos de diálogo de dados, consulte [Módulos de registro de dados](../../../workfront-fusion/apps-and-their-modules/datadog-modules.md).

## Conector de evento e módulos agora disponíveis

Agora você pode usar o Workfront Fusion 2.0 para se conectar à sua conta de evento.

Com os módulos de evento, você pode:

* Criar uma solicitação de reunião
* Ler registros como contatos, eventos ou convidados
* Listar registros com base em critérios que você especificar
* Registre-se ou adicione convites para eventos específicos
* Atualizar ou excluir contatos
* Efetuar uma chamada de API personalizada

Para obter informações sobre os módulos de evento disponíveis, consulte [Módulos de conversão](../../../workfront-fusion/apps-and-their-modules/cvent-modules.md).

## O conector e os módulos do Microsoft Dynamics 365 já estão disponíveis

Agora você pode usar o Workfront Fusion 2.0 para se conectar à sua conta do Microsoft Dynamics 365. Com os módulos do Microsoft Dynamics 365, você pode:

* Acione um cenário quando registros forem adicionados ou atualizados no Microsoft Dynamics 365
* Criar, ler, atualizar ou excluir um registro do Microsoft Dynamics 365
* Executar uma chamada de API personalizada

Para obter informações sobre os módulos disponíveis do Microsoft Dynamics 365, consulte [Módulos do Microsoft Dynamics 365](../../../workfront-fusion/apps-and-their-modules/microsoft-dynamics-365-modules.md).

## O conector e os módulos do DocuSign já estão disponíveis

Agora você pode usar o Workfront Fusion 2.0 para se conectar à sua conta de Documentação. Com os módulos de Documentação, você pode:

* Acionar um cenário quando um envelope alterar seu status
* Criar um envelope
* Ler, enviar ou adicionar um recipient a um envelope existente
* Adicionar ou modificar campos personalizados em documentos
* Baixar um documento como um campo
* Fazer upload de um arquivo para um envelope
* Executar uma chamada de API personalizada

Para obter mais informações, consulte [Módulos do DocuSign](../../../workfront-fusion/apps-and-their-modules/docusign-modules.md).

## Pesquise o histórico de execução do cenário

Facilitamos a localização de informações específicas de execuções de cenários anteriores. A nova pesquisa de texto completo da Fusion possibilita pesquisar o histórico de execução de quaisquer dados contidos em um pacote. Por exemplo, para identificar qual execução criou uma tarefa específica, você pode usar a pesquisa de texto completo para procurar essa ID de tarefa.

Anteriormente, encontrava informações de execução específicas necessárias para exibir cada execução individualmente.

Para obter mais informações, consulte [Visualizar o histórico de execução de um cenário no Adobe Workfront Fusion](../../../workfront-fusion/scenarios/view-scenario-execution-history.md).

## Atualizações para o Data Store do Fusion 2.0

Para facilitar a personalização dos armazenamentos de dados, adicionamos novas funcionalidades. Agora, ao visualizar um armazenamento de dados, você pode:

* Arrastar e soltar para reorganizar colunas
* Editar uma única célula
* Adicionar várias linhas

Para obter mais informações sobre Data Stores, consulte [Módulos do armazenamento de dados](../../../workfront-fusion/apps-and-their-modules/data-store-modules.md).

## Faça uma solicitação de autorização da Chave de API por meio do conector HTTP

Para aumentar a flexibilidade nas maneiras de acessar APIs, adicionamos um novo módulo ao conector HTTP. Agora, você pode usar o conector HTTP para fazer uma solicitação quando o serviço da Web que você está acessando exigir o uso de uma chave de API.

Para obter mais informações, consulte [Módulos HTTP](../../../workfront-fusion/apps-and-their-modules/http-modules/http-modules-1.md).

## Novas funções disponíveis no painel de mapeamento

Para ajudar você a personalizar e simplificar fórmulas em seus módulos, adicionamos novas funções.

* O

   ```
   omit
   ```

   é uma função geral que omite as chaves fornecidas do objeto e retorna o restante.
* O

   ```
   pick
   ```

   é uma função geral que escolhe somente as teclas fornecidas do objeto.
* O

   ```
   escapeMarkdown
   ```

   é uma função de string que escapa de todas as tags Markdown em um texto.

Para obter mais informações sobre as funções omitir e selecionar, consulte [Funções gerais no Adobe Workfront Fusion](../../../workfront-fusion/functions/general-functions.md).

Para obter mais informações sobre a função escapeMarkdown , consulte [Funções de string no Adobe Workfront Fusion](../../../workfront-fusion/functions/string-functions.md).
