---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
title: Tentar tratamento de erros novamente em [!DNL Adobe Workfront Fusion]
description: Em alguns casos, é útil executar novamente um módulo com falha por algumas vezes, se houver uma chance de que o motivo da falha possa passar ao longo do tempo.
author: Becky
feature: Workfront Fusion
exl-id: 1058905c-6c95-4a8c-8956-e1606f1486d9
source-git-commit: 184033c8957e955b3011f7e0845a73029f6b7aba
workflow-type: tm+mt
source-wordcount: '639'
ht-degree: 0%

---

# Tentar tratamento de erros novamente em [!DNL Adobe Workfront Fusion]

Em alguns casos, é útil executar novamente um módulo com falha se houver uma chance de o motivo da falha poder passar ao longo do tempo.

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] para automação e integração de trabalho] </p><p>[!UICONTROL [!DNL Workfront Fusion] para Automação de Trabalho]</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produto</td> 
   <td>Sua organização deve comprar [!DNL Adobe Workfront Fusion] bem como [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo.</td> 
  </tr> 
 </tbody> 
</table>

Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com seu [!DNL Workfront] administrador.

Para obter informações sobre [!DNL Adobe Workfront Fusion] licenças, consulte [[!DNL Adobe Workfront Fusion] licenças](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Soluções alternativas para a [!UICONTROL Tentar novamente] diretiva de tratamento de erros

[!UICONTROL Adobe Workfront Fusion] atualmente não oferece a variável [!UICONTROL Tentar novamente] diretiva de tratamento de erros, embora duas soluções alternativas possam ser empregadas para imitar sua funcionalidade. Para obter mais informações, consulte [Diretivas para tratamento de erros no Adobe Workfront Fusion](../../workfront-fusion/errors/directives-for-error-handling.md).

### Use o [!UICONTROL Quebra] diretiva

1. No painel de configurações do cenário, ative a opção **[!UICONTROL Permitir armazenamento de execuções incompletas]** opção.

   Para obter mais informações, consulte [O painel de configurações de cenário em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-settings-panel.md).

1. Anexe uma rota do manipulador de erros ao módulo, conforme descrito em [Tratamento de erros em [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-handling.md).
1. Vincule o [!UICONTROL Quebra] diretiva para a rota do manipulador de erros e configure-a.

   Para obter mais informações, consulte [Diretivas relativas ao tratamento de erros [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/errors/directives-for-error-handling.md).

   ![](assets/break-directive-350x241.png)

#### Desvantagens

* O intervalo mínimo de tentativas é de um minuto.
* Se o módulo estiver processando vários pacotes e o processamento de um pacote falhar, a execução parcial (somente o pacote que causou o erro) será movida para a pasta de execuções incompletas e agendada para tentativas de acordo com o [!UICONTROL Quebra] configurações de diretiva. No entanto, a execução atual continua e o módulo continua a processar os pacotes subsequentes. Você pode ativar o &quot;[!UICONTROL Processamento sequencial]&quot; na [!UICONTROL Configurações de cenário] para impedir que o cenário seja executado novamente até que a execução armazenada na pasta Execuções incompletas seja resolvida com êxito.

   Para obter mais informações sobre execuções incompletas, consulte [Exibir e resolver execuções incompletas em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md).

### Use o [!UICONTROL Repetidor] módulo

1. Aplique o **[!UICONTROL Repetidor]** e defina seu **[!UICONTROL Repetir]** para o número máximo de tentativas.
1. Vincule o módulo que apresenta falha potencial ao **[!UICONTROL Repetidor]** módulo.
1. Anexe uma rota do manipulador de erros para este módulo (consulte [Tratamento de erros em [!DNL Adobe Workfront Fusio]n](../../workfront-fusion/errors/error-handling.md)).
1. Vincule o **[!UICONTROL Ferramentas] > [!UICONTROL Suspensão]** para a rota do manipulador de erros e defina seu **[!UICONTROL Atraso]** para o número de segundos entre as tentativas.

1. Vincule o **[!UICONTROL Ignorar]** após **[!UICONTROL Ferramentas] > [!UICONTROL Suspensão]** módulo (consulte [Diretivas para tratamento de erros no Adobe Workfront Fusion](../../workfront-fusion/errors/directives-for-error-handling.md)).

1. Vincule o **[!UICONTROL Ferramentas] > [!UICONTROL Definir variável]** após o módulo potencialmente com falha e configure-o para armazenar o resultado do módulo em uma variável nomeada, por exemplo, `Result`.

1. Vincule o **[!UICONTROL Agregador de matriz]** após a **[!UICONTROL Ferramentas] > [!UICONTROL Definir variável]** e escolha a **[!DNL Repeater]** em seu campo Módulo de origem .

1. Vincule o **[!UICONTROL Ferramentas] > [!UICONTROL Obter variável]** para **[!UICONTROL Agregador de matriz]** e configure-o para obter o valor da variável `Result` variável.

1. Insira o **[!UICONTROL Ferramentas] > [!UICONTROL Obter variável]** entre **[!UICONTROL Repetidor]** e o módulo com falha potencial e configure-o obtenha o valor da variável `Result` variável.

1. Inserir um filtro entre isto **[!UICONTROL Ferramentas] > [!UICONTROL Obter variável]** e o módulo que pode falhar para continuar somente se a variável `Result` não existe.

>[!INFO]
>
>**Exemplo:** Este é um exemplo de cenário no qual a variável [!UICONTROL HTTP] >[!UICONTROL Fazer uma solicitação] representa o módulo que possivelmente apresenta falha:
>
>![](assets/http-make-request-350x116.png)
>
>Se o resultado do módulo com falha potencial for muito complexo para ser armazenado em uma variável simples, você pode usar um armazenamento de dados para armazenar/recuperar o resultado. O armazenamento de dados conteria apenas um registro. A chave do registro pode ser, por exemplo, `Result`.
>
>Para obter mais informações sobre armazenamentos de dados, consulte [Armazenamento de dados em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/data-stores.md)

#### Desvantagens

Essa solução alternativa pode parecer um pouco complexa demais e também é mais exigente em termos de operações.
