---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Tipos de módulos
description: '"O Adobe Workfront Fusion distingue cinco tipos de módulos: módulos de ação, módulos de pesquisa, módulos de acionador, agregadores e iteradores. Agregadores e Iteradores são para cenários avançados.'''
author: Becky
feature: Workfront Fusion
exl-id: 58b4aa76-6c4c-47fc-a42c-c5286da5633a
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '973'
ht-degree: 0%

---

# Tipos de módulos

A[!UICONTROL Adobe Workfront Fusion] O distingue cinco tipos de módulos: módulos de ação, módulos de pesquisa, módulos de acionador, agregadores e iteradores. Agregadores e Iteradores são para cenários avançados.

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
   <p>Requisito de licença atual: Não [!DNL Workfront Fusion] requisito de licença.</p>
   <p>Ou</p>
   <p>Requisito de licença herdada: [!UICONTROL [!DNL Workfront Fusion] para Automação e integração do trabalho] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produto</td> 
   <td>Sua organização deve comprar o Adobe Workfront Fusion e o Adobe Workfront para usar a funcionalidade descrita neste artigo.</td> 
  </tr> 
 </tbody> 
</table>

Para descobrir seu plano, tipo de licença ou acesso, entre em contato com o administrador do Workfront.

Para obter informações sobre [!DNL Adobe Workfront Fusion] licenças, consulte [[!DNL Adobe Workfront Fusion] licenças](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Módulos de ação

Os módulos de ação são o tipo mais comum de módulo. Um módulo de ação típico retorna um único pacote, que então passa para o próximo módulo para processamento.

Diferentemente dos módulos de acionamento, os módulos de ação podem ser colocados no início, no meio ou no final de um cenário. Os cenários podem conter um número ilimitado de módulos de ação.

>[!INFO]
>
>**Exemplos:**
>
>* **[!DNL Workfront]> [!UICONTROL Carregar um arquivo]** envia um arquivo para [!DNL Workfront] e retorna seu identificador.
>* **[!UICONTROL Imagem] > [!UICONTROL Redimensionar]** recebe uma imagem, redimensiona-a para dimensões especificadas e passa a imagem redimensionada para a próxima ação.

O tipo de ação tem quatro subtipos: Criar, Ler, Atualizar e Excluir. O subtipo Update permite as três operações a seguir:

* **Apagar o conteúdo de um campo**. Essa operação ocorre quando o conteúdo do campo é avaliado para apagar palavras-chave (não deve ser confundido com *vazio*).

  ![](assets/erase-content-of-field.png)

* **Deixar o conteúdo de um campo inalterado**. Essa operação ocorre quando o campo é deixado vazio ou o conteúdo do campo é avaliado como vazio (representado por meio de nulo no JSON).

  ![](assets/leave-content-field-unchanged-350x231.png)

* **Substituir o conteúdo de um campo**. Esta operação ocorre em todos os outros casos que não os descritos acima.

>[!NOTE]
>
>* Se você não vir a variável `erase` no painel de mapeamento, o módulo não é um módulo de atualização ou não foi atualizado para as especificações mais recentes do aplicativo.
>* &quot;[!UICONTROL Empty]&quot; não altera o conteúdo do campo. Se for necessário apagar o campo, você poderá usar a seguinte fórmula:
>
>![](assets/formula-ifempty-name-erase.png)
>
>No momento, não é possível deixar um campo inalterado quando seu conteúdo é avaliado como vazio.

## Pesquisar módulos

Uma Pesquisa típica retorna zero, um ou mais pacotes, que passam para o próximo módulo para processamento.

Você pode colocar Pesquisas no início, no meio ou no fim de um cenário.

Os cenários podem conter um número ilimitado de pesquisas.

>[!INFO]
>
>**Exemplo:**
>
>**[!DNL Workfront]> [!UICONTROL Ler registros relacionados]**  O lê registros que correspondem à consulta de pesquisa especificada em um determinado objeto pai

## Módulos de acionamento

Os acionadores geram pacotes quando há uma alteração em um determinado serviço. A alteração pode ser uma criação de novos registros, exclusão de um registro, atualização de um registro e assim por diante.

Cada acionador pode retornar zero, um ou mais pacotes que, em seguida, passam para o próximo módulo para processamento.

Os acionadores podem ser posicionados somente no início de um cenário.

Cada cenário pode conter apenas um Acionador.

[!DNL Workfront Fusion] O distingue entre dois tipos de acionadores: acionadores de pesquisa e acionadores instantâneos.

### Acionadores de sondagem

Os acionadores de pesquisa consultam regularmente um determinado serviço, mesmo que não tenha havido alterações desde a execução anterior. Recomendamos que você agende um cenário contendo um acionador de sondagem para ser executado em intervalos regulares. Se houver uma *alterar*, o acionador retorna pacotes que contêm informações sobre a alteração. Se não houver *alterar*, o acionador não gera nenhum pacote. Para obter instruções sobre como agendar um cenário, consulte [Agendar um cenário no [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/schedule-a-scenario.md).

Os acionadores de pesquisa permitem selecionar o primeiro pacote que devem ser emitido por meio do painel da época. O painel é exibido automaticamente depois que você salva um acionador ou altera as configurações dele. Para obter mais informações, consulte [Escolha onde um módulo de acionador começa em [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/modules/choose-where-trigger-module-starts.md).

>[!NOTE]
>
>As configurações feitas no painel da época afetam somente a primeira execução do módulo. Depois que o módulo é executado, ele lembra do último pacote emitido e anula as configurações feitas por meio do painel da época.

>[!INFO]
>
>**Exemplos:**
>
>* **[!DNL Workfront]> [!UICONTROL Observar registros]** retorna arquivos que foram adicionados recentemente desde a última vez que o cenário foi executado
>
>* **[!DNL Google Sheets]> [!UICONTROL Observar linhas]** retorna novas linhas adicionadas pelo usuário desde a última vez que o cenário foi executado

### Acionadores instantâneos

Os disparadores instantâneos permitem que o serviço notifique [!DNL Workfront Fusion] sobre um *alterar* imediatamente. Recomendamos que você agende um cenário contendo um acionador instantâneo para ser executado imediatamente. Para obter instruções, consulte [Programar um cenário no Adobe Workfront Fusion](../../workfront-fusion/scenarios/schedule-a-scenario.md). Consulte também [Acionadores instantâneos (webhooks) no [!DNL Adobe Workfront Fusion]](../../workfront-fusion/webhooks/instant-triggers-webhooks.md) para obter detalhes sobre como os dados de entrada são tratados.

>[!INFO]
>
>**Exemplos:**
>
>* **[!DNL Workfront]> [!UICONTROL Assistir a eventos]** retorna informações quando um determinado tipo de evento ocorre no Workfront, como a criação de uma tarefa.
>* **[!DNL Google Sheets]> [!UICONTROL Observar alterações]** retorna informações sempre que uma célula é atualizada.

## Agregadores

Um Agregador é um tipo de módulo que acumula vários pacotes em um único pacote.

Cada Agregador retorna apenas um pacote, que então passa para o próximo módulo para processamento adicional.

Você pode colocar Agregadores somente no meio de um cenário.

Os cenários podem conter um número ilimitado de agregadores.

>[!INFO]
>
>**Exemplos:**
>
>* **[!UICONTROL Arquivar] > [!UICONTROL Criar um arquivo]** compacta arquivos recebidos em um arquivo zip
>* **[!UICONTROL CSV] > [!UICONTROL Agregar em CSV]** mescla várias cadeias de caracteres de um arquivo CSV em uma única linha
>* **[!UICONTROL Ferramentas] > [!UICONTROL Agregador de texto]** combina várias cadeias de caracteres em uma única cadeia

Para obter mais informações, consulte [Módulo agregador em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/aggregator-module.md).

## Iteradores

Um Iterador é um tipo de módulo que divide matrizes em vários conjuntos separados.

Cada iterador retorna um ou mais pacotes, que então passam para o próximo módulo para processamento.

É possível colocar iteradores somente no meio de um cenário.

Os cenários podem conter um número ilimitado de iteradores.

>[!INFO]
>
>**Exemplo:**
>
>**[!UICONTROL E-mail] > [!UICONTROL Recuperar anexos]** divide uma matriz de anexos em conjuntos separados

Para obter mais informações, consulte [Módulo Iterador em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/iterator-module.md) e [Mapear uma matriz no [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-an-array.md).
