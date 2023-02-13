---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Execução do cenário, ciclos e fases em [!DNL Adobe Workfront Fusion]
description: Este artigo descreve eventos que ocorrem enquanto uma [!DNL Adobe Workfront Fusion] estiver em execução, como inicialização, operações, confirmações e reversões.
author: Becky
feature: Workfront Fusion
exl-id: 5403f476-226d-4268-affc-8e06b1117684
source-git-commit: 59941ea1ce523a0d1036138a83f771b058049b34
workflow-type: tm+mt
source-wordcount: '502'
ht-degree: 0%

---

# Execução do cenário, ciclos e fases em [!DNL Adobe Workfront Fusion]

[!DNL Adobe Workfront Fusion] é um sistema transacional, semelhante a bancos de dados relacionais. Cada execução de cenário começa com a fase de inicialização, continua com pelo menos um ciclo composto pelas fases de operação e confirmação/reversão e termina com a fase de finalização:

>[!INFO]
>
>**Exemplo**
>
>Inicialização
>
>Ciclo nº 1
>
>Funcionamento (leitura ou escrita)
>
>Confirmar ou reverter
>
>Ciclo nº 2
>
>Funcionamento (leitura ou escrita)
>
>Confirmar ou reverter
>
>...
>
>Ciclo #N
>
>Funcionamento (leitura ou escrita)
>
>Confirmar ou reverter
>
>Finalização

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

## Inicialização

Durante a fase de inicialização, todas as conexões necessárias (conexão com um banco de dados, serviço de email e assim por diante) são criadas. Eles também são verificados se cada módulo é capaz de executar as operações desejadas.

## Ciclos

Cada ciclo representa uma unidade de trabalho indissociável composta por uma série de operações. É possível definir o número máximo de ciclos no [!UICONTROL configurações de cenário] painel. O número padrão é 1.

Para obter mais informações, consulte [O painel de configurações de cenário em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-settings-panel.md).

## Operação

Durante a operação de leitura e/ou escrita da fase de operação:

* A operação de leitura consiste em obter dados de um serviço que é processado por outros módulos de acordo com um cenário predefinido. Por exemplo, a variável [!UICONTROL Dropbox] >[!UICONTROL Assistir arquivos] O módulo retorna novos pacotes (arquivos) criados desde a última execução do cenário.
* A operação de escrita consiste em enviar dados para um determinado serviço para processamento posterior. Por exemplo, a variável [!DNL Dropbox] >[!UICONTROL Carregar um arquivo] o módulo faz upload de um arquivo para um [!DNL Dropbox] pasta.

## Confirmar

Se a fase de operação for bem-sucedida para todos os módulos, a fase de confirmação começará durante a qual todas as operações executadas pelos módulos serão confirmadas. Isso significa que [!DNL Workfront Fusion] O envia informações para todos os serviços envolvidos na fase de operação sobre o seu sucesso.

## Reversão

Se ocorrer um erro durante a operação ou a fase de confirmação em qualquer módulo, a fase será abortada e a fase de reversão será iniciada, tornando todas as operações durante o ciclo especificado nulas. Alguns módulos não oferecem suporte para reversão e as operações executadas por esses módulos não podem ser retornadas. Para obter mais informações, consulte [Módulos ACID](#acid-modules) seção.

## Finalização

Durante a fase de finalização, as conexões abertas (por exemplo, conexões FTP, conexões de banco de dados e assim por diante) são fechadas e o cenário é concluído.

## Módulos ACID

Todos [!DNL Workfront Fusion] os módulos que oferecem suporte para reversão (também conhecidos como transaccionalidade) são marcados com a tag ACID.

![](assets/acid-modules-350x189.png)

Os módulos não marcados com essa tag não podem ser revertidos para seu estado inicial quando ocorrerem erros em outros módulos. Um exemplo típico de um módulo não ACID é o [!UICONTROL Email] >[!UICONTROL Enviar um email] ação. Depois que o email é enviado, não é possível desfazer o envio.
