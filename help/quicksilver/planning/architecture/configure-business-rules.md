---
title: Configurar Regras de Negócios do Tipo de Registro
description: Você pode configurar regras de negócios do tipo registro que definem como os registros desse tipo são gerenciados no Adobe Workfront Planning.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
source-git-commit: 159b845c7b755117197d18f8474c01d4b19d53b8
workflow-type: tm+mt
source-wordcount: '249'
ht-degree: 6%

---


# Configurar regras de negócios do tipo de registro

{{planning-important-intro}}

<!--
<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the release to Preview, the same features are also available monthly in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>
-->

Você pode configurar regras de negócios do tipo registro que definem como os registros desse tipo são gerenciados no Adobe Workfront Planning.

## Requisitos de acesso

+++ Expanda para exibir os requisitos de acesso para executar as etapas deste artigo:  

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
</tr>   
<tr> 
   <td role="rowheader"><p>Pacote do Adobe Workfront</p></td> 
   <td> 
<ul> 
<li><p>Qualquer Workfront ou Fluxo de trabalho com um pacote do Planning</p></li>
Ou
<li><p>Qualquer pacote do Planning quando adquirido como um produto independente</p></li></ul>
   </td> </tr>
  <tr> 
   <td role="rowheader"><p>Licença do Adobe Workfront</p></td> 
   <td><p>Workflow Standard</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>licença do Adobe Planning</p></td> 
   <td><p>Planejamento padrão</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Configuração do nível de acesso</p></td> 
   <td> <p>Você deve adicionar um Workflow e um tipo de licença do Planning ao nível de acesso quando tiver um Workflow e um pacote do Planning</p>   
</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Permissões de objeto</p></td> 
   <td>   <p>Gerenciar permissões para um espaço de trabalho e um tipo de registro</p>  
   <p>Os administradores do sistema têm permissões para todos os espaços de trabalho, incluindo aqueles que não criaram</p>  </td> 
  </tr>  
</tbody> 
</table>

Para obter mais informações sobre requisitos de acesso do Workfront, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Considerações ao configurar regras de negócios

* É possível configurar regras para quando os registros podem ser editados ou excluídos.
* Não é possível configurar regras para quando os registros são criados. Qualquer pessoa com permissões de Gerenciar para o tipo de registro pode criar registros.
* É possível criar uma condição para a regra de negócios que faça referência a todos os tipos de campo, exceto para o seguinte:
  * Campos de fórmula
  * Campos de pesquisa
  * Campos de referência

## Configurar regras de negócios

1. Ir para um tipo de registro.
1. Clique no menu **Mais** ![Mais menu](assets/more-menu.png) à direita do nome do tipo de registro e clique em Regras de negócio.



