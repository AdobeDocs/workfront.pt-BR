---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: conector
navigation-topic: apps-and-their-modules
title: Módulos do Microsoft SQL Server
description: Você pode usar o  [!DNL Adobe Workfront Fusion] para se conectar ao Microsoft SQL Server.
author: Becky
feature: Workfront Fusion
exl-id: d79cf00d-a81e-4d88-ac4a-f80b7b5a92b3
source-git-commit: 7d5f7c21fe38d43fb5601c81b8a31cc80587848f
workflow-type: tm+mt
source-wordcount: '502'
ht-degree: 0%

---

# [!DNL Microsoft SQL Server] módulos

Você pode usar o [!DNL Adobe Workfront Fusion] para se conectar ao [!UICONTROL Microsoft SQL Server].

## Requisitos de acesso

Você deve ter o seguinte acesso para usar a funcionalidade neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plano*</td>
  <td> <p>[!UICONTROL Pro] ou superior</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licença*</td>
   <td> <p>[!UICONTROL Plano], [!UICONTROL Trabalho]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licença**</td> 
   <td>
   <p>Requisito de licença atual: nenhum requisito de licença [!DNL Workfront Fusion].</p>
   <p>Ou</p>
   <p>Requisito de licença herdada: [!UICONTROL [!DNL Workfront Fusion] para Automação e Integração do Trabalho] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produto</td> 
   <td>
   <p>Requisito atual do produto: se você tiver o Plano [!DNL Adobe Workfront] da [!UICONTROL Select] ou da [!UICONTROL Prime], sua organização deve comprar o [!DNL Adobe Workfront Fusion] e o [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo. [!DNL Workfront Fusion] está incluído no plano [!DNL Workfront] do [!UICONTROL Ultimate].</p>
   <p>Ou</p>
   <p>Requisito de produto herdado: sua organização deve comprar o [!DNL Adobe Workfront Fusion] e o [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Para saber que plano, tipo de licença ou acesso você tem, contate o administrador do [!DNL Workfront].

Para obter informações sobre [!DNL Adobe Workfront Fusion] licenças, consulte [[!DNL Adobe Workfront Fusion] licenças](../../workfront-fusion/get-started/license-automation-vs-integration.md).



## Conectando o serviço [!DNL Microsoft SQL Server] a [!DNL Workfront Fusion]

Para obter instruções sobre como conectar sua conta do [!DNL Microsoft SQL Server] ao [!UICONTROL Workfront Fusion], consulte [Criar uma conexão com o [!UICONTROL Adobe Workfront Fusion] - Instruções básicas](../../workfront-fusion/connections/connect-to-fusion-general.md)

>[!NOTE]
>
>Alguns aplicativos do Microsoft usam a mesma conexão, que está vinculada a permissões de usuário individuais. Portanto, ao criar uma conexão, a tela de consentimento de permissões exibe todas as permissões que foram concedidas anteriormente à conexão deste usuário, além de todas as novas permissões necessárias para o aplicativo atual.
>
>Por exemplo, se um usuário tiver permissões de &quot;Tabela de leitura&quot; concedidas por meio do conector do Excel e criar uma conexão no conector do Outlook para ler emails, a tela de consentimento de permissões mostrará a permissão &quot;Tabela de leitura&quot; já concedida e a permissão &quot;Gravar email&quot; recém-necessária.

## Usando módulos [!DNL Microsoft SQL Server]

Você pode executar a lógica personalizada diretamente no servidor de banco de dados por meio de procedimentos armazenados. [!DNL Adobe Workfront Fusion] carrega a interface de parâmetros de entrada/saída e o conjunto de registros dinamicamente de modo que cada parâmetro ou valor possa ser mapeado individualmente. Antes de começar a configurar seu cenário, verifique se a conta que você está usando para se conectar ao banco de dados tem acesso de leitura às visualizações `INFORMATION_SCHEMA.ROUTINES` e `INFORMATION_SCHEMA.PARAMETERS`.

Quando [!DNL Fusion] estabelece a conexão com o destino [!DNL SQL server], o usuário [!DNL Fusion] identifica o Host (o nome de domínio ou endereço IP onde o servidor está hospedado) e a porta. O [!DNL Fusion] pode se conectar a qualquer host e porta disponíveis.

Para obter informações sobre endereços IP específicos usados por [!DNL Workfront Fusion], consulte [Endereços IP para acessar [!DNL Adobe Workfront Fusion]](../../workfront-fusion/get-started/ip-addresses-for-fusion.md)

Para saber mais sobre como criar um procedimento armazenado, consulte a documentação do [!DNL Microsoft SQL Server].

>[!NOTE]
>
>[!DNL Workfront Fusion] não dá suporte a vários conjuntos de registros. Somente o primeiro é processado.

## Solução de problemas de erro [!UICONTROL ER_LOCK_WAIT_TIMEOUT: Tempo limite de espera de bloqueio excedido; tente reiniciar a transação]

Esse erro ocorre quando você modifica os mesmos dados usando vários módulos. É causado por transações SQL.

Quando qualquer módulo SQL é executado, ele inicia uma transação. A transação é concluída após a execução completa do cenário.

Se outro módulo tentar acessar os mesmos dados, ele precisará aguardar até que a transação anterior seja concluída. Como a primeira transação será concluída após a conclusão do cenário, a segunda transação nunca poderá começar.

### Solução:

Ative a Confirmação automática. A confirmação automática conclui (confirma) cada transação imediatamente após a execução do módulo ser concluída.

1. Clique no ícone ![](assets/scenario-settings-icon.png)Configurações de cenário[!UICONTROL na parte inferior da tela.]
1. Clique na caixa de seleção **[!UICONTROL Confirmação automática]**.
1. Clique em **[!UICONTROL OK]** para salvar as configurações do cenário.
