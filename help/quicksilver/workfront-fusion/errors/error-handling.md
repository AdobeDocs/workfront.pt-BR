---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
title: Tratamento de erros em [!DNL Adobe Workfront Fusion]
description: Quando ocorrem erros durante a execução de um cenário, geralmente ocorre porque um serviço não está disponível devido a uma falha, um serviço responde com dados inesperados ou a validação de dados de entrada falha.
author: Becky
feature: Workfront Fusion
exl-id: a08c18a0-1797-4126-827a-1ea7e11d4bad
source-git-commit: 97f91d663df86341a079894cff04d07c18b7bf08
workflow-type: tm+mt
source-wordcount: '604'
ht-degree: 0%

---

# Tratamento de erros em [!DNL Adobe Workfront Fusion]

Quando ocorrem erros durante a execução de um cenário, geralmente ocorre porque um serviço não está disponível devido a uma falha, um serviço responde com dados inesperados ou a validação de dados de entrada falha.

>[!NOTE]
>
>Se um módulo gerar um erro durante a execução do cenário e não houver uma rota de tratamento de erros anexada ao módulo, uma lógica de tratamento de erros padrão será executada conforme descrito em [Processamento de erros no [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-processing.md).

Ao adicionar uma rota do manipulador de erros a um módulo, você pode substituir a lógica padrão de tratamento de erros pela sua. [!DNL Adobe Workfront Fusion] O oferece 5 diretivas diferentes, qualquer uma delas pode ser inserida no final de suas rotas do manipulador de erros. Para obter mais informações, consulte [Diretivas relativas ao tratamento de erros [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/directives-for-error-handling.md).

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

## Rota do manipulador de erros

Para adicionar uma rota do manipulador de erros a um módulo (vamos chamá-lo de Módulo X), clique com o botão direito do mouse no módulo e selecione **[!UICONTROL Adicionar manipulador de erros]**:

![](assets/error-handler-route.png)

O módulo mostra uma lista de Diretivas, bem como os aplicativos que estão sendo usados em seu cenário. Se o Módulo X for o último módulo em sua rota, será necessário escolher uma das diretivas. Ou você pode adicionar um ou mais módulos à sua rota. Nesse caso, a variável [!UICONTROL Ignorar] A diretiva é aplicada por padrão ao Módulo X e, em caso de erro, os módulos subsequentes nessa rota são processados.

![](assets/directives-350x426.png)

Como você pode ver abaixo, se ocorrer um erro ao executar o [!UICONTROL Criar uma pasta] , o [!UICONTROL Ignorar] a diretiva será aplicada automaticamente e o cenário será movido para o próximo módulo na rota do manipulador de erros se o filtro &quot;Erro de dados ocorre&quot; retornar um ou mais pacotes.

No entanto, se não houver erro, o cenário será movido para a variável [!UICONTROL Listar todos os arquivos em um módulo de pasta] na rota regular.

![](assets/if-there-is-no-error-350x234.png)

Além disso, para diferenciar uma rota do manipulador de erros de uma rota regular, a primeira é composta de círculos transparentes, como mostrado acima.

## Diretivas de tratamento de erros

As diretivas são brevemente explicadas a seguir. Para obter mais informações, consulte [Diretivas relativas ao tratamento de erros [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/directives-for-error-handling.md).

Há um total de cinco diretivas que podem ser agrupadas nas seguintes categorias com base em se uma execução de cenário deve continuar ou não:

As diretivas a seguir garantem que a execução de um cenário continue:

* **[!UICONTROL Retomar]** permite especificar uma saída substituta para o módulo com o erro e o status de execução do cenário é marcado como bem-sucedido
* **[!UICONTROL Ignorar]** simplesmente ignora o erro e o status de execução do cenário é marcado como bem-sucedido
* **[!UICONTROL Quebra]** armazena a entrada na fila de execuções incompletas e o status de execução do cenário é marcado como aviso. Para obter mais informações, consulte [Exibir e resolver execuções incompletas em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md).

Por outro lado, se uma execução de cenário deve ser interrompida, você deve usar uma das seguintes diretivas:

* **[!UICONTROL Reversão]** interrompe a execução do cenário imediatamente e marca seu status como erro
* **[!UICONTROL Confirmar]** interrompe a execução do cenário imediatamente e marca seu status como sucesso

## Recursos adicionais

* [Diretivas relativas ao tratamento de erros [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/directives-for-error-handling.md)
* [Tratamento de erros avançado em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/advanced-error-handling.md) (inclui a configuração do Cenário de Dropbox referenciado acima)
