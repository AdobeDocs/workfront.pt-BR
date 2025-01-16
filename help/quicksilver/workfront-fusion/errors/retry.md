---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
title: Repetir tratamento de erros em  [!DNL Adobe Workfront Fusion]
description: A documentação do Adobe Workfront Fusion foi movida para um novo local. Este artigo foi descontinuado, mas contém um link para o novo artigo que aborda essa funcionalidade.
author: Becky
feature: Workfront Fusion
exl-id: 1058905c-6c95-4a8c-8956-e1606f1486d9
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '727'
ht-degree: 0%

---

# Repetir tratamento de erros em [!DNL Adobe Workfront Fusion]

>[!IMPORTANT]
>
>A documentação do Adobe Workfront Fusion foi movida para um novo local.
>
>As informações neste artigo agora podem ser encontradas no artigo:
>
>* [Configurar solução alternativa de tratamento de erros `retry`](https://experienceleague.adobe.com/docs/workfront-fusion/using/create-scenarios/configure-error-handling/retry.html)
>
>Atualize todos os marcadores.
>
>Este artigo não está mais sendo atualizado e será removido em breve.

Em alguns casos, é útil executar novamente um módulo com falha se houver uma chance de o motivo da falha passar do tempo.

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
   <p>Requisito de licença herdada: [!UICONTROL [!DNL Workfront Fusion] para Automação e Integração do Trabalho] </p>
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

## Soluções alternativas para a diretiva de manipulação de erros [!UICONTROL Repetir]

Atualmente, o [!UICONTROL Adobe Workfront Fusion] não oferece a diretiva de manipulação de erros [!UICONTROL Retry], embora duas soluções alternativas possam ser empregadas para simular sua funcionalidade. Para obter mais informações, consulte [Diretivas para tratamento de erros no Adobe Workfront Fusion](../../workfront-fusion/errors/directives-for-error-handling.md).

### Usar a diretiva [!UICONTROL Break]

1. No painel de configurações do cenário, habilite a opção **[!UICONTROL Permitir o armazenamento de Execuções Incompletas]**.

   Para obter mais informações, consulte [O painel de configurações de cenário em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-settings-panel.md).

1. Anexe uma rota de manipulador de erros ao módulo, conforme descrito em [Tratamento de erros no [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-handling.md).
1. Vincule a diretiva [!UICONTROL Break] à rota do manipulador de erros e configure-a.

   Para obter mais informações, consulte [Diretivas para manipulação de erros no [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/errors/directives-for-error-handling.md).

   ![](assets/break-directive-350x241.png)

#### Desvantagens

* O intervalo mínimo de novas tentativas é de um minuto.
* Se o módulo estiver processando vários pacotes e o processamento de um pacote falhar, a execução parcial (somente o pacote que causou o erro) será movida para a pasta de execuções incompletas e agendada para novas tentativas de acordo com as configurações da diretiva [!UICONTROL Break]. No entanto, a execução atual continua e o módulo continua a processar os pacotes subsequentes. Você pode habilitar a opção &quot;[!UICONTROL Processamento sequencial]&quot; nas [!UICONTROL Configurações de cenário] para impedir que o cenário seja executado novamente até que a execução armazenada na pasta Execuções incompletas seja resolvida com êxito.

  Para obter mais informações sobre execuções incompletas, consulte [Exibir e resolver execuções incompletas em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md).

### Usar o módulo [!UICONTROL Repetidor]

1. Empregue o módulo **[!UICONTROL Repetidor]** e defina seu campo **[!UICONTROL Repetições]** para o número máximo de tentativas.
1. Vincule o módulo com falha potencial ao módulo **[!UICONTROL Repetidor]**.
1. Anexe uma rota de manipulador de erros a este módulo (consulte [Tratamento de erros em [!DNL Adobe Workfront Fusio]n](../../workfront-fusion/errors/error-handling.md)).
1. Vincule o módulo **[!UICONTROL Tools] > [!UICONTROL Sleep]** à rota do manipulador de erros e defina seu campo **[!UICONTROL Delay]** como o número de segundos entre as tentativas.

1. Vincule a diretiva **[!UICONTROL Ignore]** após o módulo **[!UICONTROL Tools] > [!UICONTROL Sleep]** (consulte [Diretivas para tratamento de erros no Adobe Workfront Fusion](../../workfront-fusion/errors/directives-for-error-handling.md)).

1. Vincule o módulo **[!UICONTROL Tools] > [!UICONTROL Set variable]** após o módulo com falha potencial e configure-o para armazenar o resultado do módulo em uma variável nomeada, por exemplo, `Result`.

1. Vincule o módulo **[!UICONTROL Array aggregator]** após **[!UICONTROL Tools] > [!UICONTROL Set variable]** e escolha o módulo **[!DNL Repeater]** em seu campo Módulo do Source.

1. Vincule o módulo **[!UICONTROL Tools] > [!UICONTROL Get variable]** ao módulo **[!UICONTROL Array aggregator]** e configure-o para obter o valor da variável `Result`.

1. Insira o módulo **[!UICONTROL Tools] > [!UICONTROL Get variable]** entre o módulo **[!UICONTROL Repeater]** e o módulo com falha potencial, e configure-o para obter o valor da variável `Result`.

1. Insira um filtro entre este módulo **[!UICONTROL Ferramentas] > [!UICONTROL Obter variável]** e o módulo com falha potencial para continuar somente se a variável `Result` não existir.

>[!INFO]
>
>**Exemplo:** Aqui está uma amostra de cenário em que o módulo [!UICONTROL HTTP] >[!UICONTROL Fazer uma solicitação] representa o módulo com falha potencial:
>
>![](assets/http-make-request-350x116.png)
>
>Se o resultado do módulo com falha potencial for muito complexo para ser armazenado em uma variável simples, você poderá empregar um armazenamento de dados para armazenar/recuperar o resultado. O armazenamento de dados conteria apenas um registro. A chave do registro pode ser, por exemplo, `Result`.
>
>Para obter mais informações sobre armazenamentos de dados, consulte [Armazenamentos de Dados em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/data-stores.md)

#### Drawback

Essa solução alternativa pode parecer um pouco complexa demais e também é mais exigente em termos de operações.
