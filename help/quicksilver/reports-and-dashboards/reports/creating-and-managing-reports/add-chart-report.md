---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Adicionar um gráfico a um relatório
description: Você pode aprimorar seus relatórios adicionando um gráfico. É possível adicionar gráficos a relatórios existentes ou a relatórios que você está criando.
author: Nolan
feature: Reports and Dashboards
exl-id: 9b58d68c-4b7b-4344-bde3-7c65e2e1aac8
source-git-commit: 68d93ccb8b96f802ef0a612e7e41cf168e34e863
workflow-type: tm+mt
source-wordcount: '2757'
ht-degree: 0%

---

# Adicionar um gráfico a um relatório

<!--Audited: 01/2024-->

Você pode aprimorar seus relatórios adicionando um gráfico. É possível adicionar gráficos a relatórios existentes ou a relatórios que você está criando.

Antes de adicionar um gráfico a um relatório, você deve criar uma Exibição e um Agrupamento para o relatório.

Não é possível adicionar gráficos à maioria dos relatórios, a menos que você agrupe as informações no relatório primeiro. O único gráfico que pode ser adicionado sem um agrupamento é um gráfico de medidor.

Para obter informações sobre exibições, consulte [Visão geral das exibições no Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

Para obter mais informações sobre agrupamentos, consulte [Visão geral de agrupamentos no Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

Se o relatório exibir muitos itens, um gráfico não será criado. Nesse caso, você também deve adicionar um Filtro ao relatório para reduzir o número de resultados em seu relatório.

Para obter mais informações sobre filtros, consulte [Visão geral dos filtros](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Atual: Plano </p>
   Ou
   <p>Novo: Padrão</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuração do nível de acesso</td> 
   <td> <p>Editar acesso a relatórios, painéis, calendários</p> <p>Editar acesso a Filtros, Visualizações, Agrupamentos</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões para um relatório</p>  </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir seu plano, tipo de licença ou acesso, entre em contato com o administrador do Workfront. Para obter mais informações sobre requisitos de acesso, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Adicionar um gráfico a um relatório

1. Ir para um relatório existente ou criar um novo relatório. Para obter mais informações sobre como criar um novo relatório, consulte [Criar um relatório personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
1. (Condicional) Se você foi para um relatório existente, clique em **Ações de Relatório** > **Editar**.

1. Certifique-se de que o **Colunas (Exibir)** A guia foi atualizada para exibir as informações que você deseja inserir no gráfico do relatório.

   Para obter informações sobre como criar ou modificar a Exibição do relatório, consulte [Criar ou editar exibições no Adobe Workfront](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-edit-views.md).

1. Clique em **Agrupamentos** e adicione um agrupamento.

   >[!TIP]
   >
   >* Você só pode adicionar um gráfico a um relatório quando os resultados do relatório são agrupados.
   >* Os agrupamentos em modo de texto não são suportados em gráficos. Para obter mais informações sobre agrupamentos em modo de texto, consulte [Modo de edição de texto em um agrupamento](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-grouping.md).
   >* Se você adicionar um único agrupamento que representa uma métrica, todos os gráficos, exceto um gráfico de pizza, serão exibidos no agrupamento com a mesma cor.

   Para obter mais informações sobre a criação de agrupamentos, consulte [Criar agrupamentos no Adobe Workfront](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-groupings.md).

1. Selecione o **Gráfico** guia.
1. Clique em um tipo de gráfico para selecioná-lo.\
   ![](assets/qs-report-builder-chart-350x265.png)

1. Selecione entre os seguintes tipos de gráficos:

   * [Gráfico de colunas](#column-chart)
   * [Gráfico de barras](#bar-chart)
   * [Gráfico de pizza](#pie-chart)
   * [Gráfico de linhas](#line-chart)
   * [Gráfico de medição](#gauge-chart)
   * [Gráfico de bolhas](#bubble-chart)

1. Clique em **Salvar + Fechar** para salvar o gráfico e o relatório.

### Gráfico de colunas {#column-chart}

Para adicionar um **Coluna** gráfico para o seu relatório:

1. Comece a adicionar um gráfico ao seu relatório, conforme descrito em [Adicionar um gráfico a um relatório](#add-a-chart-to-a-report).
1. No **Eixo esquerdo (Y)** , selecione os valores que deseja incluir no eixo Y do gráfico, bem como a forma como deseja que as informações sejam resumidas.
1. No **Eixo inferior (X)** selecione o Grouping que deseja incluir no gráfico.
1. (Opcional) Selecione **Cores Personalizadas** para atribuir suas cores preferidas a cada uma das colunas.\
   Para obter mais informações sobre como personalizar as cores do gráfico, consulte [Personalizar cores do gráfico](#customize-chart-colors).

1. (Opcional) Selecione **Mostrar em 3D** para exibir o gráfico em uma exibição tridimensional.
1. (Opcional) **Colunas de grupo**: selecione esta opção para definir como deseja que as colunas sejam agrupadas.\
   Selecione entre as seguintes opções:

   * Clique em uma das seguintes opções para selecionar como as colunas agrupadas serão exibidas:

      * **Lado a lado**
      * **Empilhado**
      * **Empilhado a 100%**

   * Selecione o Agrupamento que deseja incluir no gráfico na **Agrupar dados por** menu suspenso.
   * (Opcional) Selecione **Cores Personalizadas** para personalizar as cores das colunas.\
     Para obter mais informações sobre como personalizar as cores do gráfico, consulte [Personalizar cores do gráfico](#customize-chart-colors).

1. (Opcional) Selecione **Gráfico Combinado** para incluir um valor adicional no gráfico, bem como a forma como você deseja que as informações sejam resumidas.\
   Considere as seguintes opções:

   * **Plotar no eixo secundário**: selecione essa opção para plotar os dados no lado direito do gráfico.
   * **Tipo de gráfico**: selecione se deseja que esse valor adicional seja exibido como uma linha ou uma terceira coluna.\
     ![](assets/qs-column-chart-350x163.png)

1. Clique em **Salvar + Fechar** para salvar o gráfico e o relatório.

### Gráfico de barras {#bar-chart}

Para adicionar um **Barra** gráfico para o seu relatório:

1. Comece a adicionar um gráfico ao seu relatório, conforme descrito em [Adicionar um gráfico a um relatório](#add-a-chart-to-a-report).
1. No **Eixo inferior (X)** , selecione os valores que deseja incluir no eixo X do gráfico, bem como a forma como deseja que as informações sejam resumidas.
1. No **Eixo esquerdo (Y)** selecione o Grouping que deseja incluir no gráfico.
1. (Opcional) Selecione **Cores Personalizadas** para personalizar as cores das barras.\
   Para obter mais informações sobre como personalizar as cores do gráfico, consulte [Personalizar cores do gráfico](#customize-chart-colors).

1. (Opcional) Selecione **Mostrar em 3D** para exibir o gráfico em uma exibição tridimensional.
1. (Opcional) Selecione **Barras de grupo** para definir como você deseja que as barras sejam agrupadas.\
   Selecione entre as seguintes opções:

   * Clique em uma das seguintes opções para selecionar como as barras agrupadas serão exibidas:

      * **Lado a lado**
      * **Empilhado**
      * **Empilhado a 100%**

   * Selecione como deseja agrupar as informações no gráfico a partir da **Agrupar dados por** menu suspenso.
   * (Opcional) Selecione **Cores Personalizadas** para personalizar as cores das colunas.\
     Para obter mais informações sobre como personalizar as cores do gráfico, consulte [Personalizar cores do gráfico](#customize-chart-colors).

1. (Opcional) Selecione **Gráfico Combinado** para incluir um valor adicional no gráfico, bem como a forma como você deseja que as informações sejam resumidas.\
   ![](assets/qs-bar-chart-350x167.png)

1. Clique em **Salvar + Fechar** para salvar o gráfico e o relatório.

>[!IMPORTANT]
>
>Limite os gráficos de barras a 23 ou menos barras, já que os gráficos de barras que incluem mais de 23 barras não exibirão corretamente todos os rótulos de barras.

### Gráfico de pizza {#pie-chart}

Para adicionar um **Pizza** gráfico para o seu relatório:

1. Comece a adicionar um gráfico ao seu relatório, conforme descrito em [Adicionar um gráfico a um relatório](#add-a-chart-to-a-report).
1. No **Valores** selecione os valores que deseja exibir no relatório, bem como a forma como deseja que eles sejam resumidos.\
   No **Cunhas** selecione o Grouping que deseja incluir no gráfico. O Agrupamento é representado pelas fatias do gráfico.

1. (Opcional) Selecione **Cores Personalizadas** para personalizar as cores das cunhas no gráfico.\
   Para obter mais informações sobre como personalizar as cores do gráfico, consulte [Personalizar cores do gráfico](#customize-chart-colors).

1. (Opcional) Selecione **Mostrar em 3D** para exibir o gráfico em uma exibição tridimensional.
1. No **Mostrar resultados como** selecione como deseja que os resultados sejam exibidos no gráfico. Considere as seguintes opções:

   * **Porcentagem**: os resultados do gráfico são exibidos como uma porcentagem.
   * **Números**: os resultados do gráfico são exibidos como um número.\
     ![](assets/qs-pie-chart-350x171.png)

1. Clique em **Salvar + Fechar** para salvar o gráfico e o relatório.

### Gráfico de linhas {#line-chart}

Para adicionar um **Linha** gráfico para o seu relatório:

1. Comece a adicionar um gráfico ao seu relatório, conforme descrito em [Adicionar um gráfico a um relatório](#add-a-chart-to-a-report).
1. No **Eixo esquerdo (Y)** , selecione os valores que deseja incluir no eixo Y do gráfico, bem como a forma como deseja que as informações sejam resumidas.
1. No **Eixo inferior (X)** selecione o Grouping que deseja incluir no gráfico.
1. (Opcional) Selecione uma cor para personalizar a cor da linha.
1. (Opcional) Selecione **Linhas de grupo**, para selecionar um agrupamento adicional para o gráfico.\
   (Opcional) Selecione **Cores Personalizadas** para personalizar as cores do novo agrupamento.\
   Para obter mais informações sobre como personalizar as cores do gráfico, consulte [Personalizar cores do gráfico](#customize-chart-colors).

1. (Opcional) Selecione **Gráfico Combinado** para combinar suas linhas por um valor adicional.\
   Considere entre as seguintes opções:

   * Selecione o valor que deseja incluir no gráfico e como deseja que as informações sejam resumidas.
   * Selecione o **Plotar no eixo secundário** para plotar os dados no lado direito do gráfico.\
     ![](assets/qs-line-chart-350x172.png)

1. Clique em **Salvar + Fechar** para salvar o gráfico e o relatório.

### Gráfico de medição {#gauge-chart}

A **Medidor** o gráfico exibe o número de registros que atendem a um determinado critério em um formato de medidor. O indicador do medidor aponta para o número de registros que atendem aos critérios selecionados na exibição e no agrupamento do relatório. Não é necessário um agrupamento de relatório para configurar um gráfico de medidor.

Para adicionar um **Medidor** gráfico para o seu relatório:

1. Comece a adicionar um gráfico ao seu relatório, conforme descrito em [Adicionar um gráfico a um relatório](#add-a-chart-to-a-report).
1. No **Valores** selecione os valores que deseja exibir no relatório, bem como a forma como deseja que eles sejam resumidos. Se você selecionar **Contagem de registros**, os valores exibidos são o objeto do relatório.

1. No **Indicadores** selecione o Grouping que deseja incluir no gráfico. O Agrupamento é representado pela linha indicadora no gráfico.\
   Se você tiver um Agrupamento que contenha dois itens, dois indicadores serão exibidos no gráfico.\
   Por exemplo, se você tiver um Agrupamento de Status de Projeto e houver dois status de projeto (Atual e Em Retenção), seu gráfico Medição conterá dois indicadores de medição. Eles apontarão para o número de projetos que estão nesse status.\
   (Opcional) Selecione **Total** no **Indicadores** para exibir o total dos objetos selecionados na variável **Valores** campo.

1. No **Faixa de valores** especifique o intervalo de valores e a cor para representar esses valores a serem exibidos no gráfico Gauge.
1. (Opcional) Clique em **Adicionar outra faixa de valores** para adicionar intervalos de valor adicionais ao gráfico.\
   ![](assets/qs-gauge-chart-350x181.png)

1. Clique em **Salvar + Fechar** para salvar o gráfico e o relatório.

### Gráfico de bolhas {#bubble-chart}

É possível exibir até três campos de um objeto em uma **Bolha** gráfico. Isso significa que você pode exibir até quatro pontos de dados em um gráfico de bolhas. Cada entidade com três campos associados é exibida como um círculo que expressa dois dos campos em sua localização dentro dos eixos X e Y. O terceiro campo é representado pelo tamanho do círculo.

Para adicionar um **Bolha** gráfico para o seu relatório:

1. Comece a adicionar um gráfico ao seu relatório, conforme descrito em [Adicionar um gráfico a um relatório](#add-a-chart-to-a-report).
1. No **Eixo esquerdo (Y)** selecione os valores que deseja incluir no eixo Y do gráfico. Os valores são da exibição do relatório. Especifique como deseja que as informações sejam resumidas.
1. No **Campo do eixo inferior (X)**, selecione os valores que deseja incluir no eixo X do gráfico. Os valores são da exibição do relatório. Especifique como deseja que as informações sejam resumidas.

   >[!NOTE]
   >
   >Certifique-se de que haja pelo menos uma coluna resumida para que esse campo fique ativo.\
   >Para obter mais informações sobre o resumo das informações em uma coluna do relatório, consulte [Criar um relatório personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. No **Tamanho da bolha** selecione os valores que deseja representar pelo tamanho das bolhas no gráfico. Os valores são da exibição do relatório. Especifique como deseja que as informações sejam resumidas.

   >[!NOTE]
   >
   >Certifique-se de que haja pelo menos uma coluna resumida para que esse campo fique ativo.\
   >Para obter mais informações sobre o resumo das informações em uma coluna do relatório, consulte [Criar um relatório personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. No **Bolhas** selecione o Grouping que deseja incluir no gráfico. O Agrupamento é representado pelo posicionamento das bolhas no gráfico.
1. No **Cor da bolha** selecione o campo que você deseja que seja representado pelas cores das bolhas.

   ![](assets/qs-bubble-chart-350x103.png)


   A variável **Cor da bolha** pode ser um Agrupamento definido no relatório, mas só estará disponível quando você selecionar a variável **Nome** coluna do objeto do relatório na variável **Bolhas** campo.

   Por exemplo, se você selecionou **Nome da tarefa** em um relatório de tarefa, é possível adicionar **Status da tarefa** como o **Cor da bolha** campo.

   ![](assets/bubbles-field-correct-can-select-bubbles-color-example.png)

   No entanto, se você selecionou **Status da tarefa** para o **Bolhas** , não é possível selecionar um **Cor da bolha** campo. Além disso, não é possível selecionar **Nome do projeto** para o **Cor da bolha** , mesmo ao selecionar **Nome da tarefa** para o **Bolha** campo.

   ![](assets/bubbles-field-wrong-cannot-select-bubbles-color-example.png)


1. Clique em **Salvar + Fechar** para salvar as alterações no construtor de interfaces.

## Exportar um gráfico

É possível exportar um gráfico para um arquivo PDF.

Para exportar um gráfico:

1. Clique em **Exportar** para exportar o gráfico para .pdf.\
   Um arquivo .pdf é baixado no computador.

1. Abra o arquivo .pdf.\
   O arquivo exportado inclui as seguintes informações:

   * Uma imagem do gráfico.
   * Um título que é o nome do relatório.
   * Um nome de arquivo exclusivo que é o nome do relatório.
   * Um rodapé com a data e hora em que o relatório foi exportado e o número da página.

## Personalizar cores do gráfico {#customize-chart-colors}

Você pode permitir que o Workfront selecione as cores dos elementos no seu gráfico, ou pode personalizá-las enquanto adiciona um gráfico aos seus relatórios. Se o gráfico contiver um único Agrupamento que represente uma métrica, como um relatório de tarefa que mostra o número de tarefas agrupadas por Data de Conclusão Real, cada resultado no Agrupamento será exibido na mesma cor.

Você só pode escolher uma cor para os campos exibidos na Exibição do relatório. Você pode escolher várias cores, uma para cada opção, para os campos exibidos no Agrupamento do relatório.

>[!IMPORTANT]
>
>Para campos de data, é possível selecionar apenas uma cor para os elementos do gráfico.

Para personalizar as cores do gráfico:

1. Ao criar um relatório, vá para a página **Gráfico** no construtor de relatórios.
1. Selecione um tipo de gráfico para adicionar ao seu relatório.\
   Para obter mais informações sobre como adicionar um gráfico ao relatório, consulte [Adicionar um gráfico a um relatório](#add-a-chart-to-a-report).

1. Clique em **Cores Personalizadas** quando esse campo estiver disponível.\
   A caixa de diálogo Cores Personalizadas é exibida.\
   ![](assets/custom-colors-in-charts-350x286.png)

   >[!NOTE]
   >
   >É possível associar cores personalizadas a qualquer campo que possa ser agrupado por e com alguns campos que podem ser exibidos em uma exibição, incluindo campos personalizados. Os campos personalizados ou as opções personalizadas dos campos escolhidos na caixa de diálogo Cor personalizada fazem distinção entre maiúsculas e minúsculas.

1. Considere selecionar qualquer uma das seguintes opções:

   * **Usar uma cor**: todos os elementos do gráfico serão exibidos na cor selecionada.

      1. Comece digitando o nome de uma opção do campo selecionado e selecione uma cor. Essa opção é exibida na cor selecionada no gráfico.
      1. (Opcional) Especifique um valor de cor hexadecimal para a cor, em vez de selecionar um dentre as amostras de cores disponíveis\
         Ou\
         Clique no seletor de cores exibido após clicar no código hexadecimal e selecione outra cor.

   * **Adicionar cor**: Continue a adicionar cores personalizadas para todas as outras opções possíveis do campo selecionado.
   * **Remover tudo**: selecione esta opção para remover todas as cores e opções do campo selecionado acima.
   * **Opções avançadas**: selecione entre as seguintes opções:

      * **Sem valor**: selecione esse campo e uma cor personalizada para exibir a coluna do gráfico que agrupa itens de &quot;valor nulo&quot;. Esses itens não podem ser agrupados por nenhuma das opções do campo selecionado no seu agrupamento.
      * **Todos os outros valores**: selecione esse campo e uma cor personalizada para exibir todos os outros elementos do gráfico cujas opções não estão selecionadas acima.

        >[!NOTE]
        >
        >As cores usadas mais recentemente são exibidas na parte superior da caixa de diálogo Cores Personalizadas. Quando você passa o mouse sobre uma cor que foi usada recentemente, o nome do campo associado a ela é exibido.

1. Clique no &quot;x&quot; no canto superior direito de Cores personalizadas para fechar a caixa de diálogo Cores personalizadas. As cores selecionadas são salvas automaticamente.
1. Clique em **Salvar + Fechar** para salvar o gráfico e executar o relatório.

## Remover um gráfico de um relatório

Para remover um gráfico de um relatório:

1. Abra o **Gráfico** do report builder.
1. Passe o mouse sobre o ícone do tipo de gráfico escolhido e um botão &quot;x&quot; aparecerá no canto superior direito do ícone.
1. Clique no &quot;x&quot; para remover o gráfico.
1. Clique em **Salvar + Fechar**.

## Limitações ao trabalhar com gráficos

Esteja ciente das seguintes limitações ao trabalhar com gráficos:

* A variável **Visualização do gráfico** à direita do Report Builder não contiver dados reais do seu relatório. Você deve salvar o gráfico e visualizá-lo a partir da **Gráfico** para ver o gráfico com seus dados.

* Alguns elementos do gráfico não são editáveis:

   * Não é possível alterar o tipo de fonte nem o tamanho nos valores de cada elemento.
   * Não é possível alterar os nomes dos eixos no gráfico.

* Não é possível editar a legenda do gráfico.
* Ao usar campos calculados para seus agrupamentos, não é possível clicar nos elementos do gráfico.
* O número máximo de pontos de dados que podem ser exibidos em um gráfico é quatro, em um gráfico de bolhas. Todos os outros tipos de gráficos exibem dois ou no máximo três pontos de dados.
