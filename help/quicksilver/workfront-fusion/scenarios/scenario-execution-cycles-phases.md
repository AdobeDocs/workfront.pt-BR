---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Execução de cenário, ciclos e fases em [!DNL Adobe Workfront Fusion]
description: Este artigo descreve os eventos que ocorrem enquanto uma [!DNL Adobe Workfront Fusion] o cenário está em execução, como inicialização, operações, confirmações e reversões.
author: Becky
feature: Workfront Fusion
exl-id: 5403f476-226d-4268-affc-8e06b1117684
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '550'
ht-degree: 1%

---

# Execução de cenário, ciclos e fases em [!DNL Adobe Workfront Fusion]

[!DNL Adobe Workfront Fusion] é um sistema transacional, semelhante aos bancos de dados relacionais. Cada execução de cenário começa com a fase de inicialização, continua com pelo menos um ciclo composto pelas fases de operação e confirmação/reversão e termina com a fase de finalização:

>[!INFO]
>
>**Exemplo**
>
>Inicialização
>
>Ciclo #1
>
>Operação (leitura ou gravação)
>
>Confirmar ou reverter
>
>Ciclo #2
>
>Operação (leitura ou gravação)
>
>Confirmar ou reverter
>
>..
>
>Ciclo #N
>
>Operação (leitura ou gravação)
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
   <td role="rowheader">Licença [!UICONTROL Adobe Workfront Fusion]**</td> 
  <td>
   <p>Requisito de licença atual: Não [!DNL Workfront Fusion] requisito de licença.</p>
   <p>Ou</p>
   <p>Requisito de licença herdada: [!UICONTROL [!DNL Workfront Fusion] para Automação e Integração do Trabalho], [!UICONTROL [!DNL Workfront Fusion] para automação de trabalho]</p>
   </td>  
  </tr> 
  <tr> 
   <td role="rowheader">Produto</td> 
   <td>
   <p>Requisito atual do produto: se você tiver o [!UICONTROL Select] ou o [!UICONTROL Prime] [!DNL Adobe Workfront] Planejar, sua organização deve comprar [!DNL Adobe Workfront Fusion] bem como [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo. [!DNL Workfront Fusion] está incluído no [!UICONTROL Ultimate] [!DNL Workfront] plano.</p>
   <p>Ou</p>
   <p>Requisito de produto herdado: sua organização deve comprar [!DNL Adobe Workfront Fusion] bem como [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Para descobrir que plano, tipo de licença ou acesso você tem, entre em contato com o [!DNL Workfront] administrador.

Para obter informações sobre [!DNL Adobe Workfront Fusion] licenças, consulte [[!DNL Adobe Workfront Fusion] licenças](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Inicialização

Durante a fase de inicialização, todas as conexões necessárias (conexão com um banco de dados, serviço de email e assim por diante) são criadas. Elas também são verificadas se cada módulo é capaz de executar as operações desejadas.

## Ciclos

Cada ciclo representa uma unidade indivisível de trabalho composta por uma série de operações. É possível definir o número máximo de ciclos no [!UICONTROL configurações de cenário] painel. O número padrão é 1.

Para obter mais informações, consulte [O painel de configurações do cenário no [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-settings-panel.md).

## Operação

Durante a fase de operação, a operação de leitura e/ou gravação é realizada:

* A operação de leitura consiste em obter dados de um serviço que é processado por outros módulos de acordo com um cenário predefinido. Por exemplo, a variável [!UICONTROL Dropbox] >[!UICONTROL Observar arquivos] O módulo retorna novos pacotes (arquivos) criados desde a última execução do cenário.
* A operação de gravação consiste em enviar dados para um determinado serviço para processamento adicional. Por exemplo, a variável [!DNL Dropbox] >[!UICONTROL Carregar um arquivo] O módulo carrega um arquivo em um [!DNL Dropbox] pasta.

## Confirmar

Se a fase de operação for bem-sucedida para todos os módulos, a fase de confirmação começará durante a qual todas as operações executadas pelos módulos serão confirmadas. Isso significa que [!DNL Workfront Fusion] envia informações sobre o sucesso para todos os serviços envolvidos na fase de operação.

## Reversão

Se ocorrer um erro durante a operação ou a fase de confirmação em qualquer módulo, a fase será abortada e a fase de reversão será iniciada, anulando todas as operações durante o ciclo fornecido. Alguns módulos não são compatíveis com a reversão e as operações executadas por esses módulos não podem ser retomadas. Para obter mais informações, consulte a [Módulos ACID](#acid-modules) seção.

## Finalização

Durante a fase de finalização, as conexões abertas (por exemplo, conexões FTP, conexões de banco de dados e assim por diante) são fechadas e o cenário é concluído.

## Módulos ACID

Todos [!DNL Workfront Fusion] Os módulos que oferecem suporte à reversão (também conhecidos como transacionalidade) são marcados com a tag ACID.

![](assets/acid-modules-350x189.png)

Os módulos não marcados com essa tag não podem ser revertidos para seu estado inicial quando ocorrem erros em outros módulos. Um exemplo típico de um módulo não-ACID é o [!UICONTROL E-mail] >[!UICONTROL Enviar um e-mail] ação. Depois que o email é enviado, não é possível desfazer o envio.
