---
filename: aem-assets-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: conector
navigation-topic: apps-and-their-modules
title: Módulos do Adobe Experience Manager Assets
description: Com o [!DNL Adobe Experience Manager Assets] conector para [!DNL Adobe Workfront Fusion], you can start a scenario based on events in your [!DNL Adobe Experience Manager Assets] criar, carregar e atualizar ativos e copiar ou mover pastas e ativos.
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: 0749f230-8cab-464f-863c-9cb4870125d1
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1496'
ht-degree: 0%

---

# [!DNL Adobe Experience Manager Assets] módulos

Com o [!DNL Adobe Experience Manager Assets] conector para [!DNL Adobe Workfront Fusion], você pode iniciar um cenário com base nos eventos em [!DNL Adobe Experience Manager Assets] criar, carregar e atualizar ativos e copiar ou mover pastas e ativos.

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

* Você deve ter um [!DNL Adobe Experience Manager Assets] para usar esses módulos.
* Você deve configurar [!UICONTROL Servidor para servidor] fluxo no [!DNL Adobe Developer console].

   Para obter instruções sobre como configurar [!UICONTROL Servidor para servidor] fluxo no [!DNL Adobe Developer console], consulte [Gerar tokens de acesso para APIs do lado do servidor](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/implementing/developing/generating-access-tokens-for-server-side-apis.html#the-server-to-server-flow).

## Connect [!DNL Adobe Experience Manager Assets] para [!DNL Workfront Fusion] {#connect-adobe-experience-manager-assets-to-workfront-fusion}

Para criar uma conexão para [!DNL Adobe Experience Manager Assets] módulos:

1. Clique em [!UICONTROL Adicionar] ao lado do [!UICONTROL Conexão] caixa.

2. Selecione o tipo de conexão que você está criando:

   * **[!DNL AEM Assets as a Cloud Service]**

      Essa configuração requer informações do [!DNL Adobe Admin Console].

   * **[!DNL AEM Assets Basic]**

      Essa configuração requer um nome de usuário e senha.

3. Preencha os campos do tipo de conexão que você está criando.

   Para [!DNL AEM Assets as a Cloud Service], consulte [Configure a conexão para [!DNL AEM Assets as a Cloud Service]](#configure-the-connection-for-aem-assets-as-a-cloud-service).

   Para [!UICONTROL AEM Assets Basic], consulte [Configure a conexão para [!UICONTROL AEM Assets Basic]](#configure-the-connection-for-aem-assets-basic).

4. Clique em **[!UICONTROL Continuar]** para salvar a conexão e retornar ao módulo.


### Configure a conexão para [!DNL AEM Assets as a Cloud Service]

>[!NOTE]
>
>As informações desses campos são geradas como parte da configuração do [!UICONTROL Servidor para servidor] fluxo no [!DNL Adobe Developer Console]. Você pode encontrar esses valores no arquivo JSON de credenciais de serviço gerado como parte dessa configuração.
>
>Para obter instruções sobre como configurar [!UICONTROL Servidor para servidor] fluxo no [!UICONTROL Console do Adobe Developer], consulte [Gerar tokens de acesso para APIs do lado do servidor](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/implementing/developing/generating-access-tokens-for-server-side-apis.html#the-server-to-server-flow).


<table style="table-layout:auto"> 
          <col/>
          <col/>
          <tbody>
              <tr>
                  <td role="rowheader">[!UICONTROL Nome da conexão]</td>
                  <td>
                      <p>Introduza um nome para esta ligação</p>
                  </td>
              </tr>
              <tr>
                  <td role="rowheader">[!UICONTROL URL da instância sem uma barra à direita]</td>
                  <td>Insira o URL do [!DNL Adobe Experience Manager] instância. Não inclua uma barra <code>/</code> no final do URL.</td>
              </tr>
              <tr>
                  <td role="rowheader">[!UICONTROL Client ID]</td>
                  <td>Insira a ID do cliente gerada na configuração do [!UICONTROL Server-to-server].</td>
              </tr>
              <tr>
                  <td role="rowheader">[!UICONTROL Segredo do cliente]</td>
                  <td>Insira o Segredo do cliente gerado na configuração do [!UICONTROL Server-to-server].</td>
              </tr>
              <tr>
                  <td role="rowheader">[!UICONTROL ID da conta técnica]</td>
                  <td>Insira a ID da conta técnica. Este é o campo "[!UICONTROL id]" no arquivo JSON de credenciais do cliente.</td>
              </tr>
              <tr>
                  <td role="rowheader">[!UICONTROL ID da organização]</td>
                  <td class="">Insira a ID da organização. Este é o campo "[!UICONTROL org]" no arquivo JSON de credenciais do cliente.</td>
              </tr>
              <tr>
                  <td role="rowheader">[!UICONTROL Metscópios]</td>
                  <td>Insira os metadados gerados na configuração do [!UICONTROL Server-to-server].</td>
              </tr>
              <tr>
                  <td role="rowheader">[!UICONTROL Chave privada]</td>
                  <td>Insira a Chave privada gerada na configuração do [!UICONTROL Server-to-server]. Para extrair a chave privada, clique em [!UICONTROL Extrair] e insira o arquivo a ser extraído e a senha do arquivo.</td>
              </tr>
          </tbody>
      </table>


### Configure a conexão para [!DNL AEM Assets Basic]

<table style="table-layout:auto"> 
        <col/>
        <col />
        <tbody>
            <tr>
                <td role="rowheader">[!UICONTROL Nome da conexão]</td>
                <td>
                    <p>Introduza um nome para esta ligação</p>
                </td>
            </tr>
            <tr>
                <td role="rowheader">[!UICONTROL URL da instância sem uma barra à direita]</td>
                <td>Insira o URL do seu [!DNL Adobe Experience Manager] instância. Não inclua uma barra <code>/</code> no final do URL.</td>
            </tr>
            <tr>
                <td role="rowheader">[!UICONTROL Nome de usuário]</td>
                <td>Insira o nome de usuário para o [!DNL AEM Assets] conta que esta conexão usa.</td>
            </tr>
            <tr>
                <td role="rowheader">[!UICONTROL Senha]</td>
                <td>Digite a senha do [!DNL AEM Assets] conta que esta conexão usa.</td>
            </tr>
        </tbody>
    </table>


## [!DNL Adobe Experience Manager Assets] módulos e seus campos

Ao configurar [!DNL Adobe Experience Manager Essentials] módulos, [!DNL Workfront Fusion] exibe os campos listados abaixo. Junto com esses, [!DNL Adobe Experience Manager Essentials] podem ser exibidos, dependendo de fatores como seu nível de acesso no aplicativo ou serviço. Um título em negrito em um módulo indica um campo obrigatório.

Se o botão de mapa for exibido acima de um campo ou função, é possível usá-lo para definir variáveis e funções para esse campo. Para obter mais informações, consulte [Mapear informações de um módulo para outro no [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### [!UICONTROL Copiar uma pasta ou um ativo]

Esse módulo de ação copia uma pasta ou ativo para outro local na conta do Adobe Experience Manager Assets.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Adobe Experience Manager Assets] para [!DNL Workfront Fusion], consulte <a href="#connect-adobe-experience-manager-assets-to-workfront-fusion" class="MCXref xref">Connect [!DNL Adobe Experience Manager Assets] para [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de registro]</td> 
   <td> <p>Selecione se deseja copiar uma pasta ou um ativo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Pasta] / [!UICONTROL Seleção de ativos]</td> 
   <td>Selecione ou mapeie a pasta ou ativo que deseja copiar.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Caminho de destino]</td> 
   <td>Selecione ou mapeie o caminho para o local da nova pasta ou ativo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nome da pasta copiada] / [!UICONTROL ativo]</td> 
   <td>Insira um nome para a nova pasta ou ativo. O nome da pasta que é exibida em [!DNL Adobe Experience Manager Assets] é igual ao nome original. O nome inserido aqui aparece no URL da nova pasta ou ativo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Copiar filhos]</td> 
   <td>Ative essa opção para copiar qualquer subpasta ou ativo dentro da pasta.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Substituir]</td> 
   <td>Ative essa opção para substituir qualquer pasta ou ativo no local de destino que tenha o mesmo nome da pasta ou ativo que está sendo copiado.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Criar um registro]

Esse módulo de ação cria uma pasta ou um comentário de ativo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Adobe Experience Manager Assets] para [!DNL Workfront Fusion], consulte <a href="#connect-adobe-experience-manager-assets-to-workfront-fusion" class="MCXref xref">Connect [!DNL Adobe Experience Manager Assets] para [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de objeto]</td> 
   <td> <p>Selecione se deseja criar uma pasta ou um comentário em um ativo.</p> 
    <ul> 
     <li> <p>[!UICONTROL Pasta]</p> <p>Preencha os seguintes campos:</p> 
      <ul> 
       <li> <p>[!UICONTROL Name]</p> <p>Insira um nome para a pasta. Esse nome aparecerá no caminho do arquivo, portanto, não deve incluir espaços ou outros caracteres. </p> </li> 
       <li> <p>[!UICONTROL Título]</p> <p>Insira um título para a pasta, que pode ser exibida em vez do nome.</p> </li> 
      </ul> </li> 
     <li> <p>[!UICONTROL Comentário do ativo]</p> <p>Preencha os seguintes campos:</p> 
      <ul> 
       <li> <p>[!UICONTROL Seleção de ativos]</p> <p>Selecione ou mapeie a ID do ativo ao qual deseja adicionar um comentário.</p> </li> 
       <li> <p>[!UICONTROL Comentário]</p> <p>Insira o texto do comentário.</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Excluir um registro]

Esse módulo de ação exclui uma pasta, ativo ou representação.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Adobe Experience Manager Assets] para [!DNL Workfront Fusion], consulte <a href="#connect-adobe-experience-manager-assets-to-workfront-fusion" class="MCXref xref">Connect [!DNL Adobe Experience Manager Assets] para [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de registro]</td> 
   <td> <p>Selecione se deseja excluir uma pasta, ativo ou representação.</p> 
    <ul> 
     <li> <p>[!UICONTROL Pasta]</p> <p>Selecione a pasta a ser excluída selecionando as pastas em seu caminho.</p> </li> 
     <li> <p>[!UICONTROL Asset] </p> <p>Selecione o ativo selecionando as pastas em seu caminho e, em seguida, o ativo que deseja excluir.</p> </li> 
     <li> <p>[!UICONTROL Representação]</p> <p>Selecione a representação selecionando as pastas em seu caminho.</p> <p>Insira ou mapeie o nome da representação.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Obter uma lista de pastas]

Esse módulo de ação recupera uma representação de uma pasta existente e de suas entidades filhas (pastas ou ativos).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Adobe Experience Manager Assets] para [!DNL Workfront Fusion], consulte <a href="#connect-adobe-experience-manager-assets-to-workfront-fusion" class="MCXref xref">Connect [!DNL Adobe Experience Manager Assets] para [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Pasta]</td> 
   <td>Selecione ou mapeie a pasta que deseja recuperar. Para adicionar subpastas ao caminho, clique no ícone de adição e selecione a subpasta.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Efetuar uma chamada de API personalizada]

Esse módulo de ação faz uma chamada de API personalizada para a [!DNL Adobe Experience Manager Assets] API.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Adobe Experience Manager Assets] para [!DNL Workfront Fusion], consulte <a href="#connect-adobe-experience-manager-assets-to-workfront-fusion" class="MCXref xref">Connect [!DNL Adobe Experience Manager Assets] para [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL URL]</p> </td> 
   <td> <p>Insira um caminho relativo ao [!DNL Adobe Experience Manager] URL base.</p> </td> 
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
   <td> <p>Insira a sequência de consulta da solicitação. Para cada par de chave/valor, clique em <b>[!UICONTROL Adicionar item]</b> e insira a [!UICONTROL Chave] e o [!UICONTROL Valor].</p> </td> 
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

### [!UICONTROL Mover uma pasta ou um ativo]

Esse módulo de ação move o ativo ou a pasta no caminho especificado para um novo local.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Adobe Experience Manager Assets] para [!DNL Workfront Fusion], consulte <a href="#connect-adobe-experience-manager-assets-to-workfront-fusion" class="MCXref xref">Connect [!DNL Adobe Experience Manager Assets] para [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de registro]</td> 
   <td> <p>Selecione se deseja mover uma pasta ou um ativo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Pasta] / [!UICONTROL Ativo]</td> 
   <td>Selecione ou mapeie a pasta ou ativo que deseja mover.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Caminho de destino]</td> 
   <td>Selecione ou mapeie o caminho para o local onde deseja mover a pasta ou o ativo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nome da pasta movida] / [!UICONTROL ativo]</td> 
   <td>Insira um novo nome para a pasta ou ativo movido. O nome da pasta que é exibida em [!DNL Adobe Experience Manager Assets] é igual ao nome original. O nome inserido aqui aparece no URL da pasta ou ativo movido.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Substituir]</td> 
   <td>Ative essa opção para substituir qualquer pasta ou ativo no local de destino que tenha o mesmo nome da pasta ou ativo que está sendo copiado.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Atualizar um registro]

Este módulo de ação atualiza um registro existente.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Adobe Experience Manager Assets] para [!DNL Workfront Fusion], consulte <a href="#connect-adobe-experience-manager-assets-to-workfront-fusion" class="MCXref xref">Connect [!DNL Adobe Experience Manager Assets] para [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de registro]</td> 
   <td> <p>Selecione se deseja excluir metadados de ativos ou uma representação de ativos.</p> 
    <ul> 
     <li> <p>[!UICONTROL Metadados do ativo]</p> 
      <ul> 
       <li> <p>Selecione o ativo para o qual deseja atualizar os metadados.</p> </li> 
       <li> <p>Informe o novo título do ativo.</p> </li> 
      </ul> </li> 
     <li> <p>[!UICONTROL Representação de ativos]</p> 
      <ul> 
       <li> <p>Selecione o ativo para o qual deseja atualizar a representação.</p> </li> 
       <li> <p>Selecione um arquivo de origem de um módulo anterior ou mapeie o nome e os dados do arquivo de origem.</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Fazer upload de um ativo]

Este módulo de ação carrega um ativo no seu [!DNL Adobe Experience Manager Assets] conta.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Adobe Experience Manager Assets] para [!DNL Workfront Fusion], consulte <a href="#connect-adobe-experience-manager-assets-to-workfront-fusion" class="MCXref xref">Connect [!DNL Adobe Experience Manager Assets] para [!DNL Workfront Fusion]</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Destino]</td> 
   <td> <p>Selecione a pasta onde deseja fazer upload de um ativo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Arquivo de origem]</td> 
   <td>Insira ou mapeie o nome e os dados do arquivo de origem.</td> 
  </tr> 
 </tbody> 
</table>
