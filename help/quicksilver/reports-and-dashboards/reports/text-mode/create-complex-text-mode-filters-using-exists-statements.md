---
product-area: reporting
navigation-topic: text-mode-reporting
title: Criar filtros complexos do Modo de texto usando instruções EXISTENTES
description: Criar filtros complexos do Modo de texto usando instruções EXISTENTES
author: Nolan
feature: Reports and Dashboards
exl-id: 106f7c9d-46cc-46c5-ae34-93fd13a36c14
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '2803'
ht-degree: 0%

---

# Criar filtros complexos do Modo de texto usando instruções EXISTENTES

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: do not EVER&nbsp;delete this article as long as Text Mode still exists in the system.&nbsp;Google ordered this article to be written and we wrote it with the help of consultants, so the use case is very complex and very hard to understand without this. It is also very much used by many customers)</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;Alina: **~ Replace screen shot of icons when list/ reporting UI changes)</p>
-->

>[!IMPORTANT]
>
>Este artigo requer uma compreensão completa da API do Adobe Workfront e da interface de relatório do modo de texto. Para obter informações sobre a API do Workfront, consulte [Noções básicas da API](../../../wf-api/general/api-basics.md).\
>Para obter informações sobre como usar o modo de texto, consulte [Visão geral do modo de texto](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

## Visão geral dos relacionamentos de objetos no Workfront

Todos os objetos são vinculados a outros objetos no banco de dados do Workfront.

Entender a hierarquia e a interdependência de objetos ajuda a descobrir quais objetos podem ser referenciados nos relatórios.

Para obter informações sobre quais objetos estão no Workfront e sobre sua hierarquia e interdependência, consulte [Entender objetos no Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

Ao criar filtros, é possível fazer referência a outros objetos conectados ao objeto do filtro dentro de até dois níveis de relacionamento usando a interface de relatório padrão.

Por exemplo, você pode fazer referência à ID do Portfolio em um filtro de edição para exibir somente os problemas em projetos associados a um determinado portfólio usando a interface padrão. Nesse caso, o portfólio está a dois níveis de emissões.

No entanto, você não pode fazer referência ao Proprietário do Portfolio em um filtro de edição usando a interface padrão para exibir somente problemas de projetos associados a portfólios, onde o proprietário é um usuário específico. Você deve usar o modo de texto para acessar o campo Nome do proprietário do Portfolio, que está a três níveis dos problemas.

![issue_to_portfolio_owner_ight_line_icons.PNG](assets/issue-to-portfolio-owner-sraight-line-icons-350x83.png)

Para obter uma lista completa de objetos no Workfront, consulte o [API Explorer](../../../wf-api/general/api-explorer.md).

Para obter informações sobre como navegar no API Explorer e localizar objetos, consulte [Uso do API Explorer](../../../wf-api/general/using-api-explorer.md).

Ao criar filtros, você deve criar instruções complexas na interface do modo texto para fazer referência a esses tipos de objetos.

Para obter informações sobre a criação de filtros complexos, consulte [Visão geral de filtros complexos de modo de texto que usam instruções EXISTS](#overview-of-complex-text-mode-filters-that-use-exists-statements) seção.

## Visão geral de filtros de modo de texto complexos que usam instruções EXISTS {#overview-of-complex-text-mode-filters-that-use-exists-statements}

Considere o seguinte ao criar filtros que abrangem vários níveis na hierarquia de objetos ou filtrar objetos ausentes:

* Você deve criar filtros complexos quando quiser fazer referência a objetos não diretamente conectados ao objeto de filtro.
* Você deve usar uma instrução EXISTS para fazer o seguinte:

   * Crie filtros que abrangem vários níveis.
   * Crie filtros que procuram objetos que estão ausentes.\
      Por exemplo, ao criar um relatório de usuário, é possível filtrar por usuários que não registraram tempo por um determinado período.

Considere as seguintes regras ao usar as instruções EXISTS em um filtro:

* Há três objetos que podem ser referenciados em um filtro EXISTENTE:

   * O objeto do filtro (Objeto Original).
   * O objeto cujo campo você deseja referenciar (Objeto de destino).
   * O objeto que conecta o Original e os Objetos de Destino, caso eles não estejam diretamente conectados um ao outro (Objeto de Vinculação).

* Os filtros que usam EXISTS contêm duas instruções separadas vinculadas por um sinal de igual:

   * A instrução antes do sinal de igual se refere ao objeto ao qual você está se referindo (o Objeto de vinculação ou de destino).
   * A declaração depois do sinal de igual se refere ao objeto que você está referindo (o Objeto Original).

* Você deve usar o código de objeto do Objeto de vinculação para conectar suas instruções.\
   Você pode encontrar o código de objeto de todos os objetos no API Explorer.\
   Para obter informações sobre o API Explorer, consulte o [API Explorer](https://one.workfront.com/s/api-explorer).

* Quando um objeto de vinculação está ausente, pois o original e os objetos de destino estão conectados diretamente entre si, é possível usar o código de objeto do objeto de destino em vez do objeto de vinculação.
* É possível fazer referência a vários campos (Campos de Direcionamento) no mesmo objeto (Objeto de Direcionamento), nesse caso, é necessário conectar as linhas que fazem referência aos campos por E.\
   Para obter um exemplo de filtragem para mais de um campo que pertence ao Objeto de destino, consulte o [Exemplo 4: Filtrar por vários campos: tarefas por Nome do proprietário do Portfolio e ID do Scorecard de alinhamento do Portfolio](#example-4-filter-by-multiple-fields-tasks-by-portfolio-owner-name-and-portfolio-alignment-scorecard-id) neste artigo.

* O único modificador suportado para uma instrução EXISTS é NOTEXISTS.

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plano Adobe Workfront*</td> 
   <td> <p>Qualquer Um</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Plano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a filtros, visualizações, agrupamentos</p> <p>Editar o acesso a Relatórios, Painéis, Calendários para editar filtros em um relatório</p> <p>Observação: Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões de um relatório para editar filtros em um relatório</p> <p>Gerenciar permissões em um filtro para editá-lo</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

## Criar filtros de modo de texto complexos que abrangem vários níveis na hierarquia de objetos

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina: ***[This information is somewhat duplicated from the section below: Create Text-Mode Filters for Missing Objects])</p>
-->

Você pode criar um filtro que faça referência a objetos em vários níveis da hierarquia de objetos na qual o objeto de filtro existe. Por exemplo, você pode criar um filtro de problemas para problemas que estão em projetos que não estão associados a um determinado Portfolio Proprietário.

Você sempre deve usar uma instrução EXISTS e a interface do modo de texto para criar esse filtro.

Para obter exemplos de filtros, consulte a [Exemplo 1: Filtrar problemas por Nome do Proprietário do Portfolio](#example-1-filter-for-issues-by-portfolio-owner-name) neste artigo.

Para criar um filtro que abrange vários níveis na hierarquia de objetos:

1. Identifique o objeto do filtro. Nós nos referimos a esse objeto como o Objeto original.\
   Por exemplo, Problema.
1. Identifique o campo que deseja filtrar. Nós nos referimos a esse objeto como o Campo de destino que pertence a um Objeto de destino.\
   Por exemplo, o campo ownerID (Campo de destino) que pertence ao Portfolio (Objeto de destino).
1. (Condicional) Se o Objeto original (Ocorrência) e o Campo de destino (ownerID) não estiverem diretamente conectados entre si, você deverá encontrar um terceiro objeto, um Objeto de vinculação (Projeto) que os conecta. O Objeto de Vinculação deve ter pelo menos um campo referenciado nas guias Campos ou Referências do Objeto Original (Campo de Vinculação exibido no Objeto Original) e também deve ter um Campo de Vinculação ao Objeto de Destino exibido nas guias Campos ou Referências do Objeto de Vinculação. O Campo de vinculação ao objeto de destino que é exibido no objeto de vinculação (ou no campo de vinculação exibido no objeto de vinculação) deve corresponder ao campo de destino.\
   Por exemplo, a ID (Projeto) (Campo de vinculação exibido no Objeto Original) é referenciada de Problemas (Objeto Original). (Portfolio) ownerID (Vinculando campo ao objeto de destino) é exibido na guia Fields do Projeto (Vinculando objeto). Portfolio ownerID também é um campo no Objeto de destino (Portfolio). O Campo de vinculação no Objeto de vinculação corresponde ao Campo de destino.\
   ![portfólio_id_in_the_project_api_object.PNG](assets/portfolio-id-in-the-project-api-object-350x88.png)

1. Usando o API Explorer, identifique a variável **Código do objeto** do Objeto de Vinculação (Projeto).\
   Por exemplo, o Código de objeto do projeto é PROJ.\
   ![project_objCode_in_the_API.PNG](assets/project-objcode-in-the-api-350x84.png)

1. Crie um filtro para o Objeto original.\
   Por exemplo, crie um filtro Problema .\
   Para obter informações sobre como criar filtros, consulte [Visão geral dos filtros no Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. Clique em **Alternar para o modo de texto**.
1. Cole o exemplo de fórmula a seguir na interface de modo de texto do novo filtro e substitua o texto sugerido pelos objetos e campos corretos:

   ```
   EXISTS:A:$$OBJCODE=<Object code of the Linking Object>
   EXISTS:A:<Linking Field on the Linking Object>=FIELD:<Linking Field displayed on the Original Object>
   EXISTS:A:<Target Object>:<Target Field>=<Your value for the Target Field>
   ```

   Para obter um exemplo de uso dos campos identificados acima, consulte o [Exemplo 1: Filtrar problemas por Nome do Proprietário do Portfolio](#example-1-filter-for-issues-by-portfolio-owner-name) neste artigo.

1. Clique em **Salvar filtro**.

## Criar filtros de modo de texto complexo para objetos ausentes

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina: **^[This information is somewhat duplicated from the section above: Create Text-Mode Filters that Span Multiple Levels in the Object Hierarchy])</p>
-->

Você pode criar um filtro que faça referência a objetos que estão ausentes. Por exemplo, você pode criar um filtro de usuário que mostra quais usuários não registraram horas no Workfront.

Você sempre deve usar um *EXISTE* e a interface do modo de texto para criar esse filtro.

Para obter exemplos de filtros para objetos ausentes, consulte as seguintes seções neste artigo:

* [Exemplo 2: Filtrar objetos ausentes: campos personalizados que não aparecem em nenhum formulário personalizado](#example-2-filter-for-missing-objects-custom-fields-that-do-not-appear-in-any-custom-forms)
* [Exemplo 3: Filtrar objetos ausentes: usuários que não registraram tempo por um determinado período](#example-3-filter-for-missing-objects-users-who-did-not-log-time-for-a-certain-period-of-time)

Para criar um filtro que faça referência a objetos ausentes:

1. Identifique o objeto do filtro. Nós nos referimos a esse objeto como o Objeto original.\
   Por exemplo, Parâmetro ou Campo personalizado.
1. Identifique o campo que deseja filtrar. Nós nos referimos a esse objeto como o Campo de destino que pertence a um Objeto de destino.\
   Por exemplo, o campo categoryID (Campo de destino) que pertence a Categoria (Objeto de destino).
1. Como o Objeto original (Parâmetro) e o Campo de destino (categoryID) não estão diretamente conectados entre si, é necessário encontrar um terceiro objeto, um Objeto de vinculação (um Parâmetro de categoria) que os conecta. O Objeto de Vinculação deve ter pelo menos um campo referenciado nas guias Campos ou Referências do Objeto Original (Campo de Vinculação exibido no Objeto Original) e também deve ter um Campo de Vinculação ao Objeto de Destino exibido nas guias Campos ou Referências do Objeto de Vinculação. O Campo de vinculação ao objeto de destino que é exibido no objeto de vinculação (ou no campo de vinculação exibido no objeto de vinculação) deve corresponder ao campo de destino.\
   Por exemplo, a ID do Parâmetro de categoria (Campo de vinculação exibido no Objeto original) é referenciada a partir do Parâmetro (Objeto original). parameterID (Vinculação de campo ao objeto de destino) é exibido na guia Campos do parâmetro de categoria (Vínculo de objeto). O campo Vinculação ao objeto de destino, que é exibido no objeto de vinculação, corresponde ao campo de destino.
1. Usando o API Explorer, identifique a variável **Código do objeto** do Objeto de vinculação (Parâmetro de categoria).\
   Por exemplo, o Código do objeto para o parâmetro de categoria é CTGYPA.\
   ![category_parameter_objcode_in_api.PNG](assets/category-parameter-objcode-in-api-350x79.png)

1. Crie um filtro para o Objeto original.\
   Por exemplo, crie um filtro Parameter .\
   Para obter informações sobre como criar filtros, consulte [Visão geral dos filtros no Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. Clique em **Alternar para o modo de texto**.
1. (Condicional) Se você estiver filtrando objetos que estão ausentes, cole o seguinte exemplo de fórmula na interface do modo de texto do novo filtro e substitua o texto sugerido pelos objetos e campos corretos:

   ```
   EXISTS:A:$$OBJCODE=<Object code of the Linking Object><br>
   ```

   ```
   EXISTS:A:<Linking Field displayed on the Linking Object>=FIELD:<Linking Field displayed on the Original Object><br>EXISTS:A:$$EXISTSMOD=NOTEXISTS
   ```

   Para obter um exemplo dos relatórios sobre Campos personalizados que não estão associados ao Forms personalizado, consulte a [Exemplo 2: Filtrar objetos ausentes: campos personalizados que não aparecem em nenhum formulário personalizado](#example-2-filter-for-missing-objects-custom-fields-that-do-not-appear-in-any-custom-forms) neste artigo.

1. Clique em **Salvar filtro**.

## Exemplos de filtros de modo de texto que abrangem vários níveis na hierarquia de objetos

* [Exemplo 1: Filtrar problemas por Nome do Proprietário do Portfolio](#example-1-filter-for-issues-by-portfolio-owner-name)
* [Exemplo 2: Filtrar objetos ausentes: campos personalizados que não aparecem em nenhum formulário personalizado](#example-2-filter-for-missing-objects-custom-fields-that-do-not-appear-in-any-custom-forms)
* [Exemplo 3: Filtrar objetos ausentes: usuários que não registraram tempo por um determinado período](#example-3-filter-for-missing-objects-users-who-did-not-log-time-for-a-certain-period-of-time)
* [Exemplo 4: Filtrar por vários campos: tarefas por Nome do proprietário do Portfolio e ID do Scorecard de alinhamento do Portfolio](#example-4-filter-by-multiple-fields-tasks-by-portfolio-owner-name-and-portfolio-alignment-scorecard-id)

### Exemplo 1: Filtrar problemas por Nome do Proprietário do Portfolio {#example-1-filter-for-issues-by-portfolio-owner-name}

Usando a interface do modo de texto, você pode criar um filtro para uma lista de problemas para exibir somente os problemas que estão em projetos associados a um portfólio cujo proprietário é um usuário específico.

Para filtrar problemas pelo Nome do Proprietário do Portfolio:

1. Crie um filtro Issue .\
   Para obter informações sobre como criar filtros, consulte [Visão geral dos filtros no Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. Clique em **Alternar para o modo de texto**.
1. Consulte o seguinte código genérico:

   ```
   EXISTS:A:$$OBJCODE=<Object code of the Linking Object><br>
   ```

   ```
   EXISTS:A:<Linking Field on the Linking Object>=FIELD:<Linking Field displayed on the Original Object><br>EXISTS:A:<Target Object>:<Target Field>=<Your value for the Target Field>
   ```

1. Cole o seguinte código no **Definir regras de filtro para seu relatório** área para substituir o código genérico acima:

   <pre>EXISTE:A:$$OBJCODE=PROJ<br>EXISTE:A:ID=FIELD:projectID<br>EXISTE:A:portfólio:ownerID=4d94d7da001699b19edf50de15682221</pre>

   >[!NOTE]
   >
   >* O Objeto Original é o objeto do relatório: Problema
   >* O objeto de destino é o Portfolio.
   >* O objeto de vinculação é Project.
   >* O Campo de destino e o Campo de vinculação ao objeto de destino referenciado do Objeto de vinculação são ownerID.
   >* O código do Objeto de vinculação aqui é PROJ.
   >* O Campo de vinculação exibido no Objeto original é projectID e o Campo de vinculação é ID.


1. Substitua o valor do Campo de destino (ownerID) na última instrução por uma ID de usuário do seu ambiente.
1. Clique em **Salvar filtro**.

### Exemplo 2: Filtrar objetos ausentes: campos personalizados que não aparecem em nenhum formulário personalizado {#example-2-filter-for-missing-objects-custom-fields-that-do-not-appear-in-any-custom-forms}

Usando a interface de modo de texto, você pode criar um filtro para exibir Campos personalizados (Parâmetros) que não estão associados ao Forms personalizado (Categorias). Esse filtro vincula Parâmetros a Categorias, que são conectadas por meio de outro objeto, Parâmetro de categoria. Como os dois campos não estão diretamente conectados entre si e como você está filtrando informações ausentes, é necessário usar uma instrução EXISTS.

>[!IMPORTANT]
>
>Um Parâmetro é um campo como existe na Biblioteca de campos referenciada em um Formulário personalizado. Um Parâmetro de categoria é a versão de um campo que aparece em um formulário específico. Por exemplo, se o mesmo campo aparecer em 5 formulários, haverá 1 Parâmetro e 5 Parâmetros de Categoria no Banco de Dados do Workfront.

Para filtrar Campos personalizados não associados a um Formulário personalizado:

1. Crie um parâmetro ou um filtro de Campo personalizado.\
   Para obter informações sobre como criar filtros, consulte [Visão geral dos filtros no Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. Clique em **Alternar para o modo de texto**.
1. Consulte o seguinte código genérico:

   ```
   EXISTS:A:$$OBJCODE=<Object code of the Linking Object>
   ```

   ```
   EXISTS:A:<Linking Field displayed on the Linking Object>=FIELD:<Linking Field displayed on the Original Object><br>EXISTS:A:$$EXISTSMOD=NOTEXISTS
   ```

1. Cole o seguinte código no **Definir regras de filtro para seu relatório** área para substituir o código genérico acima:

   <pre>EXISTE:A:$$OBJCODE=CTGYPA<br>EXISTE:A:parameterID=FIELD:ID<br>EXISTE:A:$$EXISTSMOD=NOTEXISTS</pre>

   >[!NOTE]
   >
   >* O Objeto Original é o objeto do relatório: Parâmetro.
   >* O objeto de destino é Categoria.
   >* O Objeto de vinculação é o Parâmetro de categoria.
   >* O código do objeto de vinculação é CTGYPA.
   >* O Campo de vinculação ao objeto de destino é parameterID, pois parameterID existe tanto na Tabela de objetos de vinculação quanto na Tabela de objetos de destino.
   >* O Campo de vinculação exibido no Objeto original é ID (do Parâmetro de categoria).


1. Clique em **Salvar filtro**.

### Exemplo 3: Filtrar objetos ausentes: usuários que não registraram tempo por um determinado período {#example-3-filter-for-missing-objects-users-who-did-not-log-time-for-a-certain-period-of-time}

Usando a interface de modo de texto, você pode criar um filtro para exibir Usuários que não registraram tempo por um determinado período. Esse filtro vincula os Usuários às Horas, que são conectados diretamente um ao outro. No entanto, você deve usar uma instrução EXISTS e a interface do modo de texto para poder filtrar por informações ausentes.

Para filtrar usuários que não registraram tempo durante a semana passada:

1. Crie um filtro Usuário .\
   Para obter informações sobre como criar filtros, consulte [Visão geral dos filtros no Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. Clique em **Alternar para o modo de texto**.
1. Consulte o seguinte código genérico:

   ```
   EXISTS:A:$$OBJCODE=<Object code of the Linking Object><br>
   ```

   ```
   EXISTS:A:<Linking Field displayed on the Linking Object>=FIELD:<Linking Field displayed on the Original Object><br>EXISTS:A:$$EXISTSMOD=NOTEXISTS
   ```

1. Cole o seguinte código no **Definir regras de filtro para seu relatório** área para substituir o código genérico acima:

   ```
   EXISTS:A:$$OBJCODE=HOUR<br>EXISTS:A:ownerID=FIELD:ID<br>EXISTS:A:entryDate=$$TODAYb-1w<br>EXISTS:A:entryDate_Range=$$TODAYe-1w<br>EXISTS:A:entryDate_Mod=between<br>EXISTS:A:$$EXISTSMOD=NOTEXISTS
   ```

   >[!NOTE]
   >
   >* O Objeto Original é o objeto do relatório: Usuário.
   >* O objeto de destino é Hora.
   >* Você não precisa de um Objeto de vinculação neste exemplo porque Usuários e Horas estão diretamente conectados ao banco de dados do Workfront.
   >* Como não há um objeto de vinculação, você deve usar o Código do objeto de destino: HORA.
   >* O Campo de vinculação ao objeto de destino é ownerID (que é exibido no objeto original); o objeto de vinculação está ausente).
   >* O Campo de vinculação exibido no Objeto original é a ID (da Hora) (que é exibida no Objeto de destino; o objeto de vinculação está ausente.)
   >* O:A:A instrução entryDate refere-se aos campos que definem o Objeto de destino (Hora) e usam a mesma sintaxe de uma instrução de filtro regular. Isso garante que você exiba apenas os usuários que não registraram tempo por um período específico, neste caso, a semana anterior.
   >* O modificador NOTEXISTS indica que estamos procurando itens (Horas) que não existem para o objeto do relatório (Usuários).


1. Clique em **Salvar filtro**.

### Exemplo 4: Filtrar por vários campos: tarefas por Nome do proprietário do Portfolio e ID do Scorecard de alinhamento do Portfolio {#example-4-filter-by-multiple-fields-tasks-by-portfolio-owner-name-and-portfolio-alignment-scorecard-id}

Usando a interface de modo de texto, você pode criar um filtro que se refere a mais de um campo no Objeto de destino. Nesse caso, as instruções de filtro que fazem referência aos Campos de direcionamento devem ser conectadas por AND.

Por exemplo, você pode filtrar uma lista de tarefas para exibir somente tarefas que atendem aos seguintes critérios:

* Eles estão em um projeto associado a um portfólio cujo proprietário é um usuário específico.
* Eles estão em um projeto associado a um portfólio cujos projetos não estão associados a um scorecard de alinhamento específico.

Para filtrar tarefas pelo Nome do proprietário do Portfolio e ID do Scorecard de alinhamento do Portfolio:

1. Crie um filtro Tarefa .\
   Para obter informações sobre como criar filtros, consulte [Visão geral dos filtros no Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. Clique em **Alternar para o modo de texto**.
1. Cole o seguinte código no **Definir regras de filtro para seu relatório** Área:
   <pre>EXISTE:A:$$OBJCODE=PROJ<br>EXISTE:A:ID=FIELD:projectID<br>EXISTE:A:portfólio:ownerID=4d80ce5200000528787d57807732a33f<br>E:A:EXISTE:A:$$EXISTSMOD=NOTEXISTS<br>E:A:EXISTE:A:$$OBJCODE=PROJ<br>E:A:EXISTE:A:ID=FIELD:projectID<br>E:A:EXISTE:A:portfólio:alignmentScoreCardID=4da387b0001cbc732bb259355c33dad</pre>

   >[!NOTE]
   >
   >* O Objeto Original é o objeto do filtro: Tarefa.
   >* O objeto de destino é o Portfolio.
   >* O primeiro campo do Target é ownerID.
   >* O segundo campo de destino é a ID do scorecard de alinhamento.
   >* O objeto de vinculação é Project.
   >* O código do objeto de vinculação é PROJ.
   >* O Campo de vinculação ao objeto do Target é a ID (do Portfolio).
   >* O Campo de vinculação exibido no Objeto original é projectID.
   >* Substitua a ownerID por uma ID de usuário do seu ambiente.


1. Clique em **Salvar filtro**.
