---
content-type: overview
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Fluxo de execução de cenário no Adobe Workfront Fusion
description: Este artigo explica como um cenário é executado e como os dados fluem por ele. Ele também explica onde você pode encontrar informações sobre os dados processados e como lê-los.
author: Becky
feature: Workfront Fusion
exl-id: 95c6e969-66b4-4b57-9e62-aae0cfb9bf98
source-git-commit: 75cf9af858e90a640c45b211d36f35b684128c2f
workflow-type: tm+mt
source-wordcount: '799'
ht-degree: 0%

---

# Fluxo de execução de cenário em [!DNL Adobe Workfront Fusion]

Este artigo explica como um cenário é executado e como os dados fluem por ele. Ele também explica onde você pode encontrar informações sobre os dados processados e como lê-los.

## Requisitos de acesso

Você deve ter o seguinte acesso para usar a funcionalidade neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] plano*</td> 
   <td> <p>[!DNL Pro] ou superior</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licença*</td> 
   <td> <p>[!UICONTROL Plano], [!UICONTROL Trabalho]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença [!UICONTROL Adobe Workfront Fusion]**</td> 
   <td>
   <p>Requisito de licença atual: nenhum requisito de licença [!DNL Workfront Fusion].</p>
   <p>Ou</p>
   <p>Requisito de licença herdada: [!UICONTROL [!DNL Workfront Fusion] para Automação e Integração do Trabalho], [!UICONTROL [!DNL Workfront Fusion] para Automação do Trabalho]</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produto</td> 
   <td>
   <p>Requisito atual do produto: se você tiver o Plano [!DNL Adobe Workfront] da [!UICONTROL Select] ou da [!UICONTROL Prime], sua organização deve comprar o [!DNL Adobe Workfront Fusion] e o [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo. [!DNL Workfront Fusion] está incluído no plano [!DNL Workfront] do [!UICONTROL Ultimate].</p>
   <p>Ou</p>
   <p>Requisito de produto herdado: sua organização deve comprar o [!DNL Adobe Workfront Fusion] e o [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Para saber que plano, tipo de licença ou acesso você tem, contate o administrador do [!DNL Workfront].

Para obter informações sobre [!DNL Adobe Workfront Fusion] licenças, consulte [[!DNL Adobe Workfront Fusion] licenças](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Fluxo de execução de cenário

Depois que um cenário é configurado corretamente e ativado, ele é executado de acordo com seu agendamento definido.

À medida que o cenário começa, o primeiro módulo responde a um evento que foi definido para ser observado. Se retornar algum pacote (dados), ele passará para o módulo seguinte e o cenário continuará, passando os pacotes por cada módulo sucessivo, um por um.

Se os pacotes forem processados corretamente em todos os módulos, o cenário será marcado como sucesso na área de detalhes do cenário, conforme explicado em [Detalhes do cenário em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-detail.md).

* Para obter mais informações sobre como configurar um cenário, consulte [O editor de cenários em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-editor.md).
* Para obter mais informações sobre como ativar um cenário, consulte [Ativar ou desativar um cenário [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/activate-or-inactivate-scenario.md).
* Para obter mais informações sobre o agendamento de um cenário, consulte [Agendar um cenário em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/schedule-a-scenario.md).
* Para obter mais informações sobre módulos, consulte [Tipos de módulos](../../workfront-fusion/modules/module-types.md).

### Exemplo: [!UICONTROL [!DNL Workfront Fusion] para Automação de Trabalho]

>[!INFO]
>
>**Exemplo:** em um cenário que observa as solicitações recebidas em [!DNL Workfront] e as converte em projetos [!DNL Workfront], os dados fluiriam da seguinte maneira.
>
>O primeiro passo do cenário, executado pelo primeiro módulo, é observar as solicitações. Cada solicitação recebida é considerada um pacote. Se o módulo for executado sem encontrar nenhum pacote, o cenário terminará após o primeiro módulo.
>
>Se o primeiro módulo retornar um pacote, ele passará pelo restante do cenário. Neste exemplo, o restante do cenário consiste no segundo e último módulo, que converte a solicitação em um projeto.
>
>?![](assets/example-execution-flow-wf-only-350x157.png)

### Exemplo: [!UICONTROL [!DNL Workfront Fusion] para Automação e Integração de Trabalho]

>[!INFO]
>
>**Exemplo:** em um cenário que baixa documentos de [!DNL Adobe Workfront] e os envia para uma pasta em [!DNL Dropbox], os dados fluiriam da seguinte maneira.
>
>O primeiro passo do cenário, realizado pelo primeiro módulo, é observar os pacotes (documentos). Neste exemplo, o módulo observa pacotes em [!DNL Workfront]. Se não retornar um pacote, o cenário terminará após o primeiro módulo.
>
>Se um pacote for retornado, ele passará pelo restante do cenário. Neste exemplo, o restante do cenário consiste no segundo e último módulo, que carrega o pacote para a pasta [!DNL Dropbox].
>
>![](assets/example-wf-dropbox-scen-execution-flow-350x202.png)
>
>Se o primeiro módulo retornar vários pacotes, o primeiro pacote será carregado para [!DNL Dropbox] antes que o segundo pacote seja carregado. O segundo pacote é carregado, o terceiro e assim por diante.

## Informações sobre pacotes processados

Para cada módulo, o pacote passa por um processo de quatro etapas antes de passar para o próximo módulo ou atingir seu destino final. O processo de quatro etapas é Inicialização, Operação, Confirmar/Reverter e Finalização. Isso é chamado de processamento de transação e ajuda a explicar como os dados foram processados em um módulo.

Quando uma execução de cenário é concluída, cada módulo exibe um ícone que mostra o número de operações realizadas. Você pode clicar nesse ícone para exibir as informações detalhadas sobre os pacotes processados, no formato descrito acima. Você pode ver quais configurações de módulos foram usadas e quais pacotes foram retornados por qual módulo.

![](assets/info-processed-bundles-350x396.png)

Um módulo recebeu informações de entrada como:

* Imagem convertida
* Pasta selecionada para onde a imagem deve ser carregada
* Nome original da imagem [!DNL Facebook]

Após o processamento, o módulo retornou estas informações de saída:

* ID de imagem atribuída por [!DNL Dropbox]
* Caminho completo onde em [!DNL Dropbox] [!DNL Workfront Fusion] carregou o arquivo

As informações acima são capturadas separadamente para cada pacote, conforme marcado pelas caixas suspensas [!UICONTROL Operação 1] e [!UICONTROL Operação 2] na imagem.

Para obter mais informações sobre o processamento de transações, consulte [Execução do cenário, ciclos e fases em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

## Erro ao executar um cenário

Pode ocorrer um erro durante a execução do cenário. Por exemplo, se você excluir a pasta [!DNL Dropbox] definida como pasta de destino na configuração do módulo, o cenário será encerrado com uma mensagem de erro. Para obter mais informações sobre como tratar erros, consulte [Processamento de erros [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-processing.md).
