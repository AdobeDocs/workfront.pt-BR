---
title: Visão Geral de Campos de Fórmula
description: No Adobe Workfront Planning, é possível criar campos de fórmula que usam funções e campos existentes para calcular um novo valor personalizado.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 5027d611-916e-492d-9a44-841bdde11c94
source-git-commit: 8546311acf722c0f4d47d4663b02ff701416894a
workflow-type: tm+mt
source-wordcount: '924'
ht-degree: 4%

---

# Visão geral dos campos de fórmula

<span class="preview">As informações destacadas nesta página referem-se a funcionalidades que ainda não estão disponíveis. Ela está disponível somente no ambiente de Pré-visualização para todos os clientes. Depois das versões mensais para produção, os mesmos recursos também ficam disponíveis no ambiente de produção para clientes que ativaram versões rápidas. </span>

<span class="preview">Para obter informações sobre versões rápidas, consulte [Habilitar ou desabilitar versões rápidas para sua organização](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

Você pode criar campos personalizados no Adobe Workfront Planning fazendo referência a campos existentes e os conectando em um campo do tipo Fórmula.

Os campos de fórmula geram um novo valor usando valores existentes de outros campos em um tipo de registro e uma função que indica como os valores existentes devem ser calculados.

Para obter informações, consulte a seção &quot;Fórmula&quot; no artigo [Criar campos](/help/quicksilver/planning/fields/create-fields.md).

## Requisitos de acesso

+++ Expanda para exibir os requisitos de acesso para a funcionalidade neste artigo. 

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
<li><p>Qualquer Workfront e qualquer pacote do Planning</p></li>
Ou
<li><p>Qualquer fluxo de trabalho e qualquer pacote de planejamento</p></li></ul>
<p>Para obter mais informações sobre o que está incluído em cada pacote do Workfront Planning, entre em contato com o representante de conta da Workfront. </p> 
   </td> 
  <tr> 
   <td role="rowheader"><p>Licença do Adobe Workfront</p></td> 
   <td><p>Standard</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Permissões de objeto</p></td> 
   <td>   <p>Gerenciar permissões em um espaço de trabalho</p>  
   <p>Os administradores do sistema têm permissões para todos os espaços de trabalho, incluindo aqueles que não criaram</p>  </td> 
  </tr>  
</tbody> 
</table>

Para obter mais informações sobre requisitos de acesso do Workfront, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++   

<!--Old:

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Products</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront Planning<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront plan*</p></td> 
   <td> 
<p>Any of the following Workfront plans:</p> 
<ul><li>Select</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning is not available for legacy Workfront plans</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront Planning package*</p></td> 
   <td> 
<p>Any </p> 
<p>For more information about what is included in each Workfront Planning plan, contact your Workfront account manager. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront platform</p></td> 
   <td> 
<p>Your organization's instance of Workfront must be onboarded to the Adobe Unified Experience to be able to access Workfront Planning.</p> 
<p>For more information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront license*</p></td> 
   <td><p> Standard</p>
   <p>Workfront Planning is not available for legacy Workfront licenses</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Access level configuration</p></td> 
   <td> <p>There are no access level controls for Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td>   <p>Manage permissions to a workspace and record type </a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p> </td> 
  </tr> 
 
</tbody> 
</table> -->

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

<div class="preview">

* Quando você atualiza um campo de fórmula ou um campo que poderia impactá-lo, um alerta o notifica do impacto da alteração. O alerta é exibido nos seguintes casos:

   * Quando você atualiza um campo de fórmula (excluindo alterações de nome e descrição) quando esse campo tem campos de fórmula ou de pesquisa dependentes. O alerta lista esses campos dependentes e pergunta se você deseja continuar.

   * Ao excluir um campo usado em uma expressão de fórmula ou como um campo de pesquisa. O alerta lista a fórmula dependente e os campos de pesquisa e pergunta se você deseja continuar com a exclusão.

</div>



<div class="preview">

## Limitações de campos de fórmula

* É possível adicionar no máximo 20 campos de fórmula para um tipo de registro.

  Os campos de pesquisa de fórmula adicionados de tipos de registro conectados não contam com esse limite.

* A expressão da fórmula não pode exceder 50.000 caracteres.

* Campos de fórmula podem ser exibidos como `#ERROR!` nos seguintes casos:
   * Quando um campo usado em uma fórmula é excluído.
   * Quando um campo usado em um campo de pesquisa agregado é exibido como `#ERROR!`.

     Por exemplo, se você exibir um campo de pesquisa que contenha campos de fórmula de pesquisa agregada e um dos campos de fórmula referenciados for exibido como `#ERROR!`.
   * Quando um valor de fórmula não pode ser exibido no formato selecionado.

     Por exemplo, se eu selecionar Número para o Formato de um campo de fórmula e os campos usados na fórmula forem campos de texto que exibem apenas valores de texto não numéricos, o resultado da fórmula será exibido como `#ERROR!`, porque não é possível analisar o texto em um número.

</div>

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
