---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: conector
navigation-topic: apps-and-their-modules
title: Módulos Anaplan
description: Em um [!DNL Adobe Workfront Fusion] você pode automatizar fluxos de trabalho que usam o Anaplan, bem como conectá-lo a vários aplicativos e serviços de terceiros.
author: Becky
feature: Workfront Fusion, Workfront Integrations and Apps
exl-id: 03bcd0a4-c8ec-4f44-b1e1-b57e79595309
source-git-commit: 43b64d1371438909063d2ac81cccb90b97179dfc
workflow-type: tm+mt
source-wordcount: '1796'
ht-degree: 1%

---

# [!DNL Anaplan] Módulos

Em um [!DNL Adobe Workfront Fusion] , é possível automatizar workflows que usam [!DNL Anaplan], bem como conectá-lo a vários aplicativos e serviços de terceiros.

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

Antes de usar a variável [!DNL Anaplan] , você deve garantir que os seguintes pré-requisitos sejam atendidos:

* Você deve ter um [!UICONTROL Anaplan] conta.
* Você deve configurar Espaços de trabalho, Modelos e outros [!DNL Anaplan] objetos em [!UICONTROL Anaplan] account before [!DNL Workfront Fusion] podem interagir com eles.

## Connect [!DNL Anaplan] para [!DNL Workfront Fusion] {#connect-anaplan-to-workfront-fusion}

Para criar uma conexão para [!DNL Anaplan] módulos:

1. Clique em **[!UICONTROL Adicionar]** ao lado do [!UICONTROL Conexão] caixa.
1. Selecione o tipo de conexão.

   <table style="table-layout:auto">
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!DNL Anaplan] [!UICONTROL Básico]</td> 
      <td> <p>Um [!DNL Anaplan] A conexão [!UICONTROL Básica] requer apenas um endereço de email e senha para criar a conexão. </p> <p>Digite um nome para a conexão e, em seguida, insira seu endereço de email e a senha de seu [!DNL Anaplan] conta.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!DNL Anaplan] [!UICONTROL CA Certificate]</td> 
      <td> <p>Um [!DNL Anaplan] A conexão [!UICONTROL CA Certificate] requer uma [!UICONTROL Certificate Key], [!UICONTROL Encoded Data] e [!UICONTROL Encoded Data]. Você pode gerá-los em [!DNL Anaplan] conta. Para obter instruções, consulte o [!DNL Anaplan] documentação.</p> <p>Insira um nome para a conexão e depois insira a [!UICONTROL Chave do certificado], os [!UICONTROL Dados codificados] e os [!UICONTROL Dados codificados] que você gerou nos [!DNL Anaplan] conta.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Clique em **[!UICONTROL Continuar]** para salvar a conexão e retornar ao módulo.

## [!DNL Anaplan] módulos e seus campos

Ao configurar [!DNL Anaplan] módulos, [!DNL Workfront Fusion] exibe os campos listados abaixo. Junto com esses, [!DNL Anaplan] podem ser exibidos, dependendo de fatores como seu nível de acesso no aplicativo ou serviço. Um título em negrito em um módulo indica um campo obrigatório.

Se o botão de mapa for exibido acima de um campo ou função, é possível usá-lo para definir variáveis e funções para esse campo. Para obter mais informações, consulte [Mapear informações de um módulo para outro no [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Triggers](#triggers)
* [Ações](#actions)
* [Pesquisas](#searches)

### Triggers

#### [!DNL Watch records]

Este módulo de acionador inicia um cenário quando um registro do tipo escolhido é criado ou atualizado.

>[!NOTE]
>
>Esse módulo retorna os dados de novos registros. Ele não retorna os dados de registros existentes modificados.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Para obter instruções sobre como criar uma conexão com o [!DNL Anaplan], consulte <a href="#connect-anaplan-to-workfront-fusion" class="MCXref xref">Connect [!DNL Anaplan] para [!DNL Workfront Fusion]</a> neste artigo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Tipo de objeto a ser observado</td> 
   <td>Selecione o tipo de item que deseja observar. O cenário começa quando esse tipo de registro é criado ou atualizado.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">&lt;object&gt; ID</td> 
   <td>Insira a ID do objeto em Anaplan, como um Modelo ou Módulo, que está associada aos objetos que você deseja assistir</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Limite</td> 
   <td> <p>Insira ou mapeie o número máximo de registros para o módulo [action] durante cada ciclo de execução de cenário.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Ações

* [[!UICONTROL Criar um item de lista]](#create-a-list-item)
* [[!UICONTROL Faça uma chamada de API personalizada]](#make-a-custom-api-call)
* [[!UICONTROL Ler um registro]](#read-a-record)
* [[!UICONTROL Executar uma ação]](#run-an-action)
* [[!UICONTROL Atualizar um registro]](#update-a-record)
* [[!UICONTROL Carregar um arquivo]](#upload-a-file)

#### [!UICONTROL Criar um item de lista]

Este módulo de ação adiciona um novo item a uma lista em Anaplan.

<table style="table-layout:auto">
    <tr>
        <td>[!UICONTROL Connection]</td>
        <td>Para obter instruções sobre como criar uma conexão com o [!DNL Anaplan], consulte <a href="#connect-anaplan-to-workfront-fusion" class="MCXref xref">Connect [!DNL Anaplan] para [!DNL Workfront Fusion]</a> neste artigo.</td>
    </tr>
    <tr>
        <td>[!UICONTROL ID da Workspace]</td>
        <td>Selecione ou mapeie a ID do Espaço de trabalho de Anaplan que contém a lista onde deseja adicionar um item.</td>
    </tr>
    <tr>
        <td>[!UICONTROL ID do modelo]</td>
        <td>Selecione ou mapeie a ID do Modelo que contém a lista onde deseja adicionar um item.</td>
    </tr>
    <tr>
        <td>[!UICONTROL List ID]</td>
        <td>Selecione ou mapeie a ID da Lista onde deseja criar um item.</td>
    </tr>
    <tr>
        <td>[!UICONTROL Name]</td>
        <td>Insira um nome para o novo item.</td>
    </tr>
    <tr>
        <td>[!UICONTROL Código]</td>
        <td>Insira o código para o novo item. Os códigos são códigos gerados pelo usuário que permitem distinguir entre itens de linha com o mesmo nome.</td>
    </tr>
    <tr>
        <td>[!UICONTROL Pai]</td>
        <td>Insira o nome do item pai no qual você deseja criar o novo item.</td>
    </tr>
    <tr>
        <td>[!UICONTROL Propriedades]</td>
        <td>Se a lista que você deseja adicionar um item tiver propriedades personalizadas, selecione as propriedades para as quais deseja adicionar valores e adicione os valores.</td>
    </tr>
    <tr>
        <td>[!UICONTROL Subconjuntos]</td>
        <td>Se a lista que deseja adicionar itens tiver subconjuntos personalizados, selecione os subconjuntos aos quais deseja adicionar o item e selecione <b>[!UICONTROL Sim]</b> para adicionar o novo item a esse subconjunto.</td>
    </tr>
</table>

#### [!UICONTROL Faça uma chamada de API personalizada]

Esse módulo permite que você execute uma chamada de API personalizada para o [!DNL Anaplan] API.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Para obter instruções sobre como criar uma conexão com o [!DNL Anaplan], consulte <a href="#connect-anaplan-to-workfront-fusion" class="MCXref xref">Connect [!DNL Anaplan] para [!DNL Workfront Fusion]</a> neste artigo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL URL]</p> </td> 
   <td> <p>Insira um caminho relativo a <code>https://api.anaplan.com/2/0/</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Método]</p> </td> 
   <td> <p>Selecione o método de solicitação HTTP que você precisa configurar a chamada da API. Para obter mais informações, consulte <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">Métodos de solicitação HTTP em [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cabeçalhos]</td> 
   <td> <p>Adicione os cabeçalhos da solicitação no formato de um objeto JSON padrão.</p> <p>Por exemplo, <code>{"Content-type":"application/json"}</code></p> <p>[!DNL Workfront Fusion] adiciona cabeçalhos de autorização automaticamente.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sequência de consulta] </td> 
   <td> <p>Insira a sequência de consulta da solicitação.</p> </td> 
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

#### [!UICONTROL Excluir um registro]

Esse módulo de ação exclui um registro existente.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Para obter instruções sobre como criar uma conexão com o [!DNL Anaplan], consulte <a href="#connect-anaplan-to-workfront-fusion" class="MCXref xref">Connect [!DNL Anaplan] para [!DNL Workfront Fusion]</a> neste artigo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID da Workspace]</td> 
   <td>Selecione ou mapeie a ID do Espaço de trabalho de Anaplan que contém o objeto que deseja excluir.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID do modelo]</td> 
   <td>Insira ou mapeie a ID do Modelo que contém o objeto que você deseja excluir.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Excluir</td> 
   <td> <p>Selecione o tipo de objeto a ser excluído.</p> 
    <ul> 
     <li> <p><b>Ação</b> </p> <p>Selecione ou mapeie a ação a ser excluída.</p> </li> 
     <li> <p><b>Item de lista</b> </p> <p>Selecione a lista da qual deseja excluir um item e, em seguida, insira ou mapeie a ID ou o código do item que deseja excluir</p>  </li> 
     <li> <p><b>[!UICONTROL Arquivo]</b> </p> <p>Selecione ou mapeie o arquivo a ser excluído.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Ler um registro]

Este módulo de ação lê um único registro.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Para obter instruções sobre como criar uma conexão com o [!DNL Anaplan], consulte <a href="#connect-anaplan-to-workfront-fusion" class="MCXref xref">Connect [!DNL Anaplan] para [!DNL Workfront Fusion]</a> neste artigo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de registro]</td> 
   <td> <p>Selecione o tipo de registro a ser lido.</p> 
    <ul> 
     <li> <p><b>Modelo</b> </p> <p>Selecione ou mapeie a ID do Modelo que deseja ler</p> </li> 
     <li> <p><b>Lista de modelos</b> </p> <p>Selecione ou mapeie as IDs do Workspace e do Modelo que contêm a Lista que você deseja ler e selecione a Lista. No campo [!UICONTROL Data type] , selecione se deseja ler dados ou metadados.</p> </li> 
     <li> <p><b>Versão do modelo</b> </p> <p>Selecione ou mapeie a ID do Modelo que deseja ler.</p> </li> 
     <li> <p><b>Usuário</b> </p> <p>Selecione se deseja retornar dados sobre o proprietário da conta que está sendo usada ou outro usuário. Se você selecionar outro usuário, selecione o nome dele.</p> </li> 
     <li> <p><b>Workspace</b> </p> <p>Selecione ou mapeie a ID do espaço de trabalho que deseja ler.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Executar uma ação]

Esse módulo de ação importa, exporta, exclui ou processa uma ação.

<table style="table-layout:auto"> 
     <col/>
     <col/>
     <tbody>
      <tr>
        <td role="rowheader">[!UICONTROL Connection]</td>
        <td>Para obter instruções sobre como criar uma conexão com o [!DNL Anaplan], consulte <a href="#Connect" class="MCXref xref" >[!UICONTROL Conectar Anaplan ao Workfront Fusion]</a> neste artigo.</td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL ID da Workspace]</td>
        <td>Selecione ou mapeie a ID do [!DNL Anaplan] Espaço de trabalho onde você deseja executar a ação</td>
      </tr>
      <tr >
        <td role="rowheader">[!UICONTROL ID do modelo]</td>
        <td>Selecione ou mapeie a ID do Modelo onde deseja executar a ação.</td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Tipo de ação]</td>
        <td>
          <p>Selecione a ação que deseja executar</p>
            <ul>
              <li>
                <p><b>[!UICONTROL Excluir]</b>
                </p>
                <p>Insira ou mapeie a ID da ação que deseja excluir.</p>
              </li>
              <li>
                <p><b>[!UICONTROL Exportar]</b>
                </p>
                <p>Insira ou mapeie a ID da definição de exportação que deseja usar. Você pode exportar para os seguintes formatos de arquivo:</p>
                  <ul>
                    <li>
                      <p>XLS</p>
                    </li>
                    <li>
                      <p>XLSX</p>
                    </li>
                    <li>
                      <p>CSV</p>
                    </li>
                  </ul>
                </li>
                <li>
                  <p><b>[!UICONTROL Importar] </b>
                  </p>
                  <p style="font-weight: normal;">Insira ou mapeie a ID da definição de importação que deseja usar.</p>
                </li>
                <li>
                 <p><b>[!UICONTROL Processo]</b>
                 </p>
                  <p>Insira ou mapeie a ID do processo que deseja usar. </p>
                </li>
              </ul>
            </td>
          </tr>
        </tbody>
      </table>


#### [!UICONTROL Atualizar um registro]

Este módulo de ação atualiza um único registro em [!UICONTROL Anaplan].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Para obter instruções sobre como criar uma conexão com o [!DNL Anaplan], consulte <a href="#connect-anaplan-to-workfront-fusion" class="MCXref xref">Connect [!DNL Anaplan] para [!DNL Workfront Fusion]</a> neste artigo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de registro]</td> 
   <td> <p>Selecione o tipo de registro que deseja atualizar.</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Item da lista]</b> </p> <p>Para campos, consulte <a href="#create-a-list-item" class="MCXref xref">Criar um item de lista</a> neste artigo.</p> </li> 
     <li> <p><b>[!UICONTROL Módulo de dados da célula]</b> </p> <p>Quando você atualiza os dados da célula, todos os cálculos de downstream que usam esses dados também são atualizados.</p> <p>Preencha os seguintes campos:</p> 
      <ul> 
       <li> <p><b>[!UICONTROL ID do modelo]</b> </p> <p>Selecione ou mapeie o Modelo que contém a célula que você deseja atualizar.</p> </li> 
       <li> <p><b>[!UICONTROL ID do módulo]</b> </p> <p>Selecione ou mapeie o Módulo que contém a célula que você deseja atualizar</p> </li> 
       <li> <p><b>[!UICONTROL Nome do item da linha]</b> </p> <p>Selecione ou mapeie o item de linha da célula que deseja atualizar</p> </li> 
       <li> <p style="font-weight: bold;">[!UICONTROL Dimension ID]</p> <p>Selecione ou mapeie a dimensão que está no item de linha.</p> 
       <p><b>Nota: </b> 
       <ul>
       <li> A chave Dimension (valor) deve ser <code>dimensionName</code> (próximo) ou <code>dimensionId</code> (ID).</li>
       <li>A chave do item (valor) deve ser <code>itemName</code> (texto), <code>itemCode</code> (texto), ou <code>itemId</code> (ID).</li>
       <li>As chaves de Dimension e de item devem ser do mesmo tipo (texto ou ID).
       </ul>
        </p> 
        <p>Para obter informações sobre dimensões, procure por Dimension no [!DNL Anaplan Anapedia].</p> </li> 
       <li> <p><b>[!UICONTROL Valor]</b> </p> <p>Insira ou mapeie o novo valor para a célula.</p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Modelo ano fiscal atual]</b> </p> <p>Insira a ID do Workspace e a ID do Modelo para o qual você deseja atualizar o ano fiscal, em seguida, insira ou mapeie o novo ano para o modelo.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Carregar um arquivo]

Este módulo de ação carrega um arquivo no Anaplan. O arquivo já deve ter sido carregado para Anaplan. Você pode usar esse módulo para carregá-lo em locais adicionais dentro do Anaplan.
<table style="table-layout:auto">
<col>
<col>
<tbody>
<tr>
<td role="rowheader">[!UICONTROL Connection]</td>
<td>Para obter instruções sobre como criar uma conexão com o [!DNL Anaplan], consulte <a href="#connect-anaplan-to-workfront-fusion" class="MCXref xref">Connect [!DNL Anaplan] para [!DNL Workfront Fusion]</a> neste artigo.</td>
</tr>
<tr>
<td role="rowheader">[!UICONTROL ID da Workspace]</td>
<td>Selecione ou mapeie a ID do [!DNL Anaplan] Espaço de trabalho onde você deseja fazer upload de um arquivo.</td>
</tr>
<tr>
<td role="rowheader">[!UICONTROL ID do modelo]</td>
<td>Selecione ou mapeie a ID do Modelo onde deseja carregar um arquivo.</td>
</tr>
<tr>
<td role="rowheader">[!UICONTROL ID do arquivo]</td>
<td>Selecione ou mapeie a ID do arquivo que deseja fazer upload.</td>
</tr>
</tbody>
</table>
</div>

### Pesquisas

#### [!UICONTROL Obter registro]

Este módulo de pesquisa retorna todos os registros acessíveis do tipo selecionado.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Para obter instruções sobre como criar uma conexão com o [!DNL Anaplan], consulte <a href="#connect-anaplan-to-workfront-fusion" class="MCXref xref">Connect [!DNL Anaplan] para [!DNL Workfront Fusion]</a> neste artigo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipos de registro]</td> 
   <td> <p>Selecione o tipo de registro que deseja recuperar.</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Workspace]</b> </p> </li> 
       <li> <p><b>[!UICONTROL Modelos]</b> </p> </li> 
       <li> <p><b>[!UICONTROL Itens de linha]</b> </p> <p>Selecione ou mapeie a ID do Modelo que contém a variável [!DNL line] itens que você deseja recuperar.</p> </li> 
       <li> <p><b>[!UICONTROL Model lists]</b> </p> <p>Selecione ou mapeie a ID do Espaço de trabalho e a ID do modelo que contém as listas de Modelo que você deseja recuperar.</p> </li> 
       <li> <p><b>[!UICONTROL Modelo de calendário]</b> </p> <p>Selecione ou mapeie a ID do espaço de trabalho que contém o calendário Modelo que você deseja recuperar.</p> </li> 
       <li> <p><b>Versões de modelo</b> </p> </li> 
       <li> <p>Selecione ou mapeie [!UICONTROL ] a ID do Modelo que contém as versões do Modelo que você deseja recuperar.</p> </li> 
       <li> <p><b>[!UICONTROL Usuários]</b> </p> </li> 
       <li> <p><b>[!UICONTROL Exibições]</b> </p> <p>Selecione se deseja escolher a exibição por Módulo ou por Modelo, em seguida, selecione ou mapeie a ID do Módulo ou Modelo que contém a exibição que você deseja recuperar.</p> </li> 
      </ul> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Retornar tamanho do espaço de trabalho]</td> 
   <td>Ative essa opção para retornar uma estimativa do tamanho atual do espaço de trabalho. Essa estimativa é baseada nos tamanhos de todos os módulos contidos no espaço de trabalho.</td> 
  </tr> 
 </tbody> 
</table>
