---
title: Serviços Adobe PDF
description: Serviços Adobe PDF
author: Becky
draft: Probably
feature: Workfront Fusion, Digital Content and Documents
exl-id: e0a5736b-dbdb-43c6-83ff-e88a5625a5bf
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '3213'
ht-degree: 0%

---

# [!DNL Adobe PDF Services]

Com o [!DNL Adobe Workfront Fusion] [!DNL Adobe PDF Services], você pode extrair dados de um arquivo PDF ou gerar um novo arquivo PDF a partir dos dados fornecidos. Além disso, é possível converter uma variedade de tipos de arquivos em PDF ou PDF em outros tipos de arquivos. Os Serviços PDF também permitem combinar, compactar ou ler metadados de um arquivo PDF, bem como controlar a proteção de senha no arquivo.

Se precisar de instruções para criar um cenário, consulte [Crie um cenário em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

Para obter informações sobre módulos, consulte [Módulos em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

Para obter informações sobre a API usada para os serviços do PDF, consulte [API de geração de documento do Adobe](https://www.adobe.io/apis/documentcloud/dcsdk/doc-generation.html).

## Considerações ao usar [!DNL Adobe PDF Services]

* [Você não precisa de um [!DNL Adobe] account](#you-do-not-need-an-adobe-account)
* [[!DNL Workfront Fusion] não armazena os arquivos](#workfront-fusion-does-not-store-your-files)

### Você não precisa de um [!DNL Adobe] account

Porque [!DNL Workfront Fusion] faz parte do [!DNL Adobe] conjunto de produtos, você não precisa de um [!DNL Adobe] para usar essas ferramentas. Cada ferramenta acessa [!DNL Adobe] funcionalidade PDF sem usar uma conexão.

Embora [!DNL Workfront Fusion] não exige uma [!DNL Adobe] para usar os serviços do PDF, os módulos exigem uma conexão. Não há credenciais envolvidas nesta conexão e você fornece apenas um nome para a própria conexão.

### [!DNL Workfront Fusion] não armazena os arquivos

O [!DNL Adobe PDF Services] pode ler, converter ou modificar seus arquivos, mas nenhum [!DNL Adobe] nor [!DNL Workfront Fusion] armazene seus arquivos ou dados. Isso significa que:

* Você mantém controle sobre seus arquivos, incluindo sua segurança
* Você não precisa ter um [!UICONTROL Adobe] conta de armazenamento ou armazenamento em nuvem para usar os serviços do PDF.

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] para automação e integração de trabalho] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produto</td> 
   <td>Sua organização deve comprar [!DNL Adobe Workfront Fusion] bem como [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo.</td> 
  </tr> 
 </tbody> 
</table>

Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com seu [!DNL Workfront] administrador.

Para obter informações sobre [!DNL Adobe Workfront Fusion] licenças, consulte [[!DNL Adobe Workfront Fusion] licenças](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!DNL Adobe PDF Services] módulos e seus campos

Ao configurar [!DNL PDF Services], [!DNL Workfront Fusion] exibe os campos listados abaixo. Juntamente com esses campos, campos adicionais podem ser exibidos, dependendo de fatores como seu nível de acesso no aplicativo ou serviço. Um título em negrito em um módulo indica um campo obrigatório.

Se o botão de mapa for exibido acima de um campo ou função, é possível usá-lo para definir variáveis e funções para esse campo. Para obter mais informações, consulte [Mapear informações de um módulo para outro no [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [[!UICONTROL Gerar documento]](#generate-document)
* [[!UICONTROL Extrair texto/tabela]](#extract-text--table)
* [[!UICONTROL Combinar arquivos do PDF]](#combine-pdf-files)
* [[!UICONTROL Compactar arquivos PDF]](#compress-pdf-files)
* [[!UICONTROL Converter documento em arquivo PDF]](#convert-document-to-pdf-file)
* [[!UICONTROL Converter HTML para arquivo PDF]](#convert-html-to-pdf-file)
* [[!UICONTROL Converter imagem em arquivo PDF]](#convert-image-to-pdf-file)
* [[!UICONTROL Converter PDF para documento]](#convert-pdf-to-document)
* [[!UICONTROL Converter PDF para imagem]](#convert-pdf-to-image)
* [[!UICONTROL Linearizar um arquivo PDF]](#linearize-a-pdf-file)
* [[!UICONTROL OCR para arquivo PDF]](#ocr-for-pdf-file)
* [[!UICONTROL Manipulação de PDF page]](#pdf-page-manipulation)
* [[!UICONTROL Propriedades do arquivo PDF]](#pdf-file-properties)
* [[!UICONTROL Arquivo PDF do Protect]](#protect-pdf-file)
* [[!UICONTROL Remover proteção de um arquivo PDF]](#remove-protection-of-a-pdf-file)

### [!UICONTROL Gerar documento]

O [!UICONTROL Gerar documento] é uma maneira poderosa de criar um PDF que contenha dados selecionados. Você pode formatá-la usando um [!DNL Microsoft Word] ou fornecendo dados no formato JSON.

Para obter mais informações sobre o [!UICONTROL [!DNL Adobe PDF Services] Gerar documento] consulte a [Visão Geral da Geração de Documento](https://www.adobe.io/apis/documentcloud/dcsdk/docs.html) no [!DNL Adobe Document Services] documentação.

* [Use o [!UICONTROL Gerar documento] com um [!DNL Microsoft Word] modelo](#use-the-generate-document-module-with-a-microsoft-word-template)
* [Use o [!UICONTROL Gerar documento] módulo com JSON](#use-the-generate-document-module-with-json)

#### Use o [!UICONTROL Gerar documento] com um [!DNL Microsoft Word] modelo

<!--
>[!NOTE]
>
>For a discussion of Microsoft Word templates, see [Microsoft Word Template modules](../../workfront-fusion/apps-and-their-modules/microsoft-word-templates-modules.md). 
>
>You do not need to use Microsoft Word template modules to use a Microsoft Word template with the PDF Services Generate document module.
-->

Para usar o [!UICONTROL Gerar documento] com um [!UICONTROL Microsoft Word] , primeiro crie o template. Para obter instruções, pesquise por &quot;Criar um modelo&quot; no [!DNL Microsoft Office] documentação.

Preencha o [!UICONTROL Gerar documento] campos de módulo como se segue:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Selecione a conexão a ser usada para este módulo.</p> <p>Você não precisa de um [!DNL Adobe] para criar uma conexão PDF Services. Para obter mais informações, consulte <a href="#you-do-not-need-an-adobe-account" class="MCXref xref">Você não precisa de um [!DNL Adobe] account</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Arquivo de origem]</td> 
   <td> <p>Selecione um arquivo de origem de um módulo anterior ou mapeie o nome e os dados do arquivo de origem.</p> <p>Esse arquivo de origem é o [!DNL Microsoft Word ]template que o módulo usa para gerar o novo PDF.</p> <p>Recomendamos criar um projeto no [!DNL Workfront] para [!DNL Microsoft Word] modelos usados em [!DNL Workfront Fusion]. Em seguida, você pode usar o [!DNL Workfront] &gt; Módulo de download do [!UICONTROL document] para inserir o modelo apropriado ao seu cenário.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Formato de saída]</td> 
   <td> <p>Selecione o formato do documento gerado.</p> 
    <ul> 
     <li> <p>PDF</p> </li> 
     <li> <p>DOCX</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Dados para mesclagem]</td> 
   <td> <p>Para cada tag de valor no modelo que você deseja substituir por texto, preencha o seguinte:</p> 
    <ul> 
     <li> <p>[!UICONTROL Chave]</p> <p>Insira uma chave. No modelo, a chave é o texto mostrado na tag de valor. Por exemplo, se você deseja colocar texto na tag de valor <code>&#123;&#123;name&#125;&#125;</code>, insira <code>name </code>no campo key .</p> </li> 
     <li> <p>Tipo de valor</p> <p>Selecione se os dados no campo de valor são um valor, um objeto ou uma matriz de objetos.</p> </li> 
     <li> <p>[!UICONTROL Valor]</p> <p>Insira ou mapeie o texto que você deseja que apareça no documento gerado no lugar da tag de valor.</p> </li> 
    </ul> <p> <img src="assets/generate-with-template-350x241.png" style="width: 350;height: 241;"> </p> </td> 
  </tr> 
 </tbody> 
</table>

#### Use o [!UICONTROL Gerar documento] módulo com JSON

Para usar o [!UICONTROL Gerar documento] com JSON, preencha os campos da seguinte maneira:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Selecione a conexão a ser usada para este módulo.</p> <p>Você não precisa de um [!DNL Adobe] para criar uma conexão PDF Services. Para obter mais informações, consulte <a href="#you-do-not-need-an-adobe-account" class="MCXref xref">Você não precisa de um [!DNL Adobe] account</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Arquivo de origem]</td> 
   <td> <p>Selecione um arquivo de origem de um módulo anterior ou mapeie o nome e os dados do arquivo de origem.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Formato de saída]</td> 
   <td> <p>Selecione o formato do documento gerado.</p> 
    <ul> 
     <li> <p>PDF</p> </li> 
     <li> <p>DOCX</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Dados para mesclagem]</td> 
   <td> <p>Para usar o JSON neste módulo, você deve habilitar o mapeamento neste campo.</p> <p>Insira ou mapeie o JSON para gerar o documento. </p> <p>Você pode digitar JSON diretamente nesse campo ou mapear a saída JSON de um módulo JSON.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Extrair texto/tabela]

Este módulo de ação permite extrair dados de um arquivo PDF. O módulo gera elementos de texto individuais, como um parágrafo ou o texto em uma única célula de uma tabela.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Selecione a conexão a ser usada para este módulo.</p> <p>Você não precisa de um [!DNL Adobe] para criar uma conexão PDF Services. Para obter mais informações, consulte <a href="#you-do-not-need-an-adobe-account" class="MCXref xref">Você não precisa de um [!DNL Adobe] account</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Arquivo de origem]</td> 
   <td>Selecione um arquivo de origem de um módulo anterior ou mapeie o nome e os dados do arquivo de origem.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Elementos que devem ser extraídos como JSON]</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Texto]</p> </li> 
     <li> <p>[!UICONTROL Tabelas]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Extrair caixas delimitadoras?]</td> 
   <td>Ative essa opção para extrair dados sobre a caixa delimitadora do texto.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Incluir informações de estilo para saída?]</td> 
   <td>Ative essa opção para adicionar informações de estilo ao JSON de saída.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Combinar arquivos do PDF]

Esse módulo de ação pega vários arquivos PDF e os combina em um único arquivo PDF. Por exemplo, esse módulo pode combinar todos os documentos em um [!UICONTROL Workfront] projeto num único PDF após a conclusão do projeto.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Selecione a conexão a ser usada para este módulo.</p> <p>Você não precisa de um [!DNL Adobe] para criar uma conexão PDF Services. Para obter mais informações, consulte <a href="#you-do-not-need-an-adobe-account" class="MCXref xref">Você não precisa de um [!DNL Adobe] account</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Documentos]</td> 
   <td> <p>Você pode usar um módulo agregador para coletar documentos para combiná-los em um PDF, ou pode adicionar os documentos manualmente. </p> <p>Recomendamos o uso de um módulo [!UICONTROL Array Aggregator] para agregar a saída de um módulo anterior. Ao usar um agregador, não é necessário saber os nomes, locais ou números de arquivos que serão combinados. O uso de um agregador é, portanto, muito mais flexível e escalável do que a inserção manual dos documentos a serem combinados.</p> <p>Para usar o módulo de arquivos [!UICONTROL Combinar PDF] com um agregador, você deve habilitar o mapeamento no campo [!UICONTROL Documents]. </p> <p>Neste exemplo, o módulo [!UICONTROL Ler registros relacionados] identifica documentos associados a um projeto e o módulo [!UICONTROL Baixar documentos] baixa cada um. Todos os PDF são agregados em uma matriz, que é passada para o módulo de arquivos [!UICONTROL Combinar PDF].</p> <p> <img src="assets/combine-example-350x104.png" style="width: 350;height: 104;"> </p> <p>Você também pode inserir documentos manualmente.</p> <p>Para cada documento a ser incluído na PDF combinada:</p> 
    <ol> 
     <li value="1"> <p>Clique em [!UICONTROL Adicionar um documento]</p> </li> 
     <li value="2"> <p>No campo [!UICONTROL Source file], selecione o módulo que gera o documento que deseja incluir ou mapeie o nome e os dados do arquivo de origem. </p> </li> 
     <li value="3"> <p>(Opcional) Se desejar incluir apenas determinadas páginas do arquivo de origem, para cada intervalo de páginas que deseja adicionar, clique em <strong>[!UICONTROL Adicionar item]</strong> no campo [!UICONTROL Páginas] , insira a primeira e a última página do intervalo de páginas a ser incluído e clique em <strong>[!UICONTROL Adicionar]</strong>. É possível incluir mais de um intervalo de páginas a partir de um único documento.</p> </li> 
     <li value="4"> <p>Clique em <strong>[!UICONTROL Adicionar]</strong>. </p> </li> 
    </ol> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Compactar arquivos PDF]

Esse módulo de ação usa um arquivo PDF e o compacta. Isso pode ser útil para economizar largura de banda ou memória.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Selecione a conexão a ser usada para este módulo.</p> <p>Você não precisa de um [!DNL Adobe] para criar uma conexão PDF Services. Para obter mais informações, consulte <a href="#you-do-not-need-an-adobe-account" class="MCXref xref">Você não precisa de um [!DNL Adobe] account</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Arquivo de origem]</td> 
   <td> <p>Selecione um arquivo de origem de um módulo anterior ou mapeie o nome e os dados do arquivo de origem.</p> <p>O arquivo de origem deve estar no formato PDF. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nível de compactação]</td> 
   <td>Selecione o nível de compactação que deseja usar.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Converter documento em arquivo PDF]

Essa ferramenta converte um documento em um arquivo PDF. O arquivo de origem deve ser um dos seguintes formatos de documento:

* DOC
* XLS
* PPT
* TXT
* RTF

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Selecione a conexão a ser usada para este módulo.</p> <p>Você não precisa de um [!DNL Adobe] para criar uma conexão PDF Services. Para obter mais informações, consulte <a href="#you-do-not-need-an-adobe-account" class="MCXref xref">Você não precisa de um [!DNL Adobe] account</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Arquivo de origem]</td> 
   <td> <p>Selecione um arquivo de origem de um módulo anterior ou mapeie o nome e os dados do arquivo de origem.</p> <p>O arquivo de origem deve estar em um dos seguintes formatos:</p> 
    <ul> 
     <li> <p>DOC</p> </li> 
     <li> <p>XLS</p> </li> 
     <li> <p>PPT</p> </li> 
     <li> <p>TXT</p> </li> 
     <li> <p>RTF</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Language]</td> 
   <td> <p>Selecione o idioma padrão para o documento de origem. Isso permite que o módulo selecione uma fonte apropriada, se não a fonte estiver incluída no arquivo de origem.</p> <p>Selecione um dos seguintes idiomas:</p> 
    <ul> 
     <li> <p>en-US (Padrão): Inglês (Estados Unidos da América)</p> </li> 
     <li> <p>ca-ES: Catalão (Espanha)</p> </li> 
     <li> <p>cs-CZ: Tcheco (República Tcheca)</p> </li> 
     <li> <p>da-DK: Dinamarquês (Dinamarca)</p> </li> 
     <li> <p>de-DE: Alemão (Alemanha)</p> </li> 
     <li> <p>en-AE: Inglês (Emirados Árabes Unidos)</p> </li> 
     <li> <p>en-GB: Inglês (Reino Unido)</p> </li> 
     <li> <p>en-IL: Inglês (Israel)</p> </li> 
     <li> <p>en-US: Inglês (Estados Unidos da América)</p> </li> 
     <li> <p>es-ES: Espanhol (Espanha)</p> </li> 
     <li> <p>es-MX: Espanhol (México)</p> </li> 
     <li> <p>eu-ES: Basco (Espanha)</p> </li> 
     <li> <p>fi-FI: Finlandês (Finlândia)</p> </li> 
     <li> <p>fr-CA: Francês (Canadá)</p> </li> 
     <li> <p>fr-FR: Francês (França)</p> </li> 
     <li> <p>fr-MA: Francês (Marrocos)</p> </li> 
     <li> <p>hr-HR: Croata (Croácia)</p> </li> 
     <li> <p>hu-HU: Húngaro (Hungria)</p> </li> 
     <li> <p>it-IT: Italiano (Itália)</p> </li> 
     <li> <p>ja-JP: Japonês (Japão)</p> </li> 
     <li> <p>kr-KR: Coreano (Coreia do Sul)</p> </li> 
     <li> <p>nb-NO: Bokmål Norueguês (Noruega)</p> </li> 
     <li> <p>nl-NL: Holandês (Países Baixos)</p> </li> 
     <li> <p>pl-PL: Polonês (Polônia)</p> </li> 
     <li> <p>pt-BR: Português (Brasil)</p> </li> 
     <li> <p>pt-PT: Português (Portugal)</p> </li> 
     <li> <p>ro-RO: Romeno (Romênia)</p> </li> 
     <li> <p>ru-RU: Russo (Rússia)</p> </li> 
     <li> <p>sk-SK: Eslovaco (Eslováquia)</p> </li> 
     <li> <p>sl-SI: Esloveno (Eslovênia)</p> </li> 
     <li> <p>sv-SE: Sueco (Suécia)</p> </li> 
     <li> <p>tr-TR: Turco (Turquia)</p> </li> 
     <li> <p>uk-UA: Ucraniano (Ucrânia)</p> </li> 
     <li> <p>zh-CN: Chinês (China Continental)</p> </li> 
     <li> <p>zh-TW: Chinês (Taiwan)</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Converter HTML para arquivo PDF]

Essa ferramenta converte um arquivo HTML em um arquivo PDF.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Selecione a conexão a ser usada para este módulo.</p> <p>Você não precisa de um [!DNL Adobe] para criar uma conexão PDF Services. Para obter mais informações, consulte <a href="#you-do-not-need-an-adobe-account" class="MCXref xref">Você não precisa de um [!DNL Adobe] account</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Arquivo de origem]</td> 
   <td> <p>Selecione um arquivo de origem de um módulo anterior ou mapeie o nome e os dados do arquivo de origem.</p> <p>Importante: O arquivo de origem deve estar no formato HTML ou ZIP. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL JSON]</td> 
   <td> <p>Se o seu HTML fizer referência às variáveis do JavaScript, você poderá incluir essas variáveis aqui. </p> <p>Para cada variável, clique em <strong>[!UICONTROL Adicionar item]</strong> e inclua a chave e o valor da variável.</p> <p>Nota:   
     <ul> 
      <li> <p>Ao criar um PDF a partir de um arquivo ZIP, a garantia de origem deve incluir um elemento de script, como: <code> &lt;script src='./json.js' type='text/javascript'&gt;&lt;/script&gt;</code> </p> </li> 
      <li> <p>Ao criar um PDF a partir de um URL, o conteúdo desse objeto JSON é inserido na VM do navegador antes da renderização da página. </p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Incluir cabeçalho e rodapé]</td> 
   <td> <p>Ative essa opção para criar cabeçalhos e rodapés para o documento do PDF.</p> 
    <ul> 
     <li> <p>O cabeçalho inclui uma data e o título do documento.</p> </li> 
     <li> <p>O rodapé inclui o nome do arquivo e um número de página.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Largura da página]</td> 
   <td>Insira a largura do papel, em polegadas. O módulo usa essas informações para formatar as páginas no arquivo PDF criado.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Altura da página]</td> 
   <td>Insira a altura do papel, em polegadas. O módulo usa essas informações para formatar as páginas no arquivo PDF criado.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Converter imagem em arquivo PDF]

Essa ferramenta converte uma imagem em um arquivo PDF.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Selecione a conexão a ser usada para este módulo.</p> <p>Você não precisa de um [!DNL Adobe] para criar uma conexão PDF Services. Para obter mais informações, consulte <a href="#you-do-not-need-an-adobe-account" class="MCXref xref">Você não precisa de um [!DNL Adobe] account</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Arquivo de origem]</td> 
   <td> <p>Selecione um arquivo de origem de um módulo anterior ou mapeie o nome e o arquivo de imagem do arquivo de origem.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Converter PDF para documento]

Essa ferramenta converte um arquivo PDF em um documento. Você pode selecionar um dos formatos a seguir para o arquivo de saída.

* DOC
* DOCX
* PPTX
* XLSX
* RTF

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Selecione a conexão a ser usada para este módulo.</p> <p>Você não precisa de um [!DNL Adobe] para criar uma conexão PDF Services. Para obter mais informações, consulte <a href="#you-do-not-need-an-adobe-account" class="MCXref xref">Você não precisa de um [!DNL Adobe] account</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Arquivo de origem]</td> 
   <td> <p>Selecione um arquivo de origem de um módulo anterior ou mapeie o nome e os dados do arquivo de origem.</p> <p>O arquivo de origem deve estar no formato PDF. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Formato de arquivos de saída]</td> 
   <td> <p>Selecione o formato no qual deseja que os arquivos sejam enviados:</p> 
    <ul> 
     <li> <p>DOC</p> </li> 
     <li> <p>DOCX</p> </li> 
     <li> <p>PPTX</p> </li> 
     <li> <p>XLSX</p> </li> 
     <li> <p>RTF</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Converter PDF para imagem]

Essa ferramenta converte um PDF em uma imagem no formato PNG ou JPEG, que é então emitido como ZIP. A PDF é convertida em uma imagem por página e cada imagem termina com o número da página. Os arquivos de imagem são combinados em um arquivo ZIP.

Por exemplo, um arquivo chamado &quot;TestFile&quot; com 8 páginas produziria 8 imagens, chamadas &quot;TestFile_1&quot; por &quot;TestFile_8&quot;. A saída do módulo é um arquivo ZIP contendo as 8 imagens.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Selecione a conexão a ser usada para este módulo.</p> <p>Você não precisa de um [!DNL Adobe] para criar uma conexão PDF Services. Para obter mais informações, consulte <a href="#you-do-not-need-an-adobe-account" class="MCXref xref">Você não precisa de um [!DNL Adobe] account</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Arquivo de origem]</td> 
   <td> <p>Selecione um arquivo de origem de um módulo anterior ou mapeie o nome e os dados do arquivo de origem.</p> <p>O arquivo de origem deve estar no formato PDF. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Formato de arquivos de saída]</td> 
   <td> <p>Selecione o formato no qual deseja que os arquivos sejam enviados:</p> 
    <ul> 
     <li>Imagem PNG</li> 
     <li>JPEG</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Linearizar um arquivo PDF]

Essa ferramenta lineariza um documento do PDF para criar um documento PDF otimizado para a Web. Um documento PDF linearizado pode ser visualizado página por página sem a necessidade de baixar o documento inteiro.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Selecione a conexão a ser usada para este módulo.</p> <p>Você não precisa de um [!DNL Adobe] para criar uma conexão PDF Services. Para obter mais informações, consulte <a href="#you-do-not-need-an-adobe-account" class="MCXref xref">Você não precisa de um [!DNL Adobe] account</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Arquivo de origem]</td> 
   <td> <p>Selecione um arquivo de origem de um módulo anterior ou mapeie o nome e os dados do arquivo de origem.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL OCR para arquivo PDF]

Essa ferramenta executa o OCR (Optical Character Reconhecimento) em um arquivo e produz um PDF.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Selecione a conexão a ser usada para este módulo.</p> <p>Você não precisa de um [!DNL Adobe] para criar uma conexão PDF Services. Para obter mais informações, consulte <a href="#you-do-not-need-an-adobe-account" class="MCXref xref">Você não precisa de um [!DNL Adobe] account</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Arquivo de origem]</td> 
   <td> <p>Selecione um arquivo de origem de um módulo anterior ou mapeie o nome e os dados do arquivo de origem.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL tipo OCR]</td> 
   <td> 
    <ul> 
     <li> <p>O tipo [!UICONTROL Imagem original modificada] garante que o texto seja pesquisável e selecionável, mas modifica a imagem original durante o processo de limpeza (por exemplo, a desenha) antes de colocar uma camada de texto invisível sobre ela. Esse tipo remove artefatos indesejados e pode resultar em um documento mais legível em alguns cenários. </p> </li> 
     <li> <p>O tipo [!UICONTROL Imagem original inalterada] também sobrepõe uma camada de texto pesquisável sobre a imagem original, mas, nesse caso, a imagem original permanece inalterada. Esse tipo produz a fidelidade máxima da imagem original.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Language]</td> 
   <td>Selecione o idioma deste documento.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Manipulação de PDF page]

Esse módulo permite que você gire ou exclua seletivamente páginas em um documento PDF. Por exemplo, é possível alterar a exibição retrato para paisagem ou remover determinadas páginas do documento PDF.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Selecione a conexão a ser usada para este módulo.</p> <p>Você não precisa de um [!DNL Adobe] para criar uma conexão PDF Services. Para obter mais informações, consulte <a href="#you-do-not-need-an-adobe-account" class="MCXref xref">Você não precisa de um [!DNL Adobe] account</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Arquivo de origem]</td> 
   <td> <p>Selecione um arquivo de origem de um módulo anterior ou mapeie o nome e os dados do arquivo de origem.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ação]</td> 
   <td> <p>Selecione a ação que deseja executar no arquivo.</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Excluir]</b> </p> <p>Selecione esta opção para excluir páginas do documento.</p> </li> 
     <li> <p><b>[!UICONTROL Girar]</b> </p> <p>Selecione essa opção para girar as páginas e, em seguida, insira o ângulo, em graus no sentido horário, em que deseja girar as páginas do documento em relação à orientação inicial.</p> <p>Para girar de retrato para paisagem ou vice-versa, gire a página 90 ou 270 graus.</p> <p>Se uma página estiver de cabeça para baixo, gire-a 180 graus.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Páginas]</td> 
   <td> <p>Para cada intervalo de páginas que deseja excluir, clique em <strong>[!UICONTROL Adicionar]</strong> e insira a primeira e a última página do intervalo de páginas. </p> <p>Nota:   
     <ul> 
      <li> <p>Você pode usar números negativos para contar a partir do fim do documento. A última página de um documento é -1, a segunda para a última página é -2 e assim por diante.</p> </li> 
      <li> <p>Para excluir uma única página, defina o mesmo número de página como o início e o fim do intervalo.</p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limite]</td> 
   <td> <p>Insira ou mapeie o número máximo de registros com os quais deseja que o módulo funcione durante cada ciclo de execução de cenário.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Propriedades do arquivo PDF]

Esta ferramenta extrai informações básicas sobre o documento, como:

* Contagem de página
* Versão do PDF
* Se o arquivo está criptografado
* Se o arquivo é linerarizado
* Se o arquivo contém arquivos incorporados

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Selecione a conexão a ser usada para este módulo.</p> <p>Você não precisa de um [!DNL Adobe] para criar uma conexão PDF Services. Para obter mais informações, consulte <a href="#you-do-not-need-an-adobe-account" class="MCXref xref">Você não precisa de um [!DNL Adobe] account</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Arquivo de origem]</td> 
   <td> <p>Selecione um arquivo de origem de um módulo anterior ou mapeie o nome e os dados do arquivo de origem.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Arquivo PDF do Protect]

Esta ferramenta protege um documento PDF com uma senha de usuário ou proprietário. Também define restrições em determinados recursos, como impressão, edição e cópia no documento do PDF. Você seleciona o tipo de conteúdo a ser criptografado e o algoritmo de criptografia.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Selecione a conexão a ser usada para este módulo.</p> <p>Você não precisa de um [!DNL Adobe] para criar uma conexão PDF Services. Para obter mais informações, consulte <a href="#you-do-not-need-an-adobe-account" class="MCXref xref">Você não precisa de um [!DNL Adobe] account</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Arquivo de origem]</td> 
   <td> <p>Selecione um arquivo de origem de um módulo anterior ou mapeie o nome e os dados do arquivo de origem.</p> <p>O arquivo de origem deve estar no formato PDF. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de proteção por senha]</td> 
   <td> <p>Ative essa opção para usar senhas para criptografar o documento PDF de entrada. Se ativar essa opção, você deverá especificar e inserir um valor para um ou ambos os itens a seguir: </p> 
    <ul> 
     <li> <p>[!UICONTROL userPassword]</p> </li> 
     <li> <p>[!UICONTROL ownerPassword] </p> </li> 
    </ul> <p>Cada senha pode ter até 128 caracteres.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Encryption Algorithm]</td> 
   <td> <p>Selecione o algoritmo de criptografia. </p> 
    <ul> 
     <li> <p>[!UICONTROL AES-128 encryption]</p> <p>A senha suporta apenas caracteres LATIN-I. </p> </li> 
     <li> <p>[!UICONTROL AES-256 encryption]</p> <p>A senha suporta o conjunto de caracteres Unicode</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conteúdo para criptografar]</td> 
   <td> <p>Selecione o tipo de conteúdo a ser criptografado.</p> 
    <ul> 
     <li> <p>[!UICONTROL Todo o conteúdo]</p> </li> 
     <li> <p>[!UICONTROL Todo o conteúdo exceto metadados]</p> </li> 
     <li> <p>[!UICONTROL Somente dados incorporados] </p> </li> 
    </ul> <p>Selecionar "[!UICONTROL Somente dados incorporados]" torna ineficazes todas as permissões de acesso fornecidas.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Permissões]</td> 
   <td> <p>Selecione todas as permissões que deseja incluir para permitir a impressão, edição ou cópia de conteúdo.</p> <p>As configurações de permissão só serão usadas se [!UICONTROL ownerPassword] estiver definido no campo [!UICONTROL Password Protection Type].</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Remover proteção de um arquivo PDF]

Esta ferramenta remove a segurança (proteção por senha) de um documento PDF.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Selecione a conexão a ser usada para este módulo.</p> <p>Você não precisa de um [!DNL Adobe] para criar uma conexão PDF Services. Para obter mais informações, consulte <a href="#you-do-not-need-an-adobe-account" class="MCXref xref">Você não precisa de um [!DNL Adobe] account</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Arquivo de origem]</td> 
   <td> <p>Selecione um arquivo de origem de um módulo anterior ou mapeie o nome e os dados do arquivo de origem.</p> <p>O arquivo de origem deve estar no formato PDF.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Senha]</td> 
   <td>Digite a senha que protege o arquivo no momento.</td> 
  </tr> 
 </tbody> 
</table>
