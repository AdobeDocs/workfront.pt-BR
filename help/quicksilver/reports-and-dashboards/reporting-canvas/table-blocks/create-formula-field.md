---
title: Criar um campo de fórmula na Tela de relatórios
description: Criar um campo de fórmula na Tela de relatórios
author: Nolan
draft: Probably
feature: Reports and Dashboards
exl-id: 22a2c3d7-39db-4f5d-94f3-222ca3ee0615
source-git-commit: d649decb2875a3af4fd40c323a7836d4468bf04b
workflow-type: tm+mt
source-wordcount: '653'
ht-degree: 7%

---


# Criar um campo de fórmula na Tela de relatórios

O construtor de campos na Tela de relatórios permite criar campos que executam cálculos personalizados.

## Pré-requisitos

Antes de começar, você deve se inscrever no beta da Tela de relatórios. Para obter mais informações, consulte [Beta da Tela de Relatório: visão geral](/help/quicksilver/product-announcements/betas/reporting-canvas-beta/reporting-canvas-beta-overview.md).

## Criar um campo de fórmula

1. Crie ou navegue até um bloco de tabela, conforme descrito em [Adicionar ou editar um bloco de tabela na Tela de relatórios](../../../reports-and-dashboards/reporting-canvas/table-blocks/add-or-edit-report-table.md).
1. No cabeçalho da tabela no relatório, clique no botão **Editar** ícone ![](assets/edit-icon.png).

   ![](assets/edit-icon-table-header-350x71.png)

   >[!NOTE]
   >
   >Se você acabou de criar a tabela e ainda não adicionou nenhum campo, clique no botão Edit no centro da tabela.

1. Clique em **Novo +** na parte superior do **Campos** no painel direito.
1. Na nova página que será aberta, clique no botão **Editar** ícone ![](assets/edit-icon.png) ao lado do nome do campo no canto superior esquerdo para alterar o nome do campo de fórmula.
1. Arrastar **Funções** ou **Campos** do painel esquerdo ao construtor de campos no centro para adicioná-los ao campo de fórmula.


   >[!TIP]
   >
   >À medida que você cria o campo da fórmula, a variável **Visualização do campo** à direita exibe exemplos do campo resultante.

   Cada função contém um número de retângulos pontilhados vazios que serão usados como argumentos no cálculo de um resultado. Elas podem ser preenchidas inserindo texto ou números estáticos, arrastando e soltando um campo do painel esquerdo (usando o valor do campo no cálculo) ou arrastando e soltando outra função (criando uma função aninhada). As possíveis funções incluem:

   | Função | Descrição | Saída |
   |---|---|---|
   | SE | Compare dois argumentos com base em um modificador selecionado e execute uma ação especificada com base no valor True (Is True:) ou False (Is False:) resultante. Observação: no momento, o segundo argumento não pode ser um valor estático Verdadeiro ou Falso. Em vez disso, você pode usar uma função aninhada como ISBLANK (Nome do projeto) que sempre retorna False como uma solução alternativa. | Verdadeiro/Falso, Data, Número ou Sequência |
   | CONCAT | Mescle duas ou mais strings juntas de ponta a ponta para criar uma nova string. | String |
   | CONTÉM | Avalie se um campo de argumento de string (Texto localizado) estiver contido em outro campo de argumento de string (Dentro do texto). | Verdadeiro/Falso |
   | EM | Avaliar se o valor de um campo de argumento (Localizar) corresponder ao valor de pelo menos um outro campo de argumento (Dentro) | Verdadeiro/Falso |
   | ISBLANK | Avalie se um campo de argumento estiver em branco. | Verdadeiro/Falso |
   | LEN | Meça o comprimento (em número de caracteres) de um campo de argumento. | Número |
   | ROUND | Retorna um número arredondado com base na precisão selecionada. | Número |
   | FLOOR | Retorna o número inteiro mais próximo, arredondado para baixo. | Número |
   | NÚMERO | Retorna o maior interger menor que o valor de um argumento numérico (idêntico a uma função Floor ). | Número |
   | STRING | Converte o conteúdo de um campo de argumento em uma string | String |
   | SUBSTR | Crie uma nova string a partir de uma string maior, que contenha os caracteres entre um número de índice (Início) e outro (Fim). | String |
   | ESQUERDO | Crie uma nova string a partir de uma string maior, que contenha caracteres começando pela extremidade esquerda e contando à direita um número de caracteres (Comprimento). | String |
   | DIREITO | Crie uma nova string a partir de uma string maior, que contém caracteres começando pela extremidade direita e contando um número de caracteres (comprimento) deixado. | String |
   | SUM | Adicione os valores de dois ou mais campos de argumento juntos. | Número |
   | SUB | Subtraia os valores de dois ou mais campos de argumento (na ordem da esquerda para a direita). | Número |
   | PROD | Multiplica os valores de dois ou mais campos de argumento juntos. | Número |
   | DIV | Divida o valor de dois ou mais campos de argumento (em ordem da esquerda para a direita). | Número |
   | MÊS | Retorna um número igual ao valor do mês de uma data. | Número |
   | ANO | Retorna um número igual ao valor do ano de uma data. | Número |
   | DATEDIFF | Calcula o número total de dias entre duas datas, arredondado para uma casa decimal. | Número |
   | WEEKDAYDIFF | Calcula o número de dias da semana entre duas datas, arredondado para uma casa decimal. | Número |

   {style="table-layout:auto"}

1. Clique no botão **Voltar** no canto superior esquerdo da tela para retornar à tabela.
