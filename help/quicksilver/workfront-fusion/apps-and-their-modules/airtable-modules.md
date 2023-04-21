---
filename: airtable-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: conector
navigation-topic: apps-and-their-modules
title: Módulos aeronáuticos
description: O Adobe Workfront Fusion exige uma licença do Adobe Workfront Fusion além de uma licença da Adobe Workfront.
author: Becky
exl-id: 5d061b23-0a39-44e6-ac9b-0ef5ac7e9ab4
source-git-commit: 9460e14a66653eaf1856cdf5c1ab3213859f354a
workflow-type: tm+mt
source-wordcount: '1863'
ht-degree: 2%

---

# Módulos aeronáuticos


Com o [!DNL Airtable] conector para [!DNL Adobe Workfront Fusion], você pode iniciar um cenário com base nos eventos em [!DNL Airtable] crie, faça upload e atualize registros, pesquise registros e faça chamadas de API personalizadas para a API do Airtable.

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

## Pré-requisitos

Você deve ter uma conta do Airtable para usar a funcionalidade neste artigo.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">For more information, see the tutorial .</p>
-->

## Conectar Airtable ao Workfront Fusion {#connect-airtable-to-workfront-fusion}

<!--

1. Log in to your Airtable account.
1. Open your account overview and generate the API key.
-->
1. Abra o Workfront Fusion e o **Criar uma conexão** do módulo desejado.
1. Digite um nome para a conexão.
1. (Opcional) Clique em Mostrar configurações avançadas e insira a ID do cliente do Airtable e o Segredo do cliente.
1. Clique no botão **Continuar** para criar a conexão e retornar ao módulo.

## Módulos aeronáuticos e respectivos campos

### Registros

* [Criar um registro](#create-a-record)
* [Excluir um registro](#delete-a-record)
* [Obter um registro](#get-a-record)
* [Pesquisar registros](#search-records)
* [Atualizar um registro](#update-a-record)
* [Atualizar um registro](#upsert-a-record)
* [Ver registros](#watch-records)
* [Assista às respostas](#watch-responses)
* [Efetuar uma chamada de API](#make-an-api-call)

#### Criar um registro {#create-a-record}

Esse módulo de ação cria um novo registro.

Especifique os dados que deseja incluir no registro e onde deseja armazená-los.

O módulo retorna quaisquer campos padrão associados ao registro, juntamente com quaisquer campos e valores personalizados que a conexão acessa. Você pode mapear essas informações em módulos subsequentes do cenário.

Ao configurar esse módulo, os seguintes campos são exibidos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Conexão </td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do Airtable ao Workfront Fusion, consulte <a href="#connect-airtable-to-workfront-fusion" class="MCXref xref">Conectar Airtable ao Workfront Fusion</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td>Base </td> 
   <td> <p>Selecione a base à qual o novo registro pertencerá.</p> </td> 
  </tr> 
  <tr> 
   <td>Tabela </td> 
   <td> <p>Selecione a tabela à qual o novo registro pertencerá.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Registro</p> </td> 
   <td> <p>Insira os valores para o novo registro. Os campos disponíveis são baseados na tabela selecionada.</p> <!--<p>For more information on field types, search for "Supported field types" in the Airtable documentation.</p> 
    <ul> 
     <li> <p><strong>Text</strong>: string</p> <p>A single line of text.</p> </li> 
     <li> <p><strong>Long text</strong>: string</p> <p>Multiple lines of text, which may contain "mention tokens", for example:</p><pre>&lt;airtable:mention id="menE1i9oBaGX3DseR"&gt;@Alex&lt;/airtable:mention&gt;</pre> </li> 
     <li><strong>Attachment</strong> : Add the attachment. Airtable will download the file from the provided <code>url</code> and keep its own copy of it. If the File name field is left empty, Airtable generates the name automatically.</li> 
     <li><strong>Checkbox</strong>: Select one of the options.</li> 
     <li><strong>Multiple select</strong>: Select multiple options in the checklist.</li> 
     <li><strong>Single select</strong>: Select one option from the drop-down menu.</li> 
     <li><strong>Collaborator</strong>: Enter the email that uniquely identifies a user in Airtable who this base is shared with.</li> 
     <li><strong>Date</strong>: UTC date, for example, 2019-09-05 (ISO 8601 formatted date)</li> 
     <li>Phone number:</li> 
     <li><strong>Emails</strong>: A valid email address.</li> 
     <li><strong>URL</strong>: A valid URL (for example, airtable.com or https://airtable.com/universe).</li> 
     <li><strong>Number</strong>: Enter a number.</li> 
     <li><strong>Currency</strong>: Currency value.</li> 
     <li><strong>Percent</strong>: A percentage value. Must be higher than or equal to 0.</li> 
     <li><strong>Duration</strong>: Enter the duration time. If you need help, see the information about the duration field type in the Airtable support documentation. </li> 
     <li><strong>Rating</strong>: Enter the number. For example, "3 stars" is 3. A rating cannot be 0.</li> 
     <li><strong>Link</strong>: Enter the linked records IDs from the table. The order of record IDs will be reversed compared to what you see in the app.</li> 
     <li><strong>Rollup</strong>: Computed value: COUNT(values)</li> 
     <li><strong>Lookup</strong>: Array of long text fields</li> 
     <li><strong>Autonumber</strong>: Automatically incremented unique counter for each record.</li> 
     <li> <p><strong>Barcode</strong>: The barcode object may contain the following two properties, both of which are optional.</p> <p>Barcode data (text)</p> <p>Barcode symbology, for example, "upce" or "code39" (type)</p> </li> 
    </ul> --></td> 
  </tr> 
  <tr> 
   <td>Links inteligentes</td> 
   <td> <p>Habilite esta opção para inserir nomes em vez de IDs de registro em campos que vinculam a outra tabela. O registro é criado automaticamente na tabela vinculada se não houver correspondência.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Excluir um registro {#delete-a-record}

Esse módulo de ação exclui um registro específico.

Você especifica a ID e os locais do registro.

O módulo retorna a ID do registro e quaisquer campos associados, juntamente com quaisquer campos e valores personalizados que a conexão acessa. Você pode mapear essas informações em módulos subsequentes do cenário.

Ao configurar esse módulo, os seguintes campos são exibidos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Conexão </td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do Airtable ao Workfront Fusion, consulte <a href="#connect-airtable-to-workfront-fusion" class="MCXref xref">Conectar Airtable ao Workfront Fusion</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td>Base </td> 
   <td> <p>Selecione a base que contém o registro que deseja excluir.</p> </td> 
  </tr> 
  <tr> 
   <td>Tabela </td> 
   <td> <p>Selecione a tabela que contém o registro que deseja excluir.</p> </td> 
  </tr> 
  <tr> 
   <td>ID de registro</td> 
   <td> <p>Insira ou mapeie a ID do Airtable exclusiva do registro que você deseja que o módulo exclua. Você pode recuperar a ID, por exemplo, usando o módulo Pesquisar registros .</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Obter um registro {#get-a-record}

Este módulo de ação recupera detalhes do registro.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Conexão </td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do Airtable ao Workfront Fusion, consulte <a href="#connect-airtable-to-workfront-fusion" class="MCXref xref">Conectar Airtable ao Workfront Fusion</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td>Base </td> 
   <td> <p>Selecione a base que contém a tabela com o registro que você deseja recuperar.</p> </td> 
  </tr> 
  <tr> 
   <td>Tabela</td> 
   <td> <p> Selecione a tabela que contém o registro para o qual deseja recuperar detalhes.</p> </td> 
  </tr> 
  <tr> 
   <td>ID de registro</td> 
   <td> <p> Insira ou mapeie a ID do registro para o qual deseja recuperar detalhes.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Pesquisar registros {#search-records}

Este módulo de pesquisa procura registros em um objeto no Airtable que correspondam à consulta de pesquisa especificada.

Você pode mapear essas informações em módulos subsequentes do cenário.

Ao configurar esse módulo, os seguintes campos são exibidos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Conexão </td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do Airtable ao Workfront Fusion, consulte <a href="#connect-airtable-to-workfront-fusion" class="MCXref xref">Conectar Airtable ao Workfront Fusion</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td>Base </td> 
   <td> <p>Selecione a base que deseja pesquisar por registros.</p> </td> 
  </tr> 
  <tr> 
   <td>Tabela </td> 
   <td> <p>Selecione a tabela que deseja pesquisar por registros.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Fórmula</p> </td> 
   <td> <p>Uma fórmula usada para filtrar registros. A fórmula é avaliada para cada registro e se o resultado não for <code>0</code>, <code>false</code>, <code>""</code>, <code>NaN</code>, <code>[]</code>ou <code>#Error!</code> o registro é incluído na resposta.</p> <p>Se combinado com o <code>view</code>, somente os registros nessa visualização que satisfazem a fórmula são retornados.</p> <p>Por exemplo, para incluir apenas registros onde Nome não está vazio, passe:<code> NOT({Name} = '')</code></p> <p>Para saber mais, pesquise informações sobre referências de campo de fórmula na documentação de suporte do Airtable.</p> </td> 
  </tr> 
  <tr> 
   <td>Ordenar </td> 
   <td> <p>Selecione a direção de classificação e o campo no qual deseja classificar os resultados.</p> </td> 
  </tr> 
  <tr> 
   <td>Exibir </td> 
   <td> <p>Selecione a exibição que deseja pesquisar por registros.</p> </td> 
  </tr> 
  <tr> 
   <td>Limite</td> 
   <td> <p>Insira ou mapeie o número máximo de registros que você deseja que o módulo retorne durante cada ciclo de execução de cenário.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Atualizar um registro {#update-a-record}

Este módulo de ação atualiza um registro específico.

Você especifica a ID do registro e os novos dados que deseja que ele contenha.

O módulo retorna quaisquer campos padrão associados ao registro, juntamente com quaisquer campos e valores personalizados que a conexão acessa. Você pode mapear essas informações em módulos subsequentes do cenário.

Ao configurar esse módulo, os seguintes campos são exibidos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Conexão </td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do Airtable ao Workfront Fusion, consulte <a href="#connect-airtable-to-workfront-fusion" class="MCXref xref">Conectar Airtable ao Workfront Fusion</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td>Base </td> 
   <td> <p>Selecione a base que contém o registro que deseja atualizar.</p> </td> 
  </tr> 
  <tr> 
   <td>Tabela </td> 
   <td> <p>Selecione a tabela que contém o registro que você deseja atualizar.</p> </td> 
  </tr> 
  <tr> 
   <td>ID de registro </td> 
   <td> <p>Insira ou mapeie a ID do Airtable exclusiva do registro que você deseja que o módulo atualize. Você pode recuperar a ID, por exemplo, usando o módulo Pesquisar registros .</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Registro</p> </td> 
   <td> <p>Insira os valores para o novo registro. Os campos disponíveis dependem da tabela selecionada.</p> <!--<p>In order to delete the content of the field, use the erase function. </p>  <p>Field types (via airtable.com/api):</p> 
    <ul> 
     <li> <p><strong>Text</strong>: string</p> <p>A single line of text.</p> </li> 
     <li> <p><strong>Long text</strong>: string</p> <p>The string can contain multiple lines of text with "mention tokens." For example:</p><pre>&lt;airtable:mention id="menE1i9oBaGX3DseR"&gt;@Alex&lt;/airtable:mention&gt;</pre> </li> 
     <li><strong>Attachment</strong>: Add the attachment. Airtable will download the file from the provided url and keep its own copy of it. If the File name field is left empty, Airtable will generate the name automatically.</li> 
     <li><strong>Checkbox</strong>: Select one of the options.</li> 
     <li><strong>Multiple select</strong>: Select multiple options in the checklist.</li> 
     <li><strong>Single select</strong>: Select one option from the drop-down menu.</li> 
     <li><strong>Collaborator</strong>: Enter the email that uniquely identifies a user in Airtable who this base is shared with.</li> 
     <li><strong>Date</strong>: UTC date, for example, 2019-09-05. (ISO 8601 formatted date)</li> 
     <li><strong>Phone number</strong>: A telephone number, for example, (415) 555-9876.</li> 
     <li><strong>Email</strong>valid email address.</li> 
     <li><strong>URL</strong>: lid URL such as airtable.com or https://airtable.coiverse.</li> 
     <li><strong>Number</strongnter a number.</li> 
     <li><strong>Currency</stro Currency value.</li> 
     <li><strong>Percent</stronA percentage value; must be equal to or more than 0i> 
     <li><strong>Duration</strong>: Enter the duration time. If you need help, see the information about the duration field type in the Airtable support documentation.</li> 
     <li><strong>Rating</strong>: Enter the number. For example, "3 stars" is 3. A rating cannot be 0.</li> 
     <li><strong>Link</strong>: Enter the linked records IDs from the table. The order of record IDs is reversed compared to what you see in the app.</li> 
     <li><strong>Rollup</strong>: Computed value: COUNT(values)</li> 
     <li><strong>Lookup</strong>: Array of long text fields</li> 
     <li><strong>Autonumber</strong>: Automatically incremented unique counter for each record.</li> 
     <li> <p><strong>Barcode</strong>: The barcode object may contain the following two properties, both of which are optional.</p> <p>Barcode data (text)</p> <p>Barcode symbology, for example, "upce" or "code39" (type)</p> </li> 
    </ul> --></td> 
  </tr> 
  <tr> 
   <td>Links inteligentes</td> 
   <td> <p>Insira nomes em vez de IDs de registro em campos que vinculam a outra tabela. O registro é criado automaticamente na tabela vinculada se não houver correspondência.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Atualizar um registro

Esse módulo de ação atualiza ou insere um registro específico.

Você especifica a ID do registro e os novos dados que deseja que ele contenha.

O módulo retorna quaisquer campos padrão associados ao registro, juntamente com quaisquer campos e valores personalizados que a conexão acessa. Você pode mapear essas informações em módulos subsequentes do cenário.

Ao configurar esse módulo, os seguintes campos são exibidos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Conexão </td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do Airtable ao Workfront Fusion, consulte <a href="#connect-airtable-to-workfront-fusion" class="MCXref xref">Conectar Airtable ao Workfront Fusion</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td>Base </td> 
   <td> <p>Selecione a base que contém o registro que deseja atualizar.</p> </td> 
  </tr> 
  <tr> 
   <td>Tabela </td> 
   <td> <p>Selecione a tabela que contém o registro que você deseja atualizar.</p> </td> 
  </tr> 
  <tr> 
   <td>ID de registro </td> 
   <td> <p>Se estiver atualizando um registro, insira ou mapeie a ID do Airtable exclusiva do registro que você deseja que o módulo atualize. Você pode recuperar a ID, por exemplo, usando o módulo Pesquisar registros .</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Registro</p> </td> 
   <td> <p>Insira os valores para o novo registro. Os campos disponíveis dependem da tabela selecionada.</p> <!-- <p>In order to delete the content of the field, use the erase function. </p>  <p>Field types (via airtable.com/api):</p> 
    <ul> 
     <li> <p><strong>Text</strong>: string</p> <p>A single line of text.</p> </li> 
     <li> <p><strong>Long text</strong>: string</p> <p>The string can contain multiple lines of text with "mention tokens." For example:</p><pre>&lt;airtable:mention id="menE1i9oBaGX3DseR"&gt;@Alex&lt;/airtable:mention&gt;</pre> </li> 
     <li><strong>Attachment</strong>: Add the attachment. Airtable will download the file from the provided url and keep its own copy of it. If the File name field is left empty, Airtable will generate the name automatically.</li> 
     <li><strong>Checkbox</strong>: Select one of the options.</li> 
     <li><strong>Multiple select</strong>: Select multiple options in the checklist.</li> 
     <li><strong>Single select</strong>: Select one option from the drop-down menu.</li> 
     <li><strong>Collaborator</strong>: Enter the email that uniquely identifies a user in Airtable who this base is shared with.</li> 
     <li><strong>Date</strong>: UTC date, for example, 2019-09-05. (ISO 8601 formatted date)</li> 
     <li><strong>Phone number</strong>: A telephone number, for example, (415) 555-9876.</li> 
     <li><strong>Email</strong>valid email address.</li> 
     <li><strong>URL</strong>: lid URL such as airtable.com or https://airtable.coiverse.</li> 
     <li><strong>Number</strongnter a number.</li> 
     <li><strong>Currency</stro Currency value.</li> 
     <li><strong>Percent</stronA percentage value; must be equal to or more than 0i> 
     <li><strong>Duration</strong>: Enter the duration time. If you need help, see the information about the duration field type in the Airtable support documentation.</li> 
     <li><strong>Rating</strong>: Enter the number. For example, "3 stars" is 3. A rating cannot be 0.</li> 
     <li><strong>Link</strong>: Enter the linked records IDs from the table. The order of record IDs is reversed compared to what you see in the app.</li> 
     <li><strong>Rollup</strong>: Computed value: COUNT(values)</li> 
     <li><strong>Lookup</strong>: Array of long text fields</li> 
     <li><strong>Autonumber</strong>: Automatically incremented unique counter for each record.</li> 
     <li> <p><strong>Barcode</strong>: The barcode object may contain the following two properties, both of which are optional.</p> <p>Barcode data (text)</p> <p>Barcode symbology, for example, "upce" or "code39" (type)</p> </li> 
    </ul> --></td> 
  </tr> 
  <tr> 
   <td>Links inteligentes</td> 
   <td> <p>Insira nomes em vez de IDs de registro em campos que vinculam a outra tabela. O registro é criado automaticamente na tabela vinculada se não houver correspondência.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Ver registros {#watch-records}

Esse módulo de acionador inicia um cenário quando um registro é criado ou atualizado na tabela especificada.

>[!NOTE]
>
>Para usar esse módulo, o campo Hora da criação ou o campo Hora da última modificação devem ser criados na tabela.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Conexão </td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do Airtable ao Workfront Fusion, consulte <a href="#connect-airtable-to-workfront-fusion" class="MCXref xref">Conectar Airtable ao Workfront Fusion</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td>Base </td> 
   <td> <p>Selecione a base que deseja observar para novos registros.</p> </td> 
  </tr> 
  <tr> 
   <td>Tabela </td> 
   <td> <p>Selecione a tabela que deseja visualizar para novos registros.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Configuração do acionador</p> </td> 
   <td> <p>Campo Acionador</p> <p>A <code>Created Time</code> ou <code>Last Modified Time</code> campo usado para classificar registros. Se você não tiver um <code>Created Time</code> ou <code>Last Modified Time</code> no esquema, é necessário criar um. </p> <p>Campo Label</p> <p>Um campo usado como rótulo para um registro, por exemplo, na caixa de diálogo Escolher onde iniciar .</p> </td> 
  </tr> 
  <tr> 
   <td>Limite</td> 
   <td> <p>Insira ou mapeie o número máximo de registros que você deseja que o módulo assista durante cada ciclo de execução de cenário.</p> </td> 
  </tr> 
  <tr> 
   <td>Exibir</td> 
   <td> <p>Selecione a exibição que deseja usar.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Fórmula</p> </td> 
   <td> <p>Uma fórmula usada para filtrar registros. A fórmula é avaliada para cada registro e se o resultado não for <code>0</code>, <code>false</code>, <code>""</code>, <code>NaN</code>, <code>[]</code>ou <code>#Error!</code> o registro é incluído na resposta.</p> <p>Se combinado com o <code>view</code>, somente os registros nessa visualização que satisfazem a fórmula são retornados.</p> <p>Por exemplo, para incluir apenas registros onde Nome não está vazio, passe:<code> NOT({Name} = '')</code></p> <p>Para saber mais, consulte as informações sobre referências de campo de fórmula na documentação de suporte do Airtable.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Assista às respostas

Esse módulo de acionador inicia um cenário quando um formulário é enviado.

>[!NOTE]
>
>Essa funcionalidade só está disponível para o Airtable Pro Plan pago.

O URL do webhook precisa ser gerado no Workfront Fusion e adicionado à configuração do formulário no Airtable.

1. Adicione o módulo Watch New Responses ao seu cenário do Workfront Fusion.
1. Gere e copie o URL do webhook.

   Para obter instruções, consulte [Acionadores instantâneos (webhooks) no Adobe Workfront Fusion](../../workfront-fusion/webhooks/instant-triggers-webhooks.md).

1. Faça logon em sua conta do Airtable.
1. Abra a Base e a tabela que deseja usar para o formulário e crie uma Exibição de formulário.
1. Defina o formulário conforme necessário, role para baixo no formulário e ative a opção Redirecionar para URL após o envio do formulário.
1. Insira a URL do Webhook gerada na etapa 2 da caixa de diálogo exibida e adicione ?record_id={record_id} logo após a URL do webhook para incluir a ID do registro na saída do módulo, em seguida, clique em Salvar. O URL resultante terá, por exemplo, a seguinte aparência:
1. Retorne ao cenário do Workfront Fusion e execute o módulo Respostas de Monitoramento somente para carregar campos do Airtable e mapear esses campos para os outros módulos.
1. Envie o formulário no Airtable, onde a opção Redirecionar para URL após o formulário ser enviado está ativada e o URL do Webhook é adicionado (etapa 6 acima).

   O módulo Respostas de monitoramento é acionado e os dados desejados são carregados.

1. Adicione o módulo Airtable > Get a Record logo após o módulo Airtable > Watch Responses e mapeie o record_id para o campo Record ID .

Agora, toda vez que o formulário for enviado, o módulo Respostas de Observação em seu cenário do Workfront Fusion será acionado e o módulo Obter um Registro retornará os detalhes do formulário enviados.

#### Efetuar uma chamada de API

#### Chamada da API personalizada

Esse módulo de ação permite que você faça uma chamada autenticada personalizada para o [!DNL Airtable] API. Dessa forma, você pode criar uma automação de fluxo de dados que não pode ser realizada pela outra [!DNL Airtable] módulos.

A ação é baseada no tipo de entidade (tipo de objeto Allocadia) especificado.

Ao configurar esse módulo, os seguintes campos são exibidos.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Conexão</p> </td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do Airtable ao Workfront Fusion, consulte <a href="#connect-airtable-to-workfront-fusion" class="MCXref xref">Conectar Airtable ao Workfront Fusion</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">URL</td> 
   <td>Insira um caminho relativo a <code>https://api.airtable.com/}</code>. Exemplo: <code>v0/{base}/{table}</code> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Método</td> 
   <td> <p>Selecione o método de solicitação HTTP que você precisa configurar a chamada da API. Para obter mais informações, consulte <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">Métodos de solicitação HTTP em [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Cabeçalhos</td> 
   <td> <p>Adicione os cabeçalhos da solicitação no formato de um objeto JSON padrão.</p> <p>Por exemplo, <code>{"Content-type":"application/json"}</code></p> <p>[!DNL Workfront Fusion] adiciona os cabeçalhos de autorização para você.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">String de consulta</td> 
   <td> <p>Adicione a query para a chamada da API no formato de Chave e Valor</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Corpo</td> 
   <td> <p>Adicione o conteúdo do corpo para a chamada da API no formato de um objeto JSON padrão.</p> <p>Nota:  <p>Ao usar declarações condicionais como <code>if</code> no JSON, coloque as aspas fora da declaração condicional.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>
