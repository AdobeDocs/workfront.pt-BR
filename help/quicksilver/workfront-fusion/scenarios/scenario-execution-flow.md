---
content-type: overview
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Fluxo de execução do cenário no Adobe Workfront Fusion
description: Este artigo explica como um cenário é executado e como os dados fluem por ele. Ele também explica onde você pode encontrar informações sobre seus dados processados e como lê-los.
author: Becky
feature: Workfront Fusion
exl-id: 95c6e969-66b4-4b57-9e62-aae0cfb9bf98
source-git-commit: 59941ea1ce523a0d1036138a83f771b058049b34
workflow-type: tm+mt
source-wordcount: '749'
ht-degree: 0%

---

# Fluxo de execução do cenário em [!DNL Adobe Workfront Fusion]

Este artigo explica como um cenário é executado e como os dados fluem por ele. Ele também explica onde você pode encontrar informações sobre seus dados processados e como lê-los.

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
   <td role="rowheader">Licença da [!UICONTROL Adobe Workfront Fusion]**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] para automação e integração de trabalho] </p><p>[!UICONTROL [!DNL Workfront Fusion] para Automação de Trabalho] </p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produto</td> 
   <td>Sua organização deve comprar [!DNL Adobe Workfront Fusion] bem como [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo.</td> 
  </tr> 
 </tbody> 
</table>

Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com seu [!DNL Workfront] administrador.

Para obter informações sobre [!DNL Adobe Workfront Fusion] licenças, consulte [[!DNL Adobe Workfront Fusion] licenças](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Fluxo de execução do cenário

Depois que um cenário é configurado corretamente e ativado, ele é executado de acordo com seu agendamento definido.

Conforme o cenário começa, o primeiro módulo responde a um evento que foi definido para ser assistido. Se retornar qualquer pacote (dados), eles passarão para o próximo módulo e o cenário continuará, passando os pacotes por cada módulo sucessivo, um por um.

Se os pacotes forem processados corretamente em todos os módulos, o cenário será marcado como um sucesso na área de detalhes do cenário, como explicado em [Detalhes do cenário em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-detail.md).

* Para obter mais informações sobre como configurar um cenário, consulte [Configurações básicas do cenário em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/basic-scenario-settings.md).
* Para obter mais informações sobre como ativar um cenário, consulte [Ativar ou desativar um cenário em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/activate-or-inactivate-scenario.md).
* Para obter mais informações sobre como programar um cenário, consulte [Programe um cenário em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/schedule-a-scenario.md).
* Para obter mais informações sobre módulos, consulte [Tipos de módulos](../../workfront-fusion/modules/module-types.md).

### Exemplo: [!UICONTROL [!DNL Workfront Fusion] para Automação de Trabalho]

>[!INFO]
>
>**Exemplo:** Em um cenário que observa solicitações recebidas em [!DNL Workfront] e, em seguida, converte-os em [!DNL Workfront] projetos, os dados fluiriam da seguinte maneira.
>
>A primeira etapa do cenário, executada pelo primeiro módulo, é observar solicitações. Cada solicitação que chega é considerada um pacote. Se o módulo for executado sem localizar nenhum pacote, o cenário terminará após o primeiro módulo.
>
>Se o primeiro módulo retornar um pacote, ele passará pelo restante do cenário. Neste exemplo, o restante do cenário consiste no segundo e último módulo, que converte a solicitação em um projeto.
>
>?![](assets/example-execution-flow-wf-only-350x157.png)

### Exemplo: [!UICONTROL [!DNL Workfront Fusion] para automação e integração de trabalho]

>[!INFO]
>
>**Exemplo:** Em um cenário que baixa documentos de [!DNL Adobe Workfront] e os envia para uma pasta em [!DNL Dropbox], os dados fluiriam da seguinte maneira.
>
>A primeira etapa do cenário, realizada pelo primeiro módulo, é procurar pacotes (documentos). Neste exemplo, o módulo busca pacotes em [!DNL Workfront]. Se não retornar um pacote, o cenário terminará após o primeiro módulo.
>
>Se um pacote for retornado, ele passará pelo restante do cenário. Neste exemplo, o restante do cenário consiste no segundo e último módulo, que faz o upload do pacote para o [!DNL Dropbox] pasta.
>
>![](assets/example-wf-dropbox-scen-execution-flow-350x202.png)
>
>Se o primeiro módulo retornar vários pacotes, o primeiro pacote será carregado para [!DNL Dropbox] antes do upload do segundo pacote. Em seguida, o segundo pacote é carregado, depois o terceiro, e assim por diante.

## Informações sobre pacotes processados

Para cada módulo, o pacote passa por um processo de quatro etapas antes de passar para o próximo módulo ou alcançar seu destino final. O processo de quatro etapas é Inicialização, Operação, Confirmar/Reversão e Finalização. Isso é chamado de processamento de transação e ajuda a explicar como os dados foram processados em um módulo.

Quando uma execução de cenário é concluída, cada módulo exibe um ícone que mostra o número de operações executadas. Você pode clicar nesse ícone para exibir as informações detalhadas sobre os pacotes processados, no formato descrito acima. Você pode ver quais configurações de módulos foram usadas e quais pacotes foram retornados por qual módulo.

![](assets/info-processed-bundles-350x396.png)

Um módulo recebeu informações de entrada, como:

* Imagem convertida
* Pasta selecionada na qual a imagem será carregada
* Nome original do [!DNL Facebook] imagem

Após o processamento, o módulo retornou essas informações de saída:

* ID de imagem atribuída por [!DNL Dropbox]
* Caminho completo em que [!DNL Dropbox] [!DNL Workfront Fusion] o arquivo foi carregado

As informações acima são capturadas para cada pacote separadamente, conforme marcado pelas caixas suspensas [!UICONTROL Operação 1] e [!UICONTROL Operação 2] na imagem.

Para obter mais informações sobre o processamento de transações, consulte [Execução do cenário, ciclos e fases em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

## Erro ao executar um cenário

Pode ocorrer um erro durante a execução do cenário. Por exemplo, se você excluir a variável [!DNL Dropbox] pasta que você definiu como pasta de destino na configuração do módulo, o cenário termina com uma mensagem de erro. Para obter mais informações sobre como lidar com erros, consulte [Processamento de erros no [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-processing.md).
