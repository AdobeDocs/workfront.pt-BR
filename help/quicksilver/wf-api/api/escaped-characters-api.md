---
content-type: api
navigation-topic: api-navigation-topic
title: Caracteres de escape nas respostas da API
description: Caracteres de escape nas respostas da API
author: Becky
feature: Workfront API
role: Developer
exl-id: 1477b98e-1cdc-4661-b3ee-0b6ab1e8c3ee
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '202'
ht-degree: 8%

---

# Caracteres de escape nas respostas da API

A sintaxe de algumas respostas da API pode conter o caractere de escape, `\` (barra invertida). Um caractere de escape indica que o caractere ou a string de caracteres que segue imediatamente o caractere de escape tem um valor especial. Por exemplo, `\t` informa ao dispositivo de leitura que `t` deve ser interpretado no sentido de que `tab` e não como a letra &quot;t&quot;. Uma string de um ou mais caracteres após a barra invertida é chamada de sequência de escape.

Sequências de escape hexadecimais exigem o uso de dígitos hexadecimais válidos. A tabela a seguir lista as sequências de escape codificadas nas respostas da API do Adobe Workfront:

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
   <td> <p>\u000<em>x</em></p> <p>Onde, <em>x</em> é o código hexadecimal dos números de 0 a 7</p> </td> 
   <td>0-7</td> 
   <td>Caracteres Unicode representados por pontos de código de 0 a 7</td> 
  </tr> 
  <tr> 
   <td>\b</td> 
   <td>8</td> 
   <td>Apagar</td> 
  </tr> 
  <tr> 
   <td>\ t</td> 
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
   <td>Feed de formulário</td> 
  </tr> 
  <tr> 
   <td>\r</td> 
   <td>13</td> 
   <td>Retorno de carro</td> 
  </tr> 
  <tr> 
   <td> <p>\u00<em>xx</em></p> <p><em>Onde, xx é o código hexadecimal dos números 14 a 31</em> </p> </td> 
   <td>14 - 31</td> 
   <td>Caracteres Unicode representados pelos pontos de código 14 a 31</td> 
  </tr> 
  <tr> 
   <td> <p>\/</p> </td> 
   <td>47</td> 
   <td>/ (Barra)</td> 
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
   <td> <p>\u<em>xxxx</em></p> <p>Onde, <em>xxxx</em> é o código hexadecimal para qualquer número acima de 127</p> </td> 
   <td>128+</td> 
   <td>Caracteres Unicode para qualquer ponto de código acima de 127</td> 
  </tr> 
 </tbody> 
</table>
