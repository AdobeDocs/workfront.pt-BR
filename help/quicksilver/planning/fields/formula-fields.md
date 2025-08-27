---
title: Visão Geral de Campos de Fórmula
description: No Adobe Workfront Planning, é possível criar campos de fórmula que usam funções e campos existentes para calcular um novo valor personalizado.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 5027d611-916e-492d-9a44-841bdde11c94
source-git-commit: 7288c6fb0f5d45758e0a82b8d1283e1f43ae94e6
workflow-type: tm+mt
source-wordcount: '684'
ht-degree: 7%

---

# Visão geral dos campos de fórmula

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

Você pode criar campos personalizados no Adobe Workfront Planning fazendo referência a campos existentes e os conectando em um campo do tipo Fórmula.

Os campos de fórmula geram um novo valor usando valores existentes de outros campos em um tipo de registro e uma função que indica como os valores existentes devem ser calculados.

Para obter informações, consulte a seção &quot;Fórmula&quot; no artigo [Criar campos](/help/quicksilver/planning/fields/create-fields.md).

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Produtos</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Planejamento do Adobe Workfront<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>plano do Adobe Workfront*</p></td> 
   <td> 
<p>Qualquer um dos seguintes planos da Workfront:</p> 
<ul><li>Selecionar</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>O Workfront Planning não está disponível para planos herdados do Workfront</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Pacote de planejamento do Adobe Workfront*</p></td> 
   <td> 
<p>Qualquer </p> 
<p>Para obter mais informações sobre o que está incluído em cada plano do Workfront Planning, entre em contato com seu gerente de conta da Workfront. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>plataforma Adobe Workfront</p></td> 
   <td> 
<p>A instância da Workfront de sua organização deve ser integrada à Adobe Unified Experience para acessar o Workfront Planning.</p> 
<p>Para obter mais informações, consulte <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Experiência unificada da Adobe para Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Licença da Adobe Workfront*</p></td> 
   <td><p> Standard</p>
   <p>O Workfront Planning não está disponível para licenças herdadas do Workfront</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Configuração do nível de acesso</p></td> 
   <td> <p>Não há controles de nível de acesso para o Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Permissões de objeto</p></td> 
   <td>   <p>Gerenciar permissões para um espaço de trabalho e tipo de registro </a> </p>  
   <p>Os administradores do sistema têm permissões para todos os espaços de trabalho, incluindo aqueles que não criaram</p> </td> 
  </tr>

</tbody> 
</table>

*Para obter mais informações sobre requisitos de acesso do Workfront, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++   

## Considerações sobre campos de fórmula

* Os campos de fórmula fazem referência a campos que pertencem ao mesmo tipo de registro.
* Você pode fazer referência a campos de outros tipos de registro somente quando você conecta outro tipo de registro ao que está criando um campo de fórmula para.
* A referência a tipos de registro conectados ou a seus campos de pesquisa em uma fórmula depende de suas permissões para os tipos de registro conectados. Se você não tiver permissões para exibir o tipo de registro, não poderá fazer referência a seus campos em uma fórmula.
* Não é possível alterar o tipo Field de um campo Formula depois de salvá-lo.
* É possível atualizar o cálculo de um campo de fórmula depois de salvá-lo, e os resultados do cálculo são atualizados automaticamente para todos os registros do mesmo tipo.
* É necessário adicionar os campos que você menciona nas fórmulas à medida que são exibidos na interface do Workfront Planning.
* Você pode fazer referência somente a campos exibidos na exibição de tabela de um tipo de registro ou na página de detalhes do registro.
* Você pode definir o formato para o valor de um cálculo de fórmula escolhendo entre as seguintes opções de formato:

   * Texto
   * Número
   * Porcentagem
   * Moeda
   * Tags
   * Data

  Para obter mais informações, consulte a seção &quot;Fórmula&quot; no artigo [Criar campos](/help/quicksilver/planning/fields/create-fields.md).
* Você pode fazer referência a campos de fórmula em novas fórmulas. Depois que o valor for atualizado em um campo referenciado em um campo de fórmula, todos os campos subsequentes que referenciam esse campo ou campos de fórmula que contêm esse campo serão atualizados automaticamente.


<!--

<div class="preview">

## Limitations of formula fields

* You can add a maximum of 20 formula fields for one record type. 

   Formula lookup fields added from connected record types do not count against this limit. 

* The formula expression cannot exceed 50,000 characters. 

* Formula fields might display as `#ERROR!` in the following cases:
   * When a field used in a formula is deleted.
   * When a field used in an aggregated lookup field displays as `#ERROR!`. 
   
      For example, if you display a lookup field that contains aggregated lookup formula fields and one of the referenced formula fields  displays as `#ERROR!`. 
   *  When a formula value cannot be displayed in the selected format. 
   
      For example, if I select Number for the Format of a formula field, and the fields used in the formula are text fields that display only non-numeric text values, the formula result will display as `#ERROR!`, because it cannot parse the text into a number.
 
 </div>
 
 -->

## Fórmulas compatíveis

Os campos de fórmula do Adobe Workfront Planning suportam a maioria das expressões dos campos calculados do Workfront.

>[!NOTE]
>
>As seguintes expressões Workfront não são suportadas para campos de fórmula do Workfront Planning:
>
><!--* SORTASCARRAY-->
><!--* SORTDESCARRAY-->
>* ADDHOUR
>* SWITCH
>* FORMATAR

<!--remove the ones commented out when we go live to Preview and Prod, if they truly are added to Planning-->

Para obter uma lista completa de expressões Workfront, consulte [Visão geral das expressões de dados calculadas](/help/quicksilver/reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

Além disso, oferecemos suporte às seguintes expressões para os campos de fórmula do Workfront Planning. As seguintes expressões não são suportadas para expressões Workfront:

<!--take these three out when they also come to WF and Lisa has added them to the WF expression article linked above-->

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Expressão</th> 
   <th>Explicação e exemplo</th> 
  </tr> 
 </thead> 
 <tbody>

<tr> 
   <td><strong>JUNÇÃO DE MATRIZ</strong> </td> 
   <td> <p>Retorna a string concatenada por delimitador.</p> <p>A expressão é formatada da seguinte maneira:

<code>ARRAYJOIN(delimitador,matriz)</code>
</p>
   </td></tr>
    <tr> 
   <td><strong>ARRAYUNIQUE</strong> </td> 
   <td> <p>Retorna a matriz com valores únicos.</p> <p>A expressão é formatada da seguinte maneira:

<code>ARRAYUNIQUE(matriz)</code>
</p>
   </td></tr>
     <tr> 
   <td><strong>ID</strong> </td> 
   <td> <p>Retorna a ID de um registro. Cada registro tem uma ID exclusiva.</p> <p>A expressão é formatada da seguinte maneira:

<code>{ID}</code>
</p>
   </td></tr>
  <tr> 
   <td><strong>JSONELEMENT</strong> </td> 
   <td> <p>Retorna os dados de JSON pelo JSONPath fornecido. Se o JSONPath não existir no JSON, um resultado vazio será retornado. </p> <p>A expressão é formatada da seguinte maneira:
      <code>JSONELEMENT(JSONString, JSONPathString) </code>
   </p>
   </td></tr>
  <tr> 
   <td><strong>SETTIMEZONE</strong> </td> 
   <td> <p>Define o fuso horário de uma data e hora para um fuso horário específico.</p> <p>A expressão é formatada da seguinte maneira:

<code>SETTIMEZONE(date,&#39;America/Los_Angeles&#39;)</code>
</p>
   </td></tr>

<tr> 
   <td><strong>SEMANA</strong> </td> 
   <td> <p>Retorna o número da semana em um ano. Como opção, é possível indicar em qual dia a semana começa (use 1 para domingo ou 2 para segunda-feira). Se omitido, as semanas começarão no domingo, por padrão.</p> <p>A expressão é formatada da seguinte maneira:

<code>WEEKOFYEAR(data,2)</code>
ou
<code>WEEKOFYEAR(data)</code>
</p>
   </td></tr>

</table>
