---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Exibição: Mesclar Informações de Várias Colunas em Uma Coluna Compartilhada'
description: É possível mesclar as informações exibidas em várias colunas separadas e exibi-las em uma coluna compartilhada.
author: Nolan
feature: Reports and Dashboards
exl-id: d4f9db12-59ce-4cfc-90dd-e611b49fafdf
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '1070'
ht-degree: 0%

---

# Exibição: mesclar informações de várias colunas em uma coluna compartilhada

<!-- Audited: 11/2024 -->

É possível mesclar as informações exibidas em várias colunas separadas e exibi-las em uma coluna compartilhada.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacote do Adobe Workfront</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td> 
   <p>Colaborador ou Solicitação para modificar uma exibição </p>
   <p>Padrão ou Plano para modificar um relatório</p>
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Editar acesso a relatórios, painéis e calendários para modificar um relatório</p> <p>Editar acesso a Filtros, Visualizações, Agrupamentos para modificar uma visualização</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões para um relatório</p>  </td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).


+++

## Considerações ao compartilhar ou mesclar colunas

* Você pode mesclar duas colunas adjacentes e exibir as informações de cada coluna separadas por uma quebra de linha, ou pode mesclar as informações em duas colunas adjacentes sem separador entre as informações de cada coluna.
* É possível mesclar as informações de mais de duas colunas aplicando a mesma sintaxe descrita neste artigo a uma coluna já compartilhada e a uma coluna adjacente.
* A linha `valueformat=HTML` é obrigatória em uma coluna compartilhada. Caso contrário, as colunas não conterão informações (estarão em branco) quando o relatório for exportado do Adobe Workfront.
* A formatação condicional pode não ser suportada em colunas mescladas.

  As seguintes exceções existem:

   * Ao exibir informações no Workfront, a formatação da primeira coluna é mantida e a formatação de todas as outras colunas é ignorada se as colunas que compõem uma coluna mesclada tiverem formatação diferente umas das outras,.
   * Ao exportar a exibição para um arquivo PDF, a formatação condicional se aplica à primeira coluna em uma coluna mesclada.
   * Ao exportar a exibição para um arquivo do Excel, as colunas mescladas são exibidas como colunas separadas. As colunas individuais também exibem suas respectivas regras de formatação condicional.

* As colunas com o atributo **viewalias** podem limitar a quantidade de colunas que podem ser mescladas. Para evitar esses limites, evite usar o atributo **viewalias**. Se você precisar incluir o atributo **viewalias** em uma coluna, verifique se ele é o último item listado na coluna.

* Se você exportar uma lista com colunas compartilhadas para um formato Excel ou Delimitado por tabulação, essas colunas serão separadas no arquivo exportado.

* Quando uma ou ambas as colunas exibem um campo do tipo `tile`, uma quebra de linha forçada é introduzida automaticamente na coluna mesclada. Por exemplo, Campos de Texto com Formatação são campos do tipo `tile`. Nesse caso, há um código de linha de `type=tile` ao visualizar as colunas no Modo de texto.

## Mesclar dados de duas colunas sem uma quebra de linha

É possível mesclar os dados de várias colunas separadas para exibi-los em uma coluna sem quebras ou espaços entre os valores de cada coluna.

>[!TIP]
>
>Essa abordagem é recomendada ao mesclar duas colunas que nunca podem mostrar um valor para o mesmo registro ao mesmo tempo. Por exemplo, em um relatório de Item de trabalho, as colunas Nome da ocorrência e Nome da tarefa podem ser mescladas sem uma quebra de linha entre elas, porque um Item de trabalho nunca pode ter um Nome da ocorrência e um Nome da tarefa ao mesmo tempo. Um Item de trabalho pode ser um Problema ou uma Tarefa no Workfront.

Para mesclar dados de duas colunas sem uma quebra de linha:

1. Ir para uma lista de objetos.
1. No menu suspenso **Exibir**, selecione um modo de exibição e clique no **ícone Editar** ![ícone Editar](assets/edit-icon.png) para editar o modo de exibição.
1. Vá para a primeira coluna que deseja mesclar e clique em **Alternar para Modo de Texto** > **Editar Modo de Texto**.
1. Adicione o seguinte texto à primeira coluna que deseja mesclar:

   `sharecol=true`

   Ao mesclar as duas primeiras colunas de uma lista ou relatório, o Workfront precede cada linha de texto que contém informações sobre o objeto na primeira coluna com `column.0.` e as linhas de texto que contêm informações sobre a segunda coluna com `column.1.`.

   Você deve preceder o número da primeira coluna com o número dessa coluna. A contagem de colunas sempre começa com a coluna mais à esquerda da lista ou relatório rotulado como `column.0.`.

   Se você compartilhar mais de uma coluna, adicione o número da coluna nas linhas de código que contêm as informações de compartilhamento para cada coluna.


   **EXEMPLO:** este é o código do modo de texto para uma coluna mesclada que contém três colunas separadas, começando com a segunda coluna da lista. Os valores mesclados são Nome do projeto, Data de início planejada e nome do Proprietário do projeto, e não há interrupção entre os três valores:

   ```
   column.1.valuefield=name
   column.1.valueformat=HTML
   column.1.sharecol=true
   column.2.valuefield=plannedStartDate
   column.2.valueformat=atDate
   column.2.sharecol=true
   column.3.valuefield=owner:name
   column.3.valueformat=HTML
   ```

   ![Coluna compartilhada sem quebras de linha](assets/shared-column-no-line-breaks-350x142.png)


1. Clique em **Concluído** e depois em **Salvar exibição**.

## Mesclar dados de duas colunas com uma quebra de linha

Faça o seguinte para mesclar os dados de várias colunas para exibi-los em uma coluna comum com uma quebra de linha entre os valores de cada coluna:

1. Ir para uma lista de objetos.
1. No menu suspenso **Exibir**, selecione um modo de exibição e clique no **ícone Editar** ![ícone Editar](assets/edit-icon.png) para editar o modo de exibição.
1. Adicione uma terceira coluna entre as duas colunas que deseja mesclar.

   >[!TIP]
   >
   >* As colunas que você deseja mesclar devem ser adjacentes entre si.
   >* Você deve clicar na primeira coluna que deseja mesclar.

1. Clique em **Alternar para Modo de Texto** > **Editar Modo de Texto** e adicione o seguinte código na coluna do meio que você adicionou na etapa 1:

   ```
   value=<br>
   valueformat=HTML
   width=1
   sharecol=true
   ```

1. Clique na primeira coluna e clique em **Alternar para Modo de Texto** > **Editar Modo de Texto** e, em seguida, adicione o seguinte texto à coluna:

   `sharecol=true`

   Ao mesclar as duas primeiras colunas de uma lista ou relatório, o Workfront precede cada linha de texto que contém informações sobre o objeto na primeira coluna com `column.0.`, a coluna com as informações de compartilhamento com `column.1.` e as linhas de texto que contêm informações sobre a segunda coluna com `column.2.`.

   Se a coluna combinada estiver no meio da exibição, as colunas serão numeradas de acordo com seu local na exibição. A contagem de colunas sempre começa com a coluna mais à esquerda da lista ou relatório rotulado como `column.0.`.

   Se você compartilhar mais de uma coluna, adicione o número da coluna nas linhas de código que contêm as informações de compartilhamento.

   **EXEMPLO:** este é o código do modo de texto para uma coluna compartilhada que contém o Nome do Projeto, a Data de Início Planejada e o nome do Proprietário do Projeto com uma quebra de linha. A coluna compartilhada é a segunda coluna de uma exibição de projeto.

   ```
   column.1.displayname=Project_StartDate_Owner
   column.1.sharecol=true
   column.1.textmode=true
   column.1.valuefield=name
   column.1.valueformat=HTML
   column.2.value=<br>
   column.2.width=1
   column.2.valueformat=HTML
   column.2.sharecol=true
   column.3.valuefield=plannedStartDate
   column.3.valueformat=atDate
   column.3.sharecol=true
   column.4.value=<br>
   column.4.width=1
   column.4.valueformat=HTML
   column.4.sharecol=true
   column.5.textmode=true
   column.5.valuefield=owner:name
   column.5.valueformat=HTML 
   ```

   ![Coluna compartilhada com quebras de linha](assets/shared-column-with-line-breaks-350x199.png)

1. Clique em **Concluído** e depois em **Salvar exibição**.
