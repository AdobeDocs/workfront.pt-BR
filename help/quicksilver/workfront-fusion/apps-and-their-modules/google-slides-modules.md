---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: conector
navigation-topic: apps-and-their-modules
title: Módulos do Google Slides
description: Os módulos do Adobe Workfront Fusion Google Slides permitem criar, atualizar, listar e/ou excluir apresentações e fazer upload de imagens para apresentações em sua conta do Google Slides.
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: 680a5328-1d50-4434-beda-7a4670a6e458
source-git-commit: 55485da1ea650121b5537a3f19d8102623ed4f43
workflow-type: tm+mt
source-wordcount: '1638'
ht-degree: 0%

---

# [!DNL Google Slides] módulos

Os módulos do [!DNL Adobe Workfront Fusion] [!DNL Google Slides] permitem criar, atualizar, listar e/ou excluir apresentações e carregar imagens para apresentações em sua conta do [!DNL Google Slides].

Para usar [!DNL Google Slides] com [!DNL Workfront Fusion], é necessário ter uma conta [!DNL Google]. Se você ainda não tiver uma conta [!DNL Google], crie uma na página de ajuda da Conta [!DNL Google].

Você também precisa de [!DNL Google Slides] em seu [!DNL Google Drive].

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
   <p>Requisito atual do produto: se você tiver o plano [!UICONTROL Select] ou [!UICONTROL Prime] [!DNL Adobe Workfront], sua organização deve comprar [!DNL Adobe Workfront Fusion] e [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo. [!DNL Workfront Fusion] está incluído no plano [!DNL Workfront] do [!UICONTROL Ultimate].</p>
   <p>Ou</p>
   <p>Requisito de produto herdado: sua organização deve comprar o [!DNL Adobe Workfront Fusion] e o [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Para saber que plano, tipo de licença ou acesso você tem, contate o administrador do [!DNL Workfront].

Para obter informações sobre [!DNL Adobe Workfront Fusion] licenças, consulte [[!DNL Adobe Workfront Fusion] licenças](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Pré-requisitos

Para usar módulos [!DNL Google Slides], você deve ter uma conta [!DNL Google].

## Informações da API de slides do Google

O conector de slides do Google usa o seguinte:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">URL base</td> 
   <td> https://slides.googleapis.com/v1</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Versão da API</td> 
   <td> v1 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Tag da API</td> 
   <td>v1.5.9</td> 
  </tr>
 </tbody> 
 </table>

## [!DNL Google Slides] módulos e seus campos

Ao configurar módulos do [!DNL Google Slides], o Workfront Fusion exibe os campos listados abaixo. Junto com esses, campos [!DNL Google Slides] adicionais podem ser exibidos, dependendo de fatores como seu nível de acesso no aplicativo ou serviço. Um título em negrito em um módulo indica um campo obrigatório.

Se você vir o botão de mapa acima de um campo ou função, poderá usá-lo para definir variáveis e funções para esse campo. Para obter mais informações, consulte [Mapear informações de um módulo para outro em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Apresentação](#presentation)
* [Outro](#other)

### Apresentação

* [[!UICONTROL Assistir Presentations]](#watch-presentations)
* [[!UICONTROL Listar Presentations]](#list-presentations)
* [[!UICONTROL Obter uma Apresentação]](#get-a-presentation)
* [[!UICONTROL Obter uma Página/Miniatura]](#get-a-pagethumbnail)
* [[!UICONTROL Criar uma Apresentação de um Modelo]](#create-a-presentation-from-a-template)
* [[!UICONTROL Carregar uma Imagem para uma Apresentação]](#upload-an-image-to-a-presentation)
* [[!UICONTROL Atualizar um Gráfico]](#refresh-a-chart)
* [[!UICONTROL Adicionar/Excluir um Slide]](#adddelete-a-slide)

#### [!UICONTROL Assistir Presentations]

Dispara quando uma nova apresentação é criada ou atualizada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão] </td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Google Slides] ao [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o [!DNL Adobe Workfront Fusion] - Instruções básicas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Observar] </td> 
   <td> <p>Selecione a opção para assistir às apresentações:</p> 
    <ul> 
     <li> <p>[!UICONTROL Data de Criação]</p> </li> 
     <li> <p>[!UICONTROL Data de Modificação]</p> </li> 
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
   <td role="rowheader">[!UICONTROL Conexão] </td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Google Slides] ao [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o [!DNL Adobe Workfront Fusion] - Instruções básicas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Escolher um local de unidade]</td> 
   <td> <p>Selecione o [!DNL Google Drive] onde estão localizadas as apresentações que deseja listar:</p> 
    <ul> 
     <li>[!UICONTROL Minha Unidade]</li> 
     <li>[!UICONTROL Compartilhado Comigo]</li> 
     <li>[!UICONTROL [!DNL Google] Unidade Compartilhada]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID da Pasta]</td> 
   <td> <p>Escolha o local da pasta das apresentações que deseja listar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limite]</td> 
   <td> <p>O número máximo de apresentações [!DNL Workfront Fusion] deve retornar durante um ciclo de execução de cenário.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obter uma Apresentação]

Obtém a versão mais recente de uma apresentação especificada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão] </td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Google Slides] ao [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o [!DNL Adobe Workfront Fusion] - Instruções básicas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Escolher uma unidade]</td> 
   <td> <p>Selecione o [!DNL Google Drive] onde estão localizadas as apresentações que deseja listar:</p> 
    <ul> 
     <li>[!UICONTROL Minha Unidade]</li> 
     <li>[!UICONTROL Compartilhado Comigo]</li> 
     <li>[!UICONTROL [!DNL Google] Unidade Compartilhada]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID da Apresentação]</td> 
   <td> <p> Selecione a apresentação que deseja recuperar.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obter uma Página/Miniatura]

Obtém a versão mais recente da página especificada ou da miniatura de uma página na apresentação.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão] </td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Google Slides] ao [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o [!DNL Adobe Workfront Fusion] - Instruções básicas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID da Apresentação]</td> 
   <td> <p> Selecione a ID de apresentação que deseja recuperar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de Objeto de Página]</td> 
   <td> <p> Selecione o slide para o qual deseja exibir os detalhes do objeto da página.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Mostrar Miniatura de Página]</td> 
   <td> <p> Marque a caixa de seleção se desejar exibir as informações de miniatura da página.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Criar uma Apresentação de um Modelo]

Cria uma nova apresentação substituindo todas as marcas como `{{Name}}`, `{{Email}}` em um modelo pelos dados fornecidos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão] </td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Google Slides] ao [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o [!DNL Adobe Workfront Fusion] - Instruções básicas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Título] </td> 
   <td> <p>Insira um nome para a nova apresentação.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Copiar uma Apresentação]</td> 
   <td> <p> Selecione a opção se estiver copiando uma apresentação existente:</p> 
    <ul> 
     <li>[!UICONTROL Por Mapeamento]</li> 
     <li>[!UICONTROL Por Lista Suspensa]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cópia de ID de Apresentação Existente]</td> 
   <td> <p> Insira o Caminho ou a ID de uma apresentação existente que você deseja copiar. Este campo aparecerá se você estiver criando a apresentação [!UICONTROL Por Mapeamento].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Escolher uma unidade]</td> 
   <td> <p>Selecione o [!DNL Google Drive] onde estão localizadas as apresentações que deseja listar:</p> 
    <ul> 
     <li>[!UICONTROL Minha Unidade]</li> 
     <li>[!UICONTROL Compartilhado Comigo]</li> 
     <li>[!UICONTROL [!DNL Google] Unidade Compartilhada]</li> 
    </ul> <p>Este campo aparecerá se você estiver criando a apresentação [!UICONTROL By Dropdown].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID da Apresentação]</td> 
   <td> <p> Selecione a ID da apresentação que deseja usar como modelo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Valores] </td> 
   <td> <p>Adicione os valores:</p> 
    <ul> 
     <li><strong>[!UICONTROL Marca]</strong>: Insira a marca que você deseja substituir na apresentação. Por exemplo, <code>&#123;&#123;Name&#125;&#125;</code></li> 
     <li><strong>[!UICONTROL Valor Substituído]</strong>: Insira o valor pelo qual a marca existente será substituída. Por exemplo, se uma string <tr><ul><tr><tr><tr><code>&#123;&#123;Name&#125;&#125;/code> in the presentation and the replaced value is Sample, then the <code>&#123;&#123;Name&#125;&#125;</code> will be replaced by <code>Sample</code>.</li> 
    </ul> </td> 
  </tr> 
   
   <td role="rowheader">[!UICONTROL New Drive Location]</td> 
   <td> <p>Select the [!DNL Google Drive] where you want to store or add the new presentation:</p> 
     
     <li>[!UICONTROL My Drive]</li> 
     <li>[!UICONTROL Shared With Me]</li> 
     <li>[!UICONTROL [!DNL Google] Shared Drive]</li> 
    </ul> </td> 
  </tr> 
   
   <td role="rowheader"> <p>[!UICONTROL New Document's Location]</p> </td> 
   <td> <p>Select the folder where you want to store or add the presentation.</p> </td> 
  </tr> 
   
   <td role="rowheader">[!UICONTROL Shared] </td> 
   <td> <p>Select if you want to share the presentation.</p> </td> 
  </tr> 
   
   <td role="rowheader">[!UICONTROL Sharing with Other's Email Address]</td> 
   <td> <p> Enter the email address with whom you want to share the presentation. If you are not entering an email address and selecting only shared field, the presentation is shareable to anyone.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Carregar uma Imagem para uma Apresentação]

Carrega uma imagem com os dados fornecidos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão] </td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Google Slides] ao [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o [!DNL Adobe Workfront Fusion] - Instruções básicas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Escolher uma Apresentação]</td> 
   <td> <p>Escolha como deseja selecionar a apresentação na qual você está fazendo upload de uma imagem.</p> 
    <ul> 
     <li>[!UICONTROL Por Mapeamento]</li> 
     <li>[!DNL By Dropdown]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Escolher uma unidade]</td> 
   <td> <p>Selecione o [!DNL Google Drive] onde estão localizadas as apresentações que deseja listar:</p> 
    <ul> 
     <li>[!UICONTROL Minha Unidade]</li> 
     <li>[!UICONTROL Compartilhado Comigo]</li> 
     <li>[!UICONTROL [!DNL Google] Unidade Compartilhada]</li> 
    </ul> <p>Este campo aparecerá se você estiver criando a apresentação [!UICONTROL By Dropdown].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID da Apresentação]</td> 
   <td> <p> Selecione a ID da Apresentação da apresentação na qual você está fazendo upload de uma imagem.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Valores]</td> 
   <td> <p>Valores Adicione os valores:</p> 
    <ul> 
     <li><strong>[!UICONTROL Marca]</strong>: Insira a marca à qual você deseja adicionar a URL.</li> 
     <li><strong>[!UICONTROL URL da Imagem]</strong>: Digite o caminho ou a URL da imagem que você deseja carregar.</li> 
    </ul> <p>Observação: as imagens devem ter menos de 50 MB, não podem exceder 25 megapixels e devem estar no formato PNG, JPEG ou GIF.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Atualizar um Gráfico]

Atualiza os dados do gráfico armazenados em uma apresentação especificada por ID.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão] </td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Google Slides] ao [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o [!DNL Adobe Workfront Fusion] - Instruções básicas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Escolher uma unidade]</td> 
   <td> <p>Selecione o [!DNL Google Drive] onde estão localizadas as apresentações que deseja listar:</p> 
    <ul> 
     <li>[!UICONTROL Minha Unidade]</li> 
     <li>[!UICONTROL Compartilhado Comigo]</li> 
     <li>[!UICONTROL [!DNL Google] Unidade Compartilhada]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID da Apresentação]</td> 
   <td> <p>Selecione a ID de Apresentação da apresentação que inclui o gráfico que você deseja atualizar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de Objeto de Gráfico]</td> 
   <td> <p> Selecione o Gráfico que deseja atualizar.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Adicionar/Excluir um Slide]

Cria um slide vazio ou exclui um slide existente na apresentação especificada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão] </td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Google Slides] ao [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o [!DNL Adobe Workfront Fusion] - Instruções básicas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Selecionar o método]</td> 
   <td> <p>Escolha se deseja adicionar um novo slide ou excluir um slide.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Presentation ID]</td> 
   <td> <p>Selecione a ID da apresentação da apresentação para a qual deseja adicionar ou excluir um slide.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de layout predefinido]</td> 
   <td> <p> Selecione o layout de slide predefinido a ser usado pelo slide adicionado. Especifique valores para quaisquer campos adicionais (como [!UICONTROL Título]).</p> 
    <ul> 
     <li>[!UICONTROL Layout em branco, sem espaços reservados]</li> 
     <li>[!UICONTROL Layout com uma legenda na parte inferior]</li> 
     <li>[!UICONTROL Layout com um título e subtítulo]</li> 
     <li>[!UICONTROL Layout com um título e um corpo]</li> 
     <li>[!UICONTROL Layout com um título e duas colunas]</li> 
     <li>[!UICONTROL Layout com apenas um título]</li> 
     <li>[!UICONTROL Layout com um título de seção]</li> 
     <li>[!UICONTROL Layout com título e subtítulo em um lado e descrição no outro]</li> 
     <li>[!UICONTROL Layout com um título e um corpo, organizados em uma única coluna]</li> 
     <li>[!UICONTROL Layout com um ponto principal]</li> 
     <li>[!DNL Layout with a big number heading]</li> 
    </ul> <p>Este campo estará disponível se você selecionou adicionar um slide.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Outro

* [[!UICONTROL Fazer uma chamada de API]](#make-an-api-call)
* [[!UICONTROL Inserir Links em uma Apresentação]](#insert-links-in-a-presentation)

#### [!UICONTROL Fazer uma chamada de API]

Executa uma chamada de API autorizada arbitrária.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão] </td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Google Slides] ao [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o [!DNL Adobe Workfront Fusion] - Instruções básicas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td> <p>Insira um caminho relativo para https://developers.google.com/slides/. Por exemplo, Apresentação.</p> <p>Para obter a lista de pontos de extremidade disponíveis, consulte a <a href="https://developers.google.com/slides/reference/rest">[!DNL Google Slides] Documentação da API</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Método]</td> 
   <td> <p>Selecione o método de solicitação HTTP necessário para configurar a chamada de API. Para obter mais informações, consulte <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">Métodos de solicitação HTTP em [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cabeçalhos]</td> 
   <td> <p>Insira os cabeçalhos de solicitação desejados. Você não precisa adicionar cabeçalhos de autorização.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cadeia de Consulta]</td> 
   <td> <p> Insira a string de consulta da solicitação.</p> </td> 
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

>[!INFO]
>
>**Exemplo:** usando uma chamada de API, você pode obter os detalhes da apresentação para a ID de apresentação inserida. Você pode encontrar a ID da apresentação na URL ao abrir a apresentação em [!DNL Google Slides].
>
>![](assets/api-call-350x13.png)
>
>A chamada de API a seguir retorna os detalhes da apresentação:
>
>![](assets/presentation-details.png)
>
>Correspondências da pesquisa podem ser encontradas na Saída do módulo em [!UICONTROL Pacote] > [!UICONTROL Corpo] > [!UICONTROL presentationId].
>
>Em nosso exemplo, os detalhes da apresentação solicitada foram retornados:
>
>![](assets/presentation-details-2.png)

#### [!UICONTROL Inserir Links em uma Apresentação]

Esse módulo torna clicáveis todos os links em uma apresentação ou insere um link em todos os textos de entrada correspondentes.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão] </td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Google Slides] ao [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o [!DNL Adobe Workfront Fusion] - Instruções básicas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Escolher uma Apresentação]</td> 
   <td> <p>Escolha como deseja selecionar a apresentação na qual você está fazendo upload de uma imagem.</p> 
    <ul> 
     <li>[!UICONTROL Por Mapeamento]</li> 
     <li>[!UICONTROL Por Lista Suspensa]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Escolher uma unidade]</td> 
   <td> <p>Selecione o [!DNL Google Drive] onde estão localizadas as apresentações que deseja listar:</p> 
    <ul> 
     <li>[!UICONTROL Minha Unidade]</li> 
     <li>[!UICONTROL Compartilhado Comigo]</li> 
     <li>[!UICONTROL [!DNL Google] Unidade Compartilhada]</li> 
    </ul> <p>Este campo aparecerá se você estiver criando a apresentação [!UICONTROL By Dropdown].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID da Apresentação]</td> 
   <td> <p>Escolha o local da pasta das apresentações que deseja listar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Selecionar]</td> 
   <td> <p>Selecione se deseja tornar clicáveis todos os links em uma apresentação ou se deseja inserir um link em todos os textos de entrada de correspondência.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Entradas de Texto]</td> 
   <td>Para cada item de texto ao qual você deseja adicionar um link, adicione o item, bem como seu link associado à lista. Toda vez que o item aparecer na apresentação, ele será vinculado automaticamente ao site especificado.</td> 
  </tr> 
 </tbody> 
</table>
