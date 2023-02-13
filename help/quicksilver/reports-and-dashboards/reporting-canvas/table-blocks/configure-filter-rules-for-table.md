---
title: Filtrar uma tabela na Tela de relatórios
description: Filtrar uma tabela na Tela de relatórios
author: Nolan
draft: Probably
feature: Reports and Dashboards
exl-id: 1838b142-d845-4795-b27f-80bfba18e9d4
source-git-commit: 61fcb4c3646f60fa5f667d874af3320360d5d286
workflow-type: tm+mt
source-wordcount: '857'
ht-degree: 1%

---


# Filtrar uma tabela na Tela de relatórios

Após adicionar um bloco de tabela a um relatório, é possível configurar filtros para limitar as informações exibidas na tabela.

Há 3 componentes em uma regra de filtro:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Campo</td> 
   <td> <p>O campo que contém as informações pelas quais você deseja filtrar a tabela .</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Operador</td> 
   <td> <p>A forma como o filtro determina em quais valores de campo são incluídos ou excluídos da tabela. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Valor</td> 
   <td> <p>Os valores no campo selecionado que são avaliados de acordo com o operador.</p> </td> 
  </tr> 
 </tbody> 
</table>

**Exemplo:** Se você quiser limitar os resultados em seu relatório para exibir apenas projetos de propriedade da Jane Doe, poderá criar uma regra de filtro com o campo &quot;Proprietário do projeto&quot;, o operador &quot;Igual a&quot; e o valor &quot;Jane Doe&quot;.

Ou você pode exibir apenas projetos que tenham um proprietário de projeto atribuído, que teria o campo &quot;Proprietário do projeto&quot; e o operador &quot;Não está em branco&quot;.

## Pré-requisitos

Antes de começar, você deve se inscrever no beta da Tela de relatórios. Para obter mais informações, consulte [Beta da Tela de Relatório: visão geral](/help/quicksilver/product-announcements/betas/reporting-canvas-beta/reporting-canvas-beta-overview.md).

## Configurar regras de filtro para uma tabela

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront, em seguida, clique em **Relatório**.

1. Clique em **Novo relatório**.

   Ou

   Vá para um relatório existente, clique no botão **Mais Menu** ícone ![](assets/more-icon.png) no cabeçalho do relatório, selecione **Editar**.

1. Para agrupar linhas em uma nova tabela, arraste ou clique duas vezes em um bloco de tabela na tela.

   Ou

   Para agrupar linhas em uma tabela existente, clique no botão **Editar** ícone ![](assets/edit-icon.png) no cabeçalho da tabela.

1. No painel direito, localize o campo pelo qual deseja filtrar a tabela e arraste-o para a seção Filtro .

   Um conjunto de regras de filtro é exibido com o nome do campo selecionado.

1. Selecione o operador desejado no menu suspenso:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Igual a</strong> </td> 
      <td> <p>Isso retorna somente uma correspondência exata do valor pesquisado.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Diferente de</strong> </td> 
      <td> <p>Isso retorna somente resultados que não são correspondências exatas do valor pesquisado.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Blank</strong> </td> 
      <td> <p>O campo existe para o objeto, mas o campo ainda não recebeu um valor.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Não Branco</strong> </td> 
      <td> <p>O campo para o qual você está filtrando existe e recebeu um valor.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Is Less Than</strong> </td> 
      <td> <p>Isso pesquisa todos os resultados com um valor menor que o inserido, sem incluir o valor inserido.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Is Less Than Or Equal To</strong> </td> 
      <td> <p>Isso pesquisa todos os resultados com um valor menor ou igual ao valor inserido.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Is Greater Than</strong> </td> 
      <td> <p>Isso pesquisa todos os resultados com um valor maior que o valor inserido, sem incluir o valor inserido.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Is Greater Than Or Equal To</strong> </td> 
      <td> <p>Isso pesquisa todos os resultados com valores maiores ou iguais ao valor inserido.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Entre</strong> </td> 
      <td> <p>Fornece 2 valores de campo obrigatórios e pesquisa por todos os resultados dentro do intervalo de ambos os campos, incluindo os valores inseridos.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Contém</strong> </td> 
      <td> <p>Isso pesquisa o texto especificado em uma string de texto inteira.</p> <p>Por exemplo, usar "Contém Inf" captura qualquer coisa com "Inf" ou "inf" nela, como a palavra "Infinity".</p> <p>Observação: O Adobe Workfront pesquisa toda a palavra ou frase inserida para cada regra de filtro. Por exemplo, se você estiver procurando por campos com a frase "novo projeto" em seu nome, o Workfront não exibirá projetos que tenham apenas "novo" ou "projeto" em seus nomes, ou frases que contenham palavras extras entre elas, como "novo projeto principal". O filtro encontra apenas projetos com a frase exata "novo projeto" no nome.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Não Contém (Distingue maiúsc. e minúsc.)</strong> </td> 
      <td> <p>Isso filtra itens cujo texto especificado está ausente.</p> <p>Por exemplo, "não contém inf" retorna qualquer campo sem "Inf" ou "inf" em seus nomes.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Insira o último valor para concluir a regra de filtro, com base no operador selecionado.

   >[!NOTE]
   >
   >Os valores inseridos aqui são **not** diferencia maiúsculas de minúsculas.

1. (Opcional) Para adicionar outra regra de filtro ao seu conjunto de regras, faça o seguinte:

   1. Arraste outro campo para a **Soltar para adicionar outra regra** na seção Filtros abaixo de sua outra regra.
   1. Repita as etapas 4 a 6.
   1. Na lista suspensa do operador à esquerda da nova regra, selecione **E** ou **OU**.

      <table style="table-layout:auto"> 
       <col> 
       </col> 
       <col> 
       </col> 
       <tbody> 
        <tr> 
         <td role="rowheader"> <p>AND</p> </td> 
         <td> <p>Ao associar regras de filtragem ou conjuntos de regras ao operador AND, você indica que deseja que todas as regras do mesmo nível sejam atendidas.</p> <p>Por padrão, as instruções em um filtro são unidas pelo operador AND .</p> </td> 
        </tr> 
        <tr> 
         <td role="rowheader"> <p>OU</p> </td> 
         <td> <p>Ao associar regras de filtragem ou conjunto de regras ao operador OU, você indica que deseja <strong>pelo menos</strong> uma regra - ou conjunto de regras - nesse nível a ser atendido.</p> </td> 
        </tr> 
       </tbody> 
      </table>

      >[!IMPORTANT]
      >
      >Operadores AND e OR no mesmo nível — conectando várias regras em um conjunto de regras ou conjuntos de regras inteiros — sempre corresponderão. Por exemplo, se você alterar o operador entre duas regras em um conjunto de regras, todos os outros operadores nesse conjunto de regras serão alterados automaticamente para corresponderem a ele.

1. (Condicional) Para adicionar um conjunto de regras de filtro adicional, faça o seguinte:

   1. Arraste o campo que deseja adicionar à variável **Adicionar um conjunto de regras** abaixo de seus outros conjuntos de regras de filtro.
   1. Repita as Etapas 4-7.
   1. Na lista suspensa do operador à esquerda do novo conjunto de regras, selecione **E** ou **OU**. Esses operadores funcionam da mesma forma que os listados na Etapa 7, mas se aplicam a conjuntos de regras inteiros, ao contrário de regras individuais em um conjunto.****
