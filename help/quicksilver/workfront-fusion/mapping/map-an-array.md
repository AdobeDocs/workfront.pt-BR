---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: mapping
title: Mapear uma matriz no  [!DNL Adobe] Workfront Fusion
description: A documentação do Adobe Workfront Fusion foi movida para um novo local. Este artigo foi descontinuado, mas contém um link para o novo artigo que aborda essa funcionalidade.
author: Becky
feature: Workfront Fusion
exl-id: 725e0c24-cb4b-46c4-9c00-4f9cc334fbc7
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '929'
ht-degree: 0%

---

# Mapear uma matriz em [!DNL Adobe Workfront Fusion]

>[!IMPORTANT]
>
>A documentação do Adobe Workfront Fusion foi movida para um novo local.
>
>As informações neste artigo agora podem ser encontradas no artigo:
>
>* [Mapear uma matriz ou elemento de matriz](https://experienceleague.adobe.com/docs/workfront-fusion/using/create-scenarios/map-data/map-an-array.html)
>
>Atualize todos os marcadores.
>
>Este artigo não está mais sendo atualizado e será removido em breve.

Uma matriz é um tipo especial de item que pode conter o seguinte:

* Um ou mais valores de texto (matriz simples)
* Uma ou mais coleções do mesmo tipo (matriz complexa)

>[!INFO]
>
>**Exemplo:** O módulo [!UICONTROL Assistir emails] retorna uma matriz de anexos para cada email. Cada anexo representa uma coleção que pode conter um nome, conteúdo, tamanho e assim por diante.

Para obter mais informações, consulte [Tipos de dados do item em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/item-data-types.md).

## Requisitos de acesso

Você deve ter o seguinte acesso para usar a funcionalidade neste artigo:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] plano*</td> 
   <td> <p>[!DNL Pro] ou superior</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licença*</td> 
   <td> <p>[!UICONTROL Plano], [!UICONTROL Trabalho]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença [!UICONTROL Adobe Workfront Fusion]**</td> 
   <td>
   <p>Requisito de licença atual: nenhum requisito de licença [!DNL Workfront Fusion].</p>
   <p>Ou</p>
   <p>Requisito de licença herdada: [!UICONTROL [!DNL Workfront Fusion] para Automação e Integração do Trabalho] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produto</td> 
   <td>
   <p>Requisito atual do produto: se você tiver o Plano [!DNL Adobe Workfront] da [!UICONTROL Select] ou da [!UICONTROL Prime], sua organização deve comprar o [!DNL Adobe Workfront Fusion] e o [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo. [!DNL Workfront Fusion] está incluído no plano [!DNL Workfront] da [!UICONTROL Ultimate].</p>
   <p>Ou</p>
   <p>Requisito de produto herdado: sua organização deve comprar o [!DNL Adobe Workfront Fusion] e o [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Para saber que plano, tipo de licença ou acesso você tem, contate o administrador do [!DNL Workfront].

Para obter informações sobre [!DNL Adobe Workfront Fusion] licenças, consulte [[!DNL Adobe Workfront Fusion] licenças](../../workfront-fusion/get-started/license-automation-vs-integration.md).



## Mapear uma matriz inteira

1. Nos módulos para os quais você está mapeando a matriz, clique no campo onde deseja mapear a matriz. Este é o campo para o qual a matriz está mapeada.

1. Na caixa exibida, mapeie o item.

   O painel permite mapear campos da mesma forma que com qualquer outro tipo de item. Se você não quiser preencher cada item separadamente, mas quiser mapear outra matriz no campo de destino, use o botão [!UICONTROL Mapear]. Nesse caso, verifique se ambos os storages (o storage de origem e o storage de destino) têm a mesma estrutura.

   Você pode adicionar qualquer número de itens a uma matriz.

É possível dividir uma matriz em pacotes individuais usando um iterador. Para obter mais informações, consulte o módulo [[!UICONTROL Iterador] em [!DNL Adobe Workfront Fusion]](/help/quicksilver/workfront-fusion/modules/iterator-module.md).

## Mapear itens em uma nova matriz

Alguns campos no Workfront Fusion permitem mapear elementos em uma matriz. Por exemplo, você pode criar uma matriz de itens de lista de verificação no módulo Workfront Boards > Adicionar item de lista de verificação. Quando o módulo é executado, todos os itens da lista de verificação são adicionados ao cartão.

Qualquer campo do módulo que exibe &quot;Adicionar item&quot; cria uma matriz.

![Adicionar item](assets/add-item.png)

Para adicionar elementos à matriz:

1. Clique em **Adicionar item**
1. No painel aberto, insira detalhes sobre o item.
1. Clique em **Adicionar**.
1. (Opcional) Repita as etapas 1 a 3 para cada elemento que você deseja adicionar à matriz .

## Mapear elementos de matriz


### Mapear elementos de matriz por número

Os elementos da matriz são exibidos como um número entre colchetes após o nome da matriz. Você pode mapear um elemento individual de uma matriz em um campo usando esse número de índice.

![](assets/map-array-1st-element.png)

>[!NOTE]
>
>A indexação de arrays no Workfront Fusion começa em 1.

Para mapear um elemento de matriz:

1. Clique no campo onde deseja mapear o elemento.

   O painel de mapeamento é aberto.

1. Localize a matriz que contém o elemento que você deseja mapear.
1. Clique na seta suspensa ao lado da matriz.
1. Clique no elemento que deseja mapear.

   O elemento é mapeado, com o índice de 1. Isso mapeia o primeiro elemento na matriz.

1. Para mapear um elemento diferente da matriz, clique em [1] e insira o número de índice do elemento de matriz que você deseja mapear.

   ![](assets/access-another-element.png)

### Mapear um elemento de matriz com uma determinada chave

Algumas matrizes contêm coleções com itens de valores-chave, como metadados, atributos e assim por diante. Para usar um desses valores, você pode pesquisar um elemento por seu valor de chave fornecido e obter o valor correspondente do item de valor. Recomendamos usar uma fórmula que empregue uma combinação das funções `map()` e `get()`.



>[!BEGINSHADEBOX]

O exemplo a seguir mostra a saída do aplicativo [!DNL Jira].

![](assets/output-of-jira-app-350x100.png)

Este exemplo obtém um nome de arquivo de uma matriz de anexos, para o anexo específico com uma ID 10108.

Esse exemplo gera a seguinte saída:

![](assets/output-from-jira-350x261.png)

A fórmula pode ser explicada da seguinte maneira:

* `map`

   1. O primeiro parâmetro da função `map()` é o item de matriz inteiro.
   1. O segundo parâmetro é o nome bruto do item de valor. Para obter o nome bruto, passe o mouse sobre o item no painel [!UICONTROL mapeamento]:

      ![](assets/obtain-raw-name-350x124.png)

      >[!NOTE]
      >
      >Todos os parâmetros diferenciam maiúsculas de minúsculas. Mesmo que neste exemplo em particular o rótulo do item difira de seu nome bruto apenas em maiúsculas, é necessário usar o nome bruto.

   1. O terceiro parâmetro é o nome bruto do item-chave:

      ![](assets/3rd-parameter-350x166.png)

   1. O quarto parâmetro é o valor de chave fornecido.

  Como a função `map()` retorna uma matriz (já que poderia haver mais elementos com o valor de chave fornecido), é necessário aplicar a função `get()` para obter seu primeiro elemento:

* `get`

   1. O primeiro parâmetro da função `get()` é o resultado da função `map()`.

   1. O segundo parâmetro é o índice do elemento. Neste exemplo, o índice é `1`.

Esse exemplo gera a seguinte saída:

![](assets/output-from-jira-350x261.png)

>[!ENDSHADEBOX]

Para obter mais informações sobre a função `map()`, consulte [Funções de matriz](/help/quicksilver/workfront-fusion/functions/array-functions.md).

Para obter mais informações sobre a função `get()`, consulte [Funções gerais](/help/quicksilver/workfront-fusion/functions/general-functions.md).

## Converter elementos de matriz em uma série de pacotes

Matrizes podem ser convertidas em uma série de conjuntos usando o módulo [!UICONTROL Iterador]. Para obter mais informações, consulte [[!UICONTROL Iterador] módulo](/help/quicksilver/workfront-fusion/modules/iterator-module.md).

![](assets/series-of-bundles.png)

