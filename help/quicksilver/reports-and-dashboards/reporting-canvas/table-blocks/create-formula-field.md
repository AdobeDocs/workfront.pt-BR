---
title: Criar um campo de fórmula na Tela de relatório
description: Criar um campo de fórmula na Tela de relatório
hidefromtoc: true
hide: true
source-git-commit: 350d64577bac677bb0cc9bcb804c32b0301bc5d4
workflow-type: tm+mt
source-wordcount: '653'
ht-degree: 7%

---


# Criar um campo de fórmula na Tela de relatório

O construtor de campos na Tela de relatório permite criar campos que executam cálculos personalizados.

## Pré-requisitos

Antes de começar, você deve se inscrever na versão beta da Tela de relatório. Para obter mais informações, consulte [Versão beta do relatório do Canvas: visão geral](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/reporting-canvas-beta-overview.md).

## Criar um campo de fórmula

1. Crie ou navegue até um bloco de tabela, conforme descrito em [Adicionar ou editar um bloco de tabela na Tela de relatório](../../../reports-and-dashboards/reporting-canvas/table-blocks/add-or-edit-report-table.md).
1. No cabeçalho da tabela do relatório, clique na guia **Editar** ícone ![](assets/edit-icon.png).

   ![](assets/edit-icon-table-header-350x71.png)

   >[!NOTE]
   >
   >Se você acabou de criar a tabela e ainda não adicionou nenhum campo, clique no botão Editar no centro da tabela.

1. Clique em **Novo +** na parte superior do **Campos** no painel direito.
1. Na nova página que é aberta, clique no link **Editar** ícone ![](assets/edit-icon.png) ao lado do nome do campo no canto superior esquerdo para alterar o nome do campo da fórmula.
1. Arrastar **Funções** ou **Campos** no painel esquerdo, acesse o construtor de campos no centro para adicioná-los ao campo de fórmula.


   >[!TIP]
   >
   >À medida que você cria o campo de fórmula, a variável **Visualização do campo** à direita, são exibidos exemplos do campo resultante.

   Cada função contém um número de retângulos pontilhados vazios que serão usados como argumentos no cálculo de um resultado. Esses podem ser preenchidos inserindo texto ou números estáticos, arrastando e soltando um campo do painel esquerdo (usando o valor do campo no cálculo) ou arrastando e soltando outra função (criando uma função aninhada). As possíveis funções incluem:

   | Função | Descrição | Output |
   |---|---|---|
   | SE | Compare dois argumentos com base em um modificador selecionado e execute uma ação especificada com base no valor resultante True (Is True:) ou False (Is False:). Observação: no momento, o segundo argumento não pode ser um valor estático Verdadeiro ou Falso. Em vez disso, você pode usar uma função aninhada como ISBLANK(Nome do projeto) que sempre retorna Falso como solução alternativa. | Verdadeiro/Falso, Data, Número ou String |
   | CONCAT | Mescle duas ou mais cadeias de caracteres juntas de ponta a ponta para criar uma nova cadeia de caracteres. | String |
   | CONTÉM | Avaliar se um campo de argumento de sequência (Localizar texto) está contido em outro campo de argumento de sequência (No texto). | Verdadeiro/Falso |
   | EM | Avaliar se o valor de um campo de argumento (Localizar) corresponde ao valor de pelo menos um outro campo de argumento (Dentro) | Verdadeiro/Falso |
   | ISBLANK | Avalie se um campo de argumento está em branco. | Verdadeiro/Falso |
   | LEN | Meça o comprimento (em número de caracteres) de um campo de argumento. | Número |
   | ROUND | Retorna um número arredondado com base na precisão selecionada. | Número |
   | FLOOR | Retorna o número inteiro mais próximo, arredondado para baixo. | Número |
   | NÚMERO | Retorna o maior número inteiro menor que o valor de um argumento numérico (idêntico a uma função Floor). | Número |
   | STRING | Converte o conteúdo de um campo de argumento em uma string | String |
   | SUBSTR | Cria uma nova cadeia de caracteres a partir de uma cadeia maior, que contém os caracteres entre um número de índice (Início) e outro (Fim). | String |
   | ESQUERDO | Cria uma nova cadeia de caracteres a partir de uma cadeia maior, que contém caracteres começando pela extremidade esquerda e contando à direita um número de caracteres (Comprimento). | String |
   | DIREITO | Cria uma nova cadeia de caracteres a partir de uma cadeia maior, que contém caracteres começando pela extremidade direita e contando à esquerda um número de caracteres (Comprimento). | String |
   | SUM | Adicione os valores de dois ou mais campos de argumento juntos. | Número |
   | SUB | Subtraia os valores de dois ou mais campos de argumento (da esquerda para a direita). | Número |
   | PROD | Multiplique os valores de dois ou mais campos de argumento. | Número |
   | DIV | Divida o valor de dois ou mais campos de argumento (da esquerda para a direita). | Número |
   | MÊS | Retorna um número igual ao valor do mês de uma data. | Número |
   | ANO | Retorna um número igual ao valor de ano de uma data. | Número |
   | DATEDIFF | Calcula o número total de dias entre duas datas, arredondado para uma casa decimal. | Número |
   | WEEKDAYDIFF | Calcula o número de dias da semana entre duas datas, arredondado para uma casa decimal. | Número |

   {style="table-layout:auto"}

1. Clique em **Voltar** seta no canto superior esquerdo da tela para retornar à tabela.
