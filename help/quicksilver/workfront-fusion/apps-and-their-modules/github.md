---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: conector
navigation-topic: apps-and-their-modules
title: Módulos do GitHub
description: Em um [!DNL Adobe Workfront Fusion] Nesse cenário, você pode automatizar workflows que usam o GitHub, bem como conectá-lo a vários aplicativos e serviços de terceiros.
author: Becky
feature: Workfront Fusion
exl-id: 5e520aab-8307-4a52-96b6-13b284f9cb53
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '1844'
ht-degree: 0%

---

# [!DNL GitHub] módulos

Em um [!DNL Adobe Workfront Fusion] cenário, é possível automatizar workflows que usam [!UICONTROL GitHub], bem como conectá-lo a vários aplicativos e serviços de terceiros.

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
   <p>Requisito de licença atual: Não [!DNL Workfront Fusion] requisito de licença.</p>
   <p>Ou</p>
   <p>Requisito de licença herdada: [!UICONTROL [!DNL Workfront Fusion] para Automação e integração do trabalho] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produto</td> 
   <td>
   <p>Requisito atual do produto: se você tiver o [!UICONTROL Select] ou o [!UICONTROL Prime] [!DNL Adobe Workfront] Planejar, sua organização deve comprar [!DNL Adobe Workfront Fusion] bem como [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo. [!DNL Workfront Fusion] está incluído no [!UICONTROL Ultimate] [!DNL Workfront] plano.</p>
   <p>Ou</p>
   <p>Requisito de produto herdado: sua organização deve comprar [!DNL Adobe Workfront Fusion] bem como [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Para descobrir que plano, tipo de licença ou acesso você tem, entre em contato com o [!DNL Workfront] administrador.

Para obter informações sobre [!DNL Adobe Workfront Fusion] licenças, consulte [[!DNL Adobe Workfront Fusion] licenças](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Pré-requisitos

Para usar [!DNL GitHub] módulos, você deve abrir um [!DNL GitHub] conta.

## Conectar [!DNL GitHub] para [!DNL Workfront Fusion]

Para obter instruções sobre como conectar seu [!DNL GitHub] conta para [!UICONTROL Workfront Fusion], consulte [Criar uma conexão com o [!UICONTROL Adobe Workfront Fusion] - Instruções básicas](../../workfront-fusion/connections/connect-to-fusion-general.md)

## [!DNL GitHub] módulos e seus campos.

Ao configurar [!DNL GitHub] módulos, [!DNL Workfront Fusion] exibe os campos listados abaixo. Junto com esses, [!DNL GitHub] Os campos podem ser exibidos, dependendo de fatores como seu nível de acesso no aplicativo ou serviço. Um título em negrito em um módulo indica um campo obrigatório.

Se você vir o botão de mapa acima de um campo ou função, poderá usá-lo para definir variáveis e funções para esse campo. Para obter mais informações, consulte [Mapear informações de um módulo para outro no [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Triggers](#triggers)
* [Ações](#actions)

### Triggers

* [[!UICONTROL Assistir Problemas]](#watch-issues)
* [[!UICONTROL Observar repositórios]](#watch-repositories)
* [[!UICONTROL Bifurcações de relógio]](#watch-forks)
* [[!UICONTROL Assistir a comentários]](#watch-comments)
* [[!UICONTROL Observar solicitações de pull]](#watch-pull-requests)

#### [!UICONTROL Assistir Problemas]

Esse módulo é acionado quando um novo problema é adicionado ou um problema existente é modificado.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL GitHub] conta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL que eu quero assistir]</td> 
   <td>Selecione se deseja observar todos os repositórios ou somente um repositório.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Repositório]</td> 
   <td>Se você optou por observar problemas em apenas um repositório, selecione o repositório que deseja observar.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Número máximo de problemas retornados]</td> 
   <td>Defina o número máximo de resultados que [!DNL Workfront Fusion] funcionará com durante um ciclo. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Observar]</td> 
   <td>Selecione se deseja observar somente novos problemas ou novos problemas e todas as alterações.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filtro]</td> 
   <td> <p>Você pode filtrar os problemas que deseja observar pela maneira como está associado a eles.</p> 
    <ul> 
     <li>[!UICONTROL Todos os problemas]</li> 
     <li>[!UICONTROL Somente problemas atribuídos a mim]</li> 
     <li>[!UICONTROL Somente problemas criados por mim]</li> 
     <li>[!UICONTROL Somente problemas que me mencionam]</li> 
     <li>[!UICONTROL Somente problemas para os quais me inscrevi para receber atualizações]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Estado]</td> 
   <td>Selecione se você deseja assistir somente a problemas abertos ou somente a problemas fechados. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Rótulos]</td> 
   <td>Adicione uma tag. O módulo observa problemas com essa tag.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Observar repositórios]

Esse módulo é acionado quando um repositório é criado ou modificado.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL GitHub] conta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Número máximo de repositórios retornados]</td> 
   <td>Defina o número máximo de resultados que [!DNL Workfront Fusion] funcionará com durante um ciclo. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Observar]</td> 
   <td>Selecione se deseja observar novos repositórios e todas as alterações ou somente novos repositórios.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Bifurcações de relógio]

Este módulo dispara quando uma nova bifurcação é criada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL GitHub] conta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Repositório]</td> 
   <td>Selecione o repositório que deseja observar por bifurcações.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Número máximo de bifurcações retornadas]</td> 
   <td>Defina o número máximo de resultados que [!DNL Workfront Fusion] funcionará com durante um ciclo. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Assistir a comentários]

Este módulo dispara quando um novo comentário é adicionado ou um comentário existente é modificado.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL GitHub] conta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Repositório]</td> 
   <td>Selecione o repositório que deseja observar.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Número de Problema]</td> 
   <td>Se quiser restringir a pesquisa apenas pesquisando novos comentários feitos em uma ocorrência específica, informe o número da ocorrência.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Número máximo de problemas retornados]</td> 
   <td>Defina o número máximo de resultados que [!DNL Workfront Fusion] funcionará com durante um ciclo. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Observar]</td> 
   <td>Selecione se deseja observar somente novos comentários ou comentários e todas as alterações.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Observar solicitações de pull]

Este módulo dispara quando uma nova solicitação de pull é adicionada ou uma solicitação de pull existente é modificada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL GitHub] conta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Repositório]</td> 
   <td>Selecione o repositório que deseja observar.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Número máximo de solicitações de pull retornadas]</td> 
   <td>Defina o número máximo de resultados que [!DNL Workfront Fusion] funcionará com durante um ciclo. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Estado]</td> 
   <td>Selecione se deseja observar solicitações [!UICONTROL somente abertura de pull], [!UICONTROL somente fechadas] ou todas as solicitações de pull. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Observar]</td> 
   <td>Selecione se deseja observar somente novas solicitações de baixa automática ou novas solicitações de baixa automática e todas as alterações.</td> 
  </tr> 
 </tbody> 
</table>

### Ações

* [[!UICONTROL Procurar um problema]](#search-for-an-issue)
* [[!UICONTROL Criar um problema]](#create-an-issue)
* [[!UICONTROL Atualizar um problema]](#update-an-issue)
* [[!UICONTROL Obter um problema]](#get-an-issue)
* [[!UICONTROL Adicionar responsáveis]](#add-assignees)
* [[!UICONTROL Remover responsáveis]](#remove-assignees)
* [[!UICONTROL Adicionar rótulos a um problema]](#add-labels-to-an-issue)
* [[!UICONTROL Remover um rótulo de um problema]](#remove-a-label-from-an-issue)
* [[!UICONTROL Criar um comentário]](#create-a-comment)
* [[!UICONTROL Listar comentários]](#list-comments)

#### [!UICONTROL Procurar um problema]

Este módulo procura por problemas que correspondam aos seus critérios de busca.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL GitHub] conta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
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
   <td role="rowheader">[!UICONTROL Direção de classificação]</td> 
   <td> <p>Selecione crescente ou decrescente. </p> <p>Para datas, seleção <strong>[!UICONTROL em ordem decrescente]</strong> retornará a data mais recente primeiro. </p> <p>Para [!UICONTROL número de comentários], selecione <strong>[!UICONTROL em ordem decrescente]</strong> retornará o problema com o maior número de comentários primeiro.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Consulta]</td> 
   <td>Insira ou mapeie a consulta de pesquisa. Para obter uma descrição detalhada das opções de pesquisa, consulte <a href="https://docs.github.com/en/github/searching-for-information-on-github/searching-issues-and-pull-requests">Pesquisando problemas e pull requests</a> no [!DNL GitHub] site de ajuda.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Criar um problema]

Este módulo cria um novo problema no repositório selecionado.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL GitHub] conta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Repositório]</td> 
   <td>Selecione o repositório no qual deseja criar um problema.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Atribuído]</td> 
   <td>Selecione as pessoas que você deseja atribuir à ocorrência. Os designados disponíveis incluem qualquer pessoa com permissões de gravação no repositório e membros da organização com permissões de leitura no repositório. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Etapa]</td> 
   <td>Selecione a etapa que você deseja associar à nova ocorrência. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Rótulos]</td> 
   <td>Selecione os rótulos que deseja aplicar ao novo problema. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Título]</td> 
   <td>Insira ou mapeie um título para o novo problema.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Corpo]</td> 
   <td>Insira ou mapeie o corpo do problema, como uma descrição ou informações adicionais</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Atualizar um problema]

Este módulo atualiza um existente [!DNL GitHub] problema.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL GitHub] conta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Repositório]</td> 
   <td>Selecione o repositório no qual deseja atualizar um problema.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Atribuído]</td> 
   <td>Selecione as pessoas que você deseja atribuir à ocorrência. Os designados disponíveis incluem qualquer pessoa com permissões de gravação no repositório e membros da organização com permissões de leitura no repositório. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Etapa]</td> 
   <td>Selecione a etapa que você deseja associar à ocorrência. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Rótulos]</td> 
   <td>Selecione os rótulos que deseja aplicar ao problema. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Número]</td> 
   <td>Insira ou mapeie o número do problema que você deseja atualizar. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Estado]</td> 
   <td>Selecione o estado para o qual você deseja atualizar o problema.</td> 
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

Este módulo recupera detalhes sobre o problema especificado

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL GitHub] conta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Repositório]</td> 
   <td>Selecione o repositório que contém o problema sobre o qual deseja recuperar detalhes.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Número]</td> 
   <td>Insira ou mapeie o número do problema sobre o qual você deseja recuperar detalhes. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Adicionar responsáveis]

Este módulo adiciona responsáveis ao problema especificado

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL GitHub] conta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Repositório]</td> 
   <td>Selecione o repositório que contém o problema ao qual você deseja adicionar atribuídos.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Atribuído]</td> 
   <td>Selecione as pessoas que você deseja atribuir à ocorrência. Os designados disponíveis incluem qualquer pessoa com permissões de gravação no repositório e membros da organização com permissões de leitura no repositório. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Número]</td> 
   <td>Insira ou mapeie o número do problema ao qual você deseja adicionar atribuídos. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Remover responsáveis]

Este módulo remove os atribuídos do problema especificado.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL GitHub] conta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Repositório]</td> 
   <td>Selecione o repositório que contém o problema do qual você deseja remover os atribuídos.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Atribuído]</td> 
   <td>Selecione as pessoas que você deseja remover do problema. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Número]</td> 
   <td>Informe ou mapeie o número do problema do qual deseja remover os designados. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Adicionar rótulos a um problema]

Este módulo adiciona rótulos a um problema. Os rótulos são definidos no nível do repositório e só podem ser criados por alguém com acesso de gravação ao repositório.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL GitHub] conta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Repositório]</td> 
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

Este módulo remove um único rótulo de um problema.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL GitHub] conta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Repositório]</td> 
   <td>Selecione o repositório que contém o problema do qual deseja remover um rótulo.</td> 
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

Este módulo cria um comentário sobre o problema especificado.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL GitHub] conta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Repositório]</td> 
   <td>Selecione o repositório que contém o problema no qual deseja criar um comentário.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Número]</td> 
   <td>Insira ou mapeie o número do problema no qual deseja criar um comentário.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Corpo]</td> 
   <td>Insira ou mapeie o conteúdo do comentário.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Listar comentários]

Este módulo lista todos os comentários sobre o problema especificado.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão]</td> 
   <td> <p>Para obter instruções sobre como conectar seu [!DNL GitHub] conta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Criar uma conexão com o [!DNL Adobe Workfront Fusion] - Instruções básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Repositório]</td> 
   <td>Selecione o repositório que contém o problema do qual deseja listar comentários.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Número]</td> 
   <td>Insira ou mapeie o número da ocorrência da qual deseja listar comentários.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Desde]</td> 
   <td>O módulo retornará comentários criados após essa data. Para obter uma lista de formatos de data compatíveis, consulte <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Coerção de tipo em [!DNL Adobe Workfront Fusion]</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Número máximo de comentários retornados]</td> 
   <td>Defina o número máximo de resultados que [!DNL Workfront Fusion] funcionará com durante um ciclo. </td> 
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
