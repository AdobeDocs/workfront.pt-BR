---
title: Aprimoramentos no projeto do terceiro trimestre de 2025
description: Aprimoramentos no projeto do terceiro trimestre de 2025
author: Becky
feature: Product Announcements
recommendations: noDisplay, noCatalog
hide: true
hidefromtoc: true
exl-id: 33fa5a61-5300-402c-9f80-f2701f7999a8
source-git-commit: 3ff70fcc949644d511c876add10d2c58901cb197
workflow-type: tm+mt
source-wordcount: '515'
ht-degree: 0%

---

# Aprimoramentos no projeto do terceiro trimestre de 2025

Esta página descreve as melhorias no Project feitas com a versão do terceiro trimestre de 2025 para o ambiente de Pré-visualização. Esses aprimoramentos serão disponibilizados no ambiente de Produção, conforme observado.

Para obter uma lista de todas as alterações disponíveis neste momento no ciclo de lançamento do terceiro trimestre de 2025, consulte [Visão geral da versão do terceiro trimestre de 2025](/help/quicksilver/product-announcements/product-releases/25-q3-release-activity/25-q3-release-overview.md).

## Alteração na forma como as Horas efetivas são armazenadas no banco de dados para chamadas de API

>[!NOTE]
>
>* Visualização: com a próxima versão da API, agendada para posteriormente em 2025
>* Versão rápida de produção: com a próxima versão da API, programada para ser lançada em 2025
>* Produção para todos os clientes: com a próxima versão da API, programada para mais tarde em 2025

Esta atualização introduz uma mudança na forma como as Horas efetivas de projetos, tarefas e problemas são armazenadas no banco de dados. A partir desta atualização, as Horas Efetivas usarão um campo de valor de `actualWorkRequiredDouble` (com um valor em horas).

Antes desta atualização, as Horas Efetivas eram armazenadas com um campo de valor de `actualWorkRequired` (com um valor em minutos). Esta atualização garantirá uma contagem mais precisa para as Horas efetivas ao calculá-las usando uma chamada de API.

Devido a essa alteração, talvez seja necessário atualizar qualquer chamada de API que se refira ao campo de valor original. Você não deve fazer alterações se estiver usando um campo de valor de `actualWorkRequiredExpression` nas chamadas de API.

Esta atualização não altera os cálculos de Horas efetivas de projetos, tarefas e problemas nas colunas de campos personalizados calculados.

## Atualizar no usando o controle deslizante Porcentagem concluída em um cabeçalho de tarefa ou problema

>[!NOTE]
>
>* Visualização: 27 de maio de 2025
>* Versão rápida de produção: 27 de maio de 2025
>* Produção para todos os clientes: 27 de maio de 2025

Atualizamos a forma como o controle deslizante de porcentagem concluída funciona para tarefas e problemas.

A seguinte funcionalidade está disponível:

* Quando você desliza a bolha azul Porcentagem concluída no cabeçalho de uma tarefa ou problema, a Porcentagem concluída da tarefa ou problema será atualizada em incrementos de cinco pontos. Antes desta atualização, ao deslizar a bolha azul Porcentagem concluída, as tarefas ou problemas eram atualizados em incrementos de um ponto.

* Você pode clicar duas vezes na bolha azul e atualizá-la manualmente com qualquer número desejado sem usar o controle deslizante. Essa funcionalidade não foi alterada.

Não há outras alterações introduzidas para atualizar a Porcentagem concluída das tarefas e problemas em outras áreas do Workfront.

Para obter informações, consulte [Exibir e atualizar Porcentagem Concluída para tarefas](/help/quicksilver/manage-work/projects/updating-work-in-a-project/view-update-percent-complete-for-tasks.md).

## Mais transparência ao usar o Assistente de IA em projetos, tarefas e problemas

>[!NOTE]
>
>* Visualização: 19 de maio de 2025
>* Versão rápida de produção: 19 de maio de 2025
>* Produção para todos os clientes: 19 de maio de 2025

Para deixar mais claro como o Assistente de IA está localizando respostas para perguntas sobre projetos, tarefas e problemas da Workfront, adicionamos essas informações à resposta da pergunta. Agora, o Assistente de IA inclui suas informações de pesquisa na saída. Você pode usar essas informações como uma maneira de verificar se o Assistente do AI identificou corretamente a pergunta que você estava fazendo e de entender o contexto da resposta.

Anteriormente, essas informações não estavam disponíveis na resposta do Assistente de IA.

Para obter informações sobre como usar o Assistente de IA para obter informações sobre itens do Workfront, consulte [Usar o Assistente de IA para trabalhar com projetos, tarefas e problemas](/help/quicksilver/workfront-basics/ai-assistant/work-with-pti-through-ai-assisant.md).
