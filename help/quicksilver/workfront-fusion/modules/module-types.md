---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Tipos de módulos
description: '"O Adobe Workfront Fusion distingue cinco tipos de módulos: módulos de ação, módulos de pesquisa, módulos de acionador, agregadores e iteradores. Agregadores e Iteradores são para cenários avançados.'
author: Becky
feature: Workfront Fusion
exl-id: 58b4aa76-6c4c-47fc-a42c-c5286da5633a
source-git-commit: e58ff769015b8c4e34b34eea653f55a296eea371
workflow-type: tm+mt
source-wordcount: '963'
ht-degree: 0%

---

# Tipos de módulos

A[!UICONTROL Adobe Workfront Fusion] distingue cinco tipos de módulos: módulos de ação, módulos de pesquisa, módulos de acionador, agregadores e iteradores. Agregadores e Iteradores são para cenários avançados.

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] para automação e integração de trabalho] </p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produto</td> 
   <td>Sua organização deve comprar o Adobe Workfront Fusion e a Adobe Workfront para usar a funcionalidade descrita neste artigo.</td> 
  </tr> 
 </tbody> 
</table>

Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

Para obter informações sobre [!DNL Adobe Workfront Fusion] licenças, consulte [[!DNL Adobe Workfront Fusion] licenças](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Módulos de ação

Os módulos de ação são o tipo mais comum de módulo. Um módulo de ação típico retorna um único pacote, que passa para o próximo módulo para processamento.

Diferentemente dos módulos de acionador, os módulos de ação podem ser colocados no início, no meio ou no fim de um cenário. Os cenários podem conter um número ilimitado de módulos de ação.

>[!INFO]
>
>**Exemplos:**
>
>* **[!DNL Workfront]> [!UICONTROL Carregar um arquivo]** envia um arquivo para [!DNL Workfront] e retorna seu identificador.
>* **[!UICONTROL Imagem] > [!UICONTROL Redimensionar]** O recebe uma imagem, a redimensiona para dimensões especificadas e passa a imagem redimensionada para a próxima ação.


O tipo de Ação tem quatro subtipos: Criar, ler, atualizar e excluir. O subtipo Update permite as três operações a seguir:

* **Apagar o conteúdo de um campo**. Essa operação ocorre quando o conteúdo do campo é avaliado para apagar a palavra-chave (não confundir com *empty*).

   ![](assets/erase-content-of-field.png)

* **Deixe o conteúdo de um campo inalterado**. Essa operação ocorre quando o campo é deixado em branco ou o conteúdo do campo é avaliado como vazio (representado por null no JSON).

   ![](assets/leave-content-field-unchanged-350x231.png)

* **Substituir o conteúdo de um campo**. Esta operação tem lugar em todos os outros casos que não os acima descritos.

>[!NOTE]
>
>* Se você não vir a variável `erase` palavra-chave no painel de mapeamento, o módulo não é um módulo de atualização ou não foi atualizado para as especificações mais recentes do aplicativo.
>* &quot;[!UICONTROL Empty]&quot; não altera o conteúdo do campo. Se for necessário apagar o campo, é possível usar a seguinte fórmula:
>
>![](assets/formula-ifempty-name-erase.png)
>
>Deixar um campo inalterado quando seu conteúdo é avaliado como vazio não é possível no momento.

## Módulos de pesquisa

Uma Pesquisa típica retorna zero, um ou mais pacotes, que são passados para o próximo módulo para processamento.

Você pode colocar Pesquisas no início, no meio ou no fim de um cenário.

Os cenários podem conter um número ilimitado de Pesquisas.

>[!INFO]
>
>**Exemplo:**
>
>**[!DNL Workfront]> [!UICONTROL Ler registros relacionados]**  lê registros que correspondem à consulta de pesquisa especificada, em um objeto pai específico

## Módulos de acionador

Os acionadores geram pacotes quando houve uma alteração em um determinado serviço. A alteração pode ser uma criação de novos registros, exclusão de um registro, atualização de um registro e assim por diante.

Cada Acionador pode retornar zero, um ou mais pacotes que passam para o próximo módulo para processamento.

Os Acionadores só podem ser colocados no início de um cenário.

Cada cenário pode conter apenas um Acionador.

[!DNL Workfront Fusion] faz a distinção entre dois tipos de acionadores: Acionadores de pesquisa e acionadores Instant.

### Acionadores de pesquisa

Os acionadores de pesquisa pesquisam regularmente um determinado serviço, mesmo que não tenha havido alterações desde a execução anterior. Recomendamos que você programe um cenário contendo um acionador de pesquisa para ser executado em intervalos regulares. Se houver um *alterar*, o acionador retorna pacotes contendo informações sobre a alteração. Se não houver *alterar*, o acionador não gera nenhum pacote. Para obter instruções sobre como programar um cenário, consulte [Programe um cenário em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/schedule-a-scenario.md).

Os acionadores de pesquisa permitem selecionar o primeiro pacote que devem ser exibido por meio do painel de época. O painel é exibido automaticamente depois que você salva um acionador ou altera as configurações do acionador. Para obter mais informações, consulte [Escolha onde um módulo de acionador começa em [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/modules/choose-where-trigger-module-starts.md).

>[!NOTE]
>
>As configurações feitas no painel de época afetam apenas a primeira execução do módulo. Depois que o módulo é executado, ele lembra do último pacote de saída e anula as configurações feitas por meio do painel de época.

>[!INFO]
>
>**Exemplos:**
>
>* **[!DNL Workfront]> [!UICONTROL Registros de monitoramento]** retorna arquivos que foram adicionados recentemente desde a última vez que o cenário foi executado
>
>* **[!DNL Google Sheets]> [!UICONTROL Linhas de observação]** retorna novas linhas adicionadas pelo usuário desde a última vez em que o cenário foi executado


### Acionadores instantâneos

Acionadores instantâneos permitem que o serviço notifique [!DNL Workfront Fusion] sobre um *alterar* imediatamente. Recomendamos que você programe um cenário contendo um acionador instantâneo para ser executado imediatamente. Para obter instruções, consulte [Programar um cenário no Adobe Workfront Fusion](../../workfront-fusion/scenarios/schedule-a-scenario.md). Consulte também [Acionadores instantâneos (webhooks) em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/webhooks/instant-triggers-webhooks.md) para obter detalhes sobre como os dados recebidos são tratados.

>[!INFO]
>
>**Exemplos:**
>
>* **[!DNL Workfront]> [!UICONTROL Eventos de observação]** retorna informações quando um determinado tipo de evento ocorre no Workfront, como a criação de uma tarefa.
>* **[!DNL Google Sheets]> [!UICONTROL Monitoramento de alterações]** retorna informações sempre que uma célula é atualizada.


## Agregadores

Um Agregador é um tipo de módulo que acumula vários pacotes em um único pacote.

Cada Agregador retorna somente um pacote, que é transferido para o próximo módulo para processamento adicional.

Você pode colocar Agregadores somente no meio de um cenário.

Os cenários podem conter um número ilimitado de agregadores.

>[!INFO]
>
>**Exemplos:**
>
>* **[!UICONTROL Arquivar] > [!UICONTROL Criar um arquivo]** compacta arquivos recebidos em um arquivo zip
>* **[!UICONTROL CSV] > [!UICONTROL Agregar ao CSV]** mescla várias strings de um arquivo CSV em uma única linha
>* **[!UICONTROL Ferramentas] > [!UICONTROL Agregador de texto]** combina várias strings em uma única string


Para obter mais informações, consulte [Módulo agregador em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/aggregator-module.md).

## Iteradores

Um iterador é um tipo de módulo que divide matrizes em vários pacotes separados.

Cada iterador retorna um ou mais pacotes, que são passados para o próximo módulo para processamento.

Você pode colocar Iteradores somente no meio de um cenário.

Os cenários podem conter um número ilimitado de iteradores.

>[!INFO]
>
>**Exemplo:**
>
>**[!UICONTROL Email] > [!UICONTROL Recuperar anexos]** quebra uma matriz de anexos em pacotes separados

Para obter mais informações, consulte [Módulo iterador em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/iterator-module.md) e [Mapear uma matriz em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-an-array.md).
