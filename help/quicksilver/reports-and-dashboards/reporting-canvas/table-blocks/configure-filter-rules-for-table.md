---
title: Filtrar uma tabela na Tela de relatório
description: Filtrar uma tabela na Tela de relatório
author: Nolan
draft: Probably
feature: Reports and Dashboards
exl-id: 1838b142-d845-4795-b27f-80bfba18e9d4
hidefromtoc: true
hide: true
source-git-commit: a9c36ff874d3272e1d2de70578c420af29b9d44c
workflow-type: tm+mt
source-wordcount: '857'
ht-degree: 2%

---


# Filtrar uma tabela na Tela de relatório

Depois de adicionar um bloco de tabela a um relatório, é possível configurar filtros para limitar as informações exibidas na tabela.

Há três componentes em uma regra de filtro:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Campo</td> 
   <td> <p>O campo que contém as informações pelas quais você deseja filtrar sua tabela.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Operador</td> 
   <td> <p>A forma como o filtro determina quais valores de campo são incluídos ou excluídos da tabela. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Valor</td> 
   <td> <p>Os valores no campo selecionado são avaliados de acordo com o operador.</p> </td> 
  </tr> 
 </tbody> 
</table>

**Exemplo:** Se quiser limitar os resultados no relatório para exibir apenas os projetos pertencentes à Jane Doe, crie uma regra de filtro com o campo &quot;Proprietário do projeto&quot;, o operador &quot;Igual a&quot; e o valor &quot;Jane Doe&quot;.

Ou você pode exibir somente projetos que tenham um proprietário de projeto atribuído, que teria o campo &quot;Proprietário do projeto&quot; e o operador &quot;Não está em branco&quot;.

## Pré-requisitos

Antes de começar, você deve se inscrever na versão beta da Tela de relatório. Para obter mais informações, consulte [Versão beta do relatório do Canvas: visão geral](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/reporting-canvas-beta-overview.md).

## Configurar regras de filtro para uma tabela

1. Clique em **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront e clique em **Relatórios**.

1. Clique em **Novo relatório**.

   Ou

   Vá para um relatório existente, clique no link **Menu Mais** ícone ![](assets/more-icon.png) no cabeçalho do relatório, selecione **Editar**.

1. Para agrupar linhas em uma nova tabela, arraste ou clique duas vezes em um bloco de tabela na tela.

   Ou

   Para agrupar linhas em uma tabela existente, clique no **Editar** ícone ![](assets/edit-icon.png) no cabeçalho da tabela.

1. No painel direito, localize o campo pelo qual deseja filtrar a tabela e arraste-o para a seção Filtro.

   Um conjunto de regras de filtro é exibido com o nome do campo selecionado.

1. Selecione o operador desejado no menu suspenso:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Igual a</strong> </td> 
      <td> <p>Isso só retorna uma correspondência exata do valor pesquisado.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Não Igual a</strong> </td> 
      <td> <p>Isso só retorna resultados que não são correspondências exatas do valor pesquisado.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Blank</strong> </td> 
      <td> <p>O campo existe para o objeto, mas o campo ainda não recebeu um valor.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Não Branco</strong> </td> 
      <td> <p>O campo que você está filtrando existe e recebeu um valor.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>É menor que</strong> </td> 
      <td> <p>Pesquisa todos os resultados com um valor menor do que o inserido, sem incluir o valor inserido.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>É menor que ou igual a</strong> </td> 
      <td> <p>Pesquisa todos os resultados com um valor menor ou igual ao valor inserido.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>É maior que</strong> </td> 
      <td> <p>Pesquisa todos os resultados com um valor maior que o valor inserido, sem incluir o valor inserido.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>É maior que ou igual a</strong> </td> 
      <td> <p>Pesquisa todos os resultados com valores maiores ou iguais ao valor inserido.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Entre</strong> </td> 
      <td> <p>Fornece dois valores de campo obrigatórios e pesquisa todos os resultados na faixa de ambos os campos, incluindo os valores inseridos.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Contém</strong> </td> 
      <td> <p>Pesquisa o texto especificado em uma cadeia de caracteres de texto inteira.</p> <p>Por exemplo, usar "Contém Inf" captura qualquer coisa com "Inf" ou "inf", como a palavra "Infinito".</p> <p>Observação: O Adobe Workfront pesquisa a palavra ou frase inteira que você informa para cada regra de filtro. Por exemplo, se você estiver procurando campos com a frase "novo projeto" no nome, o Workfront não exibirá projetos que tenham somente "novo" ou "projeto" no nome ou frases que contenham palavras extras entre eles, como "novo projeto principal". O filtro localiza somente projetos com a frase exata "novo projeto" no nome.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Não Contém</strong> </td> 
      <td> <p>Isso filtra os itens que não têm texto especificado.</p> <p>Por exemplo, "não contém inf" retorna qualquer campo sem "Inf" ou "inf" em seus nomes.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Insira o último valor para concluir a regra de filtro, com base no operador selecionado.

   >[!NOTE]
   >
   >Os valores inseridos aqui são **não** distinção entre maiúsculas e minúsculas.

1. (Opcional) Para adicionar outra regra de filtro ao seu conjunto de regras, faça o seguinte:

   1. Arraste outro campo para a **Solte para adicionar outra regra** na seção Filtros abaixo da outra regra.
   1. Repita as etapas 4 a 6.
   1. Na lista suspensa de operadores à esquerda da nova regra, selecione **E** ou **OU**.

      <table style="table-layout:auto"> 
       <col> 
       </col> 
       <col> 
       </col> 
       <tbody> 
        <tr> 
         <td role="rowheader"> <p>E</p> </td> 
         <td> <p>Ao unir regras de filtro ou conjuntos de regras com o operador AND, você indica que deseja que todas as regras do mesmo nível sejam atendidas.</p> <p>Por padrão, as instruções em um filtro são unidas pelo operador AND.</p> </td> 
        </tr> 
        <tr> 
         <td role="rowheader"> <p>OU</p> </td> 
         <td> <p>Ao unir regras de filtro ou conjunto de regras com o operador OR, você indica que deseja <strong>pelo menos</strong> uma regra, ou conjunto de regras, nesse nível a ser atendido.</p> </td> 
        </tr> 
       </tbody> 
      </table>

      >[!IMPORTANT]
      >
      >Os operadores AND e OR no mesmo nível (conectar várias regras em um conjunto de regras ou conjuntos de regras inteiros juntos) sempre corresponderão. Por exemplo, se você alterar o operador entre duas regras em um conjunto de regras, todos os outros operadores nesse conjunto de regras serão alterados automaticamente para corresponder a ele.

1. (Condicional) Para adicionar um conjunto de regras de filtro adicional, faça o seguinte:

   1. Arraste o campo que deseja adicionar à **Adicionar um conjunto de regras** abaixo dos outros conjuntos de regras de filtro.
   1. Repita as etapas 4 a 7.
   1. Na lista suspensa de operadores à esquerda do novo conjunto de regras, selecione **E** ou **OU**. Esses operadores funcionam da mesma forma que os listados na Etapa 7, mas se aplicam a conjuntos de regras inteiros, não a regras individuais em um conjunto.****
