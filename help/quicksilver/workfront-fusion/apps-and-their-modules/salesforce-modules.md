---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: conector
navigation-topic: apps-and-their-modules
title: Módulos do Salesforce
description: Em um cenário do Adobe Workfront Fusion, é possível automatizar workflows que usam o Salesforce, bem como conectá-los a vários aplicativos e serviços de terceiros.
author: Becky
feature: Workfront Fusion
exl-id: 3c8adcd9-fb5f-400d-9edd-6d9fc30cc728
source-git-commit: c51169c18bef8ac8126a04c08deb88d830517b0b
workflow-type: tm+mt
source-wordcount: '2740'
ht-degree: 0%

---

# [!DNL Salesforce] módulos

Em um cenário do Adobe Workfront Fusion, é possível automatizar workflows que usam [!DNL Salesforce], bem como conectá-lo a vários aplicativos e serviços de terceiros.

Para obter uma introdução ao vídeo sobre o conector do Salesforce, consulte:

* [Salesforce](https://video.tv.adobe.com/v/3427027/){target=_blank}

Se precisar de instruções sobre como criar um cenário, consulte [Criar um cenário no [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

Para obter informações sobre módulos, consulte [Módulos no [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

>[!NOTE]
>
>* Nem todas as edições de [!DNL Salesforce] têm acesso à API. Para obter detalhes, consulte as informações sobre [!DNL Salesforce] edições com acesso à API no [!DNL Salesforce] Site da comunidade.
>* Para obter informações sobre erros específicos retornados do [!DNL Salesforce] , consulte a [!DNL Salesforce] Documentos da API. Você também pode verificar o status da [!DNL Salesforce] para qualquer possível interrupção do serviço.
>

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

## Pré-requisitos

Para usar [!DNL Salesforce] módulos, você deve ter uma [!DNL Salesforce] conta.

## Sobre a pesquisa de [!DNL Salesforce] objetos

Ao pesquisar objetos, você pode inserir palavras de pesquisa individuais ou criar uma consulta mais complexa usando curingas e operadores:

* Use o curinga asterisco (\*) como substituto para zero ou mais caracteres. Por exemplo, uma pesquisa por Ca\* encontra itens que começam com Ca
* Usar um curinga de ponto de interrogação (?) como um substituto para um caractere único. Por exemplo, uma pesquisa por João encontra itens com o termo João ou João, mas não João
* Use o operador de aspas (&quot; &quot;) para encontrar uma correspondência exata de frase. Por exemplo: &quot;reunião de segunda-feira&quot;

Para obter mais informações sobre as possibilidades de pesquisa, consulte [!DNL Salesforce] documentação do desenvolvedor sobre SOQL e SOSL.

## [!DNL Salesforce] módulos e seus campos

* [Triggers](#triggers)
* [Ações](#actions)
* [Pesquisas](#searches)

### Triggers

* [[!UICONTROL Aguardar Registros]](#watch-for-records)
* [[!UICONTROL Observar mensagens de saída]](#watch-outbound-messages)
* [[!UICONTROL Assistir a um campo]](#watch-a-field)

#### [!UICONTROL Aguardar Registros]

Esse módulo de acionamento executa um cenário quando um registro em um objeto é criado ou atualizado. O módulo retorna todos os campos padrão associados ao registro ou aos registros, juntamente com quaisquer campos e valores personalizados que a conexão acesse. Você pode mapear essas informações em módulos subsequentes no cenário.

Ao configurar esse módulo, os campos a seguir são exibidos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexão]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Salesforce] conta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipo] </td> 
   <td> <p>Selecione o tipo de [!DNL Salesforce] registre que você deseja que o módulo assista.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Campos de Registro]</td> 
   <td>Selecione os campos que você deseja que o módulo assista. Os campos disponíveis dependem do tipo de registro.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Contagem máxima de registros]</td> 
   <td> <p>Insira ou mapeie o número máximo de registros que deseja que o módulo retorne durante cada ciclo de execução de cenário.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Observar]</td> 
   <td> <p>Determine se deseja que o cenário observe somente os novos registros do tipo selecionado ou os novos registros do tipo selecionado e todas as outras alterações nos registros desse tipo.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Observar mensagens de saída]

Esse módulo de acionamento executa um cenário quando alguém envia uma mensagem. O módulo retorna todos os campos padrão associados ao registro ou aos registros, juntamente com quaisquer campos e valores personalizados que a conexão acesse. Você pode mapear essas informações em módulos subsequentes no cenário.

Este módulo requer algumas configurações adicionais:

1. Vá para a [!DNL Salesforce] página de configuração.

   Para acessar a página de configuração, localize e clique no botão com o rótulo &quot;[!UICONTROL Configuração]&quot; no canto superior direito da [!DNL Salesforce] conta. No [!DNL Salesforce] página de configuração, localize o &quot;[!UICONTROL Localização Rápida / Pesquisa]&quot; no lado esquerdo. Pesquisar por &quot;[!UICONTROL Regras de fluxo de trabalho].&quot;

1. Clique em **[!UICONTROL Regras de fluxo de trabalho]**.
1. No [!UICONTROL Regras de fluxo de trabalho] que for exibida, clique em **[!UICONTROL Nova regra]** e selecione o tipo de objeto ao qual a regra será aplicada (como &quot;[!UICONTROL Oportunidade]&quot; se estiver monitorando atualizações para registros de Oportunidade).
1. Clique em **[!UICONTROL Próxima]**.
1. Defina um nome de regra, critérios de avaliação e critérios de regra e clique em **[!UICONTROL Salvar]** e **[!UICONTROL Próxima]**.

1. Clique em **[!UICONTROL Concluído]**.
1. Na regra de fluxo de trabalho recém-criada, clique em **[!UICONTROL Editar]**..
1. No **[!UICONTROL Adicionar ação de fluxo de trabalho]** selecione **[!UICONTROL Nova mensagem de saída]**.

1. Especifique o nome, a descrição, o URL do ponto de extremidade e os campos que deseja incluir na nova mensagem de saída e clique em **[!UICONTROL Salvar]**.

   A variável **[!UICONTROL URL do ponto de extremidade]** contém o URL fornecido na variável [!DNL Salesforce] [!UICONTROL Mensagem de saída] in [!DNL Workfront Fusion].

1. Configure um cenário que comece com a variável [!UICONTROL Mensagem de saída] evento.

1. Clique em **&lt;/>** no canto inferior direito e copie o URL fornecido.
1. Retorne para a **[!UICONTROL Regras de fluxo de trabalho]** localize a regra recém-criada e clique em **[!UICONTROL Ativar]**.

Ao configurar esse módulo, os campos a seguir são exibidos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Webhook]</td> 
   <td> <p>Selecione o webhook que deseja usar para assistir mensagens de saída. Para adicionar um webhook, clique em <strong>[!UICONTROL Adicionar]</strong> e digite o nome e a conexão do webhook.</p> <p>Para obter instruções sobre como conectar seu [!DNL Salesforce] conta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o [!UICONTROL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipo de Registro] </td> 
   <td> <p>Selecione o tipo de [!DNL Salesforce] registre que você deseja que o módulo observe as mensagens de saída.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Campos]</td> 
   <td> <p>Selecione os campos que você deseja que o módulo observe para mensagens de saída. Os campos disponíveis dependem do tipo de registro.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### *[!UICONTROL Assistir a um campo]*

Este módulo de acionamento inicia um cenário quando um campo é atualizado no [!DNL Salesforce].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexão]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Salesforce] conta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipo de Registro] </td> 
   <td> <p>Selecione o tipo de registro que contém o campo que o módulo deve observar. Você deve escolher um tipo de registro que tenha o [!UICONTROL Field History] ativado no [!DNL Salesforce] configuração. Para obter mais informações, consulte <a href="https://help.salesforce.com/articleView?id=tracking_field_history.htm&amp;type=5">Rastreamento do histórico do campo</a> no [!DNL Salesforce] documentação. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Campo]</td> 
   <td> <p>Selecione os campos que você deseja que o módulo observe para alterações.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Limite]</td> 
   <td> <p>Insira ou mapeie o número máximo de campos que você deseja que o módulo retorne durante cada ciclo de execução de cenário.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Ações

* [[!UICONTROL Criar um registro]](#create-a-record)
* [[!UICONTROL Ler um Registro]](#read-a-record)
* [[!UICONTROL Excluir um Registro]](#delete-a-record)
* [[!UICONTROL Chamada de API personalizada]](#custom-api-call)
* [[!UICONTROL Fazer upload de anexo/documento]](#upload-attachmentdocument)
* [[!UICONTROL Baixar Anexo/Documento]](#download-attachmentdocument)

#### [!UICONTROL Criar um registro]

Este módulo de ação cria um novo registro em um objeto.

O módulo permite selecionar quais dos campos do objeto estão disponíveis no módulo. Isso reduz o número de campos que você deve percorrer ao configurar o módulo.

O módulo retorna a ID do registro e quaisquer campos associados, juntamente com quaisquer campos e valores personalizados que a conexão acessa. Você pode mapear essas informações em módulos subsequentes no cenário.

Ao configurar esse módulo, os campos a seguir são exibidos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexão]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Salesforce] conta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Tipo de Registro] </p> </td> 
   <td> <p>Selecione o tipo de [!DNL Salesforce] registro que você deseja que o módulo crie. Os campos ficam disponíveis com base no tipo de registro selecionado no campo [!UICONTROL Record Type]. Esses campos são baseados no [!DNL Salesforce] API.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Selecionar campos a serem mapeados]</td> 
   <td> <p>Selecione os campos que você deseja que o módulo configure ao criar o novo registro. Os campos obrigatórios estão no topo da lista. </p> <p>Os campos selecionados são abertos abaixo deste campo. Agora é possível inserir valores nesses campos.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Ler um Registro]

Este módulo de ação lê dados de um único objeto no [!DNL Salesforce].

Especifique a ID do registro.

O módulo retorna a ID do registro e quaisquer campos associados, juntamente com quaisquer campos e valores personalizados que a conexão acessa. Você pode mapear essas informações em módulos subsequentes no cenário.

Ao configurar esse módulo, os campos a seguir são exibidos.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr>
    <td>[!UICONTROL Conexão]</td>
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Salesforce] conta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr>
    <td>[!UICONTROL Tipo de Registro]</td>
    <td>Selecione o tipo de [!DNL Salesforce] registre que deseja que o módulo [action].read.</td>
  </tr> 
  <tr>
    <td>[!UICONTROL Campos de Registro]</td>
    <td>Selecione os campos que você deseja que o módulo leia. Você deve selecionar pelo menos um campo.</td>
  </tr> 
  <tr>
    <td>[!UICONTROL ID]</td>
    <td> <p>Insira ou mapeie o [!DNL Salesforce] ID do registro que você deseja que o módulo leia.</p> <p>Para obter a ID, abra o [!DNL Salesforce] no navegador e copie o texto no final do URL após a última barra (/). Por exemplo: <code>https://eu5.salesforce.com/&lt;object ID&gt;</code></p> </td>
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Excluir um Registro]

Este módulo de ação exclui um registro existente em um objeto.

Especifique a ID do registro.

O módulo retorna a ID do registro e quaisquer campos associados, juntamente com quaisquer campos e valores personalizados que a conexão acessa. Você pode mapear essas informações em módulos subsequentes no cenário.

Ao configurar esse módulo, os campos a seguir são exibidos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexão]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Salesforce] conta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipo de Registro] </td> 
   <td> <p>Selecione o tipo de [!DNL Salesforce] registro que você deseja que o módulo exclua.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID]</td> 
   <td> <p>Insira ou mapeie o [!DNL Salesforce] ID do registro que você deseja que o módulo exclua.</p> <p>Para obter a ID, abra o [!DNL Salesforce] no navegador e copie o texto no final do URL após a última barra (/). Por exemplo: <code>https://eu5.salesforce.com/&lt;object ID&gt;</code></p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Chamada de API personalizada]

Esse módulo de ação permite fazer uma chamada autenticada personalizada para o [!DNL Salesforce] API. Dessa forma, você pode criar uma automação de fluxo de dados que não pode ser realizada pelo outro [!DNL Salesforce] módulos.

O módulo retorna o seguinte:

* **[!UICONTROL Código de status]** (número): isso indica o sucesso ou a falha de sua solicitação HTTP. Esses são códigos padrão que você pode pesquisar na Internet.
* **[!UICONTROL Cabeçalhos]** (objeto): um contexto mais detalhado para o código de resposta/status que não está relacionado ao corpo de saída. Nem todos os cabeçalhos que aparecem em um cabeçalho de resposta são cabeçalhos de resposta, portanto, alguns podem não ser úteis para você.

  Os cabeçalhos de resposta dependem da solicitação HTTP escolhida ao configurar o módulo.

* **[!UICONTROL Corpo]** (objeto): dependendo da solicitação HTTP escolhida ao configurar o módulo, talvez você receba alguns dados de volta. Esses dados, como os dados de uma [!UICONTROL GET] está contido neste objeto.

Ao configurar esse módulo, os campos a seguir são exibidos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Salesforce] conta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL URL]</p> </td> 
   <td> <p>Insira um caminho relativo a<code> &lt;Instance URL&gt;/services/data/v46.0/</code>.</p> <p>Para obter a lista de endpoints disponíveis, consulte o <a href="https://developer.salesforce.com/docs/atlas.en-us.api_rest.meta/api_rest/intro_what_is_rest_api.htm">Guia do desenvolvedor da API REST do Salesforce</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Método]</p> </td> 
   td&gt; <p>Selecione o método de solicitação HTTP necessário para configurar a chamada de API. Para obter mais informações, consulte <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">Métodos de solicitação HTTP em [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cabeçalhos]</td> 
   <td> <p>Adicione os cabeçalhos da solicitação no formato de um objeto JSON padrão. Por exemplo, <code>{"Content-type":"application/json"}</code>. O Workfront Fusion adiciona os cabeçalhos de autorização para você.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cadeia de Consulta]</td> 
   <td> <p>Adicione a consulta da chamada à API na forma de um objeto JSON padrão. Por exemplo: <code>{"name":"something-urgent"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Corpo]</td> 
   <td> <p>Adicione o conteúdo do corpo para a chamada à API na forma de um objeto JSON padrão.</p> <p>Nota:  <p>Ao usar declarações condicionais como <code>if</code> no JSON, coloque as aspas fora da declaração condicional.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**Exemplo:** A chamada de API a seguir retorna a lista de todos os usuários na [!DNL Salesforce] conta:
>
>* **URL**: `query`
>
>* **Método**: [!UICONTROL GET]
>
>* **Sequência de consulta**:
>
>* **Chave**: `q`
>
>* **Valor**: `SELECT Id, Name, CreatedDate, LastModifiedDate FROM User LIMIT 10`
>
>As correspondências da pesquisa podem ser encontradas na Saída do módulo em **[!UICONTROL Pacote] > [!UICONTROL Corpo] > [!UICONTROL registros]**.
>
>No nosso exemplo, 6 usuários foram retornados:
>
>![](assets/matches-of-the-search-350x573.png)


#### [!UICONTROL Fazer upload de anexo/documento]

Esse módulo de ação faz upload de um arquivo e o anexa a um registro especificado por você ou faz upload de um documento.

O módulo retorna a ID do anexo ou documento e quaisquer campos associados, juntamente com quaisquer campos e valores personalizados que a conexão acesse. Você pode mapear essas informações em módulos subsequentes no cenário.

Ao configurar esse módulo, os campos a seguir são exibidos.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexão]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Salesforce] conta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipo de Carregamento]</td> 
   <td>Selecione se você deseja que o módulo carregue um anexo ou um documento.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID]</td> 
   <td>Insira ou mapeie a ID do objeto para o qual você deseja fazer upload de um anexo.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Pasta]</td> 
   <td>Selecione a pasta que contém o arquivo a ser carregado pelo módulo. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Arquivo de Origem]</td> 
   <td>Selecione um arquivo de origem de um módulo anterior ou mapeie o nome e os dados do arquivo de origem.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Baixar Anexo/Documento]

Este módulo de ação baixa um documento ou anexo de um registro.

Especifique a ID do registro e o tipo de download desejado.

O módulo retorna a ID do anexo ou documento e quaisquer campos associados, juntamente com quaisquer campos e valores personalizados que a conexão acesse. Você pode mapear essas informações em módulos subsequentes no cenário.

Ao configurar esse módulo, os campos a seguir são exibidos.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr>
    <td>[!UICONTROL Conexão]</td>
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Salesforce] conta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr>
    <td>[!UICONTROL Tipo de Download]</td>
    <td> <p>Especifique o tipo de arquivo que deseja baixar do Salesforce.</p> 
     <ul> 
      <li>[!UICONTROL Anexo]</li> 
      <li>[!UICONTROL Documento]</li> 
      <li>[!UICONTROL ContentDocument] (Este é um documento que foi carregado para uma biblioteca em [!DNL Saleforce CRM Content] ou [!DNL Salesforce Files].)</li> 
     </ul> </td>
  </tr> 
  <tr>
    <td> <p>[!UICONTROL ID] / </p> <p>[!UICONTROL ID de Anexo] / </p> <p>[!UICONTROL ID do Documento de Conteúdo]</p> </td>
    <td> <p>Insira ou mapeie o [!DNL Salesforce] ID do registro que você deseja baixar o módulo.</p> <p>Para obter a ID, abra o [!DNL Salesforce] no navegador e copie o texto no final do URL após a última barra (/). Por exemplo: <code>https://eu5.salesforce.com/&lt;object ID&gt;</code></p> </td>
  </tr> 
 </tbody> 
</table>


#### [!UICONTROL Atualizar um Registro]

Este módulo de ação edita um registro em um objeto.

O módulo permite selecionar quais dos campos do objeto estão disponíveis no módulo. Isso reduz o número de campos que você deve percorrer ao configurar o módulo.

O módulo retorna a ID do registro e quaisquer campos associados, juntamente com quaisquer campos e valores personalizados que a conexão acessa. Você pode mapear essas informações em módulos subsequentes no cenário.

Ao configurar esse módulo, os campos a seguir são exibidos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexão]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Salesforce] conta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID]</td> 
   <td>Insira ou mapeie a ID do registro que você deseja atualizar.</td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Tipo de Registro] </p> </td> 
   <td> <p>Selecione o tipo de [!DNL Salesforce] registro que você deseja que o módulo atualize. Os campos ficam disponíveis com base no tipo de registro selecionado no campo Tipo de registro. Esses campos são baseados no [!DNL Salesforce] API.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Selecionar campos a serem mapeados]</td> 
   <td> <p>Selecione os campos que você deseja que o módulo configure ao criar o novo registro. Os campos obrigatórios estão no topo da lista. </p> <p>Os campos selecionados são abertos abaixo deste campo. Agora é possível inserir valores nesses campos.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Pesquisas

#### [!UICONTROL Pesquisar com consulta]

Este módulo de pesquisa procura registros em um objeto no [!DNL Salesforce] que correspondam à consulta de pesquisa especificada. Você pode mapear essas informações em módulos subsequentes no cenário.

Ao configurar esse módulo, os campos a seguir são exibidos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexão]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Salesforce] conta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipo de Pesquisa]</td> 
   <td> <p>Selecione o tipo de pesquisa que deseja que o módulo execute:</p> 
    <ul> 
     <li> <p>[!UICONTROL Simples]</p> </li> 
     <li> <p>[!UICONTROL Usando SOSL (Linguagem de pesquisa de objeto do Salesforce)]</p> </li> 
     <li> <p>[!UICONTROL Usando SOQL (Linguagem de consulta de objetos do Salesforce)]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Tipo] </p> </td> 
   <td> <p>Se você selecionou o tipo de pesquisa Simples, escolha o tipo de [!DNL Salesforce] registro que você deseja que o módulo procure.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Consulta] / [!UICONTROL Consulta SOSL] / [!UICONTROL Consulta SOQL]</td> 
   <td> <p>Informe a consulta pela qual deseja pesquisar.</p> <p>Para obter mais informações sobre SOSL, consulte <a href="https://developer.salesforce.com/docs/atlas.en-us.soql_sosl.meta/soql_sosl/sforce_api_calls_sosl.htm">Linguagem de pesquisa de objeto (SOSL) do Salesforce</a> no [!DNL Salesforce] documentação.</p> <p>Para obter mais informações sobre SOQL, consulte <a href="https://developer.salesforce.com/docs/atlas.en-us.soql_sosl.meta/soql_sosl/sforce_api_calls_soql.htm">Linguagem de consulta de objetos do Salesforce (SOQL)</a> no [!DNL Salesforce] documentação.</p> <p>Observação: observe que o valor do parâmetro <code>RETURNING </code>influencia a saída do módulo. Se você usar <code>LIMIT</code>, [!DNL Fusion] O ignorará as configurações no campo [!UICONTROL Contagem máxima de registros]. Se você não definir um limite, o Fusion inserirá o valor [!UICONTROL LIMIT = Contagem máxima de registros].</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Contagem máxima de registros]</td> 
   <td> <p>Insira ou mapeie o número máximo de registros que deseja que o módulo retorne durante cada ciclo de execução de cenário.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Pesquisa]

Este módulo de ação recupera todos os registros que atendem a um determinado critério.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão]</td> 
   <td>Para obter instruções sobre como conectar seu [!DNL Salesforce] conta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o[!DNL  Adobe Workfront Fusion] - Instruções básicas</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo]</td> 
   <td> <p>Selecione o tipo de objeto que deseja pesquisar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Pesquisar critérios]</td> 
   <td>Selecione o campo pelo qual deseja pesquisar, o operador que deseja usar na consulta e o valor que está procurando no campo. Você pode conectar consultas usando AND ou OR.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Saídas]</td> 
   <td>Selecione os campos que deseja incluir na saída do módulo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conjunto de resultados]</td> 
   <td>Selecione se você deseja que o módulo retorne Todos os registros correspondentes ou somente o Primeiro registro correspondente.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Máximo]</td> 
   <td>Insira ou mapeie o número máximo de registros que você deseja que o módulo recupere durante cada ciclo de execução de cenário.</td> 
  </tr> 
 </tbody> 
</table>
