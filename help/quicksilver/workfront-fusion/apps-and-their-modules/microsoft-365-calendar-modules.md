---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;calendars
keywords: conector
navigation-topic: apps-and-their-modules
title: Calendário do Microsoft Office 365
description: Em um [!DNL Adobe Workfront Fusion] você pode automatizar workflows que usam o Microsoft Office 365 Calendar, bem como conectá-lo a vários aplicativos e serviços de terceiros.
author: Becky
feature: Workfront Fusion
exl-id: 814c285e-c106-458a-a0b1-760677634f4f
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1835'
ht-degree: 0%

---

# [!DNL Microsoft Office 365 Calendar]

Em um [!DNL Adobe Workfront Fusion] , é possível automatizar workflows que usam [!DNL Microsoft Office 365 Calendar], bem como conectá-lo a vários aplicativos e serviços de terceiros.

Para usar [!DNL Office 365 Calendar] com [!DNL Adobe Workfront Fusion], é necessário ter um [!DNL Office 365 Excel] conta. Você pode criar um em [www.office.com](http://www.office.com/).

Para obter instruções sobre como conectar sua conta do Office 365 para [!DNL Workfront Fusion], consulte [Criar uma conexão com o Adobe [!DNL Workfront Fusion] - Instruções básicas](../../workfront-fusion/connections/connect-to-fusion-general.md)

Após conceder o consentimento, você será redirecionado para a função [!UICONTROL Workfront Fusion] página de administração, onde você pode continuar criando seu cenário.

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

Para usar [!DNL Microsoft Office 365 Calendar] módulos, você deve ter um [!DNL Microsoft Office 365 Calendar] conta.

## [!DNL Microsoft Office 365 Calendar] módulos e seus campos

Ao configurar [!DNL Microsoft Office 365 Calendar] módulos, [!DNL Workfront Fusion] exibe os campos listados abaixo. Junto com esses, [!DNL Microsoft Office 365 Calendar] podem ser exibidos, dependendo de fatores como seu nível de acesso no aplicativo ou serviço. Um título em negrito em um módulo indica um campo obrigatório.

Se o botão de mapa for exibido acima de um campo ou função, é possível usá-lo para definir variáveis e funções para esse campo. Para obter mais informações, consulte [Mapear informações de um módulo para outro no [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Evento](#event)
* [Calendário](#calendar)
* [Outro](#other)

### Evento

* [[!UICONTROL Eventos de observação]](#watch-events)
* [[!UICONTROL Pesquisar eventos]](#search-events)
* [[!UICONTROL Obter um evento]](#get-an-event)
* [[!UICONTROL Criar um evento]](#create-an-event)
* [[!UICONTROL Atualizar um evento]](#update-an-event)
* [[!UICONTROL Excluir um evento]](#delete-an-event)

#### [!UICONTROL Eventos de observação]

Esse módulo de acionador recupera detalhes de um evento quando ele é criado, atualizado, excluído, iniciado ou encerrado no calendário selecionado.

>[!NOTE]
>
>Para monitorar as ocorrências excluídas de uma série de eventos, selecione [!UICONTROL Por Hora de Atualização] no [!UICONTROL Monitoramento de eventos] campo. Este módulo não observa eventos únicos excluídos ou séries de eventos excluídas.


<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Office 365] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Monitoramento de eventos]</td> 
   <td> <p>Selecione como você deseja assistir aos eventos.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Por Hora De Criação]</strong> </p> <p>Fique atento a novos eventos.</p> </li> 
     <li> <p><strong>[!UICONTROL Por Hora Atualizada]</strong> </p> <p>Fique atento aos eventos atualizados.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID do grupo de calendário]</td> 
   <td>Selecione o [!UICONTROL calendar group] que contém o calendário onde deseja assistir aos eventos.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Calendário]</td> 
   <td> <p>Selecione o calendário específico que deseja observar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filtro]</td> 
   <td>Defina as condições do filtro para filtrar os resultados por assunto, ID de evento ou corpo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limite]</td> 
   <td> <p>Insira o número máximo de mensagens [!DNL Workfront Fusion] deve retornar durante um ciclo de execução de cenário.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Pesquisar eventos]

Este módulo de pesquisa recupera detalhes de um evento quando ele é criado, atualizado, excluído, iniciado ou encerrado no calendário selecionado.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Office 365] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID do grupo de calendário]</td> 
   <td>Selecione o [!UICONTROL calendar group] que contém o calendário onde deseja assistir aos eventos.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Calendário]</td> 
   <td> <p>Selecione o calendário específico que deseja observar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filtro]</td> 
   <td> <p>Defina as condições do filtro para filtrar os resultados. Você pode filtrar pelas seguintes propriedades:</p> 
    <ul> 
     <li>[!UICONTROL Assunto]</li> 
     <li>[!UICONTROL ID do evento]</li> 
     <li>[!UICONTROL Hora da data de criação]</li> 
     <li>[!UICONTROL Data da última modificação]</li> 
     <li>[!UICONTROL Body Preview]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Pedido por]</td> 
   <td> <p>Selecione como deseja ordenar os resultados.</p> 
    <ul> 
     <li><strong>[!UICONTROL Assunto]</strong>, ascendente ou descendente</li> 
     <li><strong>[!UICONTROL Hora da data de criação]</strong>, ascendente ou descendente</li> 
     <li><strong>[!UICONTROL Data da última modificação]</strong>, ascendente ou descendente</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limite]</td> 
   <td>Insira o número máximo de eventos [!DNL Workfront Fusion] deve retornar durante um ciclo de execução de cenário.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obter um evento]

Este módulo de ação recupera detalhes do evento especificado.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Office 365] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID do evento]</td> 
   <td> <p>Insira ou mapeie a ID do evento sobre o qual deseja recuperar detalhes.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Criar um evento]

Esse módulo de ação cria um novo evento.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Office 365] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Assunto]</td> 
   <td> <p>Insira ou mapeie um título para o evento criado.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Data de início]</td> 
   <td> Insira um único ponto de tempo em que o evento começa em uma representação de data e hora combinadas. Usar o formato <code>({date}T{time}</code>; por exemplo, <code>2017-08-29T04:00:00.0000000</code>. Para obter uma lista de formatos de data e hora compatíveis, consulte <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Coação de tipo em [!DNL Adobe Workfront Fusion]</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Data final]</td> 
   <td> Insira um único ponto de tempo em que o evento termina em uma representação de data e hora combinadas. Usar o formato <code>{date}T{time}</code>; por exemplo, <code>2017-08-29T04:00:00.0000000</code>. Para obter uma lista de formatos de data e hora compatíveis, consulte <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Coação de tipo em [!DNL Adobe Workfront Fusion]</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Lembrete em]</td> 
   <td>Selecione se deseja ativar um lembrete para este evento.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Lembrete]</td> 
   <td>Insira ou mapeie o número de minutos antes do início do evento quando o lembrete deve ser acionado.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Importância]</td> 
   <td> <p>Selecione a importância desse evento.</p> 
    <ul> 
     <li>[!UICONTROL Baixo]</li> 
     <li>[!UICONTROL Médio]</li> 
     <li>[!UICONTROL Alta]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sensibilidade] </td> 
   <td> <p>Selecione a sensibilidade desse evento.</p> 
    <ul> 
     <li><strong>[!UICONTROL Normal]</strong> </li> 
     <li> <p><strong>[!UICONTROL Pessoal]</strong> </p> <p>O recipient vê uma mensagem "[!UICONTROL Tratar como Pessoal]".</p> </li> 
     <li> <p><strong>[!UICONTROL Privado]</strong> </p> <p>O recipient vê uma mensagem "[!UICONTROL Tratar como privado]". Esse evento não é encaminhado ou redirecionado pelas regras da caixa de entrada do recipient.</p> </li> 
     <li> <p><strong>[!UICONTROL Confidencial]</strong> </p> <p>O recipient vê uma mensagem "[!UICONTROL Por favor, trate isso como confidencial]". </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de conteúdo do corpo]</td> 
   <td>Selecione se o conteúdo do corpo é texto simples ou HTML.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Corpo de conteúdo]</td> 
   <td>Insira ou mapeie o corpo da mensagem associada ao evento. Ele pode estar no HTML ou no formato de texto (conforme especificado no campo [!UICONTROL Body Content Type] acima).</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Local]</td> 
   <td> <p>Insira os detalhes da localização do evento.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Resposta solicitada]</td> 
   <td>Selecionar <strong>[!UICONTROL Sim]</strong> para solicitar que o convidado envie uma resposta ao convite do evento.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Mostrar como]</td> 
   <td> <p>Selecione como deseja que o evento seja exibido para as pessoas que visualizam seu calendário.</p> 
    <ul> 
     <li>[!UICONTROL Gratuito]</li> 
     <li>[!UICONTROL Tentativa]</li> 
     <li>[!UICONTROL Ocupado]</li> 
     <li>[!UICONTROL Fora do escritório]</li> 
     <li>[!UICONTROL Trabalho em outro lugar]</li> 
     <li>[!UICONTROL Desconhecido]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Participantes]</p> </td> 
   <td> <p>Adicione participantes do evento.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Name]</strong> </p> <p>Insira o nome do participante.</p> </li> 
     <li> <p><strong>[!UICONTROL Email]</strong> </p> <p>Insira o endereço de email do participante.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Categoria]</td> 
   <td>Insira ou mapeie as categorias que você deseja que o evento exiba no calendário.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Atualizar um evento]

Esse módulo de ação atualiza um evento existente.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Office 365] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID do evento]</td> 
   <td>Insira, mapeie ou selecione a ID do evento que deseja atualizar.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Assunto]</td> 
   <td> <p>Insira ou mapeie um título para o evento criado.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Data de início]</td> 
   <td> Insira um único ponto de tempo em que o evento começa em uma representação de data e hora combinadas. Usar o formato <code>{date}T{time}</code>; por exemplo, <code>2017-08-29T04:00:00.0000000</code>. Para obter uma lista de formatos de data e hora compatíveis, consulte <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Coação de tipo em [!DNL Adobe Workfront Fusion]</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Data final]</td> 
   <td> Insira um único ponto de tempo em que o evento termina em uma representação de data e hora combinadas. Usar o formato <code>({date}T{time}</code>; por exemplo, <code>2017-08-29T04:00:00.0000000</code>. Para obter uma lista de formatos de data e hora compatíveis, consulte <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Coação de tipo em [!DNL Adobe Workfront Fusion]</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Lembrete em]</td> 
   <td>Selecione se deseja ativar um lembrete para este evento.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Lembrete]</td> 
   <td>Insira ou mapeie o número de minutos antes do início do evento quando o lembrete deve ser acionado.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Importância]</td> 
   <td> <p>Selecione a importância desse evento.</p> 
    <ul> 
     <li>[!UICONTROL Baixo]</li> 
     <li>[!UICONTROL Médio]</li> 
     <li>[!UICONTROL Alta]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sensibilidade] </td> 
   <td> <p>Selecione a sensibilidade desse evento.</p> 
    <ul> 
     <li><strong>[!UICONTROL Normal]</strong> </li> 
     <li> <p><strong>[!UICONTROL Pessoal]</strong> </p> <p>O recipient vê uma mensagem "[!UICONTROL Tratar como Pessoal]".</p> </li> 
     <li> <p><strong>[!UICONTROL Privado]</strong> </p> <p>O recipient vê uma mensagem "[!UICONTROL Tratar como privado]". Esse evento não é encaminhado ou redirecionado pelas regras da caixa de entrada do recipient.</p> </li> 
     <li> <p><strong>[!UICONTROL Confidencial]</strong> </p> <p>O recipient vê uma mensagem "[!UICONTROL Por favor, trate isso como confidencial]". </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de conteúdo do corpo]</td> 
   <td>Selecione se o conteúdo do corpo da mensagem associada ao evento é texto simples ou HTML.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Corpo de conteúdo]</td> 
   <td>Insira ou mapeie o corpo da mensagem associada ao evento. Ele pode estar no HTML ou no formato de texto (conforme especificado no campo [!UICONTROL Body Content Type] acima).</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Local]</td> 
   <td> <p>Insira os detalhes da localização do evento.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Resposta solicitada]</td> 
   <td>Selecionar <strong>[!UICONTROL Sim]</strong> para solicitar que o convidado envie uma resposta ao convite do evento.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Mostrar como]</td> 
   <td> <p>Selecione como deseja que o evento seja exibido para as pessoas que visualizam seu calendário.</p> 
    <ul> 
     <li>[!UICONTROL Gratuito]</li> 
     <li>[!UICONTROL Tentativa]</li> 
     <li>[!UICONTROL Ocupado]</li> 
     <li>[!UICONTROL Fora do escritório]</li> 
     <li>[!UICONTROL Trabalho em outro lugar]</li> 
     <li>[!DNL Unknown]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Participantes]</p> </td> 
   <td> <p>Adicione participantes do evento.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Name]</strong> </p> <p>Insira o nome do participante.</p> </li> 
     <li> <p><strong>[!UICONTROL Email]</strong> </p> <p>Insira o endereço de email do participante.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Categoria]</td> 
   <td>Insira ou mapeie as categorias que você deseja que o evento exiba no calendário.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Excluir um evento]

Esse módulo de ação exclui um evento existente.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Office 365] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID do evento]</td> 
   <td> <p>Insira ou mapeie a ID do evento que deseja excluir.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Calendário

* [[!UICONTROL Calendários de lista]](#list-calendars)
* [[!UICONTROL Obter um calendário]](#get-a-calendar)
* [[!UICONTROL Criar um calendário]](#create-a-calendar)
* [[!UICONTROL Atualizar um calendário]](#update-a-calendar)
* [[!UICONTROL Excluir um calendário]](#delete-a-calendar)

#### [!UICONTROL Calendários de lista]

Este módulo de pesquisa recupera uma lista de todos os calendários do usuário autenticado.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Office 365] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID do grupo de calendário]</td> 
   <td>Selecione o [!UICONTROL calendar group] que contém os calendários que deseja listar.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limite]</td> 
   <td>Inserir o número máximo de calendários [!DNL Workfront Fusion] deve retornar durante um ciclo de execução de cenário.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obter um calendário]

Este módulo de ação recupera detalhes sobre um único calendário.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Office 365] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID do calendário]</td> 
   <td> <p>Insira ou mapeie a ID do calendário sobre o qual deseja recuperar detalhes.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Criar um calendário]

Esse módulo de ação cria um novo calendário em sua conta do Google.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Office 365] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nome do calendário]</td> 
   <td> <p>Insira um nome para o novo calendário.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Atualizar um calendário]

Este módulo de ação edita um calendário existente.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Office 365] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID do calendário]</td> 
   <td>Insira a [!UICONTROL ID do calendário] para o calendário que deseja atualizar. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Novo nome de calendário]</td> 
   <td> <p>Insira um nome para o novo calendário.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Excluir um calendário]

Esse módulo de ação exclui um calendário existente.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Office 365] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID do calendário]</td> 
   <td>Insira a ID do [!UICONTROL Calendário] para o calendário que deseja excluir.</td> 
  </tr> 
 </tbody> 
</table>

### Outro

#### [!UICONTROL Faça uma chamada de API]

Esse módulo permite executar uma chamada de API personalizada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Office 365] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL URL]</p> </td> 
   <td> <p>Insira um caminho relativo a <code>https://graph.microsoft.com</code>. Exemplo:<code> /v1.0/me/events</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Método]</p> </td> 
   td&gt; <p>Selecione o método de solicitação HTTP que você precisa configurar a chamada da API. Para obter mais informações, consulte <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">Métodos de solicitação HTTP em [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cabeçalhos]</td> 
   <td> <p>Adicione os cabeçalhos da solicitação no formato de um objeto JSON padrão. Por exemplo, <code>{"Content-type":"application/json"}</code>. [!DNL Workfront Fusion] adiciona os cabeçalhos de autorização para você.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sequência de consulta]</td> 
   <td> <p> Adicione a query para a chamada de API no formato de um objeto JSON padrão.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Corpo]</td> 
   <td> <p>Adicione o conteúdo do corpo para a chamada da API no formato de um objeto JSON padrão.</p> <p>Nota:   <p>Ao usar declarações condicionais como <code>if</code> no JSON, coloque as aspas fora da declaração condicional.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>">  
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>
