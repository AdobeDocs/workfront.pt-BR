---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;calendars
keywords: conector
navigation-topic: apps-and-their-modules
title: Módulos do Google Calendar
description: A documentação do Adobe Workfront Fusion foi movida para um novo local. Este artigo foi descontinuado, mas contém um link para o novo artigo que aborda essa funcionalidade.
author: Becky
feature: Workfront Fusion
exl-id: 168e8fce-645d-4108-84b7-46a113c83f41
source-git-commit: efbe888d370e20c895dc40f18f999f2d01ec6337
workflow-type: tm+mt
source-wordcount: '3889'
ht-degree: 0%

---

# [!DNL Google Calendar] módulos

>[!IMPORTANT]
>
>A documentação do Adobe Workfront Fusion foi movida para um novo local.
>
>As informações neste artigo agora podem ser encontradas no artigo:
>
>* [Módulos do Calendário do Google](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/google-calendar-modules.html)
>
>Atualize todos os marcadores.
>
>Este artigo não está mais sendo atualizado e será removido em breve.

Em um cenário [!DNL Adobe Workfront Fusion], você pode automatizar fluxos de trabalho que usam o [!UICONTROL Calendário do Google], bem como conectá-lo a vários aplicativos e serviços de terceiros.

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

Para usar módulos [!DNL Google Calendar], você deve ter uma conta [!DNL Google].

## Informações da API do calendário do Google

O conector do Calendário do Google usa o seguinte:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">URL base</td> 
   <td> https://www.googleapis.com/calendar/v3</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Versão da API</td> 
   <td> v3 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Tag da API</td> 
   <td>v5.4.5</td> 
  </tr>
 </tbody> 
 </table>

## [!DNL Google Calendar] módulos e seus campos

Ao configurar módulos do [!DNL Google Calendar], o [!DNL Workfront Fusion] exibe os campos listados abaixo. Junto com esses, campos [!DNL Google Calendar] adicionais podem ser exibidos, dependendo de fatores como seu nível de acesso no aplicativo ou serviço. Um título em negrito em um módulo indica um campo obrigatório.

Se você vir o botão de mapa acima de um campo ou função, poderá usá-lo para definir variáveis e funções para esse campo. Para obter mais informações, consulte [Mapear informações de um módulo para outro em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Eventos](#events)
* [Calendários](#calendars)
* [Regras de controle de acesso](#access-control-rules)
* [Iteradores (obsoleto)](#iterators-deprecated)
* [Outro](#other)

### Eventos

* [[!UICONTROL Assistir a eventos]](#watch-events)
* [[!UICONTROL Pesquisar eventos]](#search-events)
* [[!UICONTROL Obter um evento]](#get-an-event)
* [[!UICONTROL Criar um evento]](#create-an-event)
* [[!UICONTROL Atualizar um evento]](#update-an-event)
* [[!UICONTROL Excluir um evento]](#delete-an-event)


#### [!UICONTROL Assistir a eventos]

Esse módulo de acionamento executa um cenário quando um novo evento é adicionado, atualizado, excluído, iniciado ou encerrado no calendário especificado. O módulo retorna todos os campos padrão associados ao registro ou aos registros, juntamente com quaisquer campos e valores personalizados que a conexão acesse. Você pode mapear essas informações em módulos subsequentes no cenário.

Ao configurar esse módulo, os campos a seguir são exibidos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexão] </td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Google Calendar] ao [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o Adobe [!DNL Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Calendário] </td> 
   <td> <p>Selecione o calendário com o qual deseja que o módulo funcione.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Observar Eventos]</td> 
   <td> <p>Escolha se deseja monitorar eventos por Data de Criação, Data de Atualização, Data Inicial ou Data Final.</p> </td> 
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
   <td> <p> Defina o número máximo de eventos com os quais [!DNL Workfront Fusion] trabalha durante um ciclo (o número de repetições por execução de cenário). Se o valor for definido como muito alto, a conexão pode ser interrompida no lado do serviço de terceiros especificado (tempo limite). [!DNL Workfront Fusion] não tem nenhuma influência sobre isso. Recomendamos que você defina um valor mais baixo e defina um valor mais alto para o número máximo de ciclos ou execute o cenário com mais frequência.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Pesquisar eventos]

Este módulo de ação procura um evento no calendário selecionado.

Você especifica o calendário e os parâmetros da pesquisa.

O módulo retorna a ID do evento e quaisquer campos associados, juntamente com quaisquer campos e valores personalizados que a conexão acessa. Você pode mapear essas informações em módulos subsequentes no cenário.

Ao configurar esse módulo, os campos a seguir são exibidos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexão] </td> 
   <td>Para obter instruções sobre como conectar sua conta do [!DNL Google Calendar] ao Workfront Fusion, consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o Adobe Workfront Fusion - Instruções básicas</a></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID de Calendário]</td> 
   <td> <p>Selecione o calendário que deseja pesquisar.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Data de início]</td> 
   <td> <p> Insira ou mapeie a data de início do evento. Esse módulo também recupera eventos iniciados antes dessa data, que ainda estão ocorrendo na data inicial inserida. </p> <p>Para obter uma lista de formatos de data e hora com suporte, consulte <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Coerção de tipo em [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Data de término]</td> 
   <td> <p> Insira ou mapeie a data de término do evento. </p> <p> Para obter uma lista de formatos de data e hora com suporte, consulte <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Coerção de tipo em [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Eventos únicos]</td> 
   <td> <p> Habilite esta opção para tratar eventos recorrentes como instâncias únicas. Por exemplo, se você tiver uma reunião semanal e essa opção estiver habilitada, o módulo retornará a reunião de cada semana como um evento separado.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Consulta]</td> 
   <td> <p>Informe ou mapeie o termo de pesquisa pelo qual deseja pesquisar. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ordenar por]</td> 
   <td> <p>Selecione a ordem dos eventos retornados no resultado.</p> 
    <ul> 
     <li><strong>[!UICONTROL Hora de Início]</strong>: Ordenar pela data e hora de início (em ordem crescente). Isso só está disponível ao consultar eventos únicos.</li> 
     <li><strong>[!UICONTROL Hora de Atualização]</strong>: Ordenar pela hora da última modificação (em ordem crescente).</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Limite]</td> 
   <td> <p>Defina o número máximo de eventos que [!DNL Workfront Fusion] retorna durante um ciclo de execução.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obter um evento]

Este módulo de ação retorna os metadados de um único evento no calendário especificado.

Você especifica o calendário e o evento.

O módulo retorna a ID do evento e todos os campos associados, juntamente com quaisquer campos e valores personalizados que a conexão acessa. Você pode mapear essas informações em módulos subsequentes no cenário.

Ao configurar esse módulo, os campos a seguir são exibidos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexão] </td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Google Calendar] ao [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o Adobe [!DNL Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID de Calendário]</td> 
   <td> <p>Insira ou mapeie a ID do calendário que contém o evento que você deseja obter.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID de Evento] </td> 
   <td> <p>Insira a ID do evento [!DNL Google Calendar] existente que você deseja obter.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Criar um evento]

Esse módulo de ação cria um evento.

Você especifica o calendário e os parâmetros do evento.

O módulo retorna a ID do evento e quaisquer campos associados, juntamente com quaisquer campos e valores personalizados que a conexão acessa. Você pode mapear essas informações em módulos subsequentes no cenário.

Ao configurar esse módulo, os campos a seguir são exibidos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexão] </td> 
   <td>Para obter instruções sobre como conectar sua conta do [!DNL Google Calendar] ao Workfront Fusion, consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o Adobe Workfront Fusion - Instruções básicas</a></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Criar um Evento]</td> 
   <td> <p>Selecione como deseja criar o evento.</p> 
    <ul> 
     <li><b>[!UICONTROL Em Detalhes]</b><p>Essa opção permite que você insira mais detalhes sobre o evento.<br></p></li> 
     <li><b>[!UICONTROL Rapidamente]</b><p>Você só precisa selecionar o calendário e inserir um nome para o evento. Você pode incluir detalhes de hora e local no nome, e o [!DNL Google Calendar] agendará o evento para esse local e hora.</p></li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID de Calendário]</td> 
   <td> <p>Selecione o calendário no qual deseja que o evento apareça.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Cor]</td> 
   <td>Selecione a cor que o evento mostra no calendário.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Nome do evento]</td> 
   <td> <p> Insira ou mapeie um nome para o evento. </p> <p>Observação: se você tiver selecionado [!UICONTROL Adição rápida] no campo [!UICONTROL Criar um evento], será possível incluir a data e a hora do evento, e [!DNL Workfront Fusion] criará o evento para essa data e hora. Exemplo: <code>Appointment at Capitol Hill on June 3rd 10am-10:25am</code>. Se você selecionou [!UICONTROL Adição rápida], mas não incluiu uma data e hora no nome do evento, o evento será criado a partir da hora atual e terá duração de uma hora.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Evento de dia inteiro]</td> 
   <td>Ative essa opção se o evento for um evento de dia inteiro (não requer horas de início e término).</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Data de início]</td> 
   <td> <p>Se esse for um evento de dia inteiro, insira a data de início do evento. </p> <p>Para obter uma lista de formatos de data com suporte, consulte <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Coerção de tipo em [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Data de término]</td> 
   <td> <p> Se esse for um evento de dia inteiro, insira a data de término do evento. </p> <p>Para obter uma lista de formatos de data com suporte, consulte <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Coerção de tipo em [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Descrição]</td> 
   <td>Insira ou mapeie uma descrição para o evento. Este campo suporta HTML.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Local]</td> 
   <td>Insira um local para o evento em formato de texto.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Usar as configurações padrão de lembrete para este evento]</td> 
   <td>Habilite esta opção para usar as configurações padrão de lembrete. Se você definir um lembrete personalizado no campo [!UICONTROL Lembrete], esse valor será definido como Não.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Lembrete] </td> 
   <td> <p>Adicionar lembrete para o evento. Para cada lembrete, selecione o método com o qual deseja ser lembrado e defina por quanto tempo (em minutos) antes do evento que deseja ser lembrado.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Participantes]</td> 
   <td>Adicionar os participantes ao evento. Para cada participante, insira ou mapeie seu nome e endereço de email.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Mostrar-me como]</td> 
   <td>Selecione se você deseja que as pessoas que exibem seu calendário o vejam como Ocupado ou Disponível durante este evento.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Visibilidade] </td> 
   <td> <p>Selecione a visibilidade deste evento. </p> 
    <ul> 
     <li> <p><b>[!UICONTROL Padrão]</b></p> <p>O evento tem a visibilidade definida nas configurações do calendário.</p> </li> 
     <li> <p><b>[!UICONTROL Público]</b></p> <p>Qualquer pessoa com quem o calendário é compartilhado pode ver este evento.</p> </li> 
     <li> <p><b>[!UICONTROL Privado]</b></p> <p>Somente os participantes podem ver este evento.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Enviar notificação sobre a criação de evento]</td> 
   <td> <p>Selecione se deseja enviar notificações sobre a criação de um novo evento para todos os convidados, para convidados que não sejam [!DNL Google Calendar] ou para ninguém.</p> <p>Dica: recomendamos usar a opção [!UICONTROL Nenhum] somente para casos de uso de migração.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Convidados podem modificar o evento]</td> 
   <td> <p>Ative esta opção se quiser que os convidados modifiquem este evento.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Recorrência]</td> 
   <td>Adicione todas as regras de recorrência que deseja aplicar a este evento. Cada regra exige uma lista de linhas [!UICONTROL RRULE], [!UICONTROL EXRULE], [!UICONTROL RDATE] e [!UICONTROL EXDATE] para um evento recorrente. Observe que as linhas [!UICONTROL DTSTART] e [!UICONTROL DTEND] não são permitidas neste campo; as horas de início e término do evento são especificadas nos campos de início e término. Esse campo é omitido para eventos únicos ou instâncias de eventos recorrentes. Para obter mais informações, consulte <a href="https://tools.ietf.org/html/rfc5545#section-3.8.5">RFC5545</a>.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Atualizar um evento]

Esse módulo de ação altera um evento existente.

Você especifica o calendário e a ID do evento.

O módulo retorna a ID do evento e quaisquer campos associados, juntamente com quaisquer campos e valores personalizados que a conexão acessa. Você pode mapear essas informações em módulos subsequentes no cenário.

Ao configurar esse módulo, os campos a seguir são exibidos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexão] </td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Google Calendar] ao [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o Adobe [!DNL Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Calendário] </td> 
   <td> <p>Selecione o calendário com o qual deseja trabalhar.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID de Evento] </td> 
   <td> <p>Insira a ID do evento [!DNL Google Calendar] criado anteriormente que você deseja atualizar.</p> </td> 
  </tr> 
 </tbody> 
</table>

Você pode atualizar as informações do evento inserindo novos valores no campo desejado. Para obter detalhes sobre os campos individuais, consulte [[!UICONTROL Criar um evento]](#create-an-event).

#### [!UICONTROL Excluir um evento]

Este módulo de ação exclui um evento.

Você especifica o calendário e a ID do evento.

O módulo retorna a ID do evento e quaisquer campos associados, juntamente com quaisquer campos e valores personalizados que a conexão acessa. Você pode mapear essas informações em módulos subsequentes no cenário.

Ao configurar esse módulo, os campos a seguir são exibidos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexão] </td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Google Calendar] ao [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o Adobe [!DNL Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID de Calendário]</td> 
   <td> <p>Selecione o calendário que contém o evento que você deseja excluir.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID de Evento]</td> 
   <td> <p> Insira a ID de evento de um evento [!DNL Google Calendar] criado anteriormente que você deseja excluir.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Enviar notificação sobre a exclusão do evento]</td> 
   <td>Selecione se deseja enviar notificações sobre a exclusão do evento para todos os convidados, convidados que não usam [!DNL Google Calendar] ou ninguém.</td> 
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

Este módulo de ação retorna os calendários na lista de calendários de um usuário.

O módulo retorna a ID do calendário e quaisquer campos associados, juntamente com quaisquer campos e valores personalizados que a conexão acessa. Você pode mapear essas informações em módulos subsequentes no cenário.

Ao configurar esse módulo, os campos a seguir são exibidos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão] </td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Google Calendar] ao [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o Adobe [!DNL Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Função de acesso mínimo]</td> 
   <td> <p>Selecione a função de acesso mínimo para o usuário. O módulo retorna calendários com base nesta função de acesso mínimo.</p> 
    <ul> 
     <li><strong>[!UICONTROL Reader de Disponibilidade]</strong>: O usuário pode ler informações de disponibilidade. </li> 
     <li><strong>[!UICONTROL Proprietário]</strong>: O usuário pode ler e modificar eventos e acessar listas de controle. </li> 
     <li><strong>[!UICONTROL Reader]</strong>: O usuário pode ler eventos que não são privados. </li> 
     <li><strong>[!UICONTROL Writer]</strong>: o usuário pode ler e modificar eventos.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Mostrar calendários ocultos]</td> 
   <td>Habilite esta opção para incluir calendários ocultos na lista que o módulo retorna.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limite]</td> 
   <td>Defina o número máximo de calendários que [!DNL Workfront Fusion] retorna durante um ciclo de execução.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obter um calendário]

Este módulo de ação recupera um calendário.

Você especifica a ID do calendário que deseja recuperar.

O módulo retorna a ID do registro e quaisquer campos associados, juntamente com quaisquer campos e valores personalizados que a conexão acessa. Você pode mapear essas informações em módulos subsequentes no cenário.

Ao configurar esse módulo, os campos a seguir são exibidos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão] </td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Google Calendar] ao [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o Adobe [!DNL Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de Calendário]</td> 
   <td> <p>Selecione o calendário que deseja recuperar.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Criar um calendário]

Este módulo de ação cria um novo calendário.

Você especifica um nome para o calendário.

O módulo retorna a ID do calendário e quaisquer campos associados, juntamente com quaisquer campos e valores personalizados que a conexão acessa. Você pode mapear essas informações em módulos subsequentes no cenário.

Ao configurar esse módulo, os campos a seguir são exibidos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexão] </td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Google Calendar] ao [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o Adobe [!DNL Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Nome do calendário]</td> 
   <td> <p> Insira um nome para o novo calendário.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Atualizar um calendário]

Este módulo de ação atualiza um calendário.

Você especifica a ID do calendário que deseja atualizar.

O módulo retorna a ID do calendário e quaisquer campos associados, juntamente com quaisquer campos e valores personalizados que a conexão acessa. Você pode mapear essas informações em módulos subsequentes no cenário.

Ao configurar esse módulo, os campos a seguir são exibidos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexão] </td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Google Calendar] ao [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o Adobe [!DNL Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID de Calendário]</td> 
   <td> <p>Selecione o calendário que deseja atualizar.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Nome do calendário]</td> 
   <td> <p> Digite um novo nome para o calendário.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Excluir um calendário]

Este módulo de ação exclui um calendário.

Você especifica a ID do calendário que deseja excluir.

O módulo retorna a ID do calendário e quaisquer campos associados, juntamente com quaisquer campos e valores personalizados que a conexão acessa. Você pode mapear essas informações em módulos subsequentes no cenário.

Ao configurar esse módulo, os campos a seguir são exibidos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão] </td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Google Calendar] ao [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o Adobe [!DNL Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de Calendário]</td> 
   <td> <p>Insira ou mapeie a ID do calendário que deseja excluir.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Limpar um calendário]

Este módulo de ação remove todos os eventos do calendário principal de uma conta.

Você especifica a conexão que se conecta à conta que contém o calendário que deseja limpar.

O módulo retorna a ID do calendário e quaisquer campos associados, juntamente com quaisquer campos e valores personalizados que a conexão acessa. Você pode mapear essas informações em módulos subsequentes no cenário.

Ao configurar esse módulo, os campos a seguir são exibidos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão] </td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Google Calendar] ao [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o Adobe [!DNL Workfront Fusion] - Instruções básicas</a></p> </td> 
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

Este módulo de ação retorna as regras da lista de controle de acesso em um calendário.

Ao configurar esse módulo, os campos a seguir são exibidos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão] </td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Google Calendar] ao [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o Adobe [!DNL Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de Calendário]</td> 
   <td> <p>Selecione o calendário que contém as regras de controle de acesso que você deseja recuperar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limite]</td> 
   <td>Defina o número máximo de resultados que [!DNL Workfront Fusion] retorna durante um ciclo de execução.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obter uma regra de controle de acesso]

Este módulo de ação retorna os metadados de uma regra de controle de acesso.

Ao configurar esse módulo, os campos a seguir são exibidos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão] </td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Google Calendar] ao [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o Adobe [!DNL Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de Calendário]</td> 
   <td> <p>Selecione o calendário que contém a regra de controle de acesso que você deseja recuperar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID da regra de controle de acesso]</td> 
   <td>Selecione a regra de controle de acesso que deseja recuperar.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Criar uma regra de controle de acesso]

Este módulo de ação cria uma nova regra de controle de acesso.

Você especifica um nome para o calendário.

O módulo retorna a ID da regra de controle de acesso e quaisquer campos associados, juntamente com quaisquer campos e valores personalizados que a conexão acessa. Você pode mapear essas informações em módulos subsequentes no cenário.

Ao configurar esse módulo, os campos a seguir são exibidos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexão] </td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Google Calendar] ao [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o Adobe [!DNL Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID de Calendário]</td> 
   <td> <p>Selecione o calendário no qual deseja criar uma regra de controle de acesso.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Função]</td> 
   <td> <p>Selecione a função a ser atribuída à regra de acesso. </p> 
    <ul> 
     <li><strong>[!UICONTROL Reader de Disponibilidade]</strong>: O usuário pode ler informações de disponibilidade. </li> 
     <li><strong>[!UICONTROL Proprietário]</strong>: O usuário pode ler e modificar eventos e acessar listas de controle. </li> 
     <li><strong>[!UICONTROL Reader]</strong>: O usuário pode ler eventos que não são privados. </li> 
     <li><strong>[!UICONTROL Writer]</strong>: o usuário pode ler e modificar eventos.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipo]</td> 
   <td> <p>Selecione o tipo de escopo. </p> 
    <ul> 
     <li><strong>[!UICONTROL Padrão]</strong>: O escopo público. Este é o valor padrão. </li> 
     <li><strong>[!UICONTROL Usuário]</strong>: Limita o escopo a um único usuário. </li> 
     <li><strong>[!UICONTROL Group]</strong>: Limita o escopo a um grupo. </li> 
     <li><strong>[!UICONTROL Domínio]</strong>: Limita o escopo a um domínio. </li> 
    </ul> <p>Observação: as permissões concedidas ao escopo [!UICONTROL Padrão], ou público, aplicam-se a qualquer usuário, autenticado ou não.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Valor]</td> 
   <td>Insira o endereço de email de um usuário ou grupo, ou o nome de um domínio, dependendo do tipo de escopo.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Enviar notificações]</td> 
   <td> <p>Habilite esta opção para enviar notificações sobre a alteração de acesso. </p> <p>Observação: não há notificações sobre a remoção de acesso. </p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Atualizar uma regra de controle de acesso]

Este módulo de ação atualiza uma regra de controle de acesso.

Você especifica um nome para o calendário.

O módulo retorna a ID da regra de controle de acesso e quaisquer campos associados, juntamente com quaisquer campos e valores personalizados que a conexão acessa. Você pode mapear essas informações em módulos subsequentes no cenário.

Ao configurar esse módulo, os campos a seguir são exibidos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexão] </td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Google Calendar] ao [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o Adobe [!DNL Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID de Calendário]</td> 
   <td> <p>Selecione o calendário que contém a regra de controle de acesso que você deseja atualizar.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID da regra de controle de acesso]</td> 
   <td>Selecione a regra de controle de acesso que deseja atualizar.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Função]</td> 
   <td> <p>Selecione a função a ser atribuída à regra de acesso. </p> 
    <ul> 
     <li><strong>[!UICONTROL Nenhum]</strong>: esta função não fornece acesso.</li> 
     <li><strong>[!UICONTROL Reader de Disponibilidade]</strong>: O usuário pode ler informações de disponibilidade. </li> 
     <li><strong>[!UICONTROL Proprietário]</strong>: O usuário pode ler e modificar eventos e acessar listas de controle. </li> 
     <li><strong>[!UICONTROL Reader]</strong>: O usuário pode ler eventos que não são privados. </li> 
     <li><strong>[!UICONTROL Writer]</strong>: o usuário pode ler e modificar eventos.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Enviar notificações]</td> 
   <td> <p>Habilite esta opção para enviar notificações sobre a alteração de acesso. </p> <p>Observação: não há notificações sobre a remoção de acesso. </p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Excluir uma regra de controle de acesso]

Este módulo de ação exclui uma regra de controle de acesso.

Você especifica um nome para o calendário.

O módulo retorna a ID da regra de controle de acesso e quaisquer campos associados, juntamente com quaisquer campos e valores personalizados que a conexão acessa. Você pode mapear essas informações em módulos subsequentes no cenário.

Ao configurar esse módulo, os campos a seguir são exibidos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexão] </td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Google Calendar] ao [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o Adobe [!DNL Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID de Calendário]</td> 
   <td> <p>Selecione ou mapeie a ID do calendário que contém a regra de controle de acesso que você deseja excluir.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID da regra de controle de acesso]</td> 
   <td>Selecione ou mapeie a ID da regra de controle de acesso que deseja excluir.</td> 
  </tr> 
 </tbody> 
</table>

### Iteradores (obsoleto)

Os módulos [!UICONTROL iterar anexos] e [!UICONTROL iterar participantes] foram descontinuados. Para iterar anexos ou participantes, use o módulo [!UICONTROL Controle de Fluxo] > [!UICONTROL Iterador]. Para obter mais informações, consulte [Módulo Iterador em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/iterator-module.md)

### Outro

* [[!UICONTROL Fazer uma chamada de API]](#make-an-api-call)
* [[!UICONTROL Obter Informações de Disponibilidade]](#get-freebusy-information)

#### [!UICONTROL Fazer uma chamada de API]

Este módulo permite executar uma chamada de API personalizada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão]</td> 
   <td> <p>Para obter instruções sobre como conectar sua conta do [!DNL Google Calendar] ao [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o Adobe [!DNL Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL URL]</p> </td> 
   <td>Insira um caminho relativo para <code>https://www.googleapis.com/calendar</code>. Exemplo: <code>/v3/users/me/calendarList</code></td> 
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

#### [!UICONTROL Obter Informações de Disponibilidade]

Este módulo de ação retorna informações de disponibilidade para um conjunto de calendários.

O módulo retorna a ID do calendário e quaisquer campos associados, juntamente com quaisquer campos e valores personalizados que a conexão acessa. Você pode mapear essas informações em módulos subsequentes no cenário.

Ao configurar esse módulo, os campos a seguir são exibidos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexão] </td> 
   <td>Para obter instruções sobre como conectar sua conta do [!DNL Google Calendar] ao Workfront Fusion, consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o Adobe Workfront Fusion - Instruções básicas</a></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tempo mínimo]</td> 
   <td> <p> Informe o início do intervalo para o qual deseja recuperar informações.</p> <p> Para obter uma lista de formatos de data e hora com suporte, consulte <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Coerção de tipo em [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tempo máximo]</td> 
   <td> <p> Informe o final do intervalo para o qual deseja recuperar informações. </p> <p>Para obter uma lista de formatos de data e hora com suporte, consulte <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Coerção de tipo em [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Calendários]</td> 
   <td> <p>Para cada calendário do qual deseja recuperar informações, clique em <strong>Adicionar</strong> e insira ou mapeie a ID do Calendário.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Acionar um cenário antes de um evento

Você pode acionar um cenário em um horário especificado antes de um evento com a ajuda de lembretes de email padrão do [!DNL Google Calendar] e do módulo [!UICONTROL Webhooks] >[!UICONTROL Mailhook personalizado].

1. Use o módulo [!UICONTROL Calendário do Google] >[!UICONTROL Atualizar um evento] para adicionar um lembrete de email ao seu evento:

   ![](assets/trigger-scen-before-event-350x209.png)

1. Crie um novo cenário começando com o módulo [!UICONTROL Webhooks] >[!UICONTROL Mailhook] personalizado.

   1. Copie o endereço de email do mailhook.
   1. Salve o cenário e execute-o.

1. Em [!DNL Gmail], redirecionar os lembretes de email do [!DNL Google Calendar] para o endereço de email do mailhook:

   1. Abra suas configurações do **[!UICONTROL [!DNL Gmail]]**.
   1. Abra a guia **[!UICONTROL Encaminhamento e POP/IMAP]**.
   1. Clique em **[!UICONTROL Adicionar um endereço de encaminhamento].**
   1. Cole o endereço de email dos mailhooks copiados, clique em&#x200B;**[!UICONTROL Avançar]**, confirme pressionando **[!UICONTROL Prosseguir]** na janela pop-up e clique em **[!UICONTROL OK]**.

   1. Em [!DNL Workfront Fusion], alterne para o novo cenário que deve concluir sua execução recebendo o email de confirmação.
   1. Clique no balão acima do módulo para inspecionar a saída do módulo.
   1. Expanda o item `Text` e copie o código de Confirmação:

      ![](assets/confirmation-code-350x252.png)

   1. No Gmail, cole o código de Confirmação na caixa de edição e clique em&#x200B;**[!UICONTROL Verificar]**:

      ![](assets/paste-code-350x46.png)

   1. Abra a guia **[!UICONTROL Filtros e endereços bloqueados]**.
   1. Clique em **[!UICONTROL Criar um novo filtro]**.
   1. Configure um filtro para todos os emails provenientes de `     calendar-notification@google.com` e clique em&#x200B;**[!UICONTROL Criar um filtro]**:
   1. Selecione **[!UICONTROL Encaminhá-lo para]** e escolha o endereço de email dos ganchos na lista.
   1. Clique em **[!UICONTROL Criar filtro]** para criar o filtro.

1. (Opcional) Em [!DNL Workfront Fusion], adicione o módulo [!UICONTROL Analisador de texto] > [!UICONTROL Padrão de correspondência] após o módulo [!UICONTROL Webhooks] >[!UICONTROL Mailhook personalizado] para analisar o código HTML do email para obter todas as informações necessárias.

   Por exemplo, você pode configurar o módulo da seguinte maneira para obter a ID do evento:

   *Padrão*: `<meta itemprop="eventId/googleCalendar" content="(?<evenitID>.*?)"/>`

   *Texto*: o item `HTML content` emitido do módulo [!UICONTROL Webhooks] >[!UICONTROL Mailhook] personalizado.
