---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Módulos JWT
description: A variável [!DNL Adobe Workfront Fusion] [!UICONTROL JWT] O aplicativo fornece um módulo que cria tokens JWT com base no algoritmo fornecido.
author: Becky
feature: Workfront Fusion
source-git-commit: 121aef2ee55597fee2e2adc8250dd0651ea86f17
workflow-type: tm+mt
source-wordcount: '533'
ht-degree: 0%

---

# [!UICONTROL JWT] módulo

A variável [!DNL Adobe Workfront Fusion] [!UICONTROL JWT] O aplicativo fornece um módulo que cria tokens JWT com base no algoritmo fornecido.

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

## Módulo JWT e seus campos

### Gerar JWT

Esse módulo gera um JWT com base no algoritmo selecionado.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Algoritmo]</td> 
   <td> <p>Selecione o algoritmo com o qual deseja gerar o JWT.</p> <ul>
   <li><b>HS256</b>: HMAC usando algoritmo de hash SHA-256</li>
   <li><b>HS384</b>: HMAC usando algoritmo de hash SHA-384</li>
   <li><b>HS512</b>: HMAC usando algoritmo de hash SHA-512</li>
   <li><b>RS256</b>: RSASSA-PKCS1-v1_5 usando o algoritmo de hash SHA-256</li>
   <li><b>RS384</b>: RSASSA-PKCS1-v1_5 usando o algoritmo de hash SHA-384</li>
   <li><b>RS512</b>: RSASSA-PKCS1-v1_5 usando o algoritmo de hash SHA-512</li>
   <li><b>PS256</b>: RSASSA-PSS usando algoritmo de hash SHA-256 (somente Nó ^6.12.0 OU &gt;=8.0.0)</li>
   <li><b>PS384</b>: RSASSA-PSS usando algoritmo de hash SHA-384 (somente Nó ^6.12.0 OU &gt;=8.0.0)</li>
   <li><b>PS512</b>: RSASSA-PSS usando algoritmo de hash SHA-512 (somente Nó ^6.12.0 OU &gt;=8.0.0)</li>
   <li><b>ES256</b>: ECDSA usando curva P-256 e algoritmo de hash SHA-256</li>
   <li><b>ES384</b>: ECDSA usando curva P-384 e algoritmo de hash SHA-384</li>
   <li><b>ES512</b>: ECDSA usando curva P-521 e algoritmo de hash SHA-512</li>
   </ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Carga] </td> 
   <td> <p>Para cada item de carga útil que deseja adicionar, clique em <b>Adicionar item</b> e insira a chave e o valor do item.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Opções] </td> 
   <td> <p>Para cada item de opção que você deseja adicionar, clique em <b>Adicionar item</b> e insira a chave e o valor do item.</p> <p>As seguintes chaves estão disponíveis:
   <ul>
   <li><b>algoritmo</b>: (padrão: RS256)</li>
   <li><b>expiresIn</b>: expresso em segundos ou uma string que descreve um intervalo de tempo (por exemplo, 2 dias, 10h, 7d). Um valor numérico é interpretado como uma contagem de segundos. Se você usar uma sequência de caracteres, forneça as unidades de tempo (dias, horas etc.); caso contrário, a unidade de milissegundos será usada por padrão (120 é igual a 120 ms).</li>
   <li><b>notBefore</b>: expresso em segundos ou uma string que descreve um intervalo de tempo (por exemplo, 2 dias, 10h, 7d). Um valor numérico é interpretado como uma contagem de segundos. Se você usar uma sequência de caracteres, forneça as unidades de tempo (dias, horas etc.); caso contrário, a unidade de milissegundos será usada por padrão (120 é igual a 120 ms).
</li>
   <li><b>público</b></li>
   <li><b>emissor</b></li>
   <li><b>jwtid</b></li>
   <li><b>assunto</b></li>
   <li><b>noTimestamp</b></li>
   <li><b>cabeçalho</b></li>
   <li><b>keyid</b></li>
   <li><b>mutatePayload</b>: Se <code>true</code>, a função sign modificará diretamente o objeto payload. Isso é útil se você precisar de uma referência bruta à carga após a aplicação das declarações a ela, mas antes de ela ser codificada em um token.</li>
   <li><b>allowInsecureKeySizes</b>: Se <code>true</code>, permite que chaves privadas com um módulo abaixo de 2048 sejam usadas para RSA.</li>
   <li><b>allowInvalidAsymmetricKeyTypes</b>: Se <code>true</code>, permite chaves assimétricas que não correspondem ao algoritmo especificado. Essa opção destina-se apenas à compatibilidade com versões anteriores e deve ser evitada.</li>
   </ul>
   </td> 
  </tr> 
 </tbody> 
</table>


