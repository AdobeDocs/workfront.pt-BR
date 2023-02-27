---
content-type: api
navigation-topic: api-navigation-topic
title: Caracteres extras em respostas da API
description: Caracteres extras em respostas da API
author: Becky
feature: Workfront API
exl-id: 1477b98e-1cdc-4661-b3ee-0b6ab1e8c3ee
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '202'
ht-degree: 8%

---

# Caracteres extras em respostas da API

A sintaxe de algumas respostas da API pode conter o caractere de escape, `\` (barra invertida). Um caractere de escape indica que o caractere ou a string de caracteres que imediatamente seguem o caractere de escape têm um valor especial. Por exemplo, `\t` informa o dispositivo de leitura que `t` deve ser interpretada como `tab` e não como a letra &quot;t&quot;. Uma sequência de caracteres de um ou mais caracteres após a barra invertida é chamada de sequência de escape.

As sequências hexadecimais escapadas exigem o uso de dígitos hexadecimais válidos. A tabela a seguir lista as sequências de escape que são codificadas nas respostas da API do Adobe Workfront:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Sequência de escape</strong> </th> 
   <th><strong>Caractere Unicode</strong> </th> 
   <th><strong>Representa</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>\u000<em>x</em></p> <p>Em que <em>x</em> é o código hexadecimal para os números 0 a 7</p> </td> 
   <td>0-7</td> 
   <td>Caracteres Unicode representados pelos pontos de código de 0 a 7</td> 
  </tr> 
  <tr> 
   <td>\b</td> 
   <td>8</td> 
   <td>Apagar</td> 
  </tr> 
  <tr> 
   <td>\t</td> 
   <td>9</td> 
   <td>Guia</td> 
  </tr> 
  <tr> 
   <td>\n</td> 
   <td>10</td> 
   <td>Nova linha</td> 
  </tr> 
  <tr> 
   <td>\u000b</td> 
   <td>11</td> 
   <td>Guia Vertical</td> 
  </tr> 
  <tr> 
   <td>\f</td> 
   <td>12</td> 
   <td>Feed do formulário</td> 
  </tr> 
  <tr> 
   <td>\r</td> 
   <td>13</td> 
   <td>Retorno de carro</td> 
  </tr> 
  <tr> 
   <td> <p>\u00<em>xx</em></p> <p><em>Onde, xx é o código hexadecimal para os números 14 a 31</em> </p> </td> 
   <td>14 - 31</td> 
   <td>Caracteres Unicode representados pelos pontos de código 14 a 31</td> 
  </tr> 
  <tr> 
   <td> <p>\/</p> </td> 
   <td>47</td> 
   <td>/ (barra)</td> 
  </tr> 
  <tr> 
   <td> <p>\u003c</p> </td> 
   <td>60</td> 
   <td>&lt; (Menor que)</td> 
  </tr> 
  <tr> 
   <td> <p>\\</p> </td> 
   <td>92</td> 
   <td>\ (Barra invertida)</td> 
  </tr> 
  <tr> 
   <td> <p>\u<em>xxxx</em></p> <p>Em que <em>xxxx</em> é o código hexadecimal para qualquer número acima de 127</p> </td> 
   <td>128+</td> 
   <td>Caracteres Unicode para qualquer ponto de código acima de 127</td> 
  </tr> 
 </tbody> 
</table>
