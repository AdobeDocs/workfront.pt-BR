---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;calendars
keywords: conector
navigation-topic: apps-and-their-modules
title: Módulos de calendário do Google
description: Em um [!DNL Adobe Workfront Fusion] você pode automatizar fluxos de trabalho que usam o Google Calendar, bem como conectá-lo a vários aplicativos e serviços de terceiros.
author: Becky
feature: Workfront Fusion
exl-id: 168e8fce-645d-4108-84b7-46a113c83f41
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '3773'
ht-degree: 0%

---

# [!DNL Google Calendar] módulos

Em um [!DNL Adobe Workfront Fusion] , é possível automatizar workflows que usam [!UICONTROL Calendário do Google], bem como conectá-lo a vários aplicativos e serviços de terceiros.

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

Para usar [!DNL Google Calendar] módulos, você deve ter um [!DNL Google] conta.

## [!DNL Google Calendar] módulos e seus campos

Ao configurar [!DNL Google Calendar] módulos, [!DNL Workfront Fusion] exibe os campos listados abaixo. Junto com esses, [!DNL Google Calendar] podem ser exibidos, dependendo de fatores como seu nível de acesso no aplicativo ou serviço. Um título em negrito em um módulo indica um campo obrigatório.

Se o botão de mapa for exibido acima de um campo ou função, é possível usá-lo para definir variáveis e funções para esse campo. Para obter mais informações, consulte [Mapear informações de um módulo para outro no [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Eventos](#events)
* [Calendários](#calendars)
* [Regras de controle de acesso](#access-control-rules)
* [Iteradores (obsoleto)](#iterators-deprecated)
* [Outro](#other)

### Eventos

* [[!UICONTROL Monitoramento de eventos]](#watch-events)
* [[!UICONTROL Pesquisar eventos]](#search-events)
* [[!UICONTROL Obter um evento]](#get-an-event)
* [[!UICONTROL Criar um evento]](#create-an-event)
* [[!UICONTROL Atualizar um evento]](#update-an-event)
* [[!UICONTROL Excluir um evento]](#delete-an-event)


#### [!UICONTROL Monitoramento de eventos]

Esse módulo de acionador executa um cenário quando um novo evento é adicionado, atualizado, excluído, iniciado ou encerrado no calendário especificado. O módulo retorna todos os campos padrão associados ao registro ou registros, juntamente com quaisquer campos e valores personalizados que a conexão acessa. Você pode mapear essas informações em módulos subsequentes do cenário.

Ao configurar esse módulo, os seguintes campos são exibidos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Google Calendar] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o Adobe [!DNL Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Calendário] </td> 
   <td> <p>Selecione o calendário com o qual deseja que o módulo funcione.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Eventos de monitoramento]</td> 
   <td> <p>Escolha se deseja assistir aos eventos por Data de criação, Data de atualização, Data inicial ou Data final.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Mostrar eventos excluídos]</td> 
   <td> <p>Habilite esta opção para incluir eventos que foram excluídos.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Consulta] </td> 
   <td> <p>Insira o texto que deseja pesquisar.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Limite]</td> 
   <td> <p> Defina o número máximo de eventos que [!DNL Workfront Fusion] funciona com durante um ciclo (o número de repetições por execução de cenário). Se o valor estiver definido como muito alto, a conexão pode ser interrompida no lado do serviço de terceiros fornecido (tempo limite). [!DNL Workfront Fusion] não tem influência sobre isso. Recomendamos que você defina um valor menor e defina um valor maior para o número máximo de ciclos ou execute o cenário com mais frequência.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Pesquisar eventos]

Este módulo de ação pesquisa um evento no calendário selecionado.

Especifique o calendário e os parâmetros da pesquisa.

O módulo retorna a ID do evento e quaisquer campos associados, juntamente com quaisquer campos e valores personalizados que a conexão acessa. Você pode mapear essas informações em módulos subsequentes do cenário.

Ao configurar esse módulo, os seguintes campos são exibidos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td>Para obter instruções sobre como conectar seu [!DNL Google Calendar] conta para o Workfront Fusion, consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o Adobe Workfront Fusion - Instruções básicas</a></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID do calendário]</td> 
   <td> <p>Selecione o calendário que deseja pesquisar.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Data de início]</td> 
   <td> <p> Insira ou mapeie a data em que o evento começa. Esse módulo também recupera eventos que começam antes dessa data, que ainda estão ocorrendo na data de início inserida. </p> <p>Para obter uma lista de formatos de data e hora compatíveis, consulte <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Coação de tipo em [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Data final]</td> 
   <td> <p> Insira ou mapeie a data quando o evento terminar. </p> <p> Para obter uma lista de formatos de data e hora compatíveis, consulte <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Coação de tipo em [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Eventos únicos]</td> 
   <td> <p> Ative essa opção para tratar eventos recorrentes como instâncias únicas. Por exemplo, se você tiver uma reunião semanal e essa opção estiver ativada, o módulo retornará a reunião de cada semana como um evento separado.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Consulta]</td> 
   <td> <p>Insira ou mapeie o termo de pesquisa pelo qual deseja pesquisar. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Pedido por]</td> 
   <td> <p>Selecione a ordem dos eventos retornados no resultado.</p> 
    <ul> 
     <li><strong>[!UICONTROL Hora de início]</strong>: Ordenar pela data e hora de início (crescente). Isso só está disponível ao consultar eventos únicos.</li> 
     <li><strong>[!UICONTROL Hora de atualização]</strong>: Ordenar pela última hora de modificação (crescente).</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Limite]</td> 
   <td> <p>Definir o número máximo de eventos [!DNL Workfront Fusion] retorna durante um ciclo de execução.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obter um evento]

Esse módulo de ação retorna os metadados para um único evento no calendário especificado.

Especifique o calendário e o evento.

O módulo retorna a ID do evento e todos os campos associados, juntamente com quaisquer campos e valores personalizados que a conexão acessa. Você pode mapear essas informações em módulos subsequentes do cenário.

Ao configurar esse módulo, os seguintes campos são exibidos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Google Calendar] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o Adobe [!DNL Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID do calendário]</td> 
   <td> <p>Insira ou mapeie a ID do calendário que contém o evento que deseja obter.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID do evento] </td> 
   <td> <p>Insira a ID do evento da variável [!DNL Google Calendar] evento que você deseja obter.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Criar um evento]

Esse módulo de ação cria um evento.

Especifique o calendário e os parâmetros do evento.

O módulo retorna a ID do evento e quaisquer campos associados, juntamente com quaisquer campos e valores personalizados que a conexão acessa. Você pode mapear essas informações em módulos subsequentes do cenário.

Ao configurar esse módulo, os seguintes campos são exibidos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td>Para obter instruções sobre como conectar seu [!DNL Google Calendar] conta para o Workfront Fusion, consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o Adobe Workfront Fusion - Instruções básicas</a></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Criar um evento]</td> 
   <td> <p>Selecione como deseja criar o evento.</p> 
    <ul> 
     <li><b>[!UICONTROL Em Detalhes]</b><p>Essa opção permite colocar mais detalhes sobre o evento.<br></p></li> 
     <li><b>[!UICONTROL Rapidamente]</b><p>Você só precisa selecionar o calendário e inserir um nome para o evento. Você pode incluir detalhes de hora e local no nome e [!DNL Google Calendar] O agendará o evento para esse local e hora.</p></li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID do calendário]</td> 
   <td> <p>Selecione o calendário onde deseja que o evento apareça.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Cor]</td> 
   <td>Selecione a cor que o evento exibe no calendário.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Nome do evento]</td> 
   <td> <p> Insira ou mapeie um nome para o evento. </p> <p>Observação: Se você selecionou [!UICONTROL Adição rápida] no campo [!UICONTROL Criar um evento] , é possível incluir a data e a hora do evento e [!DNL Workfront Fusion] cria o evento para essa data e hora. Exemplo: <code>Appointment at Capitol Hill on June 3rd 10am-10:25am</code>. Se você selecionou [!UICONTROL Adição rápida], mas não incluiu uma data e hora no nome do evento, o evento é criado a partir da hora atual e dura uma hora.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Evento do dia inteiro]</td> 
   <td>Ative essa opção se o evento for um evento de dia inteiro (não requer horários de início e término).</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Data de início]</td> 
   <td> <p>Se esse for um evento de dia inteiro, insira a data de início do evento. </p> <p>Para obter uma lista de formatos de data compatíveis, consulte <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Coação de tipo em [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Data final]</td> 
   <td> <p> Se esse for um evento de dia inteiro, insira a data de término do evento. </p> <p>Para obter uma lista de formatos de data compatíveis, consulte <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Coação de tipo em [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Descrição]</td> 
   <td>Insira ou mapeie uma descrição para o evento. Este campo suporta HTML.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Local]</td> 
   <td>Insira um local para o evento no formulário de texto.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Usar as configurações de lembrete padrão para este evento]</td> 
   <td>Ative esta opção para usar as configurações padrão de lembrete. Se você definir um lembrete personalizado no campo [!UICONTROL Lembrete] , esse valor será definido como Não.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Lembrete] </td> 
   <td> <p>Adicione um lembrete para o evento. Para cada lembrete, selecione o método com o qual deseja ser lembrado e defina por quanto tempo (em minutos) antes do evento que deseja lembrar.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Participantes]</td> 
   <td>Adicione os participantes ao evento. Para cada participante, insira ou mapeie seu nome e endereço de email.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Mostrar como]</td> 
   <td>Selecione se deseja que as pessoas que visualizam seu calendário o vejam como Ocupado ou Disponível durante esse evento.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Visibility] </td> 
   <td> <p>Selecione a visibilidade deste evento. </p> 
    <ul> 
     <li> <p><b>[!UICONTROL Padrão]</b></p> <p>O evento tem a visibilidade definida nas configurações do calendário.</p> </li> 
     <li> <p><b>[!UICONTROL Público]</b></p> <p>Qualquer pessoa com quem o calendário é compartilhado pode ver esse evento.</p> </li> 
     <li> <p><b>[!UICONTROL Privado]</b></p> <p>Somente os participantes podem ver esse evento.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Enviar notificação sobre a criação do evento]</td> 
   <td> <p>Selecione se deseja enviar notificações sobre a criação de um novo evento para todos os convidados, para não[!DNL Google Calendar] convidados, ou ninguém.</p> <p>Dica: Recomendamos usar a opção [!UICONTROL Nenhum] somente para casos de uso de migração.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Convidados podem modificar o evento]</td> 
   <td> <p>Ative essa opção se desejar que os convidados possam modificar esse evento.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Recorrência]</td> 
   <td>Adicione quaisquer regras de recorrência que deseja aplicar a este evento. Cada regra requer uma lista de linhas [!UICONTROL RULE], [!UICONTROL EXRULE], [!UICONTROL RDATE] e [!UICONTROL EXDATE] para um evento recorrente. Observe que as linhas [!UICONTROL DTSTART] e [!UICONTROL DTEND] não são permitidas neste campo; as horas inicial e final do evento são especificadas nos campos inicial e final. Este campo é omitido para eventos únicos ou instâncias de eventos recorrentes. Para obter mais informações, consulte <a href="https://tools.ietf.org/html/rfc5545#section-3.8.5">RFC5545</a>.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Atualizar um evento]

Esse módulo de ação altera um evento existente.

Especifique o calendário e a ID do evento.

O módulo retorna a ID do evento e quaisquer campos associados, juntamente com quaisquer campos e valores personalizados que a conexão acessa. Você pode mapear essas informações em módulos subsequentes do cenário.

Ao configurar esse módulo, os seguintes campos são exibidos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Google Calendar] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o Adobe [!DNL Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Calendário] </td> 
   <td> <p>Selecione o calendário com o qual deseja trabalhar.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID do evento] </td> 
   <td> <p>Insira a ID do evento da ID criada anteriormente [!DNL Google Calendar] que deseja atualizar.</p> </td> 
  </tr> 
 </tbody> 
</table>

Você pode atualizar as informações do evento inserindo novos valores no campo desejado. Para obter detalhes sobre os campos individuais, consulte [[!UICONTROL Criar um evento]](#create-an-event).

#### [!UICONTROL Excluir um evento]

Esse módulo de ação exclui um evento.

Especifique o calendário e a ID do evento.

O módulo retorna a ID do evento e quaisquer campos associados, juntamente com quaisquer campos e valores personalizados que a conexão acessa. Você pode mapear essas informações em módulos subsequentes do cenário.

Ao configurar esse módulo, os seguintes campos são exibidos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Google Calendar] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o Adobe [!DNL Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID do calendário]</td> 
   <td> <p>Selecione o calendário que contém o evento que deseja excluir.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID do evento]</td> 
   <td> <p> Insira a ID de evento de um evento criado anteriormente [!DNL Google Calendar] evento que deseja excluir.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Enviar notificação sobre a exclusão de eventos]</td> 
   <td>Selecione se deseja enviar notificações sobre a exclusão do evento para todos os convidados que não usam [!DNL Google Calendar]ou ninguém.</td> 
  </tr> 
 </tbody> 
</table>

### Calendários

* [[!UICONTROL Listar calendários]](#list-calendars)
* [[!UICONTROL Obter um calendário]](#get-a-calendar)
* [[!UICONTROL Criar um calendário]](#create-a-calendar)
* [[!UICONTROL Atualizar um calendário]](#update-a-calendar)
* [[!UICONTROL Excluir um calendário]](#delete-a-calendar)
* [[!UICONTROL Limpar um calendário]](#clear-a-calendar)

#### [!UICONTROL Listar calendários]

Este módulo de ação retorna os calendários na lista de calendário de um usuário.

O módulo retorna a ID do calendário e quaisquer campos associados, juntamente com quaisquer campos e valores personalizados que a conexão acessa. Você pode mapear essas informações em módulos subsequentes do cenário.

Ao configurar esse módulo, os seguintes campos são exibidos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Google Calendar] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o Adobe [!DNL Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Função de acesso mínimo]</td> 
   <td> <p>Selecione a função de acesso mínimo para o usuário. O módulo retorna calendários com base nessa função de acesso mínima.</p> 
    <ul> 
     <li><strong>[!UICONTROL Free Busy Reader]</strong>: O usuário pode ler informações de disponibilidade. </li> 
     <li><strong>[!UICONTROL Proprietário]</strong>: O usuário pode ler e modificar eventos e acessar listas de controle. </li> 
     <li><strong>[!UICONTROL Reader]</strong>: O usuário pode ler eventos que não são privados. </li> 
     <li><strong>[!UICONTROL Writer]</strong>: O usuário pode ler e modificar eventos.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Mostrar calendários ocultos]</td> 
   <td>Ative essa opção para incluir calendários ocultos na lista que o módulo retorna.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limite]</td> 
   <td>Definir o número máximo de calendários [!DNL Workfront Fusion] retorna durante um ciclo de execução.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obter um calendário]

Este módulo de ação recupera um calendário.

Especifique a ID do calendário que deseja recuperar.

O módulo retorna a ID do registro e quaisquer campos associados, juntamente com quaisquer campos e valores personalizados que a conexão acessa. Você pode mapear essas informações em módulos subsequentes do cenário.

Ao configurar esse módulo, os seguintes campos são exibidos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Google Calendar] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o Adobe [!DNL Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID do calendário]</td> 
   <td> <p>Selecione o calendário que deseja recuperar.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Criar um calendário]

Este módulo de ação cria um novo calendário.

Especifique um nome para o calendário.

O módulo retorna a ID do calendário e quaisquer campos associados, juntamente com quaisquer campos e valores personalizados que a conexão acessa. Você pode mapear essas informações em módulos subsequentes do cenário.

Ao configurar esse módulo, os seguintes campos são exibidos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Google Calendar] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o Adobe [!DNL Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Nome do calendário]</td> 
   <td> <p> Insira um nome para o novo calendário.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Atualizar um calendário]

Este módulo de ação atualiza um calendário.

Especifique a ID do calendário que deseja atualizar.

O módulo retorna a ID do calendário e quaisquer campos associados, juntamente com quaisquer campos e valores personalizados que a conexão acessa. Você pode mapear essas informações em módulos subsequentes do cenário.

Ao configurar esse módulo, os seguintes campos são exibidos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Google Calendar] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o Adobe [!DNL Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID do calendário]</td> 
   <td> <p>Selecione o calendário que deseja atualizar.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Nome do calendário]</td> 
   <td> <p> Insira um novo nome para o calendário.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Excluir um calendário]

Esse módulo de ação exclui um calendário.

Especifique a ID do calendário que deseja excluir.

O módulo retorna a ID do calendário e quaisquer campos associados, juntamente com quaisquer campos e valores personalizados que a conexão acessa. Você pode mapear essas informações em módulos subsequentes do cenário.

Ao configurar esse módulo, os seguintes campos são exibidos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Google Calendar] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o Adobe [!DNL Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID do calendário]</td> 
   <td> <p>Insira ou mapeie a ID do calendário que deseja excluir.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Limpar um calendário]

Este módulo de ação remove todos os eventos do calendário principal de uma conta.

Especifique a conexão que se conecta à conta que contém o calendário que deseja limpar.

O módulo retorna a ID do calendário e quaisquer campos associados, juntamente com quaisquer campos e valores personalizados que a conexão acessa. Você pode mapear essas informações em módulos subsequentes do cenário.

Ao configurar esse módulo, os seguintes campos são exibidos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Google Calendar] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o Adobe [!DNL Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
 </tbody> 
</table>

### Regras de controle de acesso

* [[!UICONTROL Listar regras de controle de acesso]](#list-access-control-rules)
* [[!UICONTROL Obter uma regra de controle de acesso]](#get-an-access-control-rule)
* [[!UICONTROL Criar uma regra de controle de acesso]](#create-an-access-control-rule)
* [[!UICONTROL Atualizar uma regra de controle de acesso]](#update-an-access-control-rule)
* [[!UICONTROL Excluir uma regra de controle de acesso]](#delete-an-access-control-rule)

#### [!UICONTROL Listar regras de controle de acesso]

Este módulo de ação retorna as regras na lista de controle de acesso em um calendário.

Ao configurar esse módulo, os seguintes campos são exibidos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Google Calendar] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o Adobe [!DNL Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID do calendário]</td> 
   <td> <p>Selecione o calendário que contém as regras de controle de acesso que você deseja recuperar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limite]</td> 
   <td>Definir o número máximo de resultados [!DNL Workfront Fusion] retorna durante um ciclo de execução.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obter uma regra de controle de acesso]

Este módulo de ação retorna os metadados de uma regra de controle de acesso.

Ao configurar esse módulo, os seguintes campos são exibidos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Google Calendar] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o Adobe [!DNL Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID do calendário]</td> 
   <td> <p>Selecione o calendário que contém a regra de controle de acesso que você deseja recuperar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID da regra de controle de acesso]</td> 
   <td>Selecione a regra de controle de acesso que deseja recuperar.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Criar uma regra de controle de acesso]

Esse módulo de ação cria uma nova regra de controle de acesso.

Especifique um nome para o calendário.

O módulo retorna a ID da regra de controle de acesso e quaisquer campos associados, juntamente com quaisquer campos e valores personalizados que a conexão acessa. Você pode mapear essas informações em módulos subsequentes do cenário.

Ao configurar esse módulo, os seguintes campos são exibidos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Google Calendar] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o Adobe [!DNL Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID do calendário]</td> 
   <td> <p>Selecione o calendário onde deseja criar uma regra de controle de acesso.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Função]</td> 
   <td> <p>Selecione a função a ser atribuída à regra de acesso. </p> 
    <ul> 
     <li><strong>[!UICONTROL Free Busy Reader]</strong>: O usuário pode ler informações de disponibilidade. </li> 
     <li><strong>[!UICONTROL Proprietário]</strong>: O usuário pode ler e modificar eventos e acessar listas de controle. </li> 
     <li><strong>[!UICONTROL Reader]</strong>: O usuário pode ler eventos que não são privados. </li> 
     <li><strong>[!UICONTROL Writer]</strong>: O usuário pode ler e modificar eventos.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipo]</td> 
   <td> <p>Selecione o tipo de escopo. </p> 
    <ul> 
     <li><strong>[!UICONTROL Padrão]</strong>: O âmbito público. Este é o valor padrão. </li> 
     <li><strong>[!UICONTROL Usuário]</strong>: Limita o escopo a um único usuário. </li> 
     <li><strong>[!UICONTROL Grupo]</strong>: Limita o escopo a um grupo. </li> 
     <li><strong>[!UICONTROL Domínio]</strong>: Limita o escopo a um domínio. </li> 
    </ul> <p>Observação: As permissões concedidas ao escopo [!UICONTROL Padrão] ou público se aplicam a qualquer usuário, autenticado ou não.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Valor]</td> 
   <td>Insira o endereço de email de um usuário ou grupo, ou o nome de um domínio, dependendo do tipo de escopo.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Enviar notificações]</td> 
   <td> <p>Habilite esta opção para enviar notificações sobre a alteração de acesso. </p> <p>Observação: Não há notificações sobre remoção de acesso. </p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Atualizar uma regra de controle de acesso]

Este módulo de ação atualiza uma regra de controle de acesso.

Especifique um nome para o calendário.

O módulo retorna a ID da regra de controle de acesso e quaisquer campos associados, juntamente com quaisquer campos e valores personalizados que a conexão acessa. Você pode mapear essas informações em módulos subsequentes do cenário.

Ao configurar esse módulo, os seguintes campos são exibidos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Google Calendar] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o Adobe [!DNL Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID do calendário]</td> 
   <td> <p>Selecione o calendário que contém a regra de controle de acesso que deseja atualizar.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID da regra de controle de acesso]</td> 
   <td>Selecione a regra de controle de acesso que deseja atualizar.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Função]</td> 
   <td> <p>Selecione a função a ser atribuída à regra de acesso. </p> 
    <ul> 
     <li><strong>[!UICONTROL Nenhum]</strong>: Essa função não fornece acesso.</li> 
     <li><strong>[!UICONTROL Free Busy Reader]</strong>: O usuário pode ler informações de disponibilidade. </li> 
     <li><strong>[!UICONTROL Proprietário]</strong>: O usuário pode ler e modificar eventos e acessar listas de controle. </li> 
     <li><strong>[!UICONTROL Reader]</strong>: O usuário pode ler eventos que não são privados. </li> 
     <li><strong>[!UICONTROL Writer]</strong>: O usuário pode ler e modificar eventos.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Enviar notificações]</td> 
   <td> <p>Habilite esta opção para enviar notificações sobre a alteração de acesso. </p> <p>Observação: Não há notificações sobre remoção de acesso. </p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Excluir uma regra de controle de acesso]

Esse módulo de ação exclui uma regra de controle de acesso.

Especifique um nome para o calendário.

O módulo retorna a ID da regra de controle de acesso e quaisquer campos associados, juntamente com quaisquer campos e valores personalizados que a conexão acessa. Você pode mapear essas informações em módulos subsequentes do cenário.

Ao configurar esse módulo, os seguintes campos são exibidos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Google Calendar] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o Adobe [!DNL Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID do calendário]</td> 
   <td> <p>Selecione ou mapeie a ID do calendário que contém a regra de controle de acesso que deseja excluir.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID da regra de controle de acesso]</td> 
   <td>Selecione ou mapeie a ID da regra de controle de acesso que deseja excluir.</td> 
  </tr> 
 </tbody> 
</table>

### Iteradores (obsoleto)

O [!UICONTROL iterar anexos] e [!UICONTROL iterar participantes] os módulos foram descontinuados. Para iterar anexos ou participantes, use o [!UICONTROL Controle de fluxo] > [!UICONTROL Iterador] módulo. Para obter mais informações, consulte [Módulo iterador em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/iterator-module.md)

### Outro

* [[!UICONTROL Faça uma chamada de API]](#make-an-api-call)
* [[!UICONTROL Obter informações de disponibilidade]](#get-freebusy-information)

#### [!UICONTROL Faça uma chamada de API]

Esse módulo permite executar uma chamada de API personalizada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL Google Calendar] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o Adobe [!DNL Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL URL]</p> </td> 
   <td>Insira um caminho relativo a <code>https://www.googleapis.com/calendar</code>. Exemplo: <code>/v3/users/me/calendarList</code></td> 
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

#### [!UICONTROL Obter informações de disponibilidade]

Este módulo de ação retorna informações de disponibilidade para um conjunto de calendários.

O módulo retorna a ID do calendário e quaisquer campos associados, juntamente com quaisquer campos e valores personalizados que a conexão acessa. Você pode mapear essas informações em módulos subsequentes do cenário.

Ao configurar esse módulo, os seguintes campos são exibidos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td>Para obter instruções sobre como conectar seu [!DNL Google Calendar] conta para o Workfront Fusion, consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o Adobe Workfront Fusion - Instruções básicas</a></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Horário mínimo]</td> 
   <td> <p> Insira o início do intervalo para o qual você deseja recuperar informações.</p> <p> Para obter uma lista de formatos de data e hora compatíveis, consulte <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Coação de tipo em [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tempo máximo]</td> 
   <td> <p> Insira o final do intervalo para o qual você deseja recuperar informações. </p> <p>Para obter uma lista de formatos de data e hora compatíveis, consulte <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Coação de tipo em [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Calendários]</td> 
   <td> <p>Para cada calendário do qual você deseja recuperar informações, clique em <strong>Adicionar</strong> e insira ou mapeie a ID do calendário.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Acionar um cenário antes de um evento

Você pode acionar um cenário em um horário especificado antes de um evento com a ajuda do [!DNL Google Calendar] lembretes de email e o [!UICONTROL Webhooks] >[!UICONTROL Logotipo personalizado] módulo.

1. Use o [!UICONTROL Calendário do Google] >[!UICONTROL Atualizar um evento] para adicionar um lembrete de email ao seu evento:

   ![](assets/trigger-scen-before-event-350x209.png)

1. Crie um novo cenário começando com a variável [!UICONTROL Webhooks] >[!UICONTROL Logotipo personalizado] módulo.

   1. Copie o endereço de email do mailhook.
   1. Salve o cenário e execute-o.

1. Em [!DNL Gmail]redirecione o [!DNL Google Calendar] lembretes de email para o endereço de email do mailhook:

   1. Abra seu **[!UICONTROL [!DNL Gmail]configurações]**.
   1. Abra o **[!UICONTROL Encaminhamento e POP/IMAP]** guia .
   1. Clique em **[!UICONTROL Adicionar um endereço de encaminhamento].**
   1. Cole o endereço de email dos ganchos de correio copiados, clique em &#x200B;**[!UICONTROL Próximo]** confirme se pressionando **[!UICONTROL Continue]** na janela pop-up e, em seguida, clique em **[!UICONTROL OK]**.

   1. Em [!DNL Workfront Fusion], alterne para o novo cenário que deve terminar a execução ao receber o email de confirmação.
   1. Clique na bolha acima do módulo para inspecionar a saída do módulo.
   1. Expanda o `Text` e copie o código de confirmação:

      ![](assets/confirmation-code-350x252.png)

   1. No Gmail, cole o código de confirmação na caixa de edição e clique em &#x200B;**[!UICONTROL Verificar]**:

      ![](assets/paste-code-350x46.png)

   1. Abra o **[!UICONTROL Filtros e endereços bloqueados]** guia .
   1. Clique em **[!UICONTROL Criar um novo filtro]**.
   1. Configurar um filtro para todos os emails provenientes de `     calendar-notification@google.com` e clique em &#x200B;**[!UICONTROL Criar um filtro]**:
   1. Selecionar **[!UICONTROL Encaminhar para]** e escolha o endereço de email dos anzóis na lista.
   1. Clique em **[!UICONTROL Criar filtro]** para criar o filtro.

1. (Opcional) Em [!DNL Workfront Fusion], adicione o [!UICONTROL Analisador de texto] > [!UICONTROL Corresponder padrão] após a [!UICONTROL Webhooks] >[!UICONTROL Logotipo personalizado] para analisar o código de HTML do email para obter as informações necessárias.

   Por exemplo, você pode configurar o módulo da seguinte maneira para obter a ID do evento:

   *Padrão*: `<meta itemprop="eventId/googleCalendar" content="(?<evenitID>.*?)"/>`

   *Texto*: O `HTML content` item enviado do [!UICONTROL Webhooks] >[!UICONTROL Logotipo personalizado] módulo.
