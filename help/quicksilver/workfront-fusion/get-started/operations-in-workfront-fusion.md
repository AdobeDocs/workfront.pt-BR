---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Operações no Adobe Workfront Fusion
description: Uma operação no Adobe Workfront Fusion é uma tarefa executada por um módulo. Para fins de rastreamento, qualquer ação bem-sucedida executada por um módulo é uma operação.
author: Becky
feature: Workfront Fusion
source-git-commit: 8d82fd10a6742f13f62b5479fafa5b42e567700f
workflow-type: tm+mt
source-wordcount: '331'
ht-degree: 0%

---

# Operações em [!DNL Adobe Workfront Fusion]

Uma operação em [!DNL Adobe Workfront Fusion] é uma tarefa executada por um módulo. Para fins de rastreamento, qualquer ação bem-sucedida executada por um módulo é uma operação.

## Considerações ao contar o número de operações

* Em geral, qualquer execução bem-sucedida da etapa de ação é considerada uma operação.

* O primeiro módulo em um cenário é executado apenas uma vez e é sempre contado como uma operação, mesmo que não retorne um pacote.

* O número de vezes que o restante dos módulos é executado depende do número de pacotes que eles devem processar.  Uma execução de um módulo para um pacote é uma operação. Uma exceção é o módulo agregador, que é contado como uma operação por conjunto de pacotes sendo processados.

* As operações são contadas no [!UICONTROL Finalização] estágio de uma execução de cenário.

* Veja a seguir **não** contados como operações:

   * Quaisquer etapas de filtro.

   * Qualquer ação que cause erros ou seja interrompida.

   * Qualquer rota que não seja executada porque as regras da rota não foram atendidas, como rotas de fallback ou desabilitadas.

   * Qualquer ação que não seja executada porque um filtro não permitiu a passagem de dados ou porque o cenário foi interrompido devido a um erro.

## Limites de operação

Sua organização pode ter um limite mensal de operações. Baseia-se no [!DNL Workfront] que sua organização adquiriu. A variável [!UICONTROL Ultimate] [!DNL Workfront] O plano oferece operações ilimitadas.

Se sua organização tiver um limite mensal, você será notificado quando estiver próximo do limite. Se você ultrapassar o limite, [!DNL Workfront] entrará em contato com sua organização para garantir que seu plano atenda às suas necessidades.

## Exibir o número de operações executadas nos últimos 30 dias

Você pode ver um gráfico que mostra o número de operações realizadas. Esses gráficos estão disponíveis nos seguintes locais:

* **Painel da organização**: operações usadas por toda a organização
* **Painel da equipe**: operações usadas por cenários de propriedade dessa equipe ([!DNL Adobe Experience Cloud] somente)
* **Página de detalhes do cenário**: operações usadas por esse cenário ([!DNL Adobe Experience Cloud] somente)

