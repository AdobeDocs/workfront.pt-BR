---
filename: workday-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: conector
navigation-topic: apps-and-their-modules
title: Módulos Workday
description: Em um cenário do Adobe Workfront Fusion, você pode automatizar os workflows que usam [!DNL Workday], bem como conectá-lo a vários aplicativos e serviços de terceiros.
author: Becky
exl-id: 535573e0-b6ad-43a2-b7cb-ed32d1dc8d16
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '965'
ht-degree: 2%

---

# [!DNL Workday] módulos

Em um [!DNL Adobe Workfront Fusion] , é possível automatizar workflows que usam [!DNL Workday], bem como conectá-lo a vários aplicativos e serviços de terceiros.

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

Para usar o [!DNL Workday] módulos, você deve:

* Ter um [!DNL Workday] conta.

* Crie um aplicativo OAuth em [!DNL Workday]. Para obter instruções, consulte o [!DNL Workday] documentação.

## Connect [!DNL Workday] para [!DNL Workfront Fusion]

1. Em qualquer [!DNL Workfront Fusion] módulo, clique em [!UICONTROL Adicionar] ao lado do [!UICONTROL Conexão] campo

2. Preencha os seguintes campos:

   <table style="table-layout:auto"> 
        <col/>
        <col/>
        <tbody>
            <tr>
                <td role="rowheader">
                    <p role="rowheader">[!UICONTROL Nome da conexão]</p>
                </td>
                <td>Digite um nome para a conexão</td>
            </tr>
            <tr>
                <td  role="rowheader">[!UICONTROL Workday host]</td>
                <td>Insira o endereço do [!DNL Workday] host sem <code>https://</code>. Por exemplo: <code>mycompany.workday.com</code>.</td>
            </tr>
            <tr>
                <td role="rowheader">[!UICONTROL Services URL]</td>
                <td>Insira o endereço do [!DNL Workday] serviços da Web sem <code>https://</code>. Por exemplo: <code>mycompany-services.workday.com</code>.</td>
            </tr>
            <tr>
                <td  role="rowheader">[!UICONTROL Nome do locatário]</td>
                <td>Insira o locatário para isso [!DNL Workday] conta. Seu locatário é o identificador de sua organização e pode ser visto no URL usado para fazer logon no Workday. Exemplo: no endereço <code>https://www.myworkday.com/mycompany</code>, o locatário é <code>mycompany</code>.</td>
            </tr>
            <tr>
                <td role="rowheader">[!UICONTROL Client ID]</td>
                <td>Insira a ID do cliente para o [!DNL Workday] aplicativo usado por esta conexão. Isso é obtido ao criar o aplicativo em [!DNL Workday].</td>
            </tr>
            <tr>
                <td  role="rowheader">[!UICONTROL Segredo do cliente]</td>
                <td>Insira o Segredo do cliente para o [!DNL Workday] aplicativo usado por esta conexão. Isso é obtido ao criar o aplicativo em [!DNL Workday].</td>
            </tr>
            <tr>
                <td role="rowheader">[!UICONTROL Tempo limite da sessão (min)]</td>
                <td >Insira o número de minutos após o qual o token de autorização expira.</td>
            </tr>
        </tbody>
    </table>


3. Clique em [!UICONTROL Continuar] para salvar a conexão e retornar ao módulo

## [!DNL Workday] módulos e seus campos

Ao configurar [!DNL Workday] módulos, [!DNL Workfront Fusion] exibe os campos listados abaixo. Junto com esses, [!DNL Workday] podem ser exibidos, dependendo de fatores como seu nível de acesso no aplicativo ou serviço. Um título em negrito em um módulo indica um campo obrigatório.

Se o botão de mapa for exibido acima de um campo ou função, é possível usá-lo para definir variáveis e funções para esse campo. Para obter mais informações, consulte [Mapear informações de um módulo para outro no [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Ação](#action)

* [Pesquisar](#search)


### Ação

* [[!UICONTROL Criar um registro]](#create-a-record)

* [[!UICONTROL Excluir um registro]](#delete-a-record)

* [[!UICONTROL Efetuar uma chamada de API personalizada]](#make-a-custom-api-call)

* [[!UICONTROL Atualizar um registro]](#update-a-record)


#### [!UICONTROL Criar um registro]

Esse módulo de ação cria um único registro em [!DNL Workday].

<table style="table-layout:auto"> 
    <col/>
    <col/>
    <tbody>
        <tr>
            <td role="rowheader">[!UICONTROL Connection]</td>
            <td>Para obter instruções sobre como conectar seu [!DNL Workday] conta para o Workfront Fusion, consulte <a href="#Connect" class="MCXref xre[!DNL ]f" >Connect [!DNL Workday] para [!DNL Workfront Fusion]</a>.</td>
        </tr>
        <tr>
            <td  role="rowheader">[!UICONTROL Tipo de registro]</td>
            <td>Selecione o tipo de registro que deseja criar.</td>
        </tr>
        <tr>
            <td role="rowheader">[!UICONTROL ID] </td>
            <td>Insira ou mapeie a ID do registro que deseja criar.</td>
        </tr>
        <tr>
            <td role="rowheader">[!UICONTROL ID do subrecurso]</td>
            <td >Insira ou mapeie a ID do subrecurso que deseja criar.</td>
        </tr>
    </tbody>
</table>

#### [!UICONTROL Excluir um registro]

Esse módulo de ação exclui um único registro em [!DNL Workday].

<table style="table-layout:auto"> 
    <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1">
    </col>
    <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">
    </col>
    <tbody>
        <tr>
            <td role="rowheader">[!UICONTROL Connection]</td>
            <td>Para obter instruções sobre como conectar seu [!DNL Workday] para [!DNL Workfront Fusion], consulte <a href="#Connect" class="MCXref xre[!DNL ]f" >Connect [!DNL Workday] para [!DNL Workfront Fusion]</a>.</td>
        </tr>
        <tr>
            <td  role="rowheader">[!UICONTROL Tipo de registro]</td>
            <td>Selecione o tipo de registro que deseja excluir.</td>
        </tr>
        <tr>
            <td role="rowheader">[!UICONTROL Tipo de registro específico]</td>
            <td>Selecione o tipo específico de registro que deseja excluir. Elas se baseiam no tipo de registro escolhido.</td>
        </tr>
        <tr>
            <td  role="rowheader">[!UICONTROL ID do subrecurso]</td>
            <td>Insira ou mapeie a ID do subrecurso que deseja excluir.</td>
        </tr>
        <tr>
            <td role="rowheader">[!UICONTROL ID] </td>
            <td >Insira ou mapeie a ID do registro que deseja excluir.</td>
        </tr>
    </tbody>
</table>


### [!UICONTROL Efetuar uma chamada de API personalizada]

Esse módulo de ação permite que você faça uma chamada autenticada personalizada para o [!DNL Workday] API. Dessa forma, você pode criar uma automação de fluxo de dados que não pode ser realizada pela outra [!DNL Workday] módulos.

Ao configurar esse módulo, os seguintes campos são exibidos.

O módulo retorna um código de status, juntamente com os cabeçalhos e o corpo da chamada à API.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Connection]</p> </td> 
            <td>Para obter instruções sobre como conectar seu [!DNL Workday] para [!DNL Workfront Fusion], consulte <a href="#Connect" class="MCXref xre[!DNL ]f" >Connect [!DNL Workday] para [!DNL Workfront Fusion]</a>.</td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td>Insira um caminho relativo a <code style="color: #ff1493;">https://&lt;tenantHostname>/api/&lt;serviceName>/&lt;version>/&lt;tenant></code>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Método]</td> 
   <td> <p>Selecione o método de solicitação HTTP que você precisa configurar a chamada da API. Para obter mais informações, consulte <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">Métodos de solicitação HTTP em [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cabeçalhos]</td> 
   <td> <p>Adicione os cabeçalhos da solicitação no formato de um objeto JSON padrão.</p> <p>Por exemplo, <code>{"Content-type":"application/json"}</code></p> <p>O [!UICONTROL Workfront Fusion] adiciona os cabeçalhos de autorização para você.</p> </td> 
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

#### [!UICONTROL Atualizar um registro]

Este módulo de ação atualiza um único registro em [!DNL Workday].

<table style="table-layout:auto"> 
    <col/>
    <col/>
    <tbody>
        <tr>
            <td role="rowheader">[!UICONTROL Connection]</td>
            <td>Para obter instruções sobre como conectar seu [!DNL Workday] conta para o Workfront Fusion, consulte <a href="#Connect" class="MCXref xref" >[!UICONTROL Connect [!DNL Workday] para o Workfront Fusion]</a></td>
        </tr>
        <tr>
            <td  role="rowheader">Tipo de registro</td>
            <td>Selecione o tipo de registro t[!UICONTROL ] que deseja atualizar.</td>
        </tr>
        <tr>
            <td role="rowheader">[!UICONTROL ID] </td>
            <td>Insira ou mapeie a ID do registro que deseja atualizar.</td>
        </tr>
        <tr>
            <td role="rowheader">[!UICONTROL ID do subrecurso]</td>
            <td >Insira ou mapeie a ID do subrecurso que deseja atualizar.</td>
        </tr>
    </tbody>
</table>

### Pesquisar

* [[!UICONTROL Ler um registro]](#read-a-record)

* [[!UICONTROL Listar registros]](#list-records)


#### [!UICONTROL Ler um registro]

Este módulo de ação lê um único registro.

<table style="table-layout:auto"> 
    <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1">
    </col>
    <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">
    </col>
    <tbody>
        <tr>
            <td role="rowheader">[!UICONTROL Connection]</td>
            <td>Para obter instruções sobre como conectar seu [!DNL Workday] conta para o Workfront Fusion, consulte <a href="#Connect" class="MCXref xref" >[!UICONTROL Connect [!DNL Workday] para o Workfront Fusion]</a></td>
        </tr>
        <tr>
            <td  role="rowheader">[!UICONTROL Tipo de registro]</td>
            <td>Selecione o tipo de registro que deseja excluir.</td>
        </tr>
        <tr>
            <td role="rowheader">[!UICONTROL Tipo de registro específico]</td>
            <td>Selecione o tipo específico de registro que deseja ler. Elas se baseiam no tipo de registro escolhido.</td>
        </tr>
        <tr>
            <td role="rowheader">[!UICONTROL ID] </td>
            <td >Insira ou mapeie a ID do registro que deseja excluir.</td>
        </tr>
    </tbody>
</table>

#### [!UICONTROL Listar registros]

Esse módulo de pesquisa recupera uma lista de registros do tipo especificado.

<table style="table-layout:auto"> 
      <col/>
      <col/>
      <tbody>
          <tr>
              <td role="rowheader">[!UICONTROL Connection]</td>
              <td>Para obter instruções sobre como conectar seu [!DNL Workday] para [!DNL Workfront Fusion], consulte <a href="#Connect" class="MCXref xref" >Connect [!DNL Workday] para [!DNL Workfront Fusion]</a></td>
          </tr>
          <tr>
              <td  role="rowheader">[!UICONTROL Tipo de registro]</td>
              <td>Selecione o tipo de registro que deseja recuperar.</td>
          </tr>
          <tr>
              <td role="rowheader">[!UICONTROL Limite]</td>
              <td >
                  <p>Insira ou mapeie o número máximo de registros que você deseja que o módulo recupere durante cada ciclo de execução de cenário.</p>
              </td>
          </tr>
      </tbody>
  </table>
