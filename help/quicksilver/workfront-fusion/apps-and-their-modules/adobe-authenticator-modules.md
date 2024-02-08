---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: conector
navigation-topic: apps-and-their-modules
title: Módulo Adobe Authenticator
description: Com o módulo Adobe Authenticator, você pode se conectar a qualquer produto Adobe com uma API, usando uma única conexão.
author: Becky
feature: Workfront Fusion
source-git-commit: 61a579c19228381d0aa06de3db5217614999731b
workflow-type: tm+mt
source-wordcount: '882'
ht-degree: 1%

---

# Módulos do Adobe Authenticator

O módulo Adobe Authenticator permite conectar-se a qualquer API de Adobe, usando uma única conexão. Isso permite que você se conecte mais facilmente a produtos Adobe que ainda não têm um conector Fusion dedicado.

A vantagem sobre os módulos HTTP é que você pode criar uma conexão, como em um aplicativo dedicado.

Para ver uma lista de APIs de Adobe disponíveis, consulte [APIs Adobe](https://developer.adobe.com/apis). Você pode usar somente as APIs às quais está atribuído.

## Requisitos de acesso

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront] plano</td>
      <td>
        <p>Novo: Qualquer um</p><p>Ou</p><p>Atual: [!UICONTROL Pro] ou superior</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront] licença</td>
      <td>
        <p>Novo: Padrão</p><p>Ou</p><p>Atual: [!UICONTROL Plano], [!UICONTROL Trabalho]</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront Fusion] licença</td>
      <td>
   <p>Requisito de licença Fusion atual: Não [!DNL Workfront Fusion] requisito de licença.</p>
   <p>Ou</p>
   <p>Requisito de licença herdada do Fusion: [!UICONTROL [!DNL Workfront Fusion] para Automação e integração do trabalho] </p>
   </td>
    </tr>
    <tr>
      <td role="rowheader">Produto</td>
      <td>
   <p>Novo plano do Workfront: se você tiver o [!UICONTROL Select] ou o [!UICONTROL Prime] [!DNL Adobe Workfront] Planejar, sua organização deve comprar [!DNL Adobe Workfront Fusion] bem como [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo. [!DNL Workfront Fusion] está incluído no [!UICONTROL Ultimate] [!DNL Workfront] plano.</p>
   <p>Ou</p>
   <p>Plano atual do Workfront: sua organização deve comprar [!DNL Adobe Workfront Fusion] bem como [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo.</p>
   </td>
    </tr>
  </tbody>
</table>

## Pré-requisitos

* Você deve ter acesso ao produto Adobe ao qual deseja que o módulo se conecte.
* Você deve ter acesso ao Console do Adobe Developer.
* Você deve ter um projeto no Console do Adobe Developer que inclua a API à qual deseja que o módulo se conecte. Você pode:

   * Crie um novo projeto com a API.

     Ou
   * Adicionar a API a um projeto existente.

  Para obter informações sobre como criar ou adicionar uma API a um projeto no Console do Adobe Developer, consulte [Criar um projeto](https://developer.adobe.com/dep/guides/dev-console/create-project/) na documentação do Adobe.

## Criar uma conexão

Uma conexão do Adobe Authenticator se conecta a um único projeto no Adobe Developer Console. Para usar a mesma conexão para mais de uma API de Adobe, adicione as APIs ao mesmo projeto e crie uma conexão com esse projeto.

Você pode criar conexões separadas para projetos separados, mas não pode usar uma conexão para acessar uma API que não esteja no projeto especificado nessa conexão.

>[!IMPORTANT]
>
>Com o conector do Adobe Authenticator, você tem a opção de fazer uma conexão servidor a servidor do OAuth ou uma conexão de conta de serviço (JWT). O Adobe descontinuou as credenciais do JWT, que deixarão de funcionar após 1º de janeiro de 2025. **Portanto, recomendamos criar conexões OAuth.**
>
>Para obter mais informações sobre esses tipos de conexões, consulte [Autenticação de servidor para servidor](https://developer.adobe.com/developer-console/docs/guides/authentication/ServerToServerAuthentication/) na documentação do Adobe

Para criar uma conexão:

1. Em qualquer módulo do Adobe Authenticator, clique em **Adicionar** ao lado do campo Connection.
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
          <p>Selecione se deseja criar uma conexão de servidor para servidor OAuth ou uma conexão de conta de serviço (JWT).</p>
        </td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Nome da Conexão]</td>
        <td>
          <p>Insira um nome para esta conexão.</p>
        </td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL ID do Cliente]</td>
        <td>Insira seu [!DNL Adobe] ID do cliente. Isso pode ser encontrado na seção [!UICONTROL Credenciais detalhes] do [!DNL Adobe Developer Console].
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Segredo do Cliente]</td>
        <td>Insira seu [!DNL Adobe] Segredo do cliente. Isso pode ser encontrado na seção [!UICONTROL Credenciais detalhes] do [!DNL Adobe Developer Console].
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Escopos]</td>
        <td>Se você selecionou uma conexão OAuth, insira os escopos necessários para essa conexão.</td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL ID da conta técnica]</td>
        <td>Insira seu [!DNL Adobe] ID da conta técnica. Isso pode ser encontrado na seção [!UICONTROL Credenciais detalhes] do [!DNL Adobe Developer Console].
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL ID da Organização]</td>
        <td>Se você selecionou uma conexão JWT, insira [!DNL Adobe] ID da organização. Isso pode ser encontrado na seção [!UICONTROL Credenciais detalhes] do [!DNL Adobe Developer Console].
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Metaescopos]</td>
        <td>Se você selecionou uma conexão JWT, insira os metaescopos necessários para essa conexão. </td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Chave privada]</td>
        <td>
          <p>Se você selecionou uma conexão JWT, insira a chave privada que foi gerada quando suas credenciais foram criadas no [!DNL Adobe Developer Console]. </p>
          <p>Para extrair sua chave privada ou certificado:</p>
          <ol>
            <li value="1">
              <p>Clique em <b>[!UICONTROL Extract]</b>.</p>
            </li>
            <li value="2">
              <p>Selecione o tipo de arquivo que você está extraindo.</p>
            </li>
            <li value="3">
              <p>Selecione o arquivo que contém a chave privada ou o certificado.</p>
            </li>
            <li value="4">
              <p>Digite a senha do arquivo.</p>
            </li>
            <li value="5">
              <p>Clique em <b>[!UICONTROL Salvar]</b> para extrair o arquivo e retornar à configuração da conexão.</p>
            </li>
          </ol>
        </td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Ambiente]</td>
        <td>Selecione se você está se conectando a um ambiente de produção ou não produção.</td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Tipo]</td>
        <td>Selecione se você está se conectando a uma conta de serviço ou a uma conta pessoal.</td>
      </tr>
    </tbody>
    </table>

1. Clique em **[!UICONTROL Continuar]** para salvar a conexão e retornar ao módulo.

## Módulo

### Fazer uma chamada de API personalizada

Esse módulo de ação permite fazer uma chamada para qualquer API Adobe.

>[!TIP]
>
>É necessário inserir o URL inteiro da API à qual você deseja se conectar. Este módulo não aceita URLs relativos.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
     <td role="rowheader">[!UICONTROL Conexão]</td>
     <td>Para obter instruções sobre como criar uma conexão com o módulo Adobe Authenticator, consulte <a href="#create-a-connection" class="MCXref xref" >Criar uma conexão</a> neste artigo.</td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL URL]</p>
      </td>
      <td>
        <p>Insira o URL inteiro do ponto de API ao qual deseja se conectar.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Método]</p>
   <td> <p>Selecione o método de solicitação HTTP necessário para configurar a chamada de API. Para obter mais informações, consulte <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">Métodos de solicitação HTTP em [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Cabeçalhos]</td>
      <td>
        <p>Adicione os cabeçalhos da solicitação no formulário de um objeto JSON padrão.</p>
        <p>Por exemplo, <code>{"Content-type":"application/json"}</code></p>
        <p>O Workfront Fusion adiciona cabeçalhos de autorização automaticamente.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Cadeia de Consulta]  </td>
      <td>
        <p>Insira a string de consulta da solicitação.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Corpo]</td>
   <td> <p>Adicione o conteúdo do corpo para a chamada à API na forma de um objeto JSON padrão.</p> <p>Nota:  <p>Ao usar declarações condicionais como <code>if</code> no JSON, coloque as aspas fora da declaração condicional.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td>     </tr>
     <tr>
      <td role="rowheader">[!UICONTROL Limite]  </td>
      <td>
        <p>Insira o número máximo de resultados que você deseja que o módulo retorne em um ciclo de execução.</p>
      </td>
    </tr>
  </tbody>
</table>

