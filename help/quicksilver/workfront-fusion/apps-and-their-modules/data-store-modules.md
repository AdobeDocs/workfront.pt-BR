---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Módulos de armazenamento de dados
description: Um armazenamento de dados  [!DNL Adobe Workfront Fusion] , semelhante a um banco de dados ou uma tabela simples, pode armazenar dados de cenários, possibilitando a transferência de dados entre cenários individuais ou execuções de cenário. Você pode usar um armazenamento de dados para armazenar novos dados de vários sistemas durante a sincronização.
author: Becky
feature: Workfront Fusion
exl-id: 1dc9cb88-d1b9-4a67-91fb-be980cc1ccd1
source-git-commit: 55485da1ea650121b5537a3f19d8102623ed4f43
workflow-type: tm+mt
source-wordcount: '1164'
ht-degree: 0%

---

# [!UICONTROL Módulos de armazenamento de dados]

Um armazenamento de dados [!DNL Adobe Workfront Fusion], semelhante a um banco de dados ou uma tabela simples, pode armazenar dados de cenários, possibilitando a transferência de dados entre cenários individuais ou execuções de cenário. Você pode usar um armazenamento de dados para armazenar novos dados de vários sistemas durante a sincronização.

Os módulos de armazenamento de dados permitem que você adicione, substitua, atualize, recupere, exclua, pesquise ou conte registros em seu armazenamento de dados do [!DNL Adobe Workfront Fusion].

Para obter informações sobre como criar, editar e solucionar problemas de armazenamentos de dados, consulte [Armazenamentos de Dados em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/data-stores.md)

Para obter uma introdução em vídeo aos armazenamentos de dados no Workfront Fusion, consulte:

* [Repositórios de Dados](https://video.tv.adobe.com/v/3427029/){target=_blank}

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
   <p>Requisito de licença herdada: [!UICONTROL [!DNL Workfront Fusion] para Automação e Integração do Trabalho], [!UICONTROL [!DNL Workfront Fusion] para Automação do Trabalho]</p>
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

Para usar os módulos do [!UICONTROL Repositório de Dados], primeiro crie um repositório de dados.

Para obter informações sobre como criar armazenamentos de dados, consulte [Armazenamentos de Dados no [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/modules/data-stores.md)

## [!UICONTROL Módulos de Armazenamento de Dados] e seus campos

Ao configurar módulos de Armazenamento de Dados, o [!DNL Workfront Fusion] exibe os campos listados abaixo. Junto com esses, campos adicionais do Data Store podem ser exibidos, dependendo de fatores como seu nível de acesso no aplicativo ou serviço. Um título em negrito em um módulo indica um campo obrigatório.

Se você vir o botão de mapa acima de um campo ou função, poderá usá-lo para definir variáveis e funções para esse campo. Para obter mais informações, consulte [Mapear informações de um módulo para outro em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

Todos os [!UICONTROL módulos de Armazenamento de Dados] são módulos do tipo Ação.

* [Adicionar/Substituir um Registro](#addreplace-a-record)
* [Atualizar um Registro](#update-a-record)
* [Obter um Registro](#get-a-record)
* [Verificar a existência de um registro](#check-the-existence-of-a-record)
* [Excluir um Registro](#delete-a-record)
* [Excluir todos os registros](#delete-all-records)
* [Pesquisar Registros](#search-records)
* [Contar Registros](#count-records)

### [!UICONTROL Adicionar/Substituir um Registro]

Este módulo de ação adiciona ou substitui um registro.

Especifique o armazenamento de dados e a chave do registro.

O módulo retorna a ID do registro e quaisquer campos associados, juntamente com quaisquer campos e valores personalizados que a conexão acessa. Você pode mapear essas informações em módulos subsequentes no cenário.

>[!NOTE]
>
>O módulo lança um erro quando você tenta adicionar o registro que já está no armazenamento de dados com o mesmo nome e a opção [!UICONTROL Substituir um registro existente] está desabilitada.

Ao configurar esse módulo, os campos a seguir são exibidos.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Armazenamento de dados]</td> 
   <td> <p> Selecione ou adicione o armazenamento de dados em que deseja criar um registro. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Chave] </td> 
   <td> <p>Insira a chave exclusiva do registro que você deseja que o módulo adicione ou substitua. A chave pode ser usada posteriormente para recuperar o registro. Se você deixar esse campo em branco, uma chave será gerada automaticamente.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Substituir um registro existente] </td> 
   <td> <p>Habilite esta opção para substituir o registro. O registro que você deseja substituir deve ser especificado no campo Chave acima.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Registro] </td> 
   <td> <p>Insira os valores desejados nos campos do registro.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Atualizar um Registro]

Este módulo de ação atualiza um registro.

Especifique o armazenamento de dados e a chave do registro.

O módulo retorna a ID do registro e quaisquer campos associados, juntamente com quaisquer campos e valores personalizados que a conexão acessa. Você pode mapear essas informações em módulos subsequentes no cenário.

Ao configurar esse módulo, os campos a seguir são exibidos.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Armazenamento de dados]</td> 
   <td> <p> Selecione ou adicione o armazenamento de dados em que deseja criar um registro. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Chave] </td> 
   <td> <p>Insira a chave exclusiva do registro que você deseja que o módulo atualize.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Inserir registro ausente] </td> 
   <td> <p>Ative esta opção para criar um novo registro se o registro com a chave especificada ainda não existir.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Registro]</td> 
   <td> <p> Informe os valores desejados nos campos do registro que deseja atualizar.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Obter um Registro]

Este módulo de ação recupera um registro.

Especifique o armazenamento de dados e a chave do registro.

O módulo retorna a ID do registro e quaisquer campos associados, juntamente com quaisquer campos e valores personalizados que a conexão acessa. Você pode mapear essas informações em módulos subsequentes no cenário.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Armazenamento de dados]</td> 
   <td> <p> Selecione o armazenamento de dados do qual deseja recuperar um registro</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Chave] </td> 
   <td> <p>Insira a chave exclusiva do registro que você deseja que o módulo recupere.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Verificar a Existência de um Registro]

Este módulo de ação especifica se um determinado registro existe.

Especifique o armazenamento de dados e a chave do registro.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Armazenamento de dados] </td> 
   <td> <p>Selecione o armazenamento de dados que deseja verificar a existência do registro.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Chave] </td> 
   <td> <p>Insira a chave exclusiva do registro que você deseja que o módulo verifique quanto à existência.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Excluir um Registro]

Este módulo de ação exclui um registro.

Especifique o armazenamento de dados e a chave do registro.

O módulo retorna a ID do registro e quaisquer campos associados, juntamente com quaisquer campos e valores personalizados que a conexão acessa. Você pode mapear essas informações em módulos subsequentes no cenário.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Armazenamento de dados] </td> 
   <td> <p>Selecione o armazenamento de dados que deseja verificar a existência do registro.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Chave] </td> 
   <td> <p>Insira a chave exclusiva do registro que você deseja que o módulo exclua.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Excluir todos os registros]

Esse módulo de ação exclui todos os registros de um determinado armazenamento de dados.

Você especifica o armazenamento de dados.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Armazenamento de dados] </td> 
   <td> <p>Selecione o armazenamento de dados do qual deseja excluir todos os registros.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Pesquisar Registros]

Esse módulo de pesquisa procura registros em um objeto no Armazenamento de dados que correspondam à consulta de pesquisa especificada.

Você pode mapear essas informações em módulos subsequentes no cenário.

Ao configurar esse módulo, os campos a seguir são exibidos.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Armazenamento de dados]</td> 
   <td> <p> Selecione o armazenamento de dados que deseja pesquisar.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Filtro]</p> </td> 
   <td> <p>Defina o filtro da pesquisa.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Classificar]</p> </td> 
   <td> <p style="font-weight: normal;">Para cada campo pelo qual você deseja classificar, preencha os seguintes campos:</p> <p style="font-weight: bold;">[!UICONTROL Chave]</p> <p>Selecione o nome da coluna pela qual deseja classificar os resultados.</p> <p style="font-weight: bold;">[!UICONTROL Ordem]</p> <p>Selecione se deseja classificar os resultados na ordem crescente ou decrescente.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Limite]</td> 
   <td> <p> Defina o número máximo de resultados de pesquisa [!DNL Workfront Fusion] retornos durante um ciclo de execução.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Continuar a execução da rota mesmo se o módulo não retornar resultados]</td> 
   <td> <p> Se ativado, a rota da qual este módulo faz parte continua sendo processada mesmo que este módulo não retorne resultados.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Contar Registros]

Esse módulo de ação numera os registros em um armazenamento de dados.

Você especifica o armazenamento de dados.

Ao configurar esse módulo, os campos a seguir são exibidos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Armazenamento de dados] </td> 
   <td> <p>Selecione o armazenamento de dados que contém os registros que você deseja contar.</p> </td> 
  </tr> 
 </tbody> 
</table>
