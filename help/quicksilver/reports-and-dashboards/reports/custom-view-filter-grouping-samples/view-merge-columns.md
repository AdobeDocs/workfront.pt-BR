---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: "Exibição: mesclar informações de várias colunas em uma coluna compartilhada"
description: É possível mesclar as informações exibidas em várias colunas separadas e exibi-las em uma coluna compartilhada.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: d4f9db12-59ce-4cfc-90dd-e611b49fafdf
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '977'
ht-degree: 0%

---

# Exibição: mesclar informações de várias colunas em uma coluna compartilhada

É possível mesclar as informações exibidas em várias colunas separadas e exibi-las em uma coluna compartilhada.

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront*</td> 
   <td> <p>Qualquer Um</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Solicitação para modificar uma exibição </p>
   <p>Planejar a modificação de um relatório</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a relatórios, painéis e calendários para modificar um relatório</p> <p>Editar acesso a Filtros, Visualizações, Agrupamentos para modificar uma visualização</p> <p><b>Nota</b>

Se você ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões para um relatório</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir seu plano, tipo de licença ou acesso, entre em contato com o administrador do Workfront.

## Considerações ao compartilhar ou mesclar colunas

* Você pode mesclar duas colunas adjacentes e exibir as informações de cada coluna separadas por uma quebra de linha, ou pode mesclar as informações em duas colunas adjacentes sem separador entre as informações de cada coluna.
* É possível mesclar as informações de mais de duas colunas aplicando a mesma sintaxe descrita neste artigo a uma coluna já compartilhada e a uma coluna adjacente.
* O

   ```
   valueformat=HTML
   ```

   a linha é obrigatória em uma coluna compartilhada. Caso contrário, as colunas não conterão informações (estarão em branco) quando o relatório for exportado do Adobe Workfront.
* A formatação condicional pode não ser suportada em colunas mescladas.

   As seguintes exceções existem:

   * Ao exibir informações no Workfront, a formatação da primeira coluna é mantida e a formatação de todas as outras colunas é ignorada se as colunas que compõem uma coluna mesclada tiverem formatação diferente umas das outras,.
   * Ao exportar a exibição para um arquivo PDF, a formatação condicional se aplica à primeira coluna em uma coluna mesclada.
   * Ao exportar a exibição para um arquivo do Excel, as colunas mescladas são exibidas como colunas separadas. As colunas individuais também exibem suas respectivas regras de formatação condicional.

* Colunas com o **viewalias** O atributo pode limitar a quantidade de colunas que podem ser mescladas. Para evitar esses limites, evite usar a variável **viewalias** atributo. Se você precisar incluir a variável **viewalias** em uma coluna, verifique se esse é o último item listado na coluna.

* Se você exportar uma lista com colunas compartilhadas para um formato Excel ou Delimitado por tabulação, essas colunas serão separadas no arquivo exportado.

## Mesclar dados de duas colunas sem uma quebra de linha

É possível mesclar os dados de várias colunas separadas para exibi-los em uma coluna sem quebras ou espaços entre os valores de cada coluna.

>[!TIP]
>
>Essa abordagem é recomendada ao mesclar duas colunas que nunca podem mostrar um valor para o mesmo registro ao mesmo tempo. Por exemplo, em um relatório de Item de trabalho, as colunas Nome da ocorrência e Nome da tarefa podem ser mescladas sem uma quebra de linha entre elas, porque um Item de trabalho nunca pode ter um Nome da ocorrência e um Nome da tarefa ao mesmo tempo. Um Item de trabalho pode ser um Problema ou uma Tarefa no Workfront.

Para fazer isso:

1. Usando o modo de texto para uma exibição, adicione o seguinte texto à primeira coluna que deseja mesclar:

   ```
   sharecol=true
   ```

   Ao mesclar as duas primeiras colunas de uma lista ou relatório, o Workfront precede cada linha de texto que contém informações sobre o objeto na primeira coluna com

   ```
   column.0.
   ```

   e as linhas de texto que contêm informações sobre a segunda coluna com

   ```
   column.1.
   ```

   .\
   Você deve preceder o número da primeira coluna com o número dessa coluna. A contagem de colunas sempre começa com a coluna mais à esquerda da lista ou do relatório rotulado como

   ```
   column.0.
   ```

   .

   Se você compartilhar mais de uma coluna, adicione o número da coluna nas linhas de código que contêm as informações de compartilhamento para cada coluna.

   **Exemplo:** Este é o código do modo de texto para uma coluna mesclada que contém três colunas separadas, começando com a segunda coluna da lista. Os valores mesclados são Nome do projeto, Data de início planejada e nome do Proprietário do projeto, e não há interrupção entre os três valores:

   ```
   column.1.valuefield=name
   ```

   ```
   column.1.valueformat=HTML
   ```

   ```
   column.1.sharecol=true
   ```

   ```
   column.2.valuefield=plannedStartDate
   ```

   ```
   column.2.valueformat=atDate
   ```

   ```
   column.2.sharecol=true
   ```

   ```
   column.3.valuefield=owner:name
   ```

   ```
   column.3.valueformat=HTML
   ```

   <pre><img src="assets/shared-column-no-line-breaks-350x142.png" style="width: 350;height: 142;"></pre>

1. Clique em **Salvar**, depois **Salvar visualização**.

## Mesclar dados de duas colunas com uma quebra de linha

Faça o seguinte para mesclar os dados de várias colunas para exibi-los em uma coluna comum com uma quebra de linha entre os valores de cada coluna:

1. Adicione uma terceira coluna entre as duas colunas que deseja mesclar.

   >[!TIP]
   * As colunas que você deseja mesclar devem ser adjacentes entre si.
   * Você deve clicar na primeira coluna que deseja mesclar.


1. Clique em **Alternar para modo de texto** e adicione o seguinte código na coluna do meio que você adicionou na etapa 1:

   ```
   value=<br>
   ```

   ```
   valueformat=HTML
   ```

   ```
   width=1
   ```

   ```
   sharecol=true
   ```

1. Adicione o seguinte texto à primeira coluna:

   ```
   sharecol=true
   ```

   Ao mesclar as duas primeiras colunas de uma lista ou relatório, o Workfront precede cada linha de texto que contém informações sobre o objeto na primeira coluna com

   ```
   column.0.
   ```

   , a coluna com as informações de compartilhamento com

   ```
   column.1.
   ```

   e as linhas de texto que contêm informações sobre a segunda coluna com

   ```
   column.2.
   ```

   . Se a coluna combinada estiver no meio da exibição, as colunas serão numeradas de acordo com seu local na exibição. A contagem de colunas sempre começa com a coluna mais à esquerda da lista ou do relatório rotulado como

   ```
   column.0.
   ```

   .

   Se você compartilhar mais de uma coluna, adicione o número da coluna nas linhas de código que contêm as informações de compartilhamento.

   **Exemplo:** Este é o código do modo de texto para uma coluna compartilhada que contém o Nome do Projeto, a Data de Início Planejada e o nome do Proprietário do Projeto com uma quebra de linha. A coluna compartilhada é a segunda coluna de uma exibição de projeto.

   ```
   column.1.displayname=Project_StartDate_Owner
   ```

   ```
   column.1.sharecol=true
   ```

   ```
   column.1.textmode=true
   ```

   ```
   column.1.valuefield=name
   ```

   ```
   column.1.valueformat=HTML
   ```

   ```
   column.2.value=<br>
   ```

   ```
   column.2.width=1
   ```

   ```
   column.2.valueformat=HTML
   ```

   ```
   column.2.sharecol=true
   ```

   ```
   column.3.valuefield=plannedStartDate
   ```

   ```
   column.3.valueformat=atDate
   ```

   ```
   column.3.sharecol=true
   ```

   ```
   column.4.value=<br>
   ```

   ```
   column.4.width=1
   ```

   ```
   column.4.valueformat=HTML
   ```

   ```
   column.4.sharecol=true
   ```

   ```
   column.5.textmode=true
   ```

   ```
   column.5.valuefield=owner:name
   ```

   ```
   column.5.valueformat=HTML
   ```

   <pre><img src="assets/shared-column-with-line-breaks-350x199.png" style="width: 350;height: 199;"></pre>

1. Clique em **Salvar**, depois **Salvar visualização**.
