---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;calendars
keywords: conector
navigation-topic: apps-and-their-modules
title: Calendário do Microsoft Office 365
description: Em um cenário  [!DNL Adobe Workfront Fusion] , você pode automatizar fluxos de trabalho que usam o Calendário do Microsoft Office 365, bem como conectá-lo a vários aplicativos e serviços de terceiros.
author: Becky
feature: Workfront Fusion
exl-id: 814c285e-c106-458a-a0b1-760677634f4f
source-git-commit: 7d5f7c21fe38d43fb5601c81b8a31cc80587848f
workflow-type: tm+mt
source-wordcount: '1999'
ht-degree: 0%

---

# [!DNL Microsoft Office 365 Calendar]

Em um cenário [!DNL Adobe Workfront Fusion], você pode automatizar fluxos de trabalho que usam [!DNL Microsoft Office 365 Calendar], bem como conectá-los a vários aplicativos e serviços de terceiros.

Para usar [!DNL Office 365 Calendar] com [!DNL Adobe Workfront Fusion], é necessário ter uma conta [!DNL Office 365 Excel]. Você pode criar um em [www.office.com](https://www.office.com/).

Para obter instruções sobre como conectar sua conta do Office 365 ao [!DNL Workfront Fusion], consulte [Criar uma conexão com o Adobe [!DNL Workfront Fusion] - Instruções básicas](../../workfront-fusion/connections/connect-to-fusion-general.md)

Após consentir, você será redirecionado de volta para a página de administração do [!UICONTROL Workfront Fusion], na qual poderá continuar criando seu cenário.

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
   <p>Requisito atual do produto: se você tiver o Plano [!DNL Adobe Workfront] da [!UICONTROL Select] ou da [!UICONTROL Prime], sua organização deve comprar o [!DNL Adobe Workfront Fusion] e o [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo. [!DNL Workfront Fusion] está incluído no plano [!DNL Workfront] do [!UICONTROL Ultimate].</p>
   <p>Ou</p>
   <p>Requisito de produto herdado: sua organização deve comprar o [!DNL Adobe Workfront Fusion] e o [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Para saber que plano, tipo de licença ou acesso você tem, contate o administrador do [!DNL Workfront].

Para obter informações sobre [!DNL Adobe Workfront Fusion] licenças, consulte [[!DNL Adobe Workfront Fusion] licenças](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Pré-requisitos

Para usar módulos [!DNL Microsoft Office 365 Calendar], você deve ter uma conta [!DNL Microsoft Office 365 Calendar].

## Conectando o serviço [!DNL Office 365 Calendar] a [!DNL Workfront Fusion]

Para obter instruções sobre como conectar sua conta do [!DNL Office 365 Calendar] ao [!UICONTROL Workfront Fusion], consulte [Criar uma conexão com o [!UICONTROL Adobe Workfront Fusion] - Instruções básicas](../../workfront-fusion/connections/connect-to-fusion-general.md)

>[!NOTE]
>
>Alguns aplicativos do Microsoft usam a mesma conexão, que está vinculada a permissões de usuário individuais. Portanto, ao criar uma conexão, a tela de consentimento de permissões exibe todas as permissões que foram concedidas anteriormente à conexão deste usuário, além de todas as novas permissões necessárias para o aplicativo atual.
>
>Por exemplo, se um usuário tiver permissões de &quot;Tabela de leitura&quot; concedidas por meio do conector do Excel e criar uma conexão no conector do Outlook para ler emails, a tela de consentimento de permissões mostrará a permissão &quot;Tabela de leitura&quot; já concedida e a permissão &quot;Gravar email&quot; recém-necessária.

## [!DNL Microsoft Office 365 Calendar] módulos e seus campos

Ao configurar módulos do [!DNL Microsoft Office 365 Calendar], o [!DNL Workfront Fusion] exibe os campos listados abaixo. Junto com esses, campos [!DNL Microsoft Office 365 Calendar] adicionais podem ser exibidos, dependendo de fatores como seu nível de acesso no aplicativo ou serviço. Um título em negrito em um módulo indica um campo obrigatório.

Se você vir o botão de mapa acima de um campo ou função, poderá usá-lo para definir variáveis e funções para esse campo. Para obter mais informações, consulte [Mapear informações de um módulo para outro em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Evento](#event)
* [Calendário](#calendar)
* [Outro](#other)

### Evento

* [[!UICONTROL Assistir a Eventos]](#watch-events)
* [[!UICONTROL Pesquisar Eventos]](#search-events)
* [[!UICONTROL Obter um Evento]](#get-an-event)
* [[!UICONTROL Criar um Evento]](#create-an-event)
* [[!UICONTROL Atualizar um Evento]](#update-an-event)
* [[!UICONTROL Excluir um Evento]](#delete-an-event)

#### [!UICONTROL Assistir a Eventos]

Este módulo de acionador recupera detalhes de um evento quando ele é criado, atualizado, excluído, iniciado ou encerrado no calendário selecionado.

>[!NOTE]
>
>Para procurar ocorrências excluídas de uma série de eventos, selecione [!UICONTROL Por Horário Atualizado] no campo [!UICONTROL Assistir eventos]. Este módulo não observa eventos únicos excluídos ou séries de eventos excluídas.


<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão] </td> 
   <td role="rowheader">[!UICONTROL Conexão] </td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Office 365] ao [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Observar eventos]</td> 
   <td> <p>Selecione como deseja assistir aos eventos.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL por Hora de Criação]</strong> </p> <p>Fique atento a novos eventos.</p> </li> 
     <li> <p><strong>[!UICONTROL por Tempo Atualizado]</strong> </p> <p>Fique atento aos eventos atualizados.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID do Grupo de Calendários]</td> 
   <td>Selecione o [!UICONTROL grupo de calendários] que contém o calendário no qual você deseja assistir aos eventos.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Calendário]</td> 
   <td> <p>Selecione o calendário específico que deseja assistir.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filtro]</td> 
   <td>Defina as condições de filtro para filtrar os resultados por assunto, ID de evento ou corpo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limite]</td> 
   <td> <p>Insira o número máximo de mensagens que [!DNL Workfront Fusion] deve retornar durante um ciclo de execução de cenário.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Pesquisar Eventos]

Este módulo de pesquisa recupera detalhes de um evento quando ele é criado, atualizado, excluído, iniciado ou encerrado no calendário selecionado.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão] </td> 
   <td role="rowheader">[!UICONTROL Conexão] </td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Office 365] ao [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID do Grupo de Calendários]</td> 
   <td>Selecione o [!UICONTROL grupo de calendários] que contém o calendário no qual você deseja assistir aos eventos.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Calendário]</td> 
   <td> <p>Selecione o calendário específico que deseja assistir.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filtro]</td> 
   <td> <p>Defina as condições de filtro para filtrar os resultados. Você pode filtrar pelas seguintes propriedades:</p> 
    <ul> 
     <li>[!UICONTROL Assunto]</li> 
     <li>[!UICONTROL ID de Evento]</li> 
     <li>[!UICONTROL Data/Hora de Criação]</li> 
     <li>[!UICONTROL Data/Hora da Última Modificação]</li> 
     <li>[!UICONTROL Visualização do Corpo]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ordenar por]</td> 
   <td> <p>Selecione como deseja ordenar os resultados.</p> 
    <ul> 
     <li><strong>[!UICONTROL Subject]</strong>, crescente ou decrescente</li> 
     <li><strong>[!UICONTROL Data Hora de Criação]</strong>, crescente ou decrescente</li> 
     <li><strong>[!UICONTROL Data e Hora da Última Modificação]</strong>, crescente ou decrescente</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limite]</td> 
   <td>Insira o número máximo de eventos que [!DNL Workfront Fusion] deve retornar durante um ciclo de execução de cenário.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obter um Evento]

Este módulo de ação recupera detalhes do evento especificado.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão] </td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Office 365] ao [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de Evento]</td> 
   <td> <p>Insira ou mapeie a ID do evento sobre o qual deseja recuperar detalhes.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Criar um Evento]

Este módulo de ação cria um novo evento.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão] </td> 
   <td role="rowheader">[!UICONTROL Conexão] </td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Office 365] ao [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Assunto]</td> 
   <td> <p>Insira ou mapeie um título para o evento criado.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Data de início]</td> 
   <td> Insira um único ponto no tempo quando o evento começa em uma representação combinada de data e hora. Use o formato <code>({date}T{time}</code>; por exemplo, <code>2017-08-29T04:00:00.0000000</code>. Para obter uma lista de formatos de data e hora com suporte, consulte <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Coerção de tipo em [!DNL Adobe Workfront Fusion]</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Data de término]</td> 
   <td> Insira um único ponto no tempo quando o evento termina em uma representação combinada de data e hora. Use o formato <code>{date}T{time}</code>; por exemplo, <code>2017-08-29T04:00:00.0000000</code>. Para obter uma lista de formatos de data e hora com suporte, consulte <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Coerção de tipo em [!DNL Adobe Workfront Fusion]</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Lembrete ativado]</td> 
   <td>Selecione se deseja ativar um lembrete para este evento.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Lembrete]</td> 
   <td>Insira ou mapeie o número de minutos antes do início do evento quando o lembrete deve ser acionado.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Importância]</td> 
   <td> <p>Selecione a importância deste evento.</p> 
    <ul> 
     <li>[!UICONTROL Baixo]</li> 
     <li>[!UICONTROL Medium]</li> 
     <li>[!UICONTROL Alto]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Confidencialidade] </td> 
   <td> <p>Selecione a sensibilidade desse evento.</p> 
    <ul> 
     <li><strong>[!UICONTROL Normal]</strong> </li> 
     <li> <p><strong>[!UICONTROL Pessoal]</strong> </p> <p>O destinatário vê uma mensagem "[!UICONTROL Trata isso como Pessoal]".</p> </li> 
     <li> <p><strong>[!UICONTROL Particular]</strong> </p> <p>O destinatário vê uma mensagem "[!UICONTROL Trate isso como Privado]". Este evento não é encaminhado ou redirecionado pelas regras de caixa de entrada do destinatário.</p> </li> 
     <li> <p><strong>[!UICONTROL Confidencial]</strong> </p> <p>O destinatário vê uma mensagem "[!UICONTROL Tratar como Confidencial]". </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de conteúdo do corpo]</td> 
   <td>Selecione se o conteúdo do corpo é texto sem formatação ou HTML.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conteúdo do corpo]</td> 
   <td>Insira ou mapeie o corpo da mensagem associada ao evento. Pode estar no formato de HTML ou texto (conforme especificado no campo [!UICONTROL Body Content Type] acima).</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Local]</td> 
   <td> <p>Insira os detalhes do local do evento.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Resposta solicitada]</td> 
   <td>Selecione <strong>[!UICONTROL Sim]</strong> para solicitar que o convidado envie uma resposta ao convite de evento.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Mostrar como]</td> 
   <td> <p>Selecione como deseja que o evento seja exibido para as pessoas que visualizam seu calendário.</p> 
    <ul> 
     <li>[!UICONTROL Livre]</li> 
     <li>[!UICONTROL Provisório]</li> 
     <li>[!UICONTROL Ocupado]</li> 
     <li>[!UICONTROL Fora do escritório]</li> 
     <li>[!UICONTROL Trabalhando em outro lugar]</li> 
     <li>[!UICONTROL Desconhecido]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Participantes]</p> </td> 
   <td> <p>Adicionar participantes do evento.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Nome]</strong> </p> <p>Insira o nome do participante.</p> </li> 
     <li> <p><strong>[!UICONTROL Email]</strong> </p> <p>Insira o endereço de email do participante.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Categoria]</td> 
   <td>Insira ou mapeie as categorias que você deseja que o evento exiba como no calendário.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Atualizar um Evento]

Este módulo de ação atualiza um evento existente.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão] </td> 
   <td role="rowheader">[!UICONTROL Conexão] </td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Office 365] ao [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de Evento]</td> 
   <td>Insira, mapeie ou selecione a ID do evento que deseja atualizar.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Assunto]</td> 
   <td> <p>Insira ou mapeie um título para o evento criado.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Data de início]</td> 
   <td> Insira um único ponto no tempo quando o evento começa em uma representação combinada de data e hora. Use o formato <code>{date}T{time}</code>; por exemplo, <code>2017-08-29T04:00:00.0000000</code>. Para obter uma lista de formatos de data e hora com suporte, consulte <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Coerção de tipo em [!DNL Adobe Workfront Fusion]</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Data de término]</td> 
   <td> Insira um único ponto no tempo quando o evento termina em uma representação combinada de data e hora. Use o formato <code>({date}T{time}</code>; por exemplo, <code>2017-08-29T04:00:00.0000000</code>. Para obter uma lista de formatos de data e hora com suporte, consulte <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Coerção de tipo em [!DNL Adobe Workfront Fusion]</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Lembrete ativado]</td> 
   <td>Selecione se deseja ativar um lembrete para este evento.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Lembrete]</td> 
   <td>Insira ou mapeie o número de minutos antes do início do evento quando o lembrete deve ser acionado.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Importância]</td> 
   <td> <p>Selecione a importância deste evento.</p> 
    <ul> 
     <li>[!UICONTROL Baixo]</li> 
     <li>[!UICONTROL Medium]</li> 
     <li>[!UICONTROL Alto]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Confidencialidade] </td> 
   <td> <p>Selecione a sensibilidade desse evento.</p> 
    <ul> 
     <li><strong>[!UICONTROL Normal]</strong> </li> 
     <li> <p><strong>[!UICONTROL Pessoal]</strong> </p> <p>O destinatário vê uma mensagem "[!UICONTROL Trata isso como Pessoal]".</p> </li> 
     <li> <p><strong>[!UICONTROL Particular]</strong> </p> <p>O destinatário vê uma mensagem "[!UICONTROL Trate isso como Privado]". Este evento não é encaminhado ou redirecionado pelas regras de caixa de entrada do destinatário.</p> </li> 
     <li> <p><strong>[!UICONTROL Confidencial]</strong> </p> <p>O destinatário vê uma mensagem "[!UICONTROL Tratar como Confidencial]". </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de conteúdo do corpo]</td> 
   <td>Selecione se o conteúdo do corpo da mensagem associado ao evento é texto sem formatação ou HTML.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conteúdo do corpo]</td> 
   <td>Insira ou mapeie o corpo da mensagem associada ao evento. Pode estar no formato de HTML ou texto (conforme especificado no campo [!UICONTROL Body Content Type] acima).</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Local]</td> 
   <td> <p>Insira os detalhes do local do evento.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Resposta solicitada]</td> 
   <td>Selecione <strong>[!UICONTROL Sim]</strong> para solicitar que o convidado envie uma resposta ao convite de evento.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Mostrar como]</td> 
   <td> <p>Selecione como deseja que o evento seja exibido para as pessoas que visualizam seu calendário.</p> 
    <ul> 
     <li>[!UICONTROL Livre]</li> 
     <li>[!UICONTROL Provisório]</li> 
     <li>[!UICONTROL Ocupado]</li> 
     <li>[!UICONTROL Fora do escritório]</li> 
     <li>[!UICONTROL Trabalhando em outro lugar]</li> 
     <li>[!DNL Unknown]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Participantes]</p> </td> 
   <td> <p>Adicionar participantes do evento.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Nome]</strong> </p> <p>Insira o nome do participante.</p> </li> 
     <li> <p><strong>[!UICONTROL Email]</strong> </p> <p>Insira o endereço de email do participante.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Categoria]</td> 
   <td>Insira ou mapeie as categorias que você deseja que o evento exiba como no calendário.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Excluir um Evento]

Este módulo de ação exclui um evento existente.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão] </td> 
   <td role="rowheader">[!UICONTROL Conexão] </td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Office 365] ao [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de Evento]</td> 
   <td> <p>Informe ou mapeie a ID do evento que deseja deletar.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Calendário

* [[!UICONTROL Listar Calendários]](#list-calendars)
* [[!UICONTROL Obter um Calendário]](#get-a-calendar)
* [[!UICONTROL Criar um Calendário]](#create-a-calendar)
* [[!UICONTROL Atualizar um Calendário]](#update-a-calendar)
* [[!UICONTROL Excluir um Calendário]](#delete-a-calendar)

#### [!UICONTROL Listar Calendários]

Este módulo de pesquisa recupera uma lista de todos os calendários do usuário autenticado.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão] </td> 
   <td role="rowheader">[!UICONTROL Conexão] </td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Office 365] ao [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID do Grupo de Calendários]</td> 
   <td>Selecione o [!UICONTROL grupo de calendários] que contém os calendários que você deseja listar.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limite]</td> 
   <td>Insira o número máximo de calendários que [!DNL Workfront Fusion] deve retornar durante um ciclo de execução de cenário.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obter um Calendário]

Este módulo de ação recupera detalhes sobre um único calendário.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão] </td> 
   <td role="rowheader">[!UICONTROL Conexão] </td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Office 365] ao [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de Calendário]</td> 
   <td> <p>Insira ou mapeie a ID do calendário sobre o qual deseja recuperar detalhes.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Criar um Calendário]

Este módulo de ação cria um novo calendário em sua conta do Google.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão] </td> 
   <td role="rowheader">[!UICONTROL Conexão] </td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Office 365] ao [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nome do calendário]</td> 
   <td> <p>Insira um nome para o novo calendário.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Atualizar um Calendário]

Este módulo de ação edita um calendário existente.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão] </td> 
   <td role="rowheader">[!UICONTROL Conexão] </td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Office 365] ao [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de Calendário]</td> 
   <td>Digite a [!UICONTROL ID de Calendário] do calendário que você deseja atualizar. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nome do Novo Calendário]</td> 
   <td> <p>Insira um nome para o novo calendário.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Excluir um Calendário]

Este módulo de ação exclui um calendário existente.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão] </td> 
   <td role="rowheader">[!UICONTROL Conexão] </td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Office 365] ao [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de Calendário]</td> 
   <td>Insira a ID do [!UICONTROL Calendar] do calendário que você deseja excluir.</td> 
  </tr> 
 </tbody> 
</table>

### Outro

#### [!UICONTROL Fazer uma chamada de API]

Este módulo permite executar uma chamada de API personalizada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão]</td> 
   <td role="rowheader">[!UICONTROL Conexão] </td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Office 365] ao [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL URL]</p> </td> 
   <td> <p>Insira um caminho relativo para <code>https://graph.microsoft.com</code>. Exemplo:<code> /v1.0/me/events</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Método]</p> </td> 
   td&gt; <p>Selecione o método de solicitação HTTP necessário para configurar a chamada de API. Para obter mais informações, consulte <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">Métodos de solicitação HTTP em [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cabeçalhos]</td> 
   <td> <p>Adicione os cabeçalhos da solicitação na forma de um objeto JSON padrão. Por exemplo, <code>{"Content-type":"application/json"}</code>. [!DNL Workfront Fusion] adiciona os cabeçalhos de autorização para você.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cadeia de Consulta]</td> 
   <td> <p> Adicione a consulta da chamada à API na forma de um objeto JSON padrão.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Corpo]</td> 
   <td> <p>Adicione o conteúdo do corpo para a chamada à API na forma de um objeto JSON padrão.</p> <p>Nota:   <p>Ao usar instruções condicionais como <code>if</code> em seu JSON, coloque as aspas fora da instrução condicional.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>">  
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>
