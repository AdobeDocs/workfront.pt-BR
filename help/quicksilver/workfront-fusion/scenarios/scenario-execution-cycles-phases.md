---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Execução de cenário, ciclos e fases em  [!DNL Adobe Workfront Fusion]
description: A documentação do Adobe Workfront Fusion foi movida para um novo local. Este artigo foi descontinuado, mas contém um link para o novo artigo que aborda essa funcionalidade.
author: Becky
feature: Workfront Fusion
exl-id: 5403f476-226d-4268-affc-8e06b1117684
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '611'
ht-degree: 0%

---

# Execução de cenário, ciclos e fases em [!DNL Adobe Workfront Fusion]

>[!IMPORTANT]
>
>A documentação do Adobe Workfront Fusion foi movida para um novo local.
>
>As informações neste artigo agora podem ser encontradas no artigo:
>
>* [Execução do cenário, ciclos e fases](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/scenarios/scenario-execution-cycles-phases.html)
>
>Atualize todos os marcadores.
>
>Este artigo não está mais sendo atualizado e será removido em breve.

[!DNL Adobe Workfront Fusion] é um sistema transacional, semelhante a bancos de dados relacionais. Cada execução de cenário começa com a fase de inicialização, continua com pelo menos um ciclo composto pelas fases de operação e confirmação/reversão e termina com a fase de finalização:

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
   <p>Requisito de licença atual: nenhum requisito de licença [!DNL Workfront Fusion].</p>
   <p>Ou</p>
   <p>Requisito de licença herdada: [!UICONTROL [!DNL Workfront Fusion] para Automação e Integração do Trabalho], [!UICONTROL [!DNL Workfront Fusion] para Automação do Trabalho]</p>
   </td>  
  </tr> 
  <tr> 
   <td role="rowheader">Produto</td> 
   <td>
   <p>Requisito atual do produto: se você tiver o Plano [!DNL Adobe Workfront] da [!UICONTROL Select] ou da [!UICONTROL Prime], sua organização deve comprar o [!DNL Adobe Workfront Fusion] e o [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo. [!DNL Workfront Fusion] está incluído no plano [!DNL Workfront] da [!UICONTROL Ultimate].</p>
   <p>Ou</p>
   <p>Requisito de produto herdado: sua organização deve comprar o [!DNL Adobe Workfront Fusion] e o [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Para saber que plano, tipo de licença ou acesso você tem, contate o administrador do [!DNL Workfront].

Para obter informações sobre [!DNL Adobe Workfront Fusion] licenças, consulte [[!DNL Adobe Workfront Fusion] licenças](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Inicialização

Durante a fase de inicialização, todas as conexões necessárias (conexão com um banco de dados, serviço de email e assim por diante) são criadas. Elas também são verificadas se cada módulo é capaz de executar as operações desejadas.

## Ciclos

Cada ciclo representa uma unidade indivisível de trabalho composta por uma série de operações. É possível definir o número máximo de ciclos no painel [!UICONTROL configurações de cenário]. O número padrão é 1.

Para obter mais informações, consulte [O painel de configurações de cenário em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-settings-panel.md).

## Operação

Durante a fase de operação, a operação de leitura e/ou gravação é realizada:

* A operação de leitura consiste em obter dados de um serviço que é processado por outros módulos de acordo com um cenário predefinido. Por exemplo, o módulo [!UICONTROL Dropbox] >[!UICONTROL Watch files] retorna novos pacotes (arquivos) criados desde a última execução do cenário.
* A operação de gravação consiste em enviar dados para um determinado serviço para processamento adicional. Por exemplo, o módulo [!DNL Dropbox] >[!UICONTROL Carregar um arquivo] carrega um arquivo para uma pasta [!DNL Dropbox].

## Confirmar

Se a fase de operação for bem-sucedida para todos os módulos, a fase de confirmação começará durante a qual todas as operações executadas pelos módulos serão confirmadas. Isso significa que o [!DNL Workfront Fusion] envia informações sobre seu êxito para todos os serviços envolvidos na fase de operação.

## Reversão

Se ocorrer um erro durante a operação ou a fase de confirmação em qualquer módulo, a fase será abortada e a fase de reversão será iniciada, anulando todas as operações durante o ciclo fornecido. Alguns módulos não são compatíveis com a reversão e as operações executadas por esses módulos não podem ser retomadas. Para obter mais informações, consulte a seção [módulos ACID](#acid-modules).

## Finalização

Durante a fase de finalização, as conexões abertas (por exemplo, conexões FTP, conexões de banco de dados e assim por diante) são fechadas e o cenário é concluído.

## Módulos ACID

Todos os [!DNL Workfront Fusion] módulos que oferecem suporte à reversão (também conhecidos como transacionalidade) são marcados com a marca ACID.

![](assets/acid-modules-350x189.png)

Os módulos não marcados com essa tag não podem ser revertidos para seu estado inicial quando ocorrem erros em outros módulos. Um exemplo típico de um módulo não ACID é a ação [!UICONTROL Email] >[!UICONTROL Enviar um Email]. Depois que o email é enviado, não é possível desfazer o envio.
