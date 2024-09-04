---
title: Visão Geral de Campos de Fórmula
description: No Adobe Workfront Planning, é possível criar campos de fórmula que usam funções e campos existentes para calcular um novo valor personalizado.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 5027d611-916e-492d-9a44-841bdde11c94
source-git-commit: bd202821687453288c96147933331c8a7a6b3acb
workflow-type: tm+mt
source-wordcount: '588'
ht-degree: 7%

---

# Visão geral dos campos de fórmula

<!--when we release permissions to RECORDS and we release referring lookup fields in a formula field, update considerations to say that lookup fields from linked records depends on the permissions to the record; if they have no permissions to view a linked record, they won't be able to use that records's lookup fields in a formula-->

{{planning-important-intro}}

Você pode criar campos personalizados no Adobe Workfront Planning fazendo referência a campos existentes e os conectando em um campo do tipo Fórmula.

Os campos de fórmula geram um novo valor usando valores existentes de outros campos em um tipo de registro e uma função que indica como os valores existentes devem ser calculados.

Para obter informações, consulte a seção &quot;Fórmula&quot; no artigo [Criar campos](/help/quicksilver/planning/fields/create-fields.md).

## Requisitos de acesso

+++ Expanda para exibir os requisitos de acesso do Workfront Planning.

Para acessar o Workfront Planning, é necessário ter o seguinte:

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
   <td role="rowheader"><p>Plano de planejamento do Adobe Workfront*</p></td> 
   <td> 
<p>Qualquer </p> 
<p>Para obter mais informações sobre o que está incluído em cada plano do Workfront Planning, entre em contato com seu gerente de conta da Workfront. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>plataforma Adobe Workfront</p></td> 
   <td> 
<p>A instância da Workfront de sua organização deve ser integrada à Adobe Unified Experience para acessar todos os recursos do Workfront Planning.</p> 
<p>Para obter mais informações, consulte <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Experiência unificada do Adobe para Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Licença da Adobe Workfront*</p></td> 
   <td><p> Padrão</p>
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
   <td>   <p>Gerenciar permissões para um espaço de trabalho</a> </p>  
   <p>Os administradores do sistema têm permissões para todos os espaços de trabalho, incluindo aqueles que não criaram</p> </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Modelo de layout</p></td> 
   <td> <p>Todos os usuários, incluindo administradores do Workfront, devem receber um modelo de layout que inclua a área Planejamento no Menu principal. </p> </td> 
  </tr> 
</tbody> 
</table>

*Para obter mais informações sobre requisitos de acesso do Workfront, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--

OLD:
<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Product</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront agreement</p></td>
   <td>
<p>Your organization must be enrolled in the early access stage for Workfront Planning </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront plan</p></td>
   <td>
<p>Any</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront license*</p></td>
   <td>
   <p>New: Standard</p>
   <p>Current: Plan</p> 
  </td>
  </tr>
  
  <tr>
   <td role="rowheader"><p>Access level configuration</p></td>
   <td> <p>There are no access controls for Workfornt planining</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>Manage permissions to a workspace</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>Your Workfront or group administrator must add the Planning area in your layout template. For information, see <a href="/help/quicksilver/planning/access/access-overview.md">Access overview</a>. </p>  
</td>
  </tr>

 </tbody>
</table>

*For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). 

-->

## Considerações sobre campos de fórmula

* Os campos de fórmula fazem referência a campos que pertencem ao mesmo tipo de registro.
* Você pode fazer referência a campos de outros tipos de registro somente quando você conecta outro tipo de registro ao que está criando um campo de fórmula para.
* Não é possível alterar o tipo Field de um campo Formula depois de salvá-lo.
* É possível atualizar o cálculo de um campo de fórmula depois de salvá-lo, e os resultados do cálculo são atualizados automaticamente para todos os registros do mesmo tipo.
* É necessário adicionar os campos que você menciona nas fórmulas à medida que são exibidos na interface do Workfront Planning.
* Você pode fazer referência somente a campos exibidos na exibição de tabela de um tipo de registro ou na página de detalhes do registro.
* Você pode definir o formato para o valor de um cálculo de fórmula escolhendo entre as seguintes opções de formato:

   * Texto
   * Número
   * Percentual
   * Moeda
   * Tags
   * Data

  Para obter mais informações, consulte a seção &quot;Fórmula&quot; no artigo [Criar campos](/help/quicksilver/planning/fields/create-fields.md).

## Fórmulas compatíveis

Os campos de fórmula do Adobe Workfront Planning aceitam todas as expressões dos campos calculados do Workfront. Para obter mais informações, consulte [Visão geral das expressões de dados calculadas](/help/quicksilver/reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

Além disso, oferecemos suporte às seguintes expressões para campos de fórmula do Workfront Planning:

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
