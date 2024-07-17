---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Operações no Adobe Workfront Fusion
description: Uma operação no Adobe Workfront Fusion é uma tarefa executada por um módulo. Para fins de rastreamento, qualquer ação bem-sucedida executada por um módulo é uma operação.
author: Becky
feature: Workfront Fusion
exl-id: 34268fb6-e485-42be-b751-3ee79bbf5797
source-git-commit: abb021a6857f8016d4f8b6bcf99fe818e47faea6
workflow-type: tm+mt
source-wordcount: '332'
ht-degree: 0%

---

# Operações em [!DNL Adobe Workfront Fusion]

Uma operação em [!DNL Adobe Workfront Fusion] é uma tarefa executada por um módulo. Para fins de rastreamento, qualquer ação bem-sucedida executada por um módulo é uma operação.

## Considerações ao contar o número de operações

* Em geral, qualquer execução bem-sucedida da etapa de ação é considerada uma operação.

* O primeiro módulo em um cenário é executado apenas uma vez e é sempre contado como uma operação, mesmo que não retorne um pacote.

* O número de vezes que o restante dos módulos é executado depende do número de pacotes que eles devem processar.  Uma execução de um módulo para um pacote é uma operação. Uma exceção é o módulo agregador, que é contado como uma operação por conjunto de pacotes sendo processados.

* As operações são contadas no estágio [!UICONTROL Finalization] de execução de um cenário.

* Os itens a seguir são **não** contados como operações:

   * Quaisquer etapas de filtro.

   * Qualquer ação que cause erros ou seja interrompida.

   * Qualquer rota que não seja executada porque as regras da rota não foram atendidas, como rotas de fallback ou desabilitadas.

   * Qualquer ação que não seja executada porque um filtro não permitiu a passagem de dados ou porque o cenário foi interrompido devido a um erro.

## Limites de operação

Sua organização pode ter um limite mensal de operações. Isso se baseia no plano [!DNL Workfront] que sua organização adquiriu. O plano [!UICONTROL Ultimate] [!DNL Workfront] oferece operações ilimitadas.

Se sua organização tiver um limite mensal, você será notificado quando estiver próximo do limite. Se você ultrapassar o limite, o [!DNL Workfront] contatará sua organização para garantir que seu plano atenda às suas necessidades.

## Exibir o número de operações executadas nos últimos 30 dias

Você pode ver um gráfico que mostra o número de operações realizadas. Esses gráficos estão disponíveis nos seguintes locais:

* **Painel da organização**: operações usadas por toda a organização
* **Painel da equipe**: operações usadas pelos cenários pertencentes a esta equipe (somente [!DNL Adobe Experience Cloud])
* **Página de detalhes do cenário**: Operações usadas por este cenário (somente [!DNL Adobe Experience Cloud])
