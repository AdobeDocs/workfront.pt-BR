---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: conector
navigation-topic: apps-and-their-modules
title: Módulos Trello
description: Em um [!DNL Adobe Workfront Fusion] você pode automatizar workflows que usam o Trello, bem como conectá-lo a vários aplicativos e serviços de terceiros.
author: Becky
feature: Workfront Fusion
exl-id: 60630b23-e057-4ecf-a014-6e63b6d69b48
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '5039'
ht-degree: 0%

---

# [!UICONTROL Trello] módulos

Em um [!DNL Adobe Workfront Fusion] , é possível automatizar workflows que usam [!UICONTROL Trello], bem como conectá-lo a vários aplicativos e serviços de terceiros.

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

Para usar [!DNL Trello] módulos, você deve ter um [!UICONTROL Trello] conta.

## Connect [!UICONTROL Trello] para [!DNL Workfront Fusion]

Para obter instruções sobre como conectar seu [!UICONTROL Trello] para [!DNL Workfront Fusion], consulte [Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas](../../workfront-fusion/connections/connect-to-fusion-general.md)

## [!UICONTROL Trello] módulos e seus campos

Ao configurar [!UICONTROL Trello] módulos, [!DNL Workfront Fusion] exibe os campos listados abaixo. Junto com esses, [!UICONTROL Trello] podem ser exibidos, dependendo de fatores como seu nível de acesso no aplicativo ou serviço. Um título em negrito em um módulo indica um campo obrigatório.

Se o botão de mapa for exibido acima de um campo ou função, é possível usá-lo para definir variáveis e funções para esse campo. Para obter mais informações, consulte [Mapear informações de um módulo para outro no [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Quadros](#boards)
* [Listas](#lists)
* [Cartões](#cards)
* [Membros](#members)
* [Listas de verificação](#checklists)
* [Rótulos](#labels)
* [Comentários](#comments)

### Quadros

+++ **[!UICONTROL Quadros de observação]**

Esse módulo de acionador inicia um cenário quando um novo quadro é adicionado.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!UICONTROL Trello] ao [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limite] </td> 
   <td> <p>O número máximo de quadros [!DNL Workfront Fusion] retornará durante um ciclo de execução.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Criar um quadro]**

Este módulo de ação cria um novo quadro com as configurações selecionadas.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!UICONTROL Trello] ao [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Name] </td> 
   <td> <p>Insira ou mapeie um nome para o novo quadro.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Descrição]</td> 
   <td> <p>Insira ou mapeie a descrição do quadro, se necessário.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Organization ID]</p> </td> 
   <td> <p>Insira ou mapeie a ID da organização. A ID da organização pode ser recuperada usando outro módulo, como o módulo Atividades de monitoramento .</p> <p> <img src="assets/id-of-org.png"> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Nível de permissão]</p> </td> 
   <td> <p>Os conselhos têm regras de votação e comentário diferentes para cada nível de permissão. Por exemplo: se o seu conselho for [!UICONTROL Privado] e você definir as regras de votação e comentário como [!UICONTROL Tudo], você receberá uma mensagem de erro. </p> <p>A votação e os comentários são limitados aos seguintes grupos para cada nível de permissão:</p> 
    <ul> 
     <li><strong>[!UICONTROL Privado]</strong>: —&gt;Membros, Membros e Observadores</li> 
     <li><strong>[!UICONTROL Para organização]</strong>: —&gt;Membros, Membros e Observadores, Membros da Organização</li> 
     <li><strong>[!UICONTROL Público]</strong>: —&gt;Membros, Membros e Observadores, Membros da Organização, Todos</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Votação]</p> </td> 
   <td> <p>Selecione uma opção para especificar quem pode votar neste quadro. Consulte o campo [!UICONTROL Permissão nível] para limitações de votação em níveis de permissão.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Comentários]</p> </td> 
   <td> <p>Selecione uma opção para especificar quem pode comentar nos cartões deste quadro. Consulte o campo [!UICONTROL Permission level] para obter comentários sobre limitações nos níveis de permissão.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Convites]</p> </td> 
   <td> <p>Selecione quem pode convidar outras pessoas para este quadro.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Autoassociação]</p> </td> 
   <td> <p>Selecione se os membros da equipe podem ingressar no quadro ou se eles precisam ser convidados.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Rótulos padrão]</p> </td> 
   <td> <p>Selecione se deseja usar o conjunto padrão de rótulos para o novo quadro.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Listas padrão]</p> </td> 
   <td> <p>Selecione se deseja adicionar o conjunto padrão de listas ao quadro ([!UICONTROL Fazer], [!UICONTROL Fazendo], [!UICONTROL Concluído]).</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL ID de origem da placa]</p> </td> 
   <td> <p>Selecione ou mapeie a ID do quadro que você deseja copiar para o novo quadro.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Capas de cartão]</p> </td> 
   <td> <p>Selecionar <strong>[!UICONTROL Sim]</strong> se quiser ativar as tampas de cartão para a placa.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Fundo]</p> </td> 
   <td> <p>Selecione a cor do plano de fundo ou o plano de fundo personalizado.</p> <p>Observação: Os planos de fundo personalizados estão disponíveis somente para assinantes da [!UICONTROL Trello Gold e Business Class].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Envelhecimento da placa]</p> </td> 
   <td> <p>Selecione entre dois modos de envelhecimento do cartão. </p> 
    <ul> 
     <li><strong>[!UICONTROL Regular]</strong>: Os cartões tornam-se progressivamente mais transparentes à medida que envelhecem. </li> 
     <li><strong>[!UICONTROL Pirate]</strong>: Os cartões rasgam, amarelam e racham como um velho mapa dos piratas à medida que envelhecem.</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Editar um quadro]**

Este módulo de ação edita as configurações de uma placa existente.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!UICONTROL Trello] ao [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL ID da placa]</p> </td> 
   <td> <p>Insira ou mapeie a ID exclusiva do [!UICONTROL Trello] do quadro que você deseja que o módulo crie. Você pode recuperar a ID da placa usando outro módulo, como o módulo Placas de monitoramento</p> <p> <img src="assets/watch-boards.png"> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Novo nome]</td> 
   <td> <p> Insira ou mapeie um novo nome para o quadro.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nova descrição]</td> 
   <td> <p> Insira ou mapeie uma nova descrição do quadro, se necessário.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Organization ID]</p> </td> 
   <td> <p>Insira ou mapeie a ID exclusiva [!UICONTROL Trello] do quadro que você deseja que o módulo edite. Você pode recuperar a ID da placa usando outro módulo, como o [!DNL Watch Activities] módulo.</p> <p> <img src="assets/org-id.png"> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Assinar] </td> 
   <td> <p>Selecione uma opção para especificar se o usuário atuante está inscrito no quadro.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Nível de permissão]</p> </td> 
   <td> <p>Os conselhos têm regras de votação e comentário diferentes para cada nível de permissão. Por exemplo: se o seu conselho for [!UICONTROL Privado] e você definir as regras de votação e comentário como [!UICONTROL Tudo], você receberá uma mensagem de erro. </p> <p>A votação e os comentários são limitados aos seguintes grupos para cada nível de permissão:</p> 
    <ul> 
     <li><strong>[!UICONTROL Privado]</strong>: —&gt;Membros, Membros e Observadores</li> 
     <li><strong>[!UICONTROL Para organização]</strong>: —&gt;Membros, Membros e Observadores, Membros da Organização</li> 
     <li><strong>[!UICONTROL Público]</strong>: —&gt;Membros, Membros e Observadores, Membros da Organização, Todos</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Votação]</p> </td> 
   <td> <p>Selecione uma opção para especificar quem pode votar neste quadro. Consulte o campo [!UICONTROL Permissão nível] para limitações de votação em níveis de permissão.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Comentários]</p> </td> 
   <td> <p>Selecione uma opção para especificar quem pode comentar nos cartões deste quadro. Consulte o campo [!UICONTROL Permission level] para obter comentários sobre limitações nos níveis de permissão.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Convites] </td> 
   <td> <p>Selecione quem pode convidar pessoas para este quadro.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Autoassociação]</td> 
   <td> <p> Selecione se os membros da equipe podem ingressar no quadro ou se eles precisam ser convidados.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Capas de cartão]</td> 
   <td> <p> Selecione se as capas de cartão devem ser exibidas neste quadro.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Fundo] </td> 
   <td> <p>Selecione a cor do plano de fundo ou o plano de fundo personalizado.</p> <p>Observação: Os planos de fundo personalizados estão disponíveis somente para assinantes da [!UICONTROL Trello Gold e Business Class].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID do plano de fundo]</td> 
   <td> <p> Se tiver selecionado o uso de um plano de fundo personalizado no campo [!UICONTROL Plano de fundo], insira ou mapeie a ID do plano de fundo que deseja usar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Envelhecimento da placa]</p> </td> 
   <td> <p>Selecione entre dois modos de envelhecimento do cartão. </p> 
    <ul> 
     <li><strong>[!UICONTROL Regular]</strong>: Os cartões tornam-se progressivamente mais transparentes à medida que envelhecem. </li> 
     <li><strong>[!UICONTROL Pirate]</strong>: Os cartões rasgam, amarelam e racham como um velho mapa dos piratas à medida que envelhecem.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Feed do calendário ativado]</td> 
   <td> <p> Selecione se o feed do calendário está ativado ou não.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL &lt;color&gt; nome do rótulo]</td> 
   <td> <p> Atribua um nome ao rótulo de cor desejado.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Arquivo] </td> 
   <td> <p>Selecione uma opção para indicar se deseja arquivar (fechar) o quadro. </p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Adquira um quadro]**

Esse módulo de ação recupera os detalhes de um quadro.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!UICONTROL Trello] ao [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL ID da placa]</p> </td> 
   <td> <p>Insira ou mapeie a ID do quadro sobre o qual você deseja recuperar informações.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!DNL Search for Boards]**

Esse módulo de pesquisa recupera informações sobre um quadro especificado por você.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!UICONTROL Trello] ao [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Consulta] </td> 
   <td> <p>Insira ou mapeie o nome (ou parte do nome) do quadro sobre o qual você deseja obter informações.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Número máximo de quadros retornados]</td> 
   <td> <p> Insira o número máximo de quadros [!DNL Workfront Fusion] retornará durante um ciclo de execução. Esse valor deve ser menor ou igual a 1000.</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Parcial] </p> </td> 
   <td> <p>Por padrão, esse módulo pesquisa o conteúdo do membro em busca de correspondências exatas de cada palavra em sua query. Quando [!UICONTROL Parcial] é ativado, o módulo procura por conteúdo que comece com qualquer palavra em sua consulta.</p> <p> Por exemplo, se estiver usando a palavra "desenvolvimento" para procurar por um quadro chamado "Meu relatório de status de desenvolvimento", por padrão, você precisará pesquisar a palavra inteira. Se você tiver [!UICONTROL Parcial] ativado, poderá pesquisar por "desenvolvimento", mas não por "desenvolvimento".</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Quadros] </td> 
   <td> <p>Insira "meu" ou mapeie uma lista separada por vírgulas de IDs do quadro.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Arquivar ou desarquivar um quadro]**

Esse módulo de ação fecha ou abre novamente um quadro especificado por você .

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!UICONTROL Trello] ao [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID da placa]</td> 
   <td> <p> Insira ou mapeie a ID do quadro que deseja fechar ou reabrir.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Arquivar ou desarquivar]</td> 
   <td> <p> Selecione se deseja fechar (arquivar) ou reabrir (desarquivar) o quadro.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Atribuir um Membro a um Conselho]**

Esse módulo de ação atribui um membro a um quadro especificado por você.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!UICONTROL Trello] ao [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID da placa]</td> 
   <td> <p> Selecione o quadro ao qual deseja adicionar um membro.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Endereço de email]</td> 
   <td> <p> Insira ou mapeie o endereço de email do membro que deseja adicionar ao quadro.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Tipo de Membro]</p> </td> 
   <td> <p>Selecione o tipo de membro que deseja adicionar ao quadro.</p> 
    <ul> 
     <li><strong>[!UICONTROL Admin]</strong>: Um administrador de quadro pode executar qualquer ação de quadro no quadro.</li> 
     <li><strong>[!UICONTROL Normal]</strong>: Um membro normal é simplesmente um membro do conselho.</li> 
     <li><strong>[!UICONTROL Observer]</strong>: Um observador é um membro com acesso somente leitura ao quadro. <br>Os observadores só estão disponíveis para equipes com a [!UICONTROL Trello Business Class].</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nome completo]</td> 
   <td> <p> Insira o nome completo do usuário que deseja adicionar ao quadro.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Cancelar a atribuição de um membro de um quadro]**

Este módulo de ação remove um membro de um quadro.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!UICONTROL Trello] ao [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID da placa]</td> 
   <td> <p> Insira (mapeie ou selecione) a ID do quadro do qual você deseja remover o usuário.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Membro] </td> 
   <td> <p>Selecione o membro que deseja remover do quadro.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

### Listas

+++ **[!UICONTROL Cartões de observação movidos para uma lista]**

Esse módulo de acionador é ativado quando uma placa é movida para uma lista específica.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!UICONTROL Trello] ao [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Board]</td> 
   <td>Selecione o quadro que contém a lista que você deseja observar para os cartões.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL List]</td> 
   <td>Selecione a lista que deseja assistir para cartões.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limite] </td> 
   <td> <p>O número máximo de cartões [!DNL Workfront Fusion] retornará durante um ciclo de execução.</p>  </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Criar uma lista]**

Esse módulo de ação cria uma lista em um quadro que você especifica .

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!UICONTROL Trello] ao [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID da placa]</td> 
   <td> <p> Insira ou mapeie a ID do quadro em que deseja criar uma lista.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Name] </td> 
   <td> <p>Insira ou mapeie um nome para a nova lista.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Posição] </td> 
   <td> <p>Selecione se deseja adicionar a lista à parte superior ou anexá-la à parte inferior do cartão.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Copiar lista]</td> 
   <td> <p> Selecione como deseja inserir a ID da lista que deseja copiar.</p> 
    <ul> 
     <li> <p><strong>Inserir manualmente</strong> </p> <p>No <strong>[!UICONTROL List ID]</strong> , insira ou mapeie a ID da lista que deseja copiar.<br></p> </li> 
     <li> <p><strong>Selecionar</strong> </p> <p>Selecione o quadro que contém a lista que você deseja copiar e selecione a lista.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Editar uma lista]**

Esse módulo de ação edita uma lista existente.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!UICONTROL Trello] ao [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL List ID]</td> 
   <td> <p> Insira ou mapeie a ID da lista que deseja atualizar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Name] </td> 
   <td> <p>Insira ou mapeie um novo nome para a lista.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID da placa]</td> 
   <td> <p> Mapeie ou selecione o quadro no qual deseja mover a lista.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Posição] </td> 
   <td> <p>Selecione se deseja adicionar a lista à parte superior ou anexá-la à parte inferior do cartão.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Assinado]</td> 
   <td> <p>Ative essa opção se desejar assinar o membro ativo para a lista.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Obter uma lista]**

Este módulo de ação recupera detalhes sobre uma lista específica.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!UICONTROL Trello] ao [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL List ID]</p> </td> 
   <td> <p>Insira ou mapeie a ID da lista sobre a qual deseja recuperar informações.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

### Cartões

+++ **[!UICONTROL Cartões de observação]**

Esse módulo de acionador é ativado quando uma nova placa é adicionada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!UICONTROL Trello] ao [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Objeto assistido]</td> 
   <td> <p>Selecione o local que deseja observar para cartões.</p> 
    <ul> 
     <li><strong>[!UICONTROL Todos os cartões]</strong> </li> 
     <li> <p><strong>Cartões em placas específicas</strong> </p> <p>Selecione o quadro que deseja observar para cartões</p> </li> 
     <li> <p><strong>[!UICONTROL Cartões em lista específica]</strong> </p> <p>Selecione o quadro que contém a lista que você deseja observar para os cartões e selecione a lista.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limite] </td> 
   <td> <p>O número máximo de cartões [!DNL Workfront Fusion] retornará durante um ciclo de execução.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Criar um cartão]**

Esse módulo de ação cria um cartão em uma lista selecionada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!UICONTROL Trello] ao [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Inserir uma ID da lista]</td> 
   <td> <p> Selecione como deseja inserir a ID da lista onde deseja adicionar um cartão.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Inserir manualmente]</strong> </p> <p>No <strong>[!UICONTROL List ID]</strong> , insira ou mapeie a ID da lista onde deseja adicionar um cartão.<br></p> </li> 
     <li> <p><strong>[!UICONTROL Selecionar]</strong> </p> <p>Selecione o quadro que contém a lista que você deseja copiar e selecione a lista.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Rótulos] </td> 
   <td> <p>Para cada rótulo que você deseja adicionar ao cartão, insira a ID do rótulo. A ID pode ser recuperada, por exemplo, usando o módulo [!UICONTROL Recuperar rótulos].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Membros]</td> 
   <td>Para cada membro que deseja adicionar ao cartão, insira a ID do membro. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Name] </td> 
   <td> <p>Insira um nome para o novo cartão.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Descrição]</p> </td> 
   <td> <p>Insira a descrição do cartão.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Posição] </td> 
   <td> <p>Selecione se deseja adicionar o cartão à parte superior ou [!UICONTROL anexar] à parte inferior da lista.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Data de vencimento]</td> 
   <td> <p> Insira uma data de vencimento para o cartão. Para obter uma lista de formatos de data e hora compatíveis, consulte <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Coação de tipo em [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Vencido concluído]</td> 
   <td> <p> Ative essa opção para marcar o cartão como concluído na data de vencimento.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL do arquivo]</td> 
   <td> <p>Insira ou mapeie a URL de um arquivo que deseja adicionar como anexo ao cartão.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Arquivo de origem]</p> </td> 
   <td> <p>Insira ou mapeie as informações de um arquivo que deseja adicionar como anexo ao cartão.</p> 
    <ul> 
     <li>[!UICONTROL Nome do arquivo]: Insira ou mapeie o nome do arquivo, incluindo a extensão de arquivo.</li> 
     <li> 
     <p>Selecione um arquivo de um módulo anterior ou mapeie o nome e os dados do arquivo</p> 
     <p>Observação: Existe um limite de upload de arquivo de 10 MB por anexo. No entanto, os membros da [!UICONTROL Business Class] e da [!UICONTROL Trello Gold] têm um limite de upload de arquivo de 250 MB por anexo.</p> 
     </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Copiar cartão]</td> 
   <td> <p> Selecione como deseja inserir a ID do cartão que deseja copiar.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Inserir manualmente]</strong> </p> <p>No <strong>[!UICONTROL ID da placa]</strong> , insira ou mapeie a ID do cartão que deseja copiar.<br></p> </li> 
     <li> <p><strong>[!UICONTROL Selecionar]</strong> </p> <p>Selecione o quadro que contém o cartão que você deseja copiar, em seguida, selecione a lista que contém o cartão e selecione o cartão.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Editar um cartão]**

Esse módulo de ação edita uma placa existente.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!UICONTROL Trello] ao [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Inserir ID do cartão]</td> 
   <td> <p> Selecione como deseja inserir a ID do cartão que deseja editar.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Inserir manualmente]</strong> </p> <p>No <strong>[!UICONTROL ID da placa]</strong> , insira ou mapeie a ID do cartão que deseja editar.<br></p> </li> 
     <li> <p><strong>[!UICONTROL Selecionar]</strong> </p> <p>Selecione o quadro que contém o cartão que você deseja editar, selecione a lista que contém o cartão e selecione o cartão.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Novo nome]</td> 
   <td> <p>Insira ou mapeie um novo nome para o cartão.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Nova descrição]</p> </td> 
   <td> <p>Insira ou mapeie uma nova descrição para o cartão.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Mover um cartão]</p> </td> 
   <td> <p>Selecione o quadro ou o quadro e a lista onde deseja mover o cartão.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Rótulos] </td> 
   <td> <p>Adicione as IDs de qualquer rótulo que deseja adicionar ao cartão. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Posição] </td> 
   <td> <p>Selecione se deseja adicionar o cartão à parte superior ou [!UICONTROL anexar] à parte inferior da lista.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Data de vencimento]</td> 
   <td> <p> Insira uma data de vencimento para o cartão. Para obter uma lista de formatos de data e hora compatíveis, consulte <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Coação de tipo em [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Vencido concluído]</td> 
   <td> <p> Se esta opção estiver ativada, o cartão é marcado como concluído na data de vencimento.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Membros] </td> 
   <td> <p>Adicione ou mapeie a ID de qualquer membro que deseja adicionar ao cartão.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL ID da tampa do anexo]</p> </td> 
   <td> <p>Insira ou mapeie a ID do anexo de imagem que você deseja que o cartão use como capa.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Assinar] </td> 
   <td> <p>Selecione se o membro deve ser inscrito no cartão.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Arquivo] </td> 
   <td> <p>Selecione uma opção para indicar se deseja arquivar (fechar) o cartão. </p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Obter um cartão]**

Este módulo de ação recupera os detalhes de uma placa selecionada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!UICONTROL Trello] ao [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID da placa]</td> 
   <td> <p>Insira a ID do quadro que contém o cartão sobre o qual você deseja recuperar detalhes. Isso permite ver os nomes dos campos personalizados do quadro.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Inserir ID do cartão]</td> 
   <td> <p> Selecione como deseja inserir a ID do cartão sobre o qual deseja recuperar detalhes.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Inserir manualmente]</strong> </p> <p>No <strong>[!UICONTROL ID da placa]</strong> , insira ou mapeie a ID do cartão sobre o qual deseja recuperar detalhes.<br></p> </li> 
     <li> <p><strong>[!UICONTROL Selecionar]</strong> </p> <p>Selecione o quadro que contém o cartão sobre o qual você deseja recuperar os detalhes, em seguida, selecione a lista que contém o cartão e selecione o cartão.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Procurar Cartões]**

Este módulo de ação retorna cartões que correspondem à consulta de pesquisa.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!UICONTROL Trello] ao [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Board] </td> 
   <td> <p>Selecione os quadros que deseja pesquisar. Se nenhum quadro estiver selecionado, todos os quadros serão pesquisados.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Consulta]</p> </td> 
   <td> <p>Insira a consulta de pesquisa. Você pode refinar sua pesquisa usando os seguintes operadores de pesquisa:</p> 
    <ul> 
     <li><code><strong>-operator</strong></code> <p>Você pode adicionar "-" a qualquer operador para fazer uma pesquisa negativa, como <code>[!UICONTROL -has:members]</code> para procurar cartões sem membros atribuídos.</p> </li> 
     <li><code><strong>@name</strong></code> <p>Retorna cartões atribuídos a um membro. Você também pode usar <code>member:</code>. Use <code>@me</code> para incluir somente seus cartões.</p> </li> 
     <li><code><strong>#label</strong></code> <p>Retorna cartões rotulados. Você também pode usar <code>label:</code>. Por exemplo, <code>label:"FIX IT"</code> O retornará cartões com o rótulo chamado "FIX IT".</p> </li> 
     <li><code><strong>board:id</strong></code> <p>Retorna cartões dentro de um quadro específico. Por exemplo, <code>board:Trello</code> retornará cartões em quadros com o [!UICONTROL Trello] no nome da placa.</p> </li> 
     <li><code><strong>list:name</strong></code> <p>Retorna cartões dentro da lista com o nome "nome".</p> </li> 
     <li><code><strong>has:attachments</strong></code> <p>Retorna cartões com anexos. O <code>has</code>: operador também pode ser usado com outros atributos, como <code>has:description</code>, <code>has:cover</code>, <code>has:members</code>ou <code>has:stickers</code>.</p> </li> 
     <li><code><strong>due:day</strong></code> <p>Retorna cartões com vencimento em 24 horas. O <code>due:</code> também pode ser usado com outros cronogramas, como <code>due:week</code>, <code>due:month</code>ou <code>due:overdue</code>. Você também pode procurar por um intervalo de dias específico. Por exemplo, adicionar <code>due:14</code> a pesquisa inclui cartões que devem ser executados nos próximos 14 dias.</p> </li> 
     <li><code><strong>created:day</strong></code> <p>Retorna cartões criados nas últimas 24 horas. O<code> created:</code> também pode ser usado com outros cronogramas, como <code>created:week</code> ou <code>created:month</code>. Você também pode procurar por um intervalo de dias específico. Por exemplo, adicionar <code>created:14</code> a pesquisa inclui cartões criados nos últimos 14 dias.</p> </li> 
     <li><code><strong>edited:day</strong></code> <p>Retorna cartões editados nas últimas 24 horas. O <code>edited:</code> também pode ser usado com outros cronogramas, como <code>edited:week</code> ou <code>edited:month</code>. Você também pode procurar por um intervalo de dias específico. Por exemplo, adicionar <code>edited:21</code> a pesquisa inclui cartões editados nos últimos 21 dias.</p> </li> 
     <li><code><strong>description:</strong>, <strong>checklist:</strong>, <strong>comment:</strong>, and <strong>name:</strong></code> <p>Retorna cartões que correspondem ao texto de descrições de cartão, listas de verificação, comentários ou nomes. Por exemplo, comente: "CORRIGIR TI" retornará cartões com "CORRIGIR TI" em um comentário.</p> </li> 
     <li><code><strong>is:open</strong> and <strong>is:archived</strong></code> <p>Retorna cartões que estão abertos ou arquivados. Se nenhum dos dois for especificado, [!UICONTROL Trello] retornará ambos os tipos.</p> </li> 
     <li><code><strong>is:starred</strong> </code> <p>Inclui apenas cartões em quadros estrelados.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Número máximo de cartões retornados]</td> 
   <td> <p> O número máximo de cartões [!DNL Workfront Fusion] retornará durante um ciclo de execução. Esse valor deve ser menor ou igual a 1000.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Parcial] </td> 
   <td> <p>Por padrão, esse módulo pesquisa o conteúdo do membro em busca de correspondências exatas de cada palavra em sua query. Quando [!UICONTROL Parcial] é ativado, o módulo procura por conteúdo que comece com qualquer palavra em sua consulta.</p> <p> Por exemplo, se estiver usando a palavra "desenvolvimento" para procurar por um quadro chamado "Meu relatório de status de desenvolvimento", por padrão, você precisará pesquisar a palavra inteira. Se você tiver [!UICONTROL Parcial] ativado, poderá pesquisar por "desenvolvimento", mas não por "desenvolvimento".</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cartões] </td> 
   <td> <p>Adicione todos os cartões que você deseja pesquisar especificamente.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Arquivar ou desarquivar um cartão]**

Este módulo de ação arquiva ou envia uma placa de volta para a placa.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!UICONTROL Trello] ao [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID da placa]</td> 
   <td> <p> Insira ou mapeie a ID do cartão que deseja arquivar ou enviar de volta ao quadro.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Arquivar ou desarquivar]</td> 
   <td> <p> Selecione se deseja fechar o cartão (arquivar) ou enviá-lo de volta ao quadro (desarquivar).</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Adicionar um anexo]**

Este módulo de ação adiciona um anexo ao cartão selecionado.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!UICONTROL Trello] ao [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Inserir ID do cartão]</td> 
   <td> <p> Selecione como deseja inserir a ID do cartão sobre o qual deseja recuperar detalhes.</p> 
    <ul> 
     <li> <p><strong>Inserir manualmente</strong> </p> <p>No <strong>[!UICONTROL ID da placa]</strong> , insira ou mapeie a ID do cartão sobre o qual deseja recuperar detalhes.<br></p> </li> 
     <li> <p><strong>[!UICONTROL Selecionar]</strong> </p> <p>Selecione o quadro que contém o cartão sobre o qual você deseja recuperar os detalhes, em seguida, selecione a lista que contém o cartão e selecione o cartão.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Tipo de anexo]</p> </td> 
   <td> <p>Selecione se deseja fazer upload do arquivo diretamente ou fornecer um URL para o arquivo.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Arquivo]</strong> </p> <p>Selecione um arquivo de origem de um módulo anterior ou mapeie o nome e os dados do arquivo de origem.</p> </li> 
     <li> <p><strong>[!UICONTROL URL]</strong> </p> <p>Insira o URL do arquivo e forneça um nome para o anexo.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

+++

### Membros

+++ **[!UICONTROL Atribuir um Membro a um Conselho]**

Consulte &quot;[!UICONTROL Atribuir um Membro a um Conselho]&quot; [Quadros](#boards).

+++

+++ **[!UICONTROL Cancelar a atribuição de um membro de um quadro]**

Consulte &quot;[!UICONTROL Cancelar a atribuição de um membro de um quadro]&quot; [Quadros](#boards).

+++

+++ **[!UICONTROL Adicionar um Membro a um Cartão]**

Esse módulo de ação adiciona o membro especificado ao cartão especificado.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!UICONTROL Trello] ao [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Inserir ID de cartão e ID de membro]</p> </td> 
   <td> <p>Escolha como você deseja inserir a ID do cartão e a ID do membro.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Inserir manualmente]</strong> </p> <p>Insira ou mapeie a variável <strong>[!UICONTROL ID da placa]</strong> e <strong>[!UICONTROL ID do Membro]</strong>.</p> </li> 
     <li> <p><strong>[!UICONTROL Selecionar]</strong> </p> <p>Selecione o quadro que contém o cartão ao qual você deseja adicionar um membro e selecione a lista que contém o cartão, o próprio cartão e o membro que você deseja adicionar ao cartão.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Pesquisar por membros]**

Esse módulo de ação recupera informações sobre [!UICONTROL Trello] membros.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!UICONTROL Trello] ao [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Consulta] </td> 
   <td> <p>Insira o nome completo ou o nome de usuário do usuário que deseja localizar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Parcial] </td> 
   <td> <p>Por padrão, esse módulo pesquisa o conteúdo do membro em busca de correspondências exatas de cada palavra em sua query. Quando [!UICONTROL Parcial] é ativado, o módulo procura por conteúdo que comece com qualquer palavra em sua consulta.</p> <p> Por exemplo, se estiver usando a palavra "desenvolvimento" para procurar por um quadro chamado "Meu relatório de status de desenvolvimento", por padrão, você precisará pesquisar a palavra inteira. Se você tiver [!UICONTROL Parcial] ativado, poderá pesquisar por "desenvolvimento", mas não por "desenvolvimento".</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Número máximo de membros retornados]</td> 
   <td> <p> O número máximo de membros [!DNL Workfront Fusion] retornará durante um ciclo de execução.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

### Listas de verificação

+++ **[!UICONTROL Criar uma lista de verificação]**

Esse módulo de ação cria uma lista de verificação no cartão selecionado.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!UICONTROL Trello] ao [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Inserir uma ID de cartão]</td> 
   <td> <p> Selecione como você deseja inserir a ID do cartão, onde deseja adicionar uma lista de verificação.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Inserir manualmente]</strong> </p> <p>No <strong>[!UICONTROL ID da placa]</strong> , insira ou mapeie a ID do cartão onde deseja adicionar uma lista de verificação.<br></p> </li> 
     <li> <p><strong>[!UICONTROL Selecionar]</strong> </p> <p>Selecione o quadro que contém o cartão ao qual deseja adicionar uma lista de verificação, selecione a lista que contém o cartão e selecione o cartão.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Name] </td> 
   <td> <p>Insira ou mapeie um nome para a lista de verificação.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Posição] </td> 
   <td> <p>Selecione se deseja adicionar a lista de verificação à parte superior ou à lista de verificação [!UICONTROL anexar] na parte inferior do cartão.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Inserir ID da lista de verificação]</p> </td> 
   <td> <p>Insira ou mapeie a ID de uma lista de verificação de origem que você deseja copiar para a nova.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Criar um item da lista de verificação]**

Esse módulo de ação adiciona um item a uma lista de verificação específica.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!UICONTROL Trello] ao [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Inserir ID da lista de verificação]</td> 
   <td> <p> Selecione como você deseja inserir a ID da lista de verificação onde deseja adicionar um item.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Inserir manualmente]</strong> </p> <p>No <strong>[!UICONTROL ID da lista de verificação]</strong> , insira ou mapeie a ID do cartão onde deseja adicionar uma lista de verificação.<br></p> </li> 
     <li> <p><strong>[!UICONTROL Selecionar]</strong> </p> <p>Selecione o quadro que contém o cartão no qual você deseja adicionar uma lista de verificação, selecione a lista que contém o cartão, depois selecione o cartão e depois a lista de verificação.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Nome do item]</p> </td> 
   <td> <p>Insira ou mapeie um nome para o novo item.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Posição]</p> </td> 
   <td> <p>Selecione se deseja adicionar o item à parte superior ou [!UICONTROL append] à parte inferior da lista de verificação.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Marcado]</p> </td> 
   <td> <p>Ative essa opção se desejar adicionar o item como já selecionado.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Editar um item da lista de verificação]**

Esse módulo de ação edita uma lista de verificação existente.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!UICONTROL Trello] ao [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Inserir uma ID de cartão e uma ID de item da lista de verificação]</td> 
   <td> <p> Selecione como você deseja inserir a ID do cartão e a lista de verificação onde deseja editar um item.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Inserir manualmente]</strong> </p> <p>No <strong>[!UICONTROL ID da lista de verificação]</strong> , insira ou mapeie a ID do cartão onde deseja adicionar uma lista de verificação.</p> <p>No <strong>[!UICONTROL ID de item da lista de verificação]</strong> , insira ou mapeie a ID da lista de verificação.</p> </li> 
     <li> <p><strong>[!UICONTROL Selecionar]</strong> </p> <p>Selecione o quadro que contém o cartão no qual você deseja adicionar uma lista de verificação, selecione a lista que contém o cartão, depois selecione o cartão e depois a lista de verificação.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID da lista de verificação]</td> 
   <td>Selecione ou mapeie a lista de verificação para a qual deseja mover o item da lista de verificação.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Nome do item]</p> </td> 
   <td> <p>Insira ou mapeie um nome para o novo item.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Posição]</p> </td> 
   <td> <p>Selecione se deseja adicionar o item à parte superior ou anexar à parte inferior da lista de verificação.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Estado]</p> </td> 
   <td> <p>Selecione se o item da lista de verificação está concluído ou incompleto.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

### Rótulos

+++ **[!UICONTROL Adicionar um rótulo a um cartão]**

Esse módulo de ação adiciona um rótulo a um cartão selecionado.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!UICONTROL Trello] ao [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Inserir ID do cartão]</td> 
   <td> <p> Selecione como você deseja inserir a ID do cartão, onde deseja adicionar uma lista de verificação.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Inserir manualmente]</strong> </p> <p>No <strong>[!UICONTROL ID da placa]</strong> , insira ou mapeie a ID do cartão onde deseja adicionar uma lista de verificação. No<strong>[!UICONTROL ID da etiqueta]</strong> , insira ou mapeie a ID do rótulo que deseja adicionar.<br></p> </li> 
     <li> <p><strong>[!UICONTROL Selecionar]</strong> </p> <p>Selecione o quadro que contém o cartão ao qual deseja adicionar uma lista de verificação, selecione a lista que contém o cartão e selecione o cartão. </p> <p>Selecione o rótulo que deseja adicionar ao cartão.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

+++

### Comentários

+++ **[!UICONTROL Observar comentários]**

Recupera detalhes do comentário quando há um novo comentário em um local especificado.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!UICONTROL Trello] ao [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Objeto assistido]</td> 
   <td> <p>Selecione o local que deseja observar para ver os comentários.</p> 
    <ul> 
     <li><strong>[!UICONTROL Todos os cartões] em todos os lugares</strong> </li> 
     <li> <p><strong>[!UICONTROL Board]</strong> </p> <p>Selecione o quadro que deseja observar para ver os comentários</p> </li> 
     <li> <p><strong>[!UICONTROL List]</strong> </p> <p>Selecione o quadro que contém a lista que você deseja visualizar para comentários e selecione a lista.</p> </li> 
     <li><strong>[!UICONTROL Card]</strong> </li> 
     <li>Selecione o quadro que contém o cartão que você deseja assistir para os comentários, em seguida, selecione a lista que contém o cartão e selecione o cartão.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limite] </td> 
   <td> <p>O número máximo de comentários [!DNL Workfront Fusion] retornará durante um ciclo de execução.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Criar um comentário em um cartão]**

Esse módulo de ação adiciona um comentário a um cartão selecionado.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!UICONTROL Trello] ao [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Inserir uma ID de cartão]</td> 
   <td> <p> Selecione como deseja inserir a ID do cartão à qual deseja adicionar um comentário.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Inserir manualmente]</strong> </p> <p>No <strong>[!UICONTROL ID da placa]</strong> , insira ou mapeie a ID do cartão onde deseja adicionar um comentário.<br></p> </li> 
     <li> <p><strong>[!UICONTROL Selecionar]</strong> </p> <p>Selecione o quadro que contém o cartão ao qual deseja adicionar um comentário, em seguida, selecione a lista que contém o cartão e selecione o cartão.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Comentário] </td> 
   <td> <p>Insira o comentário que deseja adicionar ao cartão selecionado.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Listar comentários em um cartão]**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!UICONTROL Trello] ao [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Inserir uma ID de cartão]</td> 
   <td> <p> Selecione como deseja inserir a ID do cartão à qual deseja adicionar um comentário.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Inserir manualmente]</strong> </p> <p>No <strong>[!UICONTROL ID da placa]</strong> , insira ou mapeie a ID do cartão onde deseja adicionar um comentário.<br></p> </li> 
     <li> <p><strong>[!UICONTROL Selecionar]</strong> </p> <p>Selecione o quadro que contém o cartão ao qual deseja adicionar um comentário, em seguida, selecione a lista que contém o cartão e selecione o cartão.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Número máximo de comentários retornados]</td> 
   <td> <p> Insira o número máximo de comentários [!DNL Workfront Fusion] retornará durante um ciclo de execução.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Since] </td> 
   <td> <p>Defina a data de início do período em que o comentário foi criado. Para obter uma lista de formatos de data e hora compatíveis, consulte <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Coação de tipo em [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Antes] </td> 
   <td> <p>Defina a data final do período em que o comentário foi criado. Para obter uma lista de formatos de data e hora compatíveis, consulte <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Coação de tipo em [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## [!UICONTROL Trello] IDs de objeto

* [Como encontrar a ID ou o atalho de um cartão em [!DNL Trello]](#how-to-find-the-id-or-the-shortlink-of-a-card-in-trello)
* [Como encontrar IDs de outros objetos em [!DNL Trello]](#how-to-find-ids-of-other-objects-in-trello)

### Como encontrar a ID ou o atalho de um cartão em [!DNL Trello]

Se quiser editar um cartão ou criar um novo comentário, é necessário saber a ID do cartão ou seu atalho. Você pode obter essas informações da saída do [!UICONTROL Novo cartão] acionador. O atalho de um cartão também pode ser obtido abrindo o cartão e clicando no botão [!UICONTROL Compartilhar] botão. O atalho pode ser encontrado na variável [!UICONTROL Link para este cartão] , no final do URL após `https://trello.com/c/`.

![](assets/share-and-more-350x575.png)

### Como encontrar IDs de outros objetos em [!DNL Trello]

As IDs de quadro, lista e comentário só podem ser obtidas com acionadores. O [!DNL trello.com] O site da Web não mostra essas IDs.
