---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Ferramentas
description: A seção  [!DNL Adobe Workfront Fusion Tools]  inclui vários módulos úteis que podem aprimorar seu cenário.
author: Becky
feature: Workfront Fusion
exl-id: 97a68fbc-1272-43fc-b4f2-4c1c9e590741
source-git-commit: 55485da1ea650121b5537a3f19d8102623ed4f43
workflow-type: tm+mt
source-wordcount: '2283'
ht-degree: 0%

---

# [!UICONTROL Ferramentas]

A seção [!DNL Adobe Workfront Fusion Tools] inclui vários módulos úteis que podem aprimorar seu cenário.

Os módulos [!UICONTROL Ferramentas] estão disponíveis na lista de aplicativos ou no ícone ![](assets/tools-icon-small.png) de [!UICONTROL Ferramentas], na parte inferior da tela.

## Requisitos de acesso

Você deve ter o seguinte acesso para usar a funcionalidade neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plano*</td>
  <td> <p>[!UICONTROL Pro] ou superior</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licença*</td>
   <td> <p>[!UICONTROL Plano], [!UICONTROL Trabalho]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licença**</td> 
   <td>
   <p>Requisito de licença atual: nenhum requisito de licença [!DNL Workfront Fusion].</p>
   <p>Ou</p>
   <p>Requisito de licença herdada: [!UICONTROL [!DNL Workfront Fusion] para Automação e Integração do Trabalho] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produto</td> 
   <td>
   <p>Requisito atual do produto: se você tiver o plano [!UICONTROL Select] ou [!UICONTROL Prime] [!DNL Adobe Workfront], sua organização deve comprar [!DNL Adobe Workfront Fusion] e [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo. [!DNL Workfront Fusion] está incluído no plano [!DNL Workfront] do [!UICONTROL Ultimate].</p>
   <p>Ou</p>
   <p>Requisito de produto herdado: sua organização deve comprar o [!DNL Adobe Workfront Fusion] e o [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo.</p>
   </td> 
  </tr>
 </tbody> 
</table>

Para saber que plano, tipo de licença ou acesso você tem, contate o administrador do [!DNL Workfront].

Para obter informações sobre [!DNL Adobe Workfront Fusion] licenças, consulte [[!DNL Adobe Workfront Fusion] licenças](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!UICONTROL Ferramentas] e seus campos

* [Triggers](#triggers)
* [Ações](#actions)
* [Agregadores](#aggregators)
* [Transformadores](#transformers)

### Triggers

#### [!UICONTROL Gatilho básico]

Esse módulo permite criar um acionador personalizado e definir seus pacotes de entrada.

Você pode usar este módulo, por exemplo, para contatos ou qualquer outra lista agendada para ser enviada para um endereço de email especificado (como os módulos [!UICONTROL Email] >[!UICONTROL Enviar um Email] ou [!DNL Gmail] >[!UICONTROL Enviar um Email]), ou como um simples lembrete a ser acionado sempre que desejar.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Pacote]</td> 
   <td> <p>Crie pacotes personalizados adicionando itens de matriz. A matriz consiste nos pares nome - valor.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Ações

* [[!UICONTROL Obter Várias Variáveis]](#get-multiple-variables)
* [[!UICONTROL Obter Variável]](#get-variable)
* [[!UICONTROL Função de incremento]](#increment-function)
* [[!UICONTROL Definir Várias Variáveis]](#set-multiple-variables)
* [[!UICONTROL Definir Variável]](#set-variable)
* [[!UICONTROL Suspender]](#sleep)

#### [!UICONTROL Obter Várias Variáveis]

Este módulo recupera valores que foram criados anteriormente pelo módulo [!UICONTROL Set Variable] ou [!UICONTROL Set Multiple Variables].

Este módulo pode ler variáveis que foram definidas em qualquer lugar do cenário, mesmo que a variável tenha sido definida em uma rota diferente daquela em que o módulo [!UICONTROL Obter Várias Variáveis] está localizado. O único requisito é que o módulo [!UICONTROL Ferramentas] > [!UICONTROL Definir Variável] ou [!UICONTROL Ferramentas] > [!UICONTROL Definir Várias Variáveis] seja executado antes do módulo [!UICONTROL Ferramentas] > [!UICONTROL Obter Várias Variáveis]. Para obter mais informações sobre a ordem em que os módulos são executados, consulte [Módulo de roteador em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/router-module.md).

<table style="table-layout:auto">
    <tr>
        <td>[!UICONTROL Variáveis]</td>
        <td>Adicione as variáveis que você deseja que o módulo obtenha.</td>
    </tr>
    <tr>
        <td>[!UICONTROL Nome da variável]</td>
        <td>Para cada variável adicionada, mapeie o nome da variável que deseja obter.</td>
    </tr>
</table>

>[!INFO]
>
>**Exemplos:** Estes são os usos possíveis dos módulos [!UICONTROL Set]/[!UICONTROL Get (multiple) variável(is)]:
>
>* Armazenar um valor calculado para uso posterior, mesmo em uma rota diferente. Isso é útil nos casos em que o valor é usado em vários módulos e a fórmula para calcular o valor é muito complexa.
>* Para depurar uma fórmula. Se uma fórmula usada em um módulo aparentemente não fornecer um resultado correto, copie a fórmula e cole-a em um módulo [!UICONTROL Definir variável] que você insere antes do módulo relevante. Desconecte o(s) módulo(s) após o módulo [!UICONTROL Set Variable] e execute o cenário. Verifique a saída do módulo [!UICONTROL Set Variable], ajuste ou simplifique a fórmula, execute o cenário novamente e continue a fazê-lo até que o problema seja resolvido.


#### [!UICONTROL Obter Variável]

Este módulo recupera um valor criado anteriormente pelo módulo [!UICONTROL Set Variable] ou [!UICONTROL Set Multiple Variables].

Este módulo pode ler variáveis que foram definidas em qualquer lugar do cenário, mesmo que a variável tenha sido definida em uma rota diferente daquela em que o módulo [!UICONTROL Obter Variável] está localizado. O único requisito é que o módulo [!UICONTROL Ferramentas] > [!UICONTROL Definir Variável] ou [!UICONTROL Ferramentas] > [!UICONTROL Definir Várias Variáveis] seja executado antes do módulo [!UICONTROL Ferramentas] > [!UICONTROL Obter Variável]. Para obter mais informações sobre a ordem em que os módulos são executados, consulte [Módulo de roteador em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/router-module.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nome da variável]</td> 
   <td> <p>Mapeie o nome da variável que você deseja que o módulo obtenha.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Função de incremento]

Este módulo retorna um valor incrementado em 1 após cada operação do módulo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Redefinir um valor]</td> 
   <td> <p>Selecione quando deseja que o módulo incremente o valor. </p> 
    <ul> 
     <li>[!UICONTROL Após um ciclo]</li> 
     <li>[!UICONTROL Após a execução de um cenário]</li> 
     <li>[!UICONTROL Nunca]</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**Exemplo:**
>
>Um dos usos do módulo é implementar uma atribuição &quot;rodízio&quot; de tarefas, leads, emails e assim por diante aos usuários em um grupo. O algoritmo escolhe os designados de um grupo em alguma ordem racional, geralmente indo de cima para baixo de uma lista. Quando o algoritmo atinge o final da lista, ele então dá a próxima atribuição para o usuário no topo da lista e continua a fazer atribuições na lista.
>
>O cenário a seguir envia um email para o primeiro recipient após cada execução de cenário com numeração ímpar e para o segundo recipient após cada execução de cenário com numeração par.
>
>![](assets/example-email-350x246.gif)
>
>1. Para criar esse cenário:
>1. Defina o campo **[!UICONTROL Redefinir valor]** do módulo como Nunca.
>1. Defina a rota para valores ímpares. Defina o filtro para esta rota usando a função matemática de módulo que é igual a `1`:
>
>   ![](assets/odd-350x459.png)
>
>  **Observação**: não se esqueça de alterar o operador [!UICONTROL Igual a] do operador [!UICONTROL Texto] padrão para o operador [!UICONTROL Numérico].
>
>1. Defina a rota para valores pares usando a função matemática de módulo que é igual a `0`:
>
>A função de incremento adiciona uma cada vez que o cenário é executado. Os filtros verificam o incremento e agem de acordo com seu valor, garantindo que os emails sejam distribuídos uniformemente.

#### [!UICONTROL Definir Várias Variáveis]

Este módulo cria variáveis que podem ser mapeadas por outros módulos na rota. A variável também pode ser mapeada para os módulos [!UICONTROL Obter Variável] ou [!UICONTROL Obter Várias Variáveis] para qualquer rota no cenário.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Variáveis]</td> 
   <td>Adicione as variáveis que você deseja que o módulo defina.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Nome da variável] </td> 
   <td>Para cada variável, insira o nome da variável. Esse nome será exibido ao mapear a variável em outros módulos. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Valor de variável] </td> 
   <td>Para cada variável, insira o valor da variável. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tempo de vida da variável] </td> 
   <td> <p>Selecione por quanto tempo você deseja que as variáveis permaneçam válidas (mantenha o mesmo valor).</p> 
    <ul> 
     <li><strong>[!UICONTROL Um ciclo]</strong>: A variável é válida para um ciclo. Útil quando vários webhooks em uma execução de cenário são recebidos (mais webhooks = mais ciclos). </li> 
     <li><strong>[!UICONTROL One execution]</strong>: a variável é válida para uma execução de cenário. Uma execução pode conter um ou mais ciclos.</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Definir Variável]

Este módulo cria uma variável que pode ser mapeada por outros módulos na rota. A variável também pode ser mapeada para os módulos [!UICONTROL Obter Variável] ou [!UICONTROL Obter Várias Variáveis] para qualquer rota no cenário.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Nome da variável] </td> 
   <td>Insira o nome da variável. Esse nome será exibido ao mapear a variável em outros módulos. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tempo de vida da variável] </td> 
   <td> <p>Selecione por quanto tempo você deseja que as variáveis permaneçam válidas (mantenha o mesmo valor).</p> 
    <ul> 
     <li><strong>[!UICONTROL Um ciclo]</strong>: A variável é válida para um ciclo. Útil quando vários webhooks em uma execução de cenário são recebidos (mais webhooks = mais ciclos). </li> 
     <li><strong>[!UICONTROL One execution]</strong>: a variável é válida para uma execução de cenário. Uma execução pode conter um ou mais ciclos.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Valor de variável] </td> 
   <td>Insira ou mapeie o valor da variável. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Suspender]

Esse módulo permite atrasar o fluxo do cenário por até 300 segundos (5 minutos).

Essa função pode ser útil, por exemplo, para reduzir a carga do servidor de serviço [!DNL target] ou imitar o comportamento humano ao enviar SMS ou emails em massa.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!UICONTROL Atraso]</p> </td> 
   <td> <p>Insira o número de segundos durante os quais o cenário será pausado.</p> </td> 
  </tr> 
 </tbody> 
</table>

>[!TIP]
>
>Se você quiser pausar o fluxo por períodos mais longos, sugerimos dividir o cenário em dois cenários:
>
>* O primeiro cenário conteria a parte antes da pausa.
>* O segundo cenário conteria a parte depois dela.
>
>O primeiro cenário acabaria armazenando todas as informações necessárias em um armazenamento de dados junto com o carimbo de data e hora atual. O segundo cenário verificaria periodicamente o armazenamento de dados em busca de registros com um carimbo de data e hora anterior ao atraso desejado, recuperaria os registros, finalizaria o processamento dos dados e removeria os registros do armazenamento de dados.
>
>Para obter mais informações sobre armazenamentos de dados, consulte [Armazenamentos de Dados em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/data-stores.md).
>
>Para obter mais informações sobre módulos de repositório de dados específicos, consulte [[!UICONTROL Repositório de dados] módulos](../../workfront-fusion/apps-and-their-modules/data-store-modules.md).

### Agregadores

* [[!UICONTROL Agregador numérico]](#numeric-aggregator)
* [[!UICONTROL Agregador de tabela]](#table-aggregator)
* [[!UICONTROL Agregador de texto]](#text-aggregator)

#### [!UICONTROL Agregador numérico]

Esse módulo permite recuperar valores numéricos, aplicar uma das funções selecionadas (SUM, AVG, COUNT, MAX, MIN) e retornar o resultado em um pacote.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!UICONTROL módulo Source]</p> </td> 
   <td> <p>Selecione o módulo do qual deseja agregar campos.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Função de agregação]</p> </td> 
   <td> <p>Selecione a função que deseja usar para agregar os valores.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Agrupar por]</p> </td> 
   <td> <p>Defina uma expressão pela qual você deseja agrupar a saída agregada. Esta expressão pode conter um ou mais itens mapeados. Os dados agregados são, então, separados em grupos usando o valor dessa expressão. Cada grupo gera um pacote separado com uma chave (a expressão avaliada) e um valor (o valor agregado). Você pode usar a chave como um filtro nos módulos subsequentes.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Parar processamento após uma agregação vazia]</td> 
   <td>Habilite essa opção para interromper o cenário quando não houver resultados.</td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Valor]</p> </td> 
   <td> <p>Insira ou mapeie o valor que deseja agregar.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Agregador de tabela]

Este módulo mescla valores dos campos selecionados de pacotes recebidos em um único pacote usando uma coluna especificada e um separador de linha (que permite criar uma tabela).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!UICONTROL módulo Source]</p> </td> 
   <td> <p>Selecione o módulo do qual deseja agregar campos.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Campos Agregados]</td> 
   <td> <p> Selecione os campos do módulo selecionado acima que contêm valores que você deseja agregar em um pacote.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Separador de coluna]</p> </td> 
   <td> <p>Selecione ou insira o tipo de separador que separará as colunas de valor de campo no pacote resultante. Se você selecionar [!UICONTROL Outro], insira o caractere que deseja usar para separar valores no campo separador.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Separador de linha]</p> </td> 
   <td> <p>Selecione ou insira o tipo de separador que separará as linhas de valor de campo no pacote resultante. Se você selecionar [!UICONTROL Outro], insira o caractere que deseja usar para separar valores no campo separador.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Agrupar por]</p> </td> 
   <td> <p>Defina uma expressão pela qual você deseja agrupar a saída agregada. Esta expressão pode conter um ou mais itens mapeados. Os dados agregados serão, então, separados em grupos usando o valor dessa expressão. Cada grupo gera um pacote separado com uma chave (a expressão avaliada) e um valor (o valor agregado). Você pode usar a chave como um filtro nos módulos subsequentes.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Parar processamento após uma agregação vazia]</td> 
   <td>Selecione esta opção para interromper o cenário quando não houver resultados.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Agregador de texto]

Este módulo mescla os valores dos campos selecionados de pacotes recebidos em um único pacote.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!UICONTROL módulo Source]</p> </td> 
   <td> <p>Selecione o módulo do qual deseja agregar campos.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Separador de linha]</p> </td> 
   <td> <p>Selecione ou insira o tipo de separador que separará as linhas de valor de campo no pacote resultante. Se você selecionar [!UICONTROL Outro], insira o caractere que deseja usar para separar valores no campo separador.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Agrupar por]</p> </td> 
   <td> <p>Defina uma expressão contendo um ou mais itens mapeados. Os dados agregados são separados em Grupos com o mesmo valor de expressão. Cada Grupo gera um pacote separado contendo uma Chave com a expressão avaliada e o texto agregado. Ao fazer isso, você pode usar a chave como um filtro nos módulos subsequentes.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Texto]</td> 
   <td> <p> Insira ou mapeie o texto que você deseja que o módulo agregue.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Parar processamento após uma agregação vazia]</td> 
   <td>Selecione esta opção para interromper o cenário quando não houver resultados.</td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**Exemplo:** você pode usar o agregador de texto para inserir mais valores (por exemplo, nomes de clientes ou observações) em um único pacote e enviar um email contendo todos os valores no corpo do email ou no assunto do email.

### Transformadores

* [[!UICONTROL Compor uma cadeia de caracteres]](#compose-a-string)
* [[!UICONTROL Converter a codificação do texto]](#convert-the-encoding-of-the-text)
* [[!UICONTROL Alternar]](#switch)

#### [!UICONTROL Compor uma cadeia de caracteres]

Converte qualquer valor em um tipo de dados de string (texto). Isso facilita o mapeamento, por exemplo, de dados binários.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Texto]</td> 
   <td> <p>Insira ou mapeie os dados que deseja converter em texto.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Converter a codificação do texto]

Converte o texto de entrada inserido (ou dados binários) na codificação selecionada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!UICONTROL Dados de entrada]</p> </td> 
   <td> <p>Insira ou mapeie o conteúdo que deseja converter.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Página de código de dados de entrada]</td> 
   <td> <p>Selecione o tipo de codificação dos dados de entrada. </p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Página de código de dados de saída]</p> </td> 
   <td> <p>Selecione o tipo de codificação dos dados de destino (saída).</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Alternar]

Verifica o valor de entrada para obter uma correspondência com a lista de valores fornecida. Retorna a saída com base no resultado.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!UICONTROL Entrada]</p> </td> 
   <td> <p>Insira a expressão que você deseja avaliar.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Usar expressões regulares para corresponder]</td> 
   <td> <p>Ative esta opção para usar expressões regulares. O módulo determina os casos com base na expressão regular, em vez de uma correspondência exata.</p> 
    <div> 
     <p>Uma expressão regular é uma sequência de caracteres na qual cada caractere é um metacaractere, com um significado especial, ou um caractere regular que tem um significado literal. Esses caracteres e metacaracteres identificam um padrão que pode ser usado para pesquisar texto. Por exemplo, se você deseja pesquisar nomes, é possível configurar uma expressão regular para pesquisar um padrão que consiste em duas palavras consecutivas que começam com letras maiúsculas. As expressões regulares são uma ferramenta poderosa para pesquisar e manipular texto.</p> 
     <p>Uma discussão de expressões regulares está fora do escopo deste artigo. Recomendamos os seguintes recursos:</p> 
     <ul> 
      <li>Para obter a lista completa de metacaracteres, consulte <a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Regular_Expressions">Expressões regulares</a> em documentos da Web do MDN.</li> 
      <li>Para um tutorial sobre como criar expressões regulares, recomendamos <a href="https://regexone.com/">RegexOne</a>.</li> 
      <li>Para experimentar expressões regulares, recomendamos o site <a href="https://regex101.com/">Expressões regulares 101</a>. Selecione a VARIÁVEL ECMAScript (JavaScript) no painel esquerdo.</li> 
     </ul> 
    </div> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Casos] </td> 
   <td> <p>Se a entrada contiver um valor inserido no campo [!UICONTROL Padrão], o valor inserido no campo [!UICONTROL Saída] será retornado.</p> <p>Se a entrada não corresponder a nenhum dos valores definidos em um campo [!UICONTROL Padrão], uma das situações a seguir ocorrerá:</p> 
    <ul> 
     <li>O valor do campo [!UICONTROL Else] é retornado</li> 
     <li>Se não houver valor no campo [!UICONTROL Else], nenhuma saída será retornada.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Else]</p> </td> 
   <td> <p>Insira o valor retornado quando os critérios definidos no campo Casos não forem atendidos. </p> </td> 
  </tr> 
 </tbody> 
</table>
