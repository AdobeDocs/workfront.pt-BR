---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
title: Repetir tratamento de erros no [!DNL Adobe Workfront Fusion]
description: Em alguns casos, é útil reexecutar um módulo com falha por algumas vezes se houver uma chance de o motivo da falha passar do tempo.
author: Becky
feature: Workfront Fusion
exl-id: 1058905c-6c95-4a8c-8956-e1606f1486d9
source-git-commit: a3756f9345cbc9417a6fd110306dfa50aecc81a2
workflow-type: tm+mt
source-wordcount: '683'
ht-degree: 0%

---

# Repetir tratamento de erros no [!DNL Adobe Workfront Fusion]

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
   <p>Requisito de licença atual: Não [!DNL Workfront Fusion] requisito de licença.</p>
   <p>Ou</p>
   <p>Requisito de licença herdada: [!UICONTROL [!DNL Workfront Fusion] para Automação e integração do trabalho] </p>
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

## Soluções alternativas para o [!UICONTROL Tentar novamente] diretiva de tratamento de erros

[!UICONTROL Adobe Workfront Fusion] atualmente não oferece o [!UICONTROL Tentar novamente] diretiva de manipulação de erros, embora duas soluções alternativas possam ser empregadas para mimetizar sua funcionalidade. Para obter mais informações, consulte [Diretivas para tratamento de erros no Adobe Workfront Fusion](../../workfront-fusion/errors/directives-for-error-handling.md).

### Use o [!UICONTROL Interrupção] diretiva

1. No painel Configurações do cenário, ative a opção **[!UICONTROL Permitir armazenamento de execuções incompletas]** opção.

   Para obter mais informações, consulte [O painel de configurações do cenário no [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-settings-panel.md).

1. Anexe uma rota de manipulador de erros ao módulo, conforme descrito em [Tratamento de erros no [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-handling.md).
1. Vincule o [!UICONTROL Interrupção] à rota do manipulador de erros e a configure.

   Para obter mais informações, consulte [Diretivas para tratamento de erros no [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/errors/directives-for-error-handling.md).

   ![](assets/break-directive-350x241.png)

#### Desvantagens

* O intervalo mínimo de novas tentativas é de um minuto.
* Se o módulo estiver processando vários pacotes e o processamento de um pacote falhar, a execução parcial (somente o pacote que causou o erro) será movida para a pasta de execuções incompletas e agendada para novas tentativas de acordo com o [!UICONTROL Interrupção] configurações de diretiva. No entanto, a execução atual continua e o módulo continua a processar os pacotes subsequentes. Você pode ativar o &quot;[!UICONTROL Processamento sequencial]&quot; na caixa de diálogo [!UICONTROL Configurações de cenário] para impedir que o cenário seja executado novamente até que a execução armazenada na pasta Incomplete executions seja resolvida com sucesso.

  Para obter mais informações sobre execuções incompletas, consulte [Exibir e resolver execuções incompletas no [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md).

### Use o [!UICONTROL Repetidor] módulo

1. Empregue o **[!UICONTROL Repetidor]** módulo e defina seu **[!UICONTROL Repetições]** ao número máximo de tentativas.
1. Vincule o módulo com falha potencial ao **[!UICONTROL Repetidor]** módulo.
1. Anexe uma rota de manipulador de erros a este módulo (consulte [Tratamento de erros no [!DNL Adobe Workfront Fusio]n](../../workfront-fusion/errors/error-handling.md)).
1. Vincule o **[!UICONTROL Ferramentas] > [!UICONTROL Hibernar]** módulo à rota do manipulador de erros e defina sua **[!UICONTROL Atraso]** ao número de segundos entre as tentativas.

1. Vincule o **[!UICONTROL Ignorar]** diretiva após a **[!UICONTROL Ferramentas] > [!UICONTROL Hibernar]** módulo (consulte [Diretivas para tratamento de erros no Adobe Workfront Fusion](../../workfront-fusion/errors/directives-for-error-handling.md)).

1. Vincule o **[!UICONTROL Ferramentas] > [!UICONTROL Definir variável]** módulo após o módulo com falha potencial e configure-o para armazenar o resultado do módulo em uma variável chamada, por exemplo, `Result`.

1. Vincule o **[!UICONTROL Agregador de matrizes]** módulo após a variável **[!UICONTROL Ferramentas] > [!UICONTROL Definir variável]** e escolha o **[!DNL Repeater]** módulo em seu campo Módulo de origem.

1. Vincule o **[!UICONTROL Ferramentas] > [!UICONTROL Obter variável]** módulo para o **[!UICONTROL Agregador de matrizes]** módulo e configure-o para obter o valor do `Result` variável.

1. Insira o **[!UICONTROL Ferramentas] > [!UICONTROL Obter variável]** módulo entre a variável **[!UICONTROL Repetidor]** módulo e o módulo com falha potencial e configurá-lo obtenham o valor do `Result` variável.

1. Inserir um filtro entre isto **[!UICONTROL Ferramentas] > [!UICONTROL Obter variável]** módulo e o módulo com falha potencial continuarem apenas se o módulo `Result` não existe.

>[!INFO]
>
>**Exemplo:** Este é um exemplo de cenário em que a variável [!UICONTROL HTTP] >[!UICONTROL Fazer uma solicitação] O módulo representa o módulo com falha potencial:
>
>![](assets/http-make-request-350x116.png)
>
>Se o resultado do módulo com falha potencial for muito complexo para ser armazenado em uma variável simples, você poderá empregar um armazenamento de dados para armazenar/recuperar o resultado. O armazenamento de dados conteria apenas um registro. A chave do registro pode ser, por exemplo, `Result`.
>
>Para obter mais informações sobre armazenamentos de dados, consulte [Armazenamentos de dados no [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/data-stores.md)

#### Drawback

Essa solução alternativa pode parecer um pouco complexa demais e também é mais exigente em termos de operações.
