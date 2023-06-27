---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: XML
description: O aplicativo XML permite analisar um texto XML formatado por meio do módulo XML &gt; Analisar XML e convertê-lo em um pacote para disponibilizar os dados para outros módulos. Você também pode converter um pacote em um texto XML formatado através do XML &gt; Criar módulo XML
author: Becky
feature: Workfront Fusion
exl-id: 3459e930-8156-4171-8920-34f4e07bc530
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '1453'
ht-degree: 2%

---

# XML

A variável [!UICONTROL XML] permite analisar um texto XML formatado por meio da variável [!UICONTROL XML] > [!UICONTROL Analisar XML] e converta-o em um pacote para disponibilizar os dados para outros módulos. Também é possível converter um pacote em um texto XML formatado por meio da [!UICONTROL XML] > [!UICONTROL Criar XML] módulo

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
   <p>Requisito de licença atual: Não [!DNL Workfront Fusion] requisito de licença.</p>
   <p>Ou</p>
   <p>Requisito de licença herdada: [!UICONTROL [!DNL Workfront Fusion] para Automação e integração do trabalho] </p>
   </td>  
  </tr> 
  <tr> 
   <td role="rowheader">Produto</td> 
   <td>
   <p>Requisito atual do produto: se você tiver o [!UICONTROL Select] ou o [!UICONTROL Prime] [!DNL Adobe Workfront] Planejar, sua organização deve comprar [!DNL Adobe Workfront Fusion] bem como [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo. [!DNL Workfront Fusion] está incluído no [!UICONTROL Ultimate] [!DNL Workfront] plano.</p>
   <p>Ou</p>
   <p>Requisito de produto herdado: sua organização deve comprar [!DNL Adobe Workfront Fusion] bem como [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Para descobrir que plano, tipo de licença ou acesso você tem, entre em contato com o [!DNL Workfront] administrador.

Para obter informações sobre [!DNL Adobe Workfront Fusion] licenças, consulte [[!DNL Adobe Workfront Fusion] licenças](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!UICONTROL Analisar XML]

A variável [!UICONTROL XML] > [!UICONTROL Analisar XML] O módulo analisa um texto formatado XML e gera um único pacote contendo todas as informações extraídas do XML.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Estrutura de dados]</p> </td> 
   <td> <p>A estrutura de dados descreve a estrutura do XML para disponibilizar a saída do módulo no painel de mapeamento dos seguintes módulos.</p> <p>Se você tiver uma amostra do XML que deseja analisar, poderá usá-la para gerar a estrutura de dados:</p> 
    <ol> 
     <li value="1">Clique em <strong>[!UICONTROL Adicionar]</strong> botão.</li> 
     <li value="2">Clique em <strong>[!UICONTROL Gerador]</strong> botão.</li> 
     <li value="3">Copie e cole a amostra XML na <strong>[!UICONTROL Dados de exemplo]</strong> campo.</li> 
     <li value="4">Clique em <strong>[!UICONTROL Salvar]</strong>.</li> 
     <li value="5">Verifique se a estrutura de dados foi gerada com êxito.</li> 
     <li value="6"> <p>Clique em <strong>[!UICONTROL Salvar]</strong> botão para salvar a estrutura de dados.</p> <p>É possível ignorar as etapas 2 a 5 para fornecer uma estrutura de dados vazia. Se a estrutura de dados estiver vazia, a saída do módulo não estará disponível no painel de mapeamento até que o módulo tenha sido executado pelo menos uma vez.</p> </li> 
    </ol> <p>Para obter mais informações, consulte <a href="../../workfront-fusion/modules/data-structures.md" class="MCXref xref">Estruturas de dados no [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Preservar números como texto]</td> 
   <td>Habilite essa opção para garantir que os números permaneçam como valores de texto (sequência de caracteres). Caso contrário, os números serão convertidos em valores numéricos.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL XML]</p> </td> 
   <td> <p>Insira ou mapeie o texto XML formatado que deseja analisar.</p> <p>Se você usar uma fórmula, verifique se o tipo de valor do resultado é (ou pode ser forçado automaticamente a) o tipo de dados [!UICONTROL Text]. </p> <p> <img src="assets/if-you-use-a-formula-350x164.png" style="width: 350;height: 164;"> </p> <p>Se o tipo de valor do resultado for [!UICONTROL Buffer] (dados binários), use o <code>toString()</code> para convertê-la no tipo de dados Text. Para obter mais informações, consulte <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Coerção de tipo em [!DNL Adobe Workfront Fusion]</a> e <a href="../../workfront-fusion/mapping/item-data-types.md" class="MCXref xref">Tipos de dados de item no [!UICONTROL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**Exemplo:** Para baixar um arquivo XML de um URL e analisar seu conteúdo:
>
>1. Crie um novo cenário.
>1. Inserir [!UICONTROL HTTP] > [!UICONTROL Obter um arquivo] módulo
>1. Abra a configuração do módulo e configure-o da seguinte maneira:
>
>   **URL**: o URL do arquivo XML (por exemplo, `https://siftrss.com/f/rqLy05ayMBJ`)
>
>   ![](assets/url-of-xml-file-350x184.png)
>
>1. Clique em **[!UICONTROL OK]**&#x200B;para salvar e fechar a configuração do módulo.
1. Adicionar [!UICONTROL XML] > [!UICONTROL Analisar XML] módulo, conecte-o depois que a variável [!UICONTROL HTTP] > [!UICONTROL Obter um arquivo] e a configure da seguinte maneira:
>
<table style="table-layout:auto"> 
&gt;    <col> 
&gt;    <col> 
&gt;    <tbody> 
&gt;     <tr> 
&gt;      <td role="rowheader">[!UICONTROL Estrutura de dados]</td> 
&gt;      <td> 
&gt;       <ol> 
&gt;        <li value="1">Clique em <strong>[!UICONTROL Adicionar]</strong> botão.</li> 
&gt;        <li value="2">Clique em <strong>[!UICONTROL Gerador]</strong> botão.</li> 
&gt;        <li value="3">No navegador da Web, abra uma nova guia ou janela.</li> 
&gt;        <li value="4">Coloque o URL usado na terceira etapa na barra de endereços e busque o arquivo XML.</li> 
&gt;        <li value="5">Selecione todo o texto XML e copie-o para a área de transferência.</li> 
&gt;        <li value="6">Feche a guia ou janela e volte ao seu cenário.</li> 
&gt;        <li value="7">Cole o texto XML copiado no campo Dados de amostra.</li> 
&gt;        <li value="8">Clique em <strong>[!UICONTROL Salvar]</strong>.</li> 
&gt;        <li value="9">Verifique se a estrutura de dados foi gerada com êxito.</li> 
&gt;        <li value="10">Clique em <strong>[!UICONTROL Salvar]</strong> para salvar a estrutura de dados.</li> 
&gt;       </ol> <p>Você pode pular as etapas de 2 a 9 para fornecer uma estrutura de dados vazia. Se a estrutura de dados estiver vazia, a saída do módulo não estará disponível no painel de mapeamento até que o módulo tenha sido executado pelo menos uma vez.</p> </td> 
&gt;     </tr> 
&gt;     <tr> 
&gt;      <td role="rowheader">[!UICONTROL XML]</td> 
&gt;      <td> <p>Mapeie o <code>Data </code>item da saída do módulo [!UICONTROL HTTP] &gt; [!UICONTROL Obter um arquivo] no campo. Use o <code>toString()</code> para converter seu valor do tipo de dados [!UICONTROL Buffer] (dados binários) no tipo de dados [!UICONTROL Text].</p> <p>Você pode copiar e colar o código da fórmula no campo: <code>&#123;&#123;toString(1.data)&#125;&#125;</code></p> <p>Para obter mais informações sobre os tipos de dados Buffer e Texto, consulte <a href="../../workfront-fusion/mapping/item-data-types.md" class="MCXref xref">Tipos de dados de item no Adobe Workfront Fusion</a>.</p> <p> <img src="assets/paste-formula-code-350x99.png" style="width: 350;height: 99;"> </p> </td> 
&gt;     </tr> 
&gt;    </tbody> 
&gt;   </table>

## [!UICONTROL Análise de atributos XML]

Por padrão, a variável [!UICONTROL XML] > [!UICONTROL Analisar XML] o módulo coloca atributos em uma coleção especial `_attributes` como um filho do nó que tem esses atributos. Se o nó for um nó de texto e tiver atributos, duas propriedades especiais serão adicionadas: `_attributes` para atributos e `_value` para o conteúdo de texto do nó.

>[!INFO]
>
**Exemplo:** Este XML:

```
<root attr="1">
<node attr="ABC">Hello, World</node>
</root>
```

é convertido neste pacote:

![](assets/xml-converted-to-bundle.png)

## Criar XML

A variável [!UICONTROL XML] > [!UICONTROL Criar XML] O módulo converte um pacote em um texto XML formatado.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Estrutura de dados]</p> </td> 
   <td> <p>A estrutura de dados descreve a estrutura do XML resultante. Se você tiver uma amostra do XML que deseja criar, poderá usá-la para gerar a estrutura de dados:</p> 
    <ol> 
     <li value="1">Clique em <strong>[!UICONTROL Adicionar]</strong> botão.</li> 
     <li value="2">Clique em <strong>[!UICONTROL Gerador]</strong> botão.</li> 
     <li value="3">Copie e cole a amostra XML no campo Dados de amostra.</li> 
     <li value="4">Clique em <strong>[!UICONTROL Salvar]</strong> botão.</li> 
     <li value="5">Verifique se a estrutura de dados foi gerada com êxito.</li> 
     <li value="6">Clique em <strong>[!UICONTROL Salvar]</strong> para salvar a estrutura de dados.</li> 
    </ol> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nome do elemento raiz]</td> 
   <td>Insira o nome do elemento raiz do XML. O valor padrão é <code>root</code>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL IDENTIFICAÇÃO DO SISTEMA Doctype]</td> 
   <td>Insira o nome de arquivo a ser usado na variável<code> !DOCTYPE SYSTEM</code> declaração</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Doctype ID PÚBLICA]</td> 
   <td>Insira o nome de arquivo a ser usado na variável<code> !DOCTYPE PUBLIC</code> declaração</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Remover Declaração Xml]</td> 
   <td>Habilitar esta opção para remover a Declaração XML <code>&lt;?xml ... ?&gt;</code> e <code>&lt;!DOCTYPE ... &gt;</code>e deixe somente o elemento raiz XML e seu conteúdo.</td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
**Exemplo:**
>
Um caso de uso típico é a transformação de dados de um [!DNL Google] >em XML.
>
1. Coloque o [!DNL Google Sheets] > [!UICONTROL Selecionar linhas] em seu cenário para buscar os dados. Configure o módulo para recuperar linhas do [!DNL Google] planilha eletrônica. Defina o&#x200B;**[!UICONTROL Número máximo de linhas retornadas]** para um número pequeno, mas maior que um para fins de teste (Exemplo, três). Execute o [!DNL Google Sheets] clicando com o botão direito do mouse e escolhendo &quot;**[!UICONTROL Executar este módulo somente]**.&quot; Verifique a saída do módulo.
1. Conecte o [!UICONTROL Agregador de matrizes] módulo após a variável [!DNL Google Sheets] módulo. Na configuração do módulo, escolha a variável [!DNL Google Sheets] módulo no **[!UICONTROL Nó de origem]** campo. Deixe os outros campos como estão para o momento.
1. Conecte o [!UICONTROL XML] > [!UICONTROL Criar XML] módulo após a variável [!UICONTROL Agregador de matrizes] módulo.
>
A configuração do módulo requer uma estrutura de dados que descreva a estrutura da saída XML. Clique em **[!UICONTROL Adicionar]** botão para abrir a configuração da estrutura de dados. A maneira mais fácil de criar essa estrutura de dados é gerá-la automaticamente a partir de uma amostra XML.
>
1. Clique em **[!UICONTROL Gerador]** e cole sua amostra XML na caixa [!UICONTROL Dados de exemplo] campo:
>
![](assets/sample-data-field-350x146.png)
>
1. Clique em **[!UICONTROL Salvar]**. O campo Specification na estrutura Data agora contém a estrutura gerada.
1. Altere o nome da estrutura de dados para algo mais específico e clique em **[!UICONTROL Salvar]**. Um campo correspondente ao atributo de matriz raiz aparece como um campo mapeável na configuração do módulo JSON.
1. Clique em **[!UICONTROL Mapa]** ao lado do campo e mapear o `Array[]` item do [!UICONTROL Agregador de matrizes] saída para ele:
1. Clique em **[!UICONTROL OK]** para fechar a configuração do módulo XML.
1. Abra a configuração do [!UICONTROL Agregador de matrizes] módulo. Altere o **[!UICONTROL Estrutura de destino]** de Personalizado para um campo do módulo XML correspondente ao elemento XML pai.Mapeie os itens do [!DNL Google Sheets] para os campos apropriados.
1. Clique em **[!UICONTROL OK]** para fechar a configuração do módulo Array Aggregator.
1. Execute o cenário.
>
O módulo XML gera o arquivo XML correto.
>
1. Abra a configuração do [!DNL Google Sheets] e aumentar o [!UICONTROL Número máximo de linhas retornadas] para ser maior que o número de linhas na planilha para processar todos os dados.
>
O XML resultante pode ser salvo em [!DNL Dropbox], enviado como um anexo por email, carregado via FTP em um servidor e assim por diante.

## Adição de atributos XML

Se quiser adicionar atributos a um nó complexo (um nó que conterá outros nós), adicione uma coleção com o nome `_attributes` para a nota complexa em sua estrutura de dados personalizada. Esta coleção será mapeada para atributos de nó. Se quiser adicionar atributos a um nó de texto (por exemplo: `<node attr="1">abc</node>`), é necessário adicionar uma coleção `_attributes` para atributos e uma propriedade de texto `_value` para o valor deste nó na estrutura de dados personalizada.

```
{
   "name": "node",
   "type": "collection",
   "spec": [
      {
         "name": "_attributes",
         "type": "collection"
         "spec": [
            {
               "name": "attr1",
               "type": "text"
            }
         ]
      },
      {
         "name": "_value",
         "type": "text"
      }
   ]
}
```

## Solução de problemas: não é possível mapear dados do [!UICONTROL Analisar XML] módulo

Verifique se a estrutura de dados está definida corretamente. Como alternativa, você pode usar uma estrutura de dados vazia e executar o módulo pelo menos uma vez para processar uma entrada XML.
