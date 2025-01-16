---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: conector
navigation-topic: apps-and-their-modules
title: Módulos do Adobe Campaign v7/v8
description: A documentação do Adobe Workfront Fusion foi movida para um novo local. Este artigo foi descontinuado, mas contém um link para o novo artigo que aborda essa funcionalidade.
author: Becky
feature: Workfront Fusion
exl-id: 84e8fa35-0c3c-46bd-8886-88c6d8d9e1d5
source-git-commit: efbe888d370e20c895dc40f18f999f2d01ec6337
workflow-type: tm+mt
source-wordcount: '1490'
ht-degree: 1%

---

# [!DNL Adobe Campaign] módulos

>[!IMPORTANT]
>
>A documentação do Adobe Workfront Fusion foi movida para um novo local.
>
>As informações neste artigo agora podem ser encontradas no artigo:
>
>* [módulos do Adobe Campaign](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/apps-and-their-modules/adobe-connectors/adobe-campaign-classic-connector.html)
>
>Atualize todos os marcadores.
>
>Este artigo não está mais sendo atualizado e será removido em breve.

Com os módulos do [!DNL Adobe Campaign], você pode iniciar um cenário do [!DNL Adobe Workfront Fusion] com base em eventos na sua conta do [!DNL Adobe Campaign v7/v8], criar, ler ou atualizar registros, pesquisar registros usando critérios que você definiu e executar chamadas de API personalizadas.

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
   <p>Requisito atual do produto: se você tiver o plano [!UICONTROL Select] ou [!UICONTROL Prime] [!DNL Adobe Workfront], sua organização deve comprar [!DNL Adobe Workfront Fusion] e [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo. [!DNL Workfront Fusion] está incluído no plano [!DNL Workfront] da [!UICONTROL Ultimate].</p>
   <p>Ou</p>
   <p>Requisito de produto herdado: sua organização deve comprar o [!DNL Adobe Workfront Fusion] e o [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Para saber que plano, tipo de licença ou acesso você tem, contate o administrador do [!DNL Workfront].

Para obter informações sobre [!DNL Adobe Workfront Fusion] licenças, consulte [[!DNL Adobe Workfront Fusion] licenças](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Pré-requisitos

Você deve adicionar os endereços IP do Fusion a [!DNL Adobe Campaign].

* Para obter instruções sobre como adicionar endereços IP ao arquivo de incluir na lista de permissões inclui na lista de permissões do Campaign, consulte [Adicionar endereços IP ao arquivo](https://experienceleague.adobe.com/en/docs/control-panel/using/sftp-management/ip-range-allow-listing#adding-ip-addresses-allow-list) na documentação do Adobe Campaign.
* Incluir na lista de permissões Para obter uma lista de endereços IP a serem adicionados ao arquivo, consulte [Endereços IP para acessar o Adobe Workfront Fusion](/help/quicksilver/workfront-fusion/get-started/ip-addresses-for-fusion.md).

## Informações da API do Adobe Campaign

O conector do Adobe Campaign usa o seguinte:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Tag da API</td> 
   <td>v1.7.22</td> 
  </tr>
 </tbody> 
 </table>

## Conectar [!DNL Adobe Campaign] a [!DNL Adobe Workfront Fusion]

>[!IMPORTANT]
>
>É altamente recomendável criar uma conexão de servidor para servidor. A Adobe Campaign atualizou a API para aceitar somente conexões servidor para servidor. Se você estiver se conectando ao Campaign versão 8 ou superior, **deverá** criar uma conexão servidor a servidor.
>
>Para obter mais informações sobre os novos requisitos de conexão do Campaign, consulte [Migração de operadores técnicos do Campaign para o Adobe Developer Console](https://experienceleague.adobe.com/docs/campaign/technotes-ac/tn-new/ims-migration.html) na documentação do Campaign.

1. Em qualquer módulo [!DNL Adobe Campaign], clique em **[!UICONTROL Adicionar]** ao lado do campo [!UICONTROL Conexão].
1. Preencha os seguintes campos:
   <table style="table-layout:auto"> 
      <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1">
      </col>
      <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">
      </col>
      <tbody>
        <tr>
          <td role="rowheader">[!UICONTROL Tipo de conexão]</td>
          <td>
            <p>Selecione se você está criando uma conexão básica ou uma conexão de servidor para servidor.</p>
          </td>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Nome da Conexão]</td>
          <td>
            <p>Insira um nome para esta conexão.</p>
          </td>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL URL Base]</td>
          <td>Insira a URL de base que você usa para se conectar à sua instância do [!DNL Adobe Campaign].</td>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Nome de Usuário]</td>
          <td>Se você estiver criando uma conexão básica, digite seu nome de usuário do Adobe Campaign.</td>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Senha]</td>
          <td>Se você estiver criando uma conexão básica, digite sua senha do Adobe Campaign.</td>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL ID do Cliente]</td>
          <td>Se você estiver criando uma conexão servidor a servidor, digite sua [!DNL Adobe] [!UICONTROL ID do Cliente]. Isso pode ser encontrado na seção [!UICONTROL Credentials details] do [!DNL Adobe Developer Console].</td>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Segredo do Cliente]</td>
          <td>Se você estiver criando uma conexão servidor a servidor, digite o [!DNL Adobe] [!UICONTROL Client Secret]. Isso pode ser encontrado na seção [!UICONTROL Credentials details] do [!DNL Adobe Developer Console].
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Ambiente]</td>
          <td>Selecione se você está conectado a um ambiente de Produção ou Não produção.
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Tipo]</td>
          <td>Selecione se você está se conectando a uma conta de serviço ou a uma conta pessoal.
        </tr>
   </tbody>
    </table>
1. Clique em **[!UICONTROL Continuar]** para criar a conexão e voltar para o módulo.

## [!DNL Adobe Campaign] módulos e seus campos

Ao configurar módulos do [!DNL Adobe Campaign], o [!DNL Workfront Fusion] exibe os campos listados abaixo. Junto com esses, campos [!DNL Adobe Campaign] adicionais podem ser exibidos, dependendo de fatores como seu nível de acesso no aplicativo ou serviço. Um título em negrito em um módulo indica um campo obrigatório.

Se você vir o botão de mapa acima de um campo ou função, poderá usá-lo para definir variáveis e funções para esse campo. Para obter mais informações, consulte [Mapear informações de um módulo para outro em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Triggers](#triggers)
* [Ações](#actions)
* [Pesquisas](#searches)

### Triggers

#### [!UICONTROL Registros de observação]

Esse módulo de acionador agendado inicia um cenário quando um registro é alterado.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão]</td> 
   <td>Para obter instruções sobre como criar uma conexão com [!DNL Adobe Campaign], consulte <a href="#connect-adobe-campaign-to-adobe-workfront-fusion" class="MCXref xref" >Criar uma conexão com [!DNL Adobe Campaign]</a> neste artigo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filtro]</td> 
   <td>Selecione se deseja observar novos registros, registros atualizados ou ambos.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Recurso]</td> 
   <td>Selecione o recurso que deseja observar.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Campos a serem incluídos na saída]</td> 
   <td>Selecione os campos que deseja incluir na saída do módulo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Campos personalizados a serem incluídos na saída]</td> 
   <td>Para cada campo personalizado que você deseja incluir na saída, clique em <b>[!UICONTROL Adicionar]</b> e insira o nome do campo personalizado.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Número máximo de resultados retornados]</td> 
   <td>Insira ou mapeie o número máximo de registros que deseja que o módulo retorne durante cada ciclo de execução de cenário.</td> 
  </tr> 
 </tbody> 
</table>


### Ações

* [[!UICONTROL Criar um registro]](#create-a-record)
* [[!UICONTROL Fazer uma chamada de API personalizada]](#make-a-custom-api-call)
* [[!UICONTROL Excluir um registro]](#delete-record)
* [[!UICONTROL Executar uma ação]](#perform-an-action)
* [[!UICONTROL Ler um registro]](#-read-a-record)
* [[!UICONTROL Assinar ou cancelar assinatura]](#subscribe-or-unsubscribe)
* [[!UICONTROL Atualizar um registro]](#update-record)

#### [!UICONTROL Criar um registro]

Este módulo de ação cria um novo registro em [!DNL Adobe Campaign].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão]</td>
   <td>Para obter instruções sobre como criar uma conexão com [!DNL Adobe Campaign], consulte <a href="#connect-adobe-campaign-to-adobe-workfront-fusion" class="MCXref xref" >Criar uma conexão com [!DNL Adobe Campaign]</a> neste artigo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Recurso]</td> 
   <td>Selecione o tipo de registro [!DNL Adobe Campaign] que deseja criar.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Campos] </td> 
   <td>Selecione os campos para os quais deseja definir valores quando o registro for criado e preencha os valores desses campos. Os campos variam de acordo com o tipo de registro selecionado.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Campos personalizados]</td> 
   <td> Para cada campo personalizado que você deseja adicionar ao novo registro, clique em <b>[!UICONTROL Adicionar item]</b> e insira ou mapeie o nome e o valor do campo. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Fazer uma chamada de API personalizada]

Este módulo faz uma chamada de API personalizada para a API [!DNL Adobe Campaign]

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Conexão]</td>
   <td>Para obter instruções sobre como criar uma conexão com [!DNL Adobe Campaign], consulte <a href="#connect-adobe-campaign-to-adobe-workfront-fusion" class="MCXref xref" >Criar uma conexão com [!DNL Adobe Campaign]</a> neste artigo.</td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Ação]</td>
      <td><p>Selecione a ação que você deseja que a chamada de API execute.</p>
      <p>[!UICONTROL Executar consulta]</p>
      <p>[!UICONTROL Gravar]</p>
      <p>[!UICONTROL Obter entidade se mais recente]</p>
      <p>[!UICONTROL Selecionar tudo]</p>
      <p>[!UICONTROL Evento Push]</p>
    </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Cabeçalhos]</td>
      <td>
        <p>Adicione os cabeçalhos da solicitação no formulário de um objeto JSON padrão.</p>
        <p>Por exemplo, <code>{"Content-type":"application/json"}</code></p>
        <p>[!DNL Workfront Fusion] adiciona automaticamente o cabeçalho do token [!UICONTROL x-security].</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Corpo XML]</td>
   <td> <p>Adicione o conteúdo do corpo para a chamada da API em XML, sem o elemento de sessão. </td>     </tr>
  </tbody>
</table>

#### [!UICONTROL Excluir Registro]

Este módulo de ação exclui um único registro de [!DNL Adobe Campaign].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão]</td>
   <td>Para obter instruções sobre como criar uma conexão com [!DNL Adobe Campaign], consulte <a href="#connect-adobe-campaign-to-adobe-workfront-fusion" class="MCXref xref" >Criar uma conexão com [!DNL Adobe Campaign]</a> neste artigo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Recurso]</td> 
   <td>Selecione o tipo de recurso que deseja excluir.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>Insira ou mapeie a ID do recurso que deseja excluir.</td> 
  </tr> 
 </tbody> 
</table>


#### [!UICONTROL Executar uma ação]

Este módulo de ação executa uma ação selecionada em um objeto na API [!DNL Adobe Campaign].

Para obter informações sobre ações e campos específicos, consulte [[!DNL Adobe Campaign] - Documentação da API](https://experienceleague.adobe.com/developer/campaign-api/api/p-14.html).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão]</td>
   <td>Para obter instruções sobre como criar uma conexão com [!DNL Adobe Campaign], consulte <a href="#connect-adobe-campaign-to-adobe-workfront-fusion" class="MCXref xref" >Criar uma conexão com [!DNL Adobe Campaign]</a> neste artigo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ação]</td> 
   <td><p>Selecione a ação a ser executada no objeto.</p>
   <ul>
   <li><p><b>[!DNL List]</b></p><p> Para obter os campos disponíveis, consulte <a href="#search" class="MCXref xref" >[!UICONTROL Pesquisa]</a> neste artigo. </p></li>
     <li><p><b>[!UICONTROL Obter]</b></p><p> Para obter os campos disponíveis, consulte <a href="#search" class="MCXref xref" >[!UICONTROL Pesquisa]</a> neste artigo. </p></li> 
   <li><p><b>[!UICONTROL Criar]</b></p><p> Para campos disponíveis, consulte <a href="#create-a-record" class="MCXref xref" >[!UICONTROL Criar um registro]</a> neste artigo. </p></li>
   <li><p><b>[!UICONTROL Atualizar]</b></p><p> Para campos disponíveis, consulte <a href="#update-record" class="MCXref xref" >[!UICONTROL Atualizar um registro]</a> neste artigo. </p></li>
   <li><p><b>[!UICONTROL Excluir]</b></p><p> Para campos disponíveis, consulte <a href="#delete-record" class="MCXref xref" >[!UICONTROL Excluir um registro]</a> neste artigo. </p></li>
   </ul>
   </td>
</tr> 
 </tbody> 
</table>

#### [!UICONTROL Ler um registro]

Este módulo de ação lê um registro de [!DNL Adobe Campaign].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão]</td>
   <td>Para obter instruções sobre como criar uma conexão com [!DNL Adobe Campaign], consulte <a href="#connect-adobe-campaign-to-adobe-workfront-fusion" class="MCXref xref" >Criar uma conexão com [!DNL Adobe Campaign]</a> neste artigo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Recurso]</td> 
   <td>Selecione o tipo de registro [!DNL Adobe Campaign] que deseja ler.</td> 
  </tr> 
    <tr> 
   <td role="rowheader">[!UICONTROL ID] </td> 
   <td>Insira do mapa a ID do registro que você deseja ler.</td> 
  </tr> 
 <tr> 
   <td role="rowheader">[!UICONTROL Campos a serem incluídos na saída] </td> 
   <td>Selecione os campos que deseja incluir na saída do módulo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Campos personalizados a serem incluídos na saída]</td> 
   <td>Para cada campo personalizado que você deseja incluir na saída, clique em <b>[!UICONTROL Adicionar]</b> e insira o nome do campo personalizado.</td> 
  </tr> 
 </tbody> 
</table>


#### [!UICONTROL Assinar ou cancelar assinatura]

Este módulo de ação assina um usuário ou cancela a assinatura de um usuário em um serviço de informação.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão]</td>
   <td>Para obter instruções sobre como criar uma conexão com [!DNL Adobe Campaign], consulte <a href="#connect-adobe-campaign-to-adobe-workfront-fusion" class="MCXref xref" >Criar uma conexão com [!DNL Adobe Campaign]</a> neste artigo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Assinar ou cancelar assinatura]</td> 
   <td>Selecione se deseja assinar ou cancelar a assinatura do serviço de informações.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nome do serviço]</td> 
   <td>Selecione o serviço que deseja assinar ou do qual deseja cancelar a assinatura.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Endereço de email do destinatário] </td> 
   <td>Insira ou mapeie o endereço de email do usuário que deseja assinar ou cancelar a assinatura do serviço de informações.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Atualizar registro]

Este módulo de ação atualiza um único registro em [!DNL Adobe Campaign].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão]</td>
   <td>Para obter instruções sobre como criar uma conexão com [!DNL Adobe Campaign], consulte <a href="#connect-adobe-campaign-to-adobe-workfront-fusion" class="MCXref xref" >Criar uma conexão com [!DNL Adobe Campaign]</a> neste artigo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Recurso]</td> 
   <td>Selecione o tipo de registro [!DNL Adobe Campaign] que deseja criar.</td> 
  </tr> 
    <tr> 
   <td role="rowheader">[!UICONTROL ID] </td> 
   <td>Insira do mapa a ID do registro que você deseja atualizar.</td> 
  </tr> 
<tr> 
   <td role="rowheader">[!UICONTROL Campos] </td> 
   <td>Selecione os campos para os quais deseja atualizar valores e preencha os valores desses campos. Os campos variam de acordo com o tipo de registro selecionado.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Campos personalizados]</td> 
   <td> Para cada campo personalizado que você deseja atualizar, clique em <b>[!UICONTROL Adicionar item]</b> e insira ou mapeie o nome e o valor do campo. </td> 
  </tr> 
 </tbody> 
</table>

### Pesquisas

#### [!UICONTROL Pesquisa]

Este módulo de pesquisa retorna registros com base nos critérios especificados.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão]</td>
   <td>Para obter instruções sobre como criar uma conexão com [!DNL Adobe Campaign], consulte <a href="#connect-adobe-campaign-to-adobe-workfront-fusion" class="MCXref xref" >Criar uma conexão com [!DNL Adobe Campaign]</a> neste artigo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Recurso]</td> 
   <td>Selecione o tipo de registro [!DNL Adobe Campaign] que deseja criar.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limite] </td> 
   <td>Insira ou mapeie o número máximo de registros que deseja que o módulo retorne durante cada ciclo de execução de cenário.</td> 
  </tr> 
 </tbody> 
</table>
