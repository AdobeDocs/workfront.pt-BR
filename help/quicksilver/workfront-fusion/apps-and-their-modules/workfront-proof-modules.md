---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: conector
navigation-topic: apps-and-their-modules
title: Módulos de prova do Workfront
description: Em um [!DNL Adobe Workfront Fusion] , é possível automatizar workflows que usam [!DNL Workfront Proof], bem como conectá-lo a vários aplicativos e serviços de terceiros.
author: Becky
feature: Workfront Fusion, Workfront Proof, Digital Content and Documents
exl-id: f5c6fb08-880d-4432-aef1-57db13b3ecdb
source-git-commit: a79c6b2fb2b651987f973bc0d74e0eeea312c5bc
workflow-type: tm+mt
source-wordcount: '2886'
ht-degree: 0%

---

# [!DNL Workfront Proof] módulos

Em um [!DNL Adobe Workfront Fusion] , é possível automatizar workflows que usam [!DNL Workfront Proof], bem como conectá-lo a vários aplicativos e serviços de terceiros.

Isso é útil se você precisar executar tarefas que atualmente não têm suporte na revisão de texto no [!DNL Workfront] ou [!DNL Workfront Proof], como atualizar provas com base em determinados eventos e procurar os recipients de uma prova.

O [!DNL Workfront Proof] O conector não conta em relação ao número de aplicativos ativos disponíveis para sua organização. Todos os cenários, mesmo que eles usem somente a variável [!DNL Workfront Proof] aplicativo, faça a contagem em relação à contagem total de cenários de sua organização.

Se precisar de instruções para criar um cenário, consulte [Crie um cenário em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

Para obter informações sobre módulos, consulte [Módulos em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] para automação e integração de trabalho] </p>  <p>[!UICONTROL [!DNL Workfront Fusion] para Automação de Trabalho]</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produto</td> 
   <td>Sua organização deve comprar [!DNL Adobe Workfront Fusion] bem como [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo.</td> 
  </tr> 
 </tbody> 
</table>

Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com seu [!DNL Workfront] administrador.

Para obter informações sobre [!DNL Adobe Workfront Fusion] licenças, consulte [[!DNL Adobe Workfront Fusion] licenças](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!DNL Workfront Proof] módulos e seus campos

Ao configurar [!DNL Workfront Proof] módulos, [!DNL Workfront Fusion] exibe os campos listados abaixo. Junto com esses, [!DNL Workfront Proof] podem ser exibidos, dependendo de fatores como seu nível de acesso no aplicativo ou serviço. Um título em negrito em um módulo indica um campo obrigatório.

Se o botão de mapa for exibido acima de um campo ou função, é possível usá-lo para definir variáveis e funções para esse campo. Para obter mais informações, consulte [Mapear informações de um módulo para outro no [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Triggers](#triggers)
* [Ações](#actions)
* [Pesquisas](#searches)

### Triggers

* [Ver provas](#watch-proofs)
* [Fique atento ao resumo do PDF](#watch-for-pdf-summary)
* [[!UICONTROL Assistir à atividade de prova]](#watch-proof-activity)

#### [!UICONTROL Ver provas]

Esse módulo de acionador agendado executa um cenário quando alguém cria ou decide em uma prova.

O módulo retorna uma lista de todos os registros encontrados durante o período especificado, juntamente com seus tipos. Ele também retorna os valores dos campos especificados. Se o módulo encontrou decisões tomadas na prova, ele incluirá os valores anterior e atual, em campos separados. Você pode mapear essas informações em módulos subsequentes do cenário.

Isso acontece em um intervalo agendado regularmente e especificado por você.

Você deve ter permissões suficientes para acessar a prova ou as provas em [!DNL Workfront Proof] para recuperar essas informações.

Ao configurar esse módulo, os seguintes campos são exibidos.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Workfront Proof] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Tipo de registro</td> 
   <td>Selecione o tipo de [!DNL Workfront Proof] registre que você deseja que o módulo assista.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Saídas</td> 
   <td> <p>Selecione as informações que deseja incluir no pacote de saída deste módulo.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Limite</td> 
   <td> <p>Insira ou mapeie o número máximo de registros que você deseja que o módulo retorne durante cada ciclo de execução de cenário.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Fique atento ao resumo do PDF]

Esse módulo de acionador instantâneo executa um cenário quando alguém cria um PDF summary para uma prova.

Um webhook é necessário neste módulo.

O módulo retorna todos os campos padrão associados à prova, juntamente com quaisquer campos e valores personalizados que a conexão acessa. Ele também cria uma nova assinatura de evento para resumos de PDF e gera o conteúdo do atributo &quot;pdf_url&quot; enviado no payload. Você pode mapear essas informações em módulos subsequentes do cenário.

Ao configurar esse módulo, os seguintes campos são exibidos.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Workfront Proof] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Webhook]</td> 
   <td>Você pode selecionar um webhook existente ou criar um novo. Para obter mais informações, consulte <a href="../../workfront-fusion/webhooks/instant-triggers-webhooks.md" class="MCXref xref">Acionadores instantâneos (webhooks) em [!DNL Adobe Workfront Fusion]</a>. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Limite]</td> 
   <td>Insira ou mapeie o número máximo de registros que você deseja que o módulo retorne durante cada ciclo de execução de cenário.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Assistir à atividade de prova]

Esse módulo de acionador executa um cenário quando uma atividade especificada ocorre em uma prova de prova.

O módulo retorna todos os campos padrão associados à prova, juntamente com quaisquer campos e valores personalizados que a conexão acessa. Ele também cria uma nova assinatura de evento para resumos de PDF e gera o conteúdo do `pdf_url` atributo enviado na carga. Você pode mapear essas informações em módulos subsequentes do cenário.

Ao configurar esse módulo, os seguintes campos são exibidos.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Workfront Proof] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipo de atividade]</td> 
   <td>Selecione se deseja assistir a qualquer nova decisão (incluindo alterações de status da [!UICONTROL proof]) ou somente alterações de status da prova geral.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Limite]</td> 
   <td>Insira ou mapeie o número máximo de registros que você deseja que o módulo retorne durante cada ciclo de execução de cenário.</td> 
  </tr> 
 </tbody> 
</table>

### Ações

* [[!UICONTROL Criar prova]](#create-proof)
* [[!UICONTROL Chamada da API personalizada]](#custom-api-call)
* [[!UICONTROL Baixar prova]](#download-proof)
* [[!UICONTROL Ler um registro]](#read-a-record)
* [[!UICONTROL Resumo do PDF de solicitações]](#request-pdf-summary)
* [[!UICONTROL Atualizar prova]](#update-proof)
* [[!UICONTROL Carregar arquivo]](#upload-file)

#### [!UICONTROL Criar prova]

Esse módulo de ação cria uma nova prova ou uma nova versão de uma prova em [!DNL Workfront Proof].

Especifique os parâmetros para a nova prova e a prova de origem se estiver criando uma nova versão.

O módulo retorna a ID da nova prova ou versão de prova.Você pode mapear essas informações em módulos subsequentes no cenário.

Ao configurar esse módulo, os seguintes campos são exibidos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Workfront Proof] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipo de prova]</td> 
   <td> <p>Especifique se deseja que a prova criada tenha um fluxo de trabalho básico ou um [!UICONTROL Automated Workflow].</p> <p>Em seguida, preencha os campos que são exibidos para o tipo de prova escolhido. Por exemplo, se você escolher [!UICONTROL Fluxo de trabalho automatizado], preencha o <strong>[!UICONTROL Etapas do fluxo de trabalho]</strong> para configurar os estágios.</p></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Permitir download do arquivo original]</td> 
   <td>Selecione se deseja permitir que o arquivo original do qual a prova foi criada seja baixado.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Visualizador de prova clássico]</td> 
   <td>Selecione se você está usando o Visualizador de prova clássico.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Combinar todos os arquivos em uma única prova]</td> 
   <td>Ative essa opção para combinar todos os arquivos em uma única prova de várias páginas.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Criar uma nova versão de prova]</td> 
   <td>Selecione essa opção se desejar que o módulo crie uma nova versão de uma prova existente. Em seguida, no <strong>[!UICONTROL ID da prova existente]</strong> campo que exibe, mapeia ou insere a ID exclusiva da prova.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Rótulo do link personalizado]</td> 
   <td>Insira ou mapeie um rótulo para o link de prova personalizado.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL URL do link personalizado]</td> 
   <td>Insira ou mapeie o URL do link personalizado.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Notificações por email padrão para assinantes]</td> 
   <td>Digite um dos seguintes números para indicar quais das seguintes configurações padrão de notificação de email você deseja usar para a prova criada.
    <ul>
     <li><strong>1</strong> - Todos os novos comentários e respostas</li>
     <li><strong>2</strong> - Respostas aos meus comentários</li>
     <li><strong>3</strong> - Resumo diário</li>
     <li><strong>4</strong> - Resumo por hora</li>
     <li><strong>5</strong> - Apenas decisões</li>
     <li><strong>9</strong> - Desativado</li>
    </ul></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Desativar resumo do Excel]</td> 
   <td>Selecione se você deseja desativar a capacidade de baixar comentários de prova em um arquivo Excel.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Desativar resumo do PDF]</td> 
   <td>Selecione se você deseja desativar a capacidade de baixar comentários de prova em um arquivo de PDF.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Desativar email de assinatura]</td> 
   <td>Selecione se deseja desabilitar o email de assinatura para essa prova.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Ativar reprodutor incorporado]</td> 
   <td>Selecione se deseja ativar o reprodutor incorporado para esta prova.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Ativar assinaturas]</td> 
   <td>Selecione se as pessoas que não são participantes têm permissão para assinar a prova.<br>Se você selecionar essa opção, também poderá selecionar a Função padrão para assinantes, conforme descrito nesta tabela.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Ativar validação de assinaturas]</td> 
   <td>Selecione se deseja ativar a validação de email de assinatura. Se isso estiver ativado, o assinante deve clicar em um link em um email para acessar uma prova.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Ativar URL da equipe]</td> 
   <td>Selecione se deseja que a prova criada oculte ou mostre o URL da equipe.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL File Hash] <span style="font-weight: normal;">ou</span> [!UICONTROL Hash do arquivo]</td> 
   <td>Adicione a ID do arquivo ou arquivos do qual deseja criar uma prova ou provas.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Nomes de arquivo]</td> 
   <td>Adicione o nome do arquivo ou os nomes da prova criada. Este é um campo obrigatório.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Bloquear prova quando todas as decisões necessárias são tomadas]</td> 
   <td>Especifique se deseja que a prova criada seja bloqueada depois que todas as decisões necessárias forem tomadas.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Notificar destinatários sobre essa prova]</td> 
   <td>Selecione uma opção para indicar se deseja que os recipients sejam notificados quando a prova for criada.&gt;</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Nome da prova]</td> 
   <td>Digite um nome para a prova criada. Este é um campo obrigatório. Use um símbolo de barra vertical (|) para separar nomes para várias provas.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID do proprietário da prova]</td> 
   <td>Insira ou mapeie a ID do proprietário da prova. Se esse campo ficar em branco, o proprietário da prova será definido como o usuário atual.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID de referência]</td> 
   <td>Insira a ID de referência da prova.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Exigir assinatura eletrônica]</td> 
   <td>Selecione se deseja exigir que alguém que tome uma decisão em uma prova envie uma assinatura eletrônica.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Exigir logon]</td> 
   <td> <p>Especifique se deseja que a prova criada exija um logon. </p> <p>Isso é igual à configuração [!UICONTROL Login obrigatório] explicada em <a href="../../workfront-proof/wp-work-proofsfiles/manage-your-work/configure-proof-settings.md" class="MCXref xref">[!UICONTROL Definir configurações de prova] em [!DNL Workfront Proof]</a></p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Resolution ID]</td> 
   <td>Insira a ID da resolução que deseja usar para a prova. Para obter uma lista de IDs de resolução, consulte o [!DNL Workfront Proof] <a href="http://api.proofhq.com/home/objects/soapworkflowproofobject">Documentação da API</a>.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL SWF]</td> 
   <td>Insira o tipo de prova de SWF.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Mostrar] [item]</td> 
   <td>Para cada item, selecione se deseja exibi-lo na prova.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL ID da Workspace]</td> 
   <td>Insira a ID do espaço de trabalho no qual deseja criar a prova. </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Recipients]</td> 
   <td>Adicione os endereços de email dos recipients que deseja para a prova criada .</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Prazo]</td> 
   <td> <p>Especifique o prazo desejado para a prova criada. Use o seguinte formato de data:</p> <p><code>YYYY-MM-DD hh:mm</code></p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Chamada da API personalizada]

Esse módulo de ação permite que você faça uma chamada autenticada personalizada para o [!DNL Workfront Proof] API. Dessa forma, você pode criar uma automação de fluxo de dados que não pode ser realizada pela outra [!DNL Workfront Proof] módulos.

O módulo retorna o código de status, os cabeçalhos e o corpo. Você pode mapear essas informações em módulos subsequentes do cenário.

Ao configurar esse módulo, os seguintes campos são exibidos.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Workfront Proof] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Método]</td> 
   <td>Defina a ação para a chamada da API. Para ver as ações disponíveis, consulte a <a href="http://api.proofhq.com/">Documentação da API de prova</a>.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Corpo (XML)]</td> 
   <td> <p>Adicione o conteúdo do corpo para a chamada da API no formato de um objeto JSON padrão.</p> <p>Nota:  <p>Ao usar declarações condicionais como <code>if</code> no JSON, coloque as aspas fora da declaração condicional.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**Exemplo:**
>
>![](assets/wfp-api-module-example-350x586.png)

#### [!UICONTROL Baixar prova]

Esse módulo de ação baixa o arquivo de origem de uma prova específica que você identifica usando sua ID.

Especifique a ID da prova.

O módulo retorna o conteúdo do arquivo de origem usado para criar a prova.Você pode mapear essas informações em módulos subsequentes no cenário.

Você deve ter permissões suficientes para acessar o registro em [!DNL Workfront Proof] para recuperar essas informações.

Ao configurar esse módulo, os seguintes campos são exibidos.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Workfront Proof] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Proof ID]</td> 
   <td> <p>Digite a ID exclusiva da prova, encontrada na página [!UICONTROL Proof Details]. Para obter mais informações, consulte <a href="../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md" class="MCXref xref" data-mc-variable-override="">Gerenciar detalhes de prova em [!DNL Workfront Proof]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Ler um registro]

Este módulo de ação lê dados de uma única prova em [!DNL Workfront Proof].

Você especifica a ID da prova e as informações que deseja da prova.

O módulo retorna os valores dos campos escolhidos para a prova, juntamente com seus tipos. Você pode mapear essas informações em módulos subsequentes do cenário.

Você deve ter permissões suficientes para acessar o registro em [!DNL Workfront Proof] para recuperar essas informações.

Ao configurar esse módulo, os seguintes campos são exibidos.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Workfront Proof] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipo de registro]</td> 
   <td>Selecione se deseja ler uma prova, comentários de prova ou revisores de prova.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Saídas]</td> 
   <td> <p>Selecione as informações que deseja incluir no pacote de saída deste módulo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID]</td> 
   <td>Insira ou mapeie a [!DNL Workfront Proof] ID do registro que você deseja que o módulo leia.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Resumo do PDF de solicitações]

Este módulo de ação solicita o resumo do PDF para uma prova específica em [!DNL Workfront Proof].

Especifique a ID da prova.

O módulo retorna informações PDF summary. Você pode mapear essas informações em módulos subsequentes do cenário.

Você deve ter permissões suficientes para acessar o registro em [!DNL Workfront Proof] para recuperar essas informações.

Ao configurar esse módulo, os seguintes campos são exibidos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Workfront Proof] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Proof ID]</td> 
   <td> <p>Insira o [!DNL Workfront Proof] ID da prova para a qual você deseja solicitar um resumo do PDF.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL URL de retorno]</td> 
   <td>Insira ou mapeie o URL para onde deseja que o resumo do PDF seja enviado.</td> 
  </tr> 
 </tbody> 
</table>

##### Possível erro

* **Erro**: &quot;[!UICONTROL Você não tem privilégio para executar essa solicitação. O estágio deve conter pelo menos um recipient.]&quot;
* **Solução**: Certifique-se de não ser o único atribuído aos estágios do fluxo de trabalho. Deve haver outro usuário atribuído aos estágios do fluxo de trabalho.

#### [!UICONTROL Atualizar prova]

Este módulo de ação atualiza uma prova existente em [!DNL Workfront Proof].

Você especifica a ID da prova e o tipo de registro e quais campos deseja incluir na saída.

O módulo retorna quaisquer campos padrão associados ao registro, juntamente com quaisquer campos e valores personalizados que a conexão acessa. Você pode mapear essas informações em módulos subsequentes do cenário.

Você deve ter permissões suficientes para acessar o registro em [!DNL Workfront Proof] para recuperar essas informações.

Ao configurar esse módulo, os seguintes campos são exibidos.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Workfront Proof] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Proof ID]</td> 
   <td> <p>Digite a ID exclusiva da prova, encontrada na página [!UICONTROL Proof Details]. Para obter mais informações, consulte <a href="../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md" class="MCXref xref" data-mc-variable-override="">Gerenciar detalhes de prova em [!DNL Workfront Proof]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Prazo]</td> 
   <td> <p>Especifique o prazo desejado para a prova criada. Use o seguinte formato de data:</p> <p><code>YYYY-MM-DD hh:mm</code></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Notificações por email padrão para assinantes]</td> 
   <td>Selecione qual das seguintes configurações padrão de notificação de email deseja usar para a prova criada.
    <ul>
     <li> [!UICONTROL Todos os novos comentários e respostas]</li>
     <li>[!UICONTROL Respostas aos meus comentários]</li>
     <li>[!UICONTROL Resumo diário]</li>
     <li> [!UICONTROL Resumo por hora]</li>
     <li> [!UICONTROL Decisões somente]</li>
     <li> [!UICONTROL Desativado]</li>
    </ul></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Função padrão]</td> 
   <td>Selecione a função padrão para a prova.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Desativar email de assinatura]</td> 
   <td>Selecione se deseja desabilitar o email de assinatura para essa prova.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ativar assinaturas]</td> 
   <td>Selecione se as pessoas que não são participantes têm permissão para assinar a prova.<br>Se você selecionar essa opção, também poderá selecionar a [!UICONTROL Função padrão] para assinantes, conforme descrito nesta tabela.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ativar validação de assinaturas]</td> 
   <td>Selecione se deseja ativar a validação de email de assinatura. Se isso estiver ativado, o assinante deve clicar em um link em um email para acessar uma prova.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ativar URL da equipe]</td> 
   <td>Selecione se deseja que a prova criada oculte ou mostre o URL da equipe.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Bloquear prova quando todas as decisões necessárias são tomadas]</td> 
   <td>Especifique se deseja que a prova criada seja bloqueada depois que todas as decisões necessárias forem tomadas.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Mensagem]</td> 
   <td>Insira ou mapeie uma mensagem que você deseja acompanhar a prova.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Proof ID] </td> 
   <td>Insira ou mapeie a ID da prova que deseja atualizar.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Nome da prova]</td> 
   <td>Insira ou mapeie o nome da prova que deseja atualizar.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Exigir logon]</td> 
   <td> <p>Especifique se deseja que a prova criada exija um logon. </p> <p>Isso é igual à configuração [!UICONTROL Login obrigatório] explicada em <a href="../../workfront-proof/wp-work-proofsfiles/manage-your-work/configure-proof-settings.md" class="MCXref xref">[!UICONTROL Definir configurações de prova] em [!DNL Workfront Proof]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Mostrar versões como]</td> 
   <td>Selecione se deseja mostrar um link para outras versões dessa prova.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Assunto]</td> 
   <td>Inserir ou mapear o assunto da prova</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Carregar arquivo]

Este módulo de ação carrega um arquivo para uso com o [!UICONTROL Criar prova] módulo em [!DNL Workfront Proof].

O módulo retorna uma ID de hash para o arquivo carregado. Você pode mapear essas informações em módulos subsequentes do cenário.

Ao configurar esse módulo, os seguintes campos são exibidos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Workfront Proof] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Arquivo de origem]</td> 
   <td> <p>Selecione um arquivo de origem de um módulo anterior ou mapeie o nome e os dados do arquivo de origem.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Pesquisas

* [[!UICONTROL Pesquisar]](#search)
* [[!UICONTROL Listar modelos de fluxo de trabalho]](#list-workflow-templates)

#### [!UICONTROL Pesquisar]

Este módulo de pesquisa procura registros em um objeto em [!DNL Workfront Proof] que correspondem à consulta de pesquisa especificada.

O módulo retorna a ID da prova se estiver procurando uma prova. Ou retorna as IDs de usuário dos recipients, emails, nomes, posições e aliases de email, se estiver pesquisando por recipients. Você pode mapear essas informações em módulos subsequentes no cenário.

Você deve ter permissões suficientes para acessar o registro em [!DNL Workfront Proof] para recuperar essas informações.

Ao configurar esse módulo, os seguintes campos são exibidos.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Workfront Proof] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Procurar</td> 
   <td> <p>Consulte[!UICONTROL ] para selecionar o tipo de registro que deseja que o módulo procure.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Prova]</strong> </p> <p>Insira o Nome da Prova da prova que deseja pesquisar.</p> </li> 
     <li> <p><strong>[!UICONTROL Recipient]</strong> </p> <p>Insira o endereço de email do recipient que deseja pesquisar.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Conjunto de resultados]</td> 
   <td>Indique se o módulo pesquisará <strong>[!UICONTROL Todos os registros correspondentes]</strong> ou somente o <strong>[!UICONTROL Primeiro registro de correspondência]</strong>.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Classificar por]</td> 
   <td>Selecione o campo no qual deseja classificar os resultados.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Direção da classificação]</td> 
   <td> <p>Selecione se deseja classificar os resultados em ordem crescente ou decrescente.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Listar modelos de fluxo de trabalho]

Este módulo de pesquisa lista todos os modelos de fluxo de trabalho disponíveis.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Workfront Proof] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Saídas]</td> 
   <td> <p>Selecione as informações que deseja incluir no pacote de saída deste módulo.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Limite]</td> 
   <td> <p>Insira ou mapeie o número máximo de templates que você deseja que o módulo retorne durante cada ciclo de execução de cenário.</p> </td> 
  </tr> 
 </tbody> 
</table>
