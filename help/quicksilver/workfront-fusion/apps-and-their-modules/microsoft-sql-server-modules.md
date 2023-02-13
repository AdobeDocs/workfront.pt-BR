---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: conector
navigation-topic: apps-and-their-modules
title: Módulos do Microsoft SQL Server
description: Você pode usar [!DNL Adobe Workfront Fusion] para se conectar ao Microsoft SQL Server.
author: Becky
feature: Workfront Fusion
exl-id: d79cf00d-a81e-4d88-ac4a-f80b7b5a92b3
source-git-commit: c57a796ccbfb36bce58d49345e7515dd524604c5
workflow-type: tm+mt
source-wordcount: '343'
ht-degree: 0%

---

# [!DNL Microsoft SQL Server] módulos

Você pode usar [!DNL Adobe Workfront Fusion] para se conectar a [!UICONTROL Microsoft SQL Server].

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] para automação e integração de trabalho] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produto</td> 
   <td>Sua organização deve comprar [!DNL Adobe Workfront Fusion] bem como [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo.</td> 
  </tr> 
 </tbody> 
</table>

Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com seu [!DNL Workfront] administrador.

Para obter informações sobre [!DNL Adobe Workfront Fusion] licenças, consulte [[!DNL Adobe Workfront Fusion] licenças](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Usando [!DNL Microsoft SQL Server] módulos

Você pode executar sua lógica personalizada diretamente no servidor do banco de dados por meio de procedimentos armazenados. [!DNL Adobe Workfront Fusion] carrega a interface dos parâmetros de entrada/saída e do conjunto de registros dinamicamente para que cada parâmetro ou valor possa ser mapeado individualmente. Antes de começar a configurar seu cenário, verifique se a conta usada para se conectar ao banco de dados tem acesso de leitura ao `INFORMATION_SCHEMA.ROUTINES` e `INFORMATION_SCHEMA.PARAMETERS` exibições.

When [!DNL Fusion] estabelece a conexão com o [!DNL SQL server] destino, o [!DNL Fusion] O usuário identifica o Host (o nome de domínio ou endereço IP onde o servidor está hospedado) e a porta. [!DNL Fusion] pode se conectar a qualquer host e porta disponíveis.

Para obter informações sobre endereços IP específicos usados por [!DNL Workfront Fusion], consulte [Endereços IP para acessar [!DNL Adobe Workfront Fusion]](../../workfront-fusion/get-started/ip-addresses-for-fusion.md)

Para saber mais sobre como criar um procedimento armazenado, consulte [!DNL Microsoft SQL Server] documentação.

>[!NOTE]
>
>[!DNL Workfront Fusion] não suporta múltiplos conjuntos de registros. Somente o primeiro é processado.

## Erro de solução de problemas [!UICONTROL ER_LOCK_WAIT_TIMEOUT: Tempo limite de espera de bloqueio excedido; tentar reiniciar transação]

Esse erro ocorre ao modificar os mesmos dados usando vários módulos. É causado por transações SQL.

Quando qualquer módulo SQL é executado, ele inicia uma transação. A transação é concluída após a execução completa do cenário.

Se outro módulo tentar acessar os mesmos dados, ele deverá aguardar até que a transação anterior seja concluída. Como a primeira transação será concluída após a conclusão do cenário, a segunda transação nunca poderá começar.

### Solução:

Ativar Confirmação automática. A confirmação automática conclui (confirma) cada transação imediatamente após a execução do módulo ser feita.

1. Clique no botão [!UICONTROL Configurações de cenário] ícone ![](assets/scenario-settings-icon.png)na parte inferior da tela.
1. Clique no botão **[!UICONTROL Confirmação automática]** caixa de seleção.
1. Clique em **[!UICONTROL OK]** para salvar as configurações do cenário.
