---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: conector
navigation-topic: apps-and-their-modules
title: Módulos do GitHub
description: Em um [!DNL Adobe Workfront Fusion] você pode automatizar fluxos de trabalho que usam o GitHub, bem como conectá-lo a vários aplicativos e serviços de terceiros.
author: Becky
feature: Workfront Fusion
exl-id: 5e520aab-8307-4a52-96b6-13b284f9cb53
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1796'
ht-degree: 0%

---

# [!DNL GitHub] módulos

Em um [!DNL Adobe Workfront Fusion] , é possível automatizar workflows que usam [!UICONTROL GitHub], bem como conectá-lo a vários aplicativos e serviços de terceiros.

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

Para usar [!DNL GitHub] módulos, você deve ter um [!DNL GitHub] conta.

## Connect [!DNL GitHub] para [!DNL Workfront Fusion]

Para obter instruções sobre como conectar seu [!DNL GitHub] para [!UICONTROL Workfront Fusion], consulte [Criar uma conexão com [!UICONTROL Adobe Workfront Fusion] - Instruções básicas](../../workfront-fusion/connections/connect-to-fusion-general.md)

## [!DNL GitHub] e seus campos.

Ao configurar [!DNL GitHub] módulos, [!DNL Workfront Fusion] exibe os campos listados abaixo. Junto com esses, [!DNL GitHub] podem ser exibidos, dependendo de fatores como seu nível de acesso no aplicativo ou serviço. Um título em negrito em um módulo indica um campo obrigatório.

Se o botão de mapa for exibido acima de um campo ou função, é possível usá-lo para definir variáveis e funções para esse campo. Para obter mais informações, consulte [Mapear informações de um módulo para outro no [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Triggers](#triggers)
* [Ações](#actions)

### Triggers

* [[!UICONTROL Problemas de monitoramento]](#watch-issues)
* [[!UICONTROL Monitorar Repositórios]](#watch-repositories)
* [[!UICONTROL Relógios de Relógio]](#watch-forks)
* [[!UICONTROL Observar comentários]](#watch-comments)
* [[!UICONTROL Monitorar solicitações de pull]](#watch-pull-requests)

#### [!UICONTROL Problemas de monitoramento]

Esse módulo é acionado quando um novo problema é adicionado ou um problema existente é modificado.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL GitHub] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL I want to watch]</td> 
   <td>Selecione se deseja assistir a todos os repositórios ou somente a um repositório.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Repository]</td> 
   <td>Se você optou por assistir a problemas em apenas um repositório, selecione o repositório que deseja observar.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Número máximo de problemas retornados]</td> 
   <td>Defina o número máximo de resultados que [!DNL Workfront Fusion] funcionará durante um ciclo. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Watch]</td> 
   <td>Selecione se deseja procurar apenas novos problemas ou novos problemas e todas as alterações.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filtro]</td> 
   <td> <p>Você pode filtrar os problemas que deseja observar por como está associado a eles.</p> 
    <ul> 
     <li>[!UICONTROL Todos os problemas]</li> 
     <li>[!UICONTROL Somente problemas atribuídos a mim]</li> 
     <li>[!UICONTROL Somente problemas criados por mim]</li> 
     <li>[!UICONTROL Apenas problemas mencionando-me]</li> 
     <li>[!UICONTROL Somente problemas dos quais eu estou inscrito para atualizações]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Estado]</td> 
   <td>Selecione se deseja ver apenas problemas em aberto ou somente problemas fechados. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Rótulos]</td> 
   <td>Adicione uma tag. O módulo procura problemas com essa tag.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Monitorar Repositórios]

Esse módulo dispara quando um repositório é criado ou modificado.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL GitHub] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Número máximo de repositórios retornados]</td> 
   <td>Defina o número máximo de resultados que [!DNL Workfront Fusion] funcionará durante um ciclo. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Watch]</td> 
   <td>Selecione se deseja procurar novos repositórios e todas as alterações ou apenas novos repositórios.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Relógios de Relógio]

Esse módulo dispara quando uma nova bifurcação é criada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL GitHub] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Repository]</td> 
   <td>Selecione o repositório que deseja observar para as bifurcações.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Número máximo de bifurcações retornadas]</td> 
   <td>Defina o número máximo de resultados que [!DNL Workfront Fusion] funcionará durante um ciclo. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Observar comentários]

Esse módulo dispara quando um novo comentário é adicionado ou um comentário existente é modificado.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL GitHub] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Repository]</td> 
   <td>Selecione o repositório que deseja visualizar.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Número do problema]</td> 
   <td>Se quiser restringir a pesquisa pesquisando apenas novos comentários feitos em um problema específico, insira o número do problema.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Número máximo de problemas retornados]</td> 
   <td>Defina o número máximo de resultados que [!DNL Workfront Fusion] funcionará durante um ciclo. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Watch]</td> 
   <td>Selecione se deseja procurar apenas novos comentários, comentários e todas as alterações.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Monitorar solicitações de pull]

Esse módulo dispara quando uma nova solicitação de pull é adicionada ou uma solicitação de pull existente é modificada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL GitHub] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Repository]</td> 
   <td>Selecione o repositório que deseja visualizar.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Número máximo de solicitações de pull retornadas]</td> 
   <td>Defina o número máximo de resultados que [!DNL Workfront Fusion] funcionará durante um ciclo. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Estado]</td> 
   <td>Selecione se deseja assistir a solicitações do [!UICONTROL somente de pull aberto], do [!UICONTROL somente as fechadas] ou de todas as solicitações de pull. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Watch]</td> 
   <td>Selecione se deseja monitorar apenas novas solicitações de pull, ou novas solicitações de pull e todas as alterações.</td> 
  </tr> 
 </tbody> 
</table>

### Ações

* [[!UICONTROL Pesquisar por um problema]](#search-for-an-issue)
* [[!UICONTROL Criar um problema]](#create-an-issue)
* [[!UICONTROL Atualizar um problema]](#update-an-issue)
* [[!UICONTROL Obter um problema]](#get-an-issue)
* [[!UICONTROL Adicionar destinatários]](#add-assignees)
* [[!UICONTROL Remover destinatários]](#remove-assignees)
* [[!UICONTROL Adicionar rótulos a um problema]](#add-labels-to-an-issue)
* [[!UICONTROL Remover um rótulo de um problema]](#remove-a-label-from-an-issue)
* [[!UICONTROL Criar um comentário]](#create-a-comment)
* [[!UICONTROL Listar comentários]](#list-comments)

#### [!UICONTROL Pesquisar por um problema]

Este módulo pesquisa por problemas que correspondam aos seus critérios de pesquisa.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL GitHub] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Número máximo de problemas retornados]</td> 
   <td>Defina o número máximo de resultados que [!DNL Workfront Fusion] funcionará com durante um ciclo (o número de repetições por execução de cenário). </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Classificar por]</td> 
   <td> <p>Selecione como deseja classificar os resultados da pesquisa.</p> 
    <ul> 
     <li> <p>[!UICONTROL Melhor correspondência] </p> </li> 
     <li>[!UICONTROL Data de criação]</li> 
     <li>[!UICONTROL Data de atualização]</li> 
     <li>[!UICONTROL Número de comentários]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Direção da classificação]</td> 
   <td> <p>Selecione crescente ou decrescente. </p> <p>Para datas, selecione <strong>[!UICONTROL decrescente]</strong> retornará a data mais recente primeiro. </p> <p>Para [!UICONTROL número de comentários], selecionando <strong>[!UICONTROL decrescente]</strong> O retornará o problema com o maior número de comentários primeiro.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Consulta]</td> 
   <td>Insira ou mapeie sua consulta de pesquisa. Para obter uma descrição detalhada das opções de pesquisa, consulte <a href="https://docs.github.com/en/github/searching-for-information-on-github/searching-issues-and-pull-requests">Pesquisar problemas e obter solicitações</a> no [!DNL GitHub] site de ajuda.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Criar um problema]

Esse módulo cria um novo problema no repositório selecionado.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL GitHub] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Repository]</td> 
   <td>Selecione o repositório no qual deseja criar um problema.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Destinatário]</td> 
   <td>Selecione as pessoas que deseja atribuir ao problema. Os destinatários disponíveis incluem qualquer pessoa com permissões de gravação no repositório e membros da organização com permissões de leitura no repositório. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Marco]</td> 
   <td>Selecione o marco que deseja associar à nova edição. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Rótulos]</td> 
   <td>Selecione os rótulos que deseja aplicar ao novo problema. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Título]</td> 
   <td>Insira ou mapeie um título para a nova ocorrência.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Corpo]</td> 
   <td>Insira ou mapeie o corpo do problema, como uma descrição ou informações adicionais</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Atualizar um problema]

Esse módulo atualiza um [!DNL GitHub] problema.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL GitHub] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Repository]</td> 
   <td>Selecione o repositório no qual deseja atualizar um problema.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Destinatário]</td> 
   <td>Selecione as pessoas que deseja atribuir ao problema. Os destinatários disponíveis incluem qualquer pessoa com permissões de gravação no repositório e membros da organização com permissões de leitura no repositório. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Marco]</td> 
   <td>Selecione o marco que deseja associar ao problema. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Rótulos]</td> 
   <td>Selecione os rótulos que deseja aplicar ao problema. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Número]</td> 
   <td>Insira ou mapeie o número do problema que deseja atualizar. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Estado]</td> 
   <td>Selecione o estado para o qual deseja atualizar o problema.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Título]</td> 
   <td>Insira ou mapeie um título para o problema.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Corpo]</td> 
   <td>Insira ou mapeie o corpo do problema, como uma descrição ou informações adicionais</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obter um problema]

Esse módulo recupera detalhes sobre o problema especificado

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL GitHub] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Repository]</td> 
   <td>Selecione o repositório que contém o problema sobre o qual você deseja recuperar detalhes.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Número]</td> 
   <td>Insira ou mapeie o número do problema sobre o qual deseja recuperar detalhes. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Adicionar destinatários]

Esse módulo adiciona destinatários ao problema especificado

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL GitHub] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Repository]</td> 
   <td>Selecione o repositório que contém o problema ao qual deseja adicionar destinatários.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Destinatário]</td> 
   <td>Selecione as pessoas que deseja atribuir ao problema. Os destinatários disponíveis incluem qualquer pessoa com permissões de gravação no repositório e membros da organização com permissões de leitura no repositório. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Número]</td> 
   <td>Insira ou mapeie o número da ocorrência do problema ao qual deseja adicionar os destinatários. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Remover destinatários]

Esse módulo remove os destinatários do problema especificado.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL GitHub] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Repository]</td> 
   <td>Selecione o repositório que contém o problema do qual deseja remover os destinatários.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Destinatário]</td> 
   <td>Selecione as pessoas que deseja remover do problema. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Número]</td> 
   <td>Insira ou mapeie o número do problema do qual deseja remover os destinatários. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Adicionar rótulos a um problema]

Esse módulo adiciona rótulos a um problema. Rótulos são definidos no nível do repositório e só podem ser criados por alguém com acesso de gravação ao repositório.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL GitHub] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Repository]</td> 
   <td>Selecione o repositório que contém o problema ao qual deseja adicionar rótulos.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Rótulos]</td> 
   <td>Selecione os rótulos que deseja adicionar ao problema.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Número]</td> 
   <td>Insira ou mapeie o número do problema ao qual deseja adicionar rótulos.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Remover um rótulo de um problema]

Esse módulo remove um único rótulo de um problema.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL GitHub] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Repository]</td> 
   <td>Selecione o repositório que contém o problema do qual você deseja remover um rótulo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Rótulos]</td> 
   <td>Selecione o rótulo que deseja remover do problema.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Número]</td> 
   <td>Insira ou mapeie o número do problema do qual deseja remover um rótulo.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Criar um comentário]

Esse módulo cria um comentário sobre o problema especificado.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL GitHub] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Repository]</td> 
   <td>Selecione o repositório que contém o problema no qual deseja criar um comentário.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Número]</td> 
   <td>Insira ou mapeie o número da ocorrência do problema em que deseja criar um comentário.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Corpo]</td> 
   <td>Insira ou mapeie o conteúdo do comentário.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Listar comentários]

Esse módulo lista todos os comentários sobre o problema especificado.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL GitHub] para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Repository]</td> 
   <td>Selecione o repositório que contém o problema do qual deseja listar comentários.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Número]</td> 
   <td>Insira ou mapeie o número do problema do qual deseja listar comentários.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Since]</td> 
   <td>O módulo retornará comentários criados após essa data. Para obter uma lista de formatos de data compatíveis, consulte <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Coação de tipo em [!DNL Adobe Workfront Fusion]</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Número máximo de comentários retornados]</td> 
   <td>Defina o número máximo de resultados que [!DNL Workfront Fusion] funcionará durante um ciclo. </td> 
  </tr> 
 </tbody> 
</table>

<!--
<h2 data-mc-conditions="QuicksilverOrClassic.Draft mode">Troubleshooting</h2>
-->

<!--
<h3 data-mc-conditions="QuicksilverOrClassic.Draft mode">Module does not receive any events</h3>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">If a module does not receive any events, check the webhook settings in Github and make sure that:</p>
-->

<!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You have set the correct type of event that the chosen module should receive</p>
  -->

<!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You have entered the correct Payload URL</p>
  -->
