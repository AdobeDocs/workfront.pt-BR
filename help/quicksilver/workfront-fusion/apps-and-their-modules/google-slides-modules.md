---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: conector
navigation-topic: apps-and-their-modules
title: Módulos de slides Google
description: Os módulos Google Slides do Adobe Workfront Fusion permitem criar, atualizar, listar e/ou excluir apresentações e fazer upload de imagens para apresentações em sua conta Google Slides.
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: 680a5328-1d50-4434-beda-7a4670a6e458
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1575'
ht-degree: 0%

---

# [!DNL Google Slides] módulos

O [!DNL Adobe Workfront Fusion] [!DNL Google Slides] os módulos permitem criar, atualizar, listar e/ou excluir apresentações e fazer upload de imagens para apresentações em seu [!DNL Google Slides] conta.

Para usar [!DNL Google Slides] com [!DNL Workfront Fusion], é necessário ter um [!DNL Google] conta. Se você não tiver um [!DNL Google] ainda assim, você pode criar uma no [!DNL Google] Página de ajuda da conta.

Também é necessário [!DNL Google Slides] em seu [!DNL Google Drive].

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

Para usar [!DNL Google Slides] módulos, você deve ter um [!DNL Google] conta.

## [!DNL Google Slides] módulos e seus campos

Ao configurar [!DNL Google Slides] , o Workfront Fusion exibe os campos listados abaixo. Junto com esses, [!DNL Google Slides] podem ser exibidos, dependendo de fatores como seu nível de acesso no aplicativo ou serviço. Um título em negrito em um módulo indica um campo obrigatório.

Se o botão de mapa for exibido acima de um campo ou função, é possível usá-lo para definir variáveis e funções para esse campo. Para obter mais informações, consulte [Mapear informações de um módulo para outro no [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Apresentação](#presentation)
* [Outro](#other)

### Apresentação

* [[!UICONTROL Assista ao Presentations]](#watch-presentations)
* [[!UICONTROL Listar Presentations]](#list-presentations)
* [[!UICONTROL Obter uma apresentação]](#get-a-presentation)
* [[!UICONTROL Obter uma página/miniatura]](#get-a-pagethumbnail)
* [[!UICONTROL Criar uma apresentação a partir de um modelo]](#create-a-presentation-from-a-template)
* [[!UICONTROL Carregar uma imagem em uma apresentação]](#upload-an-image-to-a-presentation)
* [[!UICONTROL Atualizar um Gráfico]](#refresh-a-chart)
* [[!UICONTROL Adicionar/excluir um slide]](#adddelete-a-slide)

#### [!UICONTROL Assista ao Presentations]

Aciona quando uma nova apresentação é criada ou atualizada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Google Slides] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Watch] </td> 
   <td> <p>Selecione a opção para assistir às apresentações:</p> 
    <ul> 
     <li> <p>[!UICONTROL Data de criação]</p> </li> 
     <li> <p>[!UICONTROL Data de modificação]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limite]</td> 
   <td> <p>O número máximo de apresentações que o Workfront Fusion deve retornar durante um ciclo de execução de cenário.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Listar Presentations]

Recupera uma lista de todas as apresentações.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Google Slides] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Escolher um local de unidade]</td> 
   <td> <p>Selecione o [!DNL Google Drive] onde as apresentações que deseja listar estão localizadas:</p> 
    <ul> 
     <li>[!UICONTROL Minha unidade]</li> 
     <li>[!UICONTROL Compartilhado Comigo]</li> 
     <li>[!UICONTROL [!DNL Google] Unidade compartilhada]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID da pasta]</td> 
   <td> <p>Escolha o local da pasta das apresentações que deseja listar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limite]</td> 
   <td> <p>O número máximo de apresentações [!DNL Workfront Fusion] deve retornar durante um ciclo de execução de cenário.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obter uma apresentação]

Obtém a versão mais recente de uma apresentação especificada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Google Slides] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Escolher uma unidade]</td> 
   <td> <p>Selecione o [!DNL Google Drive] onde as apresentações que deseja listar estão localizadas:</p> 
    <ul> 
     <li>[!UICONTROL Minha unidade]</li> 
     <li>[!UICONTROL Compartilhado Comigo]</li> 
     <li>[!UICONTROL [!DNL Google] Unidade compartilhada]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID da apresentação]</td> 
   <td> <p> Selecione a apresentação que deseja recuperar.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obter uma página/miniatura]

Obtém a versão mais recente da página especificada ou da miniatura de uma página na apresentação.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Google Slides] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID da apresentação]</td> 
   <td> <p> Selecione a ID da apresentação que você deseja recuperar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID do objeto da página]</td> 
   <td> <p> Selecione o slide para o qual deseja exibir os detalhes do objeto da página.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Mostrar miniatura da página]</td> 
   <td> <p> Marque a caixa de seleção se desejar visualizar as informações de miniatura da página.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Criar uma apresentação a partir de um modelo]

Cria uma nova apresentação, substituindo todas as tags como `{{Name}}`, `{{Email}}` em um modelo com dados fornecidos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Google Slides] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Título] </td> 
   <td> <p>Insira um nome para a nova apresentação.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Copiar uma apresentação]</td> 
   <td> <p> Selecione a opção se estiver copiando uma apresentação existente:</p> 
    <ul> 
     <li>[!UICONTROL por mapeamento]</li> 
     <li>[!UICONTROL por lista suspensa]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cópia da ID de apresentação existente]</td> 
   <td> <p> Insira o Caminho ou a ID de apresentação de uma apresentação existente que você deseja copiar. Este campo será exibido se você estiver criando a apresentação [!UICONTROL By Mapping].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Escolher uma unidade]</td> 
   <td> <p>Selecione o [!DNL Google Drive] onde as apresentações que deseja listar estão localizadas:</p> 
    <ul> 
     <li>[!UICONTROL Minha unidade]</li> 
     <li>[!UICONTROL Compartilhado Comigo]</li> 
     <li>[!UICONTROL [!DNL Google] Unidade compartilhada]</li> 
    </ul> <p>Este campo será exibido se você estiver criando a apresentação [!UICONTROL por lista suspensa].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID da apresentação]</td> 
   <td> <p> Selecione a ID de apresentação da apresentação que deseja usar como modelo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Valores] </td> 
   <td> <p>Adicione os valores:</p> 
    <ul> 
     <li><strong>[!UICONTROL Tag]</strong>: Insira a tag que você deseja substituir na apresentação. Por exemplo, <code>&#123;&#123;Name&#125;&#125;</code></li> 
     <li><strong>[!UICONTROL Valor substituído]</strong>: Insira o valor com o qual a tag existente deve ser substituída. Por exemplo, se uma string <code>&#123;&#123;Name}}</code><code>Sample</code></li></ul></td></tr><tr><td role="rowheader"></td><td><p></p><ul><li></li><li></li><li></li></ul></td></tr><tr><td role="rowheader"><p></p></td><td><p></p></td></tr><tr><td role="rowheader"></td><td><p></p></td></tr><tr><td role="rowheader"></td><td><p></p></td></tr></tbody></table>

#### [!UICONTROL Carregar uma imagem em uma apresentação]

Carrega uma imagem com os dados fornecidos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Google Slides] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Escolher uma apresentação]</td> 
   <td> <p>Escolha como deseja selecionar a apresentação para a qual você está carregando uma imagem.</p> 
    <ul> 
     <li>[!UICONTROL por mapeamento]</li> 
     <li>[!DNL By Dropdown]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Escolher uma unidade]</td> 
   <td> <p>Selecione o [!DNL Google Drive] onde as apresentações que deseja listar estão localizadas:</p> 
    <ul> 
     <li>[!UICONTROL Minha unidade]</li> 
     <li>[!UICONTROL Compartilhado Comigo]</li> 
     <li>[!UICONTROL [!DNL Google] Unidade compartilhada]</li> 
    </ul> <p>Este campo será exibido se você estiver criando a apresentação [!UICONTROL por lista suspensa].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID da apresentação]</td> 
   <td> <p> Selecione a ID de apresentação da apresentação para a qual você está carregando uma imagem.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Valores]</td> 
   <td> <p>Valores Adicione os valores:</p> 
    <ul> 
     <li><strong>[!UICONTROL Tag]</strong>: Insira a tag à qual você deseja adicionar o URL.</li> 
     <li><strong>[!UICONTROL Image URL]</strong>: Insira o caminho ou URL para a imagem que você deseja fazer upload.</li> 
    </ul> <p>Observação: As imagens devem ter menos de 50 MB, não podem exceder 25 megapixels e devem estar no formato PNG, JPEG ou GIF.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Atualizar um Gráfico]

Atualiza os dados do gráfico armazenados em uma apresentação especificada pela ID.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Google Slides] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Escolher uma unidade]</td> 
   <td> <p>Selecione o [!DNL Google Drive] onde as apresentações que deseja listar estão localizadas:</p> 
    <ul> 
     <li>[!UICONTROL Minha unidade]</li> 
     <li>[!UICONTROL Compartilhado Comigo]</li> 
     <li>[!UICONTROL [!DNL Google] Unidade compartilhada]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID da apresentação]</td> 
   <td> <p>Selecione a ID de apresentação da apresentação que inclui o gráfico que você deseja atualizar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID do objeto do gráfico]</td> 
   <td> <p> Selecione o Gráfico que deseja atualizar.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Adicionar/excluir um slide]

Cria um slide vazio ou exclui um slide existente na apresentação especificada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Google Slides] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Selecionar o método]</td> 
   <td> <p>Escolha se deseja adicionar um novo slide ou excluir um slide.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Presentation ID]</td> 
   <td> <p>Selecione a ID de apresentação da apresentação para a qual deseja adicionar ou excluir um slide.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de layout predefinido]</td> 
   <td> <p> Selecione o layout de slide predefinido que deseja que o slide adicionado use. Especifique valores para qualquer campo adicional (como [!UICONTROL Título]).</p> 
    <ul> 
     <li>[!UICONTROL Layout em branco, sem espaços reservados]</li> 
     <li>[!UICONTROL Layout com uma legenda na parte inferior]</li> 
     <li>[!UICONTROL Layout com um título e subtítulo]</li> 
     <li>[!UICONTROL Layout com um título e um corpo]</li> 
     <li>[!UICONTROL Layout com um título e duas colunas]</li> 
     <li>[!UICONTROL Layout com apenas um título]</li> 
     <li>[!UICONTROL Layout com um título de seção]</li> 
     <li>[!UICONTROL Layout com um título e subtítulo em um lado e descrição no outro]</li> 
     <li>[!UICONTROL Layout com um título e um corpo, organizados em uma única coluna]</li> 
     <li>[!UICONTROL Layout com um ponto principal]</li> 
     <li>[!DNL Layout with a big number heading]</li> 
    </ul> <p>Este campo estará disponível se você tiver selecionado para adicionar um slide.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Outro

* [[!UICONTROL Faça uma chamada de API]](#make-an-api-call)
* [[!UICONTROL Inserir links em uma apresentação]](#insert-links-in-a-presentation)

#### [!UICONTROL Faça uma chamada de API]

Executa uma chamada de API autorizada arbitrária.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Google Slides] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td> <p>Insira um caminho relativo a https://developers.google.com/slides/. Por exemplo, Apresentação.</p> <p>Para obter a lista de endpoints disponíveis, consulte <a href="https://developers.google.com/slides/reference/rest">[!DNL Google Slides] Documentação da API</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Método]</td> 
   <td> <p>Selecione o método de solicitação HTTP que você precisa configurar a chamada da API. Para obter mais informações, consulte <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">Métodos de solicitação HTTP em [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cabeçalhos]</td> 
   <td> <p>Insira os cabeçalhos da solicitação desejada. Você não precisa adicionar cabeçalhos de autorização.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sequência de consulta]</td> 
   <td> <p> Insira a sequência de consulta da solicitação.</p> </td> 
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

>[!INFO]
>
>**Exemplo:** Usando uma chamada de API, você pode obter os detalhes da apresentação da ID de apresentação inserida. Você pode encontrar a ID da apresentação no URL quando abrir a apresentação no [!DNL Google Slides].
>
>![](assets/api-call-350x13.png)
>
>A chamada de API a seguir retorna os detalhes da apresentação:
>
>![](assets/presentation-details.png)
>
>As correspondências da pesquisa podem ser encontradas na Saída do módulo em [!UICONTROL Pacote] > [!UICONTROL Corpo] > [!UICONTROL presentationId].
>
>No nosso exemplo, os detalhes de apresentação solicitados foram retornados:
>
>![](assets/presentation-details-2.png)

#### [!UICONTROL Inserir links em uma apresentação]

Esse módulo torna todos os links em uma apresentação clicáveis ou insere um link em todos os textos de entrada correspondentes.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Google Slides] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Escolher uma apresentação]</td> 
   <td> <p>Escolha como deseja selecionar a apresentação para a qual você está carregando uma imagem.</p> 
    <ul> 
     <li>[!UICONTROL por mapeamento]</li> 
     <li>[!UICONTROL por lista suspensa]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Escolher uma unidade]</td> 
   <td> <p>Selecione o [!DNL Google Drive] onde as apresentações que deseja listar estão localizadas:</p> 
    <ul> 
     <li>[!UICONTROL Minha unidade]</li> 
     <li>[!UICONTROL Compartilhado Comigo]</li> 
     <li>[!UICONTROL [!DNL Google] Unidade compartilhada]</li> 
    </ul> <p>Este campo será exibido se você estiver criando a apresentação [!UICONTROL por lista suspensa].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID da apresentação]</td> 
   <td> <p>Escolha o local da pasta das apresentações que deseja listar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Selecionar]</td> 
   <td> <p>Selecione se deseja tornar todos os links em uma apresentação clicáveis ou se deseja inserir um link em todos os textos de entrada correspondentes.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Entrada de texto]</td> 
   <td>Para cada item de texto para o qual você deseja adicionar um link, adicione o item e o link associado à lista. Toda vez que o item aparece na apresentação, ele é vinculado automaticamente ao site especificado.</td> 
  </tr> 
 </tbody> 
</table>
