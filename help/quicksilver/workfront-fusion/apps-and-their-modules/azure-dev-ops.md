---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: conector
navigation-topic: apps-and-their-modules
title: Módulos do Azure DevOps
description: Em um [!DNL Adobe Workfront Fusion] , é possível automatizar workflows que usam [!DNL Azure DevOps], bem como conectá-lo a vários aplicativos e serviços de terceiros.
author: Becky
feature: Workfront Fusion
exl-id: ecaa93c9-47bb-4fe1-87b4-d2e117cc68ae
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1749'
ht-degree: 0%

---

# [!DNL Azure DevOps] módulos

Em um [!DNL Adobe Workfront Fusion] , é possível automatizar workflows que usam [!DNL Azure DevOps], bem como conectá-lo a vários aplicativos e serviços de terceiros.

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

Para usar [!DNL Azure DevOps] , você deve ter um [!DNL Azure] Conta DevOps.

## Connect [!DNL Azure DevOps] para [!DNL Workfront Fusion] {#connect-azure-devops-to-workfront-fusion}

1. Adicione um [!DNL Azure DevOps] para o seu cenário.
1. Clique em **[!UICONTROL Adicionar]** ao lado do [!UICONTROL Conexão] campo.
1. No [!UICONTROL Tipo de conexão] , selecione **[!DNL Azure DevOps]**.

   >[!IMPORTANT]
   >
   >O [!UICONTROL [!DNL Azure DevOps] (Solicitar todos os escopos)] o tipo de conexão será descontinuado em breve. Portanto, não recomendamos usá-la.

1. Preencha os seguintes campos:

   <table style="table-layout:auto">
        <tr>
            <td>[!UICONTROL Nome da conexão]</td>
            <td>Insira um nome para a conexão que você está criando.</td>
        </tr>
      <tr>
            <td>[!UICONTROL Organization]</td>
            <td>Informe o nome da organização sob a qual você criou seu [!DNL Azure DevOps] aplicativo.</td>
        </tr>
    </table>

1. Clique em **[!UICONTROL Continuar]** para concluir a configuração da conexão e continuar criando seu cenário.

## [!UICONTROL Azure DevOps] módulos e seus campos

Ao configurar [!DNL Azure DevOps] módulos, [!DNL Workfront Fusion] exibe os campos listados abaixo. Junto com esses, [!DNL Azure DevOps] podem ser exibidos, dependendo de fatores como seu nível de acesso no aplicativo ou serviço. Um título em negrito em um módulo indica um campo obrigatório.

Se o botão de mapa for exibido acima de um campo ou função, é possível usá-lo para definir variáveis e funções para esse campo. Para obter mais informações, consulte [Mapear informações de um módulo para outro no [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Triggers](#triggers)
* [Ações](#actions)
* [Pesquisas](#searches)

### Triggers

#### [!UICONTROL Observação para itens de trabalho]

Esse módulo de acionador instantâneo executa um cenário quando um registro é adicionado, atualizado ou excluído em [!UICONTROL Azure DevOps].

O módulo retorna quaisquer campos padrão associados ao registro, juntamente com quaisquer campos e valores personalizados que a conexão acessa. Você pode mapear essas informações em módulos subsequentes do cenário.

Ao configurar esse módulo, os seguintes campos são exibidos.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td> <p>Selecione ou adicione um webhook para o módulo.</p> <p>Para obter mais informações sobre webhooks nos módulos do acionador, consulte <a href="../../workfront-fusion/webhooks/instant-triggers-webhooks.md" class="MCXref xref">Acionadores instantâneos (webhooks) em [!DNL Adobe Workfront Fusion]</a>.</p> <p>Para obter informações sobre como criar um webhook, consulte <a href="../../workfront-fusion/apps-and-their-modules/webhooks-updated.md" class="MCXref xref">Webhooks</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Ações

* [Chamada da API personalizada](#custom-api-call)
* [Ler registro](#read-record)
* [Criar um registro](#create-a-record)
* [Atualizar um item de trabalho](#update-a-work-item)
* [[!UICONTROL Fazer upload de um anexo]](#upload-an-attachment)
* [Baixar um anexo](#download-an-attachment)
* [Vincular itens de trabalho]([!UICONTROL #link-work-items])

#### [!UICONTROL Chamada da API personalizada]

Esse módulo de ação permite que você faça uma chamada autenticada personalizada para o [!DNL Azure DevOps] API. Dessa forma, você pode criar uma automação de fluxo de dados que não pode ser realizada pela outra [!DNL Azure DevOps] módulos.

Ao configurar esse módulo, os seguintes campos são exibidos.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Azure DevOps] para [!DNL Workfront Fusion], consulte <a href="#connect-azure-devops-to-workfront-fusion" class="MCXref xref">Connect [!DNL Azure DevOps] para [!UICONTROL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL base]</td> 
   <td> <p>Selecione ou mapeie o URL básico usado para se conectar ao seu [!DNL Azure DevOps] account</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL relativo]</td> 
   <td> <p>Insira o URL relativo ao qual você deseja se conectar para esta chamada de API.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exemplo: </b></span></span><code>{organization}/_apis[/{area}]/{resource}</code> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Versão da API]</td> 
   <td>Selecione ou mapeie a versão do [!DNL Azure DevOps] API à qual você deseja se conectar para esta chamada de API. Se nenhuma versão estiver selecionada, [!DNL Workfront Fusion] conecta-se a [!DNL Azure DevOps] API versão 5.1.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Método]</td> 
   <td> <p>Selecione o método de solicitação HTTP que você precisa configurar a chamada da API. Para obter mais informações, consulte <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">Métodos de solicitação HTTP em [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cabeçalhos]</td> 
   <td> <p>Adicione os cabeçalhos da solicitação no formato de um objeto JSON padrão.</p> <p>Por exemplo, <code>{"Content-type":"application/json"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sequência de consulta]</td> 
   <td> <p>Adicione a query para a chamada de API no formato de um objeto JSON padrão.</p> <p>Por exemplo: <code>{"name":"something-urgent"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Corpo]</td> 
   <td> <p>Adicione o conteúdo do corpo para a chamada da API no formato de um objeto JSON padrão.</p> <p>Nota:  <p>Ao usar declarações condicionais como <code>if</code> no JSON, coloque as aspas fora da declaração condicional.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Ler registro]

Este módulo de ação lê dados de um único registro em [!DNL Azure DevOps].

Especifique a ID do registro.

O módulo retorna a ID do registro e quaisquer campos associados, juntamente com quaisquer campos e valores personalizados que a conexão acessa. Você pode mapear essas informações em módulos subsequentes do cenário.

Ao configurar esse módulo, os seguintes campos são exibidos.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Azure DevOps] para [!DNL Workfront Fusion], consulte <a href="#connect-azure-devops-to-workfront-fusion" class="MCXref xref">Connect [!DNL Azure DevOps] para [!UICONTROL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de registro]</td> 
   <td> <p>Selecione se deseja ler um projeto ou um item de trabalho</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Project]</strong>: Selecione o projeto que deseja ler.</p> </li> 
     <li> <p><strong>[!UICONTROL Item de trabalho]</strong>: Selecione o projeto que contém o item de trabalho que deseja ler e selecione o tipo de item de trabalho.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Saídas]</td> 
   <td>Selecione as informações que deseja incluir no pacote de saída deste módulo. Os campos disponíveis dependem do tipo de item de trabalho.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>Insira ou mapeie a ID do registro que deseja ler.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Criar um registro]

Esse módulo de ação cria um novo projeto ou item de trabalho.

O módulo gera a ID do objeto para o item de trabalho recém-criado ou o URL e o código de status de um projeto recém-criado.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Azure DevOps] para [!DNL Workfront Fusion], consulte <a href="#connect-azure-devops-to-workfront-fusion" class="MCXref xref">Connect [!DNL Azure DevOps] para [!UICONTROL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de registro]</td> 
   <td> <p>Selecione se deseja criar um item de trabalho ou um projeto.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Project]</strong> </p> <p>Preencha os seguintes campos:</p> 
      <ul> 
       <li> <p><strong>[!UICONTROL Name]</strong>: digite ou mapeie um nome para o novo projeto.</p> </li> 
       <li> <p><strong>[!UICONTROL Descrição]</strong>: insira ou mapeie uma descrição para o novo projeto. </p> </li> 
       <li> <p><strong>[!UICONTROL Visibility]</strong>: Selecione se deseja que o projeto seja público ou privado. Os usuários devem estar conectados à sua organização e devem ter recebido acesso ao projeto para interagir com um projeto privado. Os projetos públicos estão visíveis para usuários que não estão conectados à sua organização.</p> </li> 
       <li> <p><strong>[!UICONTROL Controle de versão]</strong>: Selecione se deseja que o projeto use [!DNL Git] ou [!UICONTROL Team Foundation Version Control (TFCV)] para controle de versão.</p> </li> 
       <li> <p><strong>[!UICONTROL Processo do item de trabalho]</strong>: Selecione o processo de trabalho que deseja usar para o projeto. As opções são [!UICONTROL Básico], [!UICONTROL Scrum], [!UICONTROL Capability Maturity Model Integration (CMMI)] e [!UICONTROL Agile].</p> <p>Para obter mais informações sobre [!DNL Azure DevOps] processos, consulte <a href="https://docs.microsoft.com/en-us/azure/devops/boards/work-items/guidance/choose-process?view=azure-devops&amp;tabs=basic-process">Escolher um Processo</a> no [!DNL Azure DevOps] Documentação.</p> </li> 
      </ul> </li> 
     <li> <p><strong>[!UICONTROL Item de trabalho]</strong> </p> <p>Preencha os seguintes campos:</p> 
      <ul> 
       <li> <p><strong>[!UICONTROL Project]</strong>: Selecione o projeto no qual deseja criar o item de trabalho.</p> </li> 
       <li> <p><strong>[!UICONTROL Tipo de item de trabalho]</strong>: Selecione o tipo de item de trabalho que deseja criar.</p> </li> 
       <li> <p><strong>[!UICONTROL Outros campos]</strong>: nesses campos, insira o valor que você deseja que o item de trabalho tenha para uma determinada propriedade. Os campos disponíveis dependem do tipo de item de trabalho.</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Atualizar um item de trabalho]

Esse módulo de ação atualiza um item de trabalho existente usando sua ID.

O módulo retorna a ID do item de trabalho atualizado.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Azure DevOps] para [!DNL Workfront Fusion], consulte <a href="#connect-azure-devops-to-workfront-fusion" class="MCXref xref">Connect [!DNL Azure DevOps] para [!UICONTROL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Project]</td> 
   <td>Selecione o projeto que contém o item de trabalho que deseja atualizar.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de item de trabalho]</td> 
   <td> <p>Selecione o tipo de item de trabalho que deseja atualizar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Outros campos]</td> 
   <td>Em cada um desses campos, insira o valor que você deseja que o item de trabalho tenha para uma determinada propriedade. Os campos disponíveis dependem do tipo de item de trabalho.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID do item de trabalho]</td> 
   <td>Insira ou mapeie a ID do item de trabalho que deseja atualizar.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Fazer upload de um anexo]

Este módulo de ação carrega um arquivo e o anexa a um item de trabalho.

O módulo retorna a ID do anexo e um URL de download para o anexo.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Azure DevOps] para [!DNL Workfront Fusion], consulte <a href="#connect-azure-devops-to-workfront-fusion" class="MCXref xref">Connect [!DNL Azure DevOps] para [!UICONTROL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Project] </td> 
   <td> <p>Selecione o projeto para onde deseja fazer upload de um anexo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID do item de trabalho]</td> 
   <td> <p>Insira ou mapeie a ID do item de trabalho onde deseja fazer upload de um anexo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Comentário]</td> 
   <td>Insira o texto de um comentário que deseja adicionar ao anexo carregado.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Arquivo de origem] </td> 
   <td>Selecione um arquivo de origem de um módulo anterior ou insira ou mapeie o nome e o conteúdo do arquivo de origem.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Baixar um anexo]

Este módulo de ação baixa um anexo.

O módulo retorna o conteúdo do arquivo do anexo.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Azure DevOps] para [!DNL Workfront Fusion], consulte <a href="#connect-azure-devops-to-workfront-fusion" class="MCXref xref">Connect [!DNL Azure DevOps] para [!UICONTROL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Anexar URL]</td> 
   <td> <p>Insira ou mapeie o URL do anexo que deseja baixar.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Vincular itens de trabalho]

Esse módulo de ação vincula dois itens de trabalho e define a relação entre eles.

O módulo retorna a ID do item de trabalho principal e de quaisquer campos associados, juntamente com quaisquer campos e valores personalizados que a conexão acessa. Você pode mapear essas informações em módulos subsequentes do cenário.

Ao configurar esse módulo, os seguintes campos são exibidos.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Azure DevOps] para [!DNL Workfront Fusion], consulte <a href="#connect-azure-devops-to-workfront-fusion" class="MCXref xref">Connect [!DNL Azure DevOps] para [!UICONTROL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID do item de trabalho]</td> 
   <td>Insira ou mapeie a ID do item de trabalho principal ao qual você deseja vincular outro item de trabalho.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de item de trabalho vinculado]</td> 
   <td>Insira ou mapeie a ID do item de trabalho que você deseja vincular ao item de trabalho principal.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de link]</td> 
   <td> <p>Defina a relação entre os itens de trabalho que deseja vincular.</p> <p>Para obter mais informações, consulte <a href="https://docs.microsoft.com/en-us/azure/devops/boards/queries/link-type-reference?view=azure-devops">Referência do tipo de link</a> na documentação do [!UICONTROL Azure DevOps].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Comentário]</td> 
   <td>Insira ou mapeie o texto de um comentário. Isso é útil para explicar o raciocínio ou a intenção do link.</td> 
  </tr> 
 </tbody> 
</table>

### Pesquisas

#### [!UICONTROL Listar itens de trabalho]

Esse módulo de ação recupera todos os itens de trabalho de um tipo específico em um [!DNL Azure DevOps] projeto.

O módulo retorna a ID do item de trabalho principal e de quaisquer campos associados, juntamente com quaisquer campos e valores personalizados que a conexão acessa. Você pode mapear essas informações em módulos subsequentes do cenário.

Ao configurar esse módulo, os seguintes campos são exibidos.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Azure DevOps] para [!DNL Workfront Fusion], consulte <a href="#connect-azure-devops-to-workfront-fusion" class="MCXref xref">Connect [!DNL Azure DevOps] para [!UICONTROL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Project]</td> 
   <td>Selecione o projeto do qual você deseja recuperar itens de trabalho.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de item de trabalho]</td> 
   <td> <p>Selecione o tipo de item de trabalho que deseja recuperar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Saídas]</td> 
   <td>Selecione as propriedades que deseja que apareçam na saída do módulo. Os campos disponíveis dependem do tipo de item de trabalho que você deseja recuperar. Você deve selecionar pelo menos uma propriedade.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limite]</td> 
   <td>Inserir ou mapear o número máximo de itens de trabalho que [!DNL Workfront Fusion] retorna durante um ciclo de execução.</td> 
  </tr> 
 </tbody> 
</table>
