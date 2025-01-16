---
filename: workday-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: conector
navigation-topic: apps-and-their-modules
title: Módulos do Workday
description: A documentação do Adobe Workfront Fusion foi movida para um novo local. Este artigo foi descontinuado, mas contém um link para o novo artigo que aborda essa funcionalidade.
author: Becky
feature: Workfront Fusion
exl-id: 535573e0-b6ad-43a2-b7cb-ed32d1dc8d16
source-git-commit: efbe888d370e20c895dc40f18f999f2d01ec6337
workflow-type: tm+mt
source-wordcount: '1080'
ht-degree: 1%

---

# [!DNL Workday] módulos

>[!IMPORTANT]
>
>A documentação do Adobe Workfront Fusion foi movida para um novo local.
>
>As informações neste artigo agora podem ser encontradas no artigo:
>
>* [módulos do Workday](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/workday-modules.html)
>
>Atualize todos os marcadores.
>
>Este artigo não está mais sendo atualizado e será removido em breve.

Em um cenário [!DNL Adobe Workfront Fusion], você pode automatizar fluxos de trabalho que usam [!DNL Workday], bem como conectá-los a vários aplicativos e serviços de terceiros.

Se você precisar de instruções sobre como criar um cenário, consulte [Criar um cenário [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

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

Para usar os módulos do [!DNL Workday], você deve:

* Ter uma conta [!DNL Workday].

* Crie um aplicativo OAuth em [!DNL Workday]. Para obter instruções, consulte a documentação do [!DNL Workday].

## Informações da API do Workday

O conector do Workday usa o seguinte:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">URL base</td> 
   <td>https://{{connection.servicesUrl}}/api</td> 
  </tr>
  <tr> 
   <td role="rowheader">Tag da API</td> 
   <td>v1.6.4</td> 
  </tr>
 </tbody> 
 </table>

## Conectar [!DNL Workday] a [!DNL Workfront Fusion]

1. Em qualquer módulo [!DNL Workfront Fusion], clique em [!UICONTROL Adicionar] ao lado do campo [!UICONTROL Conexão]

2. Preencha os seguintes campos:

   <table style="table-layout:auto"> 
        <col/>
        <col/>
        <tbody>
            <tr>
                <td role="rowheader">
                    <p role="rowheader">[!UICONTROL Nome da Conexão]</p>
                </td>
                <td>Insira um nome para a conexão</td>
            </tr>
            <tr>
                <td  role="rowheader">[!UICONTROL host Workday]</td>
                <td>Digite o endereço do host [!DNL Workday] sem <code>https://</code>. Por exemplo: <code>mycompany.workday.com</code>.</td>
            </tr>
            <tr>
                <td role="rowheader">[!UICONTROL URL DE SERVIÇOS]</td>
                <td>Insira o endereço dos serviços Web do [!DNL Workday] sem <code>https://</code>. Por exemplo: <code>mycompany-services.workday.com</code>.</td>
            </tr>
            <tr>
                <td  role="rowheader">[!UICONTROL Nome do Locatário]</td>
                <td>Insira o locatário para esta conta [!DNL Workday]. Seu locatário é o identificador da sua organização e pode ser visto no URL usado para fazer logon no Workday. Exemplo: no endereço <code>https://www.myworkday.com/mycompany</code>, o locatário é <code>mycompany</code>.</td>
            </tr>
            <tr>
                <td role="rowheader">[!UICONTROL ID do Cliente]</td>
                <td>Insira a ID do Cliente para o aplicativo [!DNL Workday] que esta conexão usa. Isso é obtido ao criar o aplicativo em [!DNL Workday].</td>
            </tr>
            <tr>
                <td  role="rowheader">[!UICONTROL Segredo do Cliente]</td>
                <td>Insira o Segredo do Cliente para o aplicativo [!DNL Workday] que esta conexão usa. Isso é obtido ao criar o aplicativo em [!DNL Workday].</td>
            </tr>
            <tr>
                <td role="rowheader">[!UICONTROL Tempo limite de sessão (min)]</td>
                <td >Insira o número de minutos após o qual o token de autorização expira.</td>
            </tr>
        </tbody>
    </table>


3. Clique em [!UICONTROL Continuar] para salvar a conexão e retornar ao módulo

## [!DNL Workday] módulos e seus campos

Ao configurar módulos do [!DNL Workday], o [!DNL Workfront Fusion] exibe os campos listados abaixo. Junto com esses, campos [!DNL Workday] adicionais podem ser exibidos, dependendo de fatores como seu nível de acesso no aplicativo ou serviço. Um título em negrito em um módulo indica um campo obrigatório.

Se você vir o botão de mapa acima de um campo ou função, poderá usá-lo para definir variáveis e funções para esse campo. Para obter mais informações, consulte [Mapear informações de um módulo para outro em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Ação](#action)

* [Pesquisar](#search)


### Ação

* [[!UICONTROL Criar um registro]](#create-a-record)

* [[!UICONTROL Excluir um registro]](#delete-a-record)

* [[!UICONTROL Fazer uma chamada de API personalizada]](#make-a-custom-api-call)

* [[!UICONTROL Atualizar um registro]](#update-a-record)


#### [!UICONTROL Criar um registro]

Este módulo de ação cria um único registro em [!DNL Workday].

<table style="table-layout:auto"> 
    <col/>
    <col/>
    <tbody>
        <tr>
            <td role="rowheader">[!UICONTROL Conexão]</td>
            <td>Para obter instruções sobre como conectar sua conta do [!DNL Workday] ao Workfront Fusion, consulte <a href="#Connect" class="MCXref xre[!DNL ]f" >Conectar [!DNL Workday] ao [!DNL Workfront Fusion]</a>.</td>
        </tr>
        <tr>
            <td  role="rowheader">[!UICONTROL Tipo de Registro]</td>
            <td>Selecione o tipo de registro que deseja criar.</td>
        </tr>
        <tr>
            <td role="rowheader">[!UICONTROL ID] </td>
            <td>Insira ou mapeie a ID do registro que deseja criar.</td>
        </tr>
        <tr>
            <td role="rowheader">[!UICONTROL ID de sub-recurso]</td>
            <td >Insira ou mapeie a ID do subrecurso que deseja criar.</td>
        </tr>
    </tbody>
</table>

#### [!UICONTROL Excluir um registro]

Este módulo de ação exclui um único registro em [!DNL Workday].

<table style="table-layout:auto"> 
    <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1">
    </col>
    <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">
    </col>
    <tbody>
        <tr>
            <td role="rowheader">[!UICONTROL Conexão]</td>
            <td>Para obter instruções sobre como conectar sua conta do [!DNL Workday] ao [!DNL Workfront Fusion], consulte <a href="#Connect" class="MCXref xre[!DNL ]f" >Conectar [!DNL Workday] ao [!DNL Workfront Fusion]</a>.</td>
        </tr>
        <tr>
            <td  role="rowheader">[!UICONTROL Tipo de registro]</td>
            <td>Selecione o tipo de registro que deseja excluir.</td>
        </tr>
        <tr>
            <td role="rowheader">[!UICONTROL Tipo de registro específico]</td>
            <td>Selecione o tipo específico de registro que deseja excluir. Baseiam-se no tipo de registro escolhido.</td>
        </tr>
        <tr>
            <td  role="rowheader">[!UICONTROL ID de sub-recurso]</td>
            <td>Insira ou mapeie a ID do subrecurso que deseja excluir.</td>
        </tr>
        <tr>
            <td role="rowheader">[!UICONTROL ID] </td>
            <td >Informe ou mapeie a ID do registro que deseja deletar.</td>
        </tr>
    </tbody>
</table>


### [!UICONTROL Fazer uma chamada de API personalizada]

Este módulo de ação permite fazer uma chamada autenticada personalizada para a API [!DNL Workday]. Dessa forma, você pode criar uma automação de fluxo de dados que não pode ser realizada pelos outros módulos do [!DNL Workday].

Ao configurar esse módulo, os campos a seguir são exibidos.

O módulo retorna o código de status a, juntamente com os cabeçalhos e o corpo da chamada de API.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Connection]</p> </td> 
            <td>Para obter instruções sobre como conectar sua conta do [!DNL Workday] ao [!DNL Workfront Fusion], consulte <a href="#Connect" class="MCXref xre[!DNL ]f" >Conectar [!DNL Workday] ao [!DNL Workfront Fusion]</a>.</td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td>Insira um caminho relativo para <code style="color: #ff1493;">https://&lt;tenantHostname>/api/&lt;serviceName>/&lt;version>/&lt;tenant></code>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Método]</td> 
   <td> <p>Selecione o método de solicitação HTTP necessário para configurar a chamada de API. Para obter mais informações, consulte <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">Métodos de solicitação HTTP em [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cabeçalhos]</td> 
   <td> <p>Adicione os cabeçalhos da solicitação no formulário de um objeto JSON padrão.</p> <p>Por exemplo, <code>{"Content-type":"application/json"}</code></p> <p>O [!UICONTROL Workfront Fusion] adiciona os cabeçalhos de autorização para você.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cadeia de Consulta]</td> 
   <td> <p>Adicione a consulta da chamada à API na forma de um objeto JSON padrão.</p> <p>Por exemplo: <code>{"name":"something-urgent"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Corpo]</td> 
   <td> <p>Adicione o conteúdo do corpo para a chamada à API na forma de um objeto JSON padrão.</p> <p>Nota:  <p>Ao usar instruções condicionais como <code>if</code> em seu JSON, coloque as aspas fora da instrução condicional.</p> 
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
            <td role="rowheader">[!UICONTROL Conexão]</td>
            <td>Para obter instruções sobre como conectar sua conta do [!DNL Workday] ao Workfront Fusion, consulte <a href="#Connect" class="MCXref xref" >[!UICONTROL Connect [!DNL Workday] to Workfront Fusion]</a></td>
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
            <td role="rowheader">[!UICONTROL ID de sub-recurso]</td>
            <td >Insira ou mapeie a ID do subrecurso que você deseja atualizar.</td>
        </tr>
    </tbody>
</table>

### Pesquisar

* [[!UICONTROL Ler um registro]](#read-a-record)

* [[!UICONTROL Listar registros]](#list-records)


#### [!UICONTROL Ler um registro]

Esse módulo de ação lê um único registro.

<table style="table-layout:auto"> 
    <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1">
    </col>
    <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">
    </col>
    <tbody>
        <tr>
            <td role="rowheader">[!UICONTROL Conexão]</td>
            <td>Para obter instruções sobre como conectar sua conta do [!DNL Workday] ao Workfront Fusion, consulte <a href="#Connect" class="MCXref xref" >[!UICONTROL Connect [!DNL Workday] to Workfront Fusion]</a></td>
        </tr>
        <tr>
            <td  role="rowheader">[!UICONTROL Tipo de registro]</td>
            <td>Selecione o tipo de registro que deseja excluir.</td>
        </tr>
        <tr>
            <td role="rowheader">[!UICONTROL Tipo de registro específico]</td>
            <td>Selecione o tipo específico de registro que deseja ler. Baseiam-se no tipo de registro escolhido.</td>
        </tr>
        <tr>
            <td role="rowheader">[!UICONTROL ID] </td>
            <td >Informe ou mapeie a ID do registro que deseja deletar.</td>
        </tr>
    </tbody>
</table>

#### [!UICONTROL Listar registros]

Este módulo de pesquisa recupera uma lista de registros do tipo especificado.

<table style="table-layout:auto"> 
      <col/>
      <col/>
      <tbody>
          <tr>
              <td role="rowheader">[!UICONTROL Conexão]</td>
              <td>Para obter instruções sobre como conectar sua conta do [!DNL Workday] ao [!DNL Workfront Fusion], consulte <a href="#Connect" class="MCXref xref" >Conectar [!DNL Workday] ao [!DNL Workfront Fusion]</a></td>
          </tr>
          <tr>
              <td  role="rowheader">[!UICONTROL Tipo de Registro]</td>
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
