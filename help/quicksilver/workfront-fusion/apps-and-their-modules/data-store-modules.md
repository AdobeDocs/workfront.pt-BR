---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Módulos do armazenamento de dados
description: Um [!DNL Adobe Workfront Fusion] o armazenamento de dados, semelhante a um banco de dados ou a uma tabela simples, pode armazenar dados de cenários, permitindo transferir dados entre cenários individuais ou execuções de cenário. Você pode usar um armazenamento de dados para armazenar novos dados de vários sistemas durante a sincronização.
author: Becky
feature: Workfront Fusion
exl-id: 1dc9cb88-d1b9-4a67-91fb-be980cc1ccd1
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1103'
ht-degree: 0%

---

# [!UICONTROL Armazenamento de dados] módulos

Um [!DNL Adobe Workfront Fusion] o armazenamento de dados, semelhante a um banco de dados ou a uma tabela simples, pode armazenar dados de cenários, permitindo transferir dados entre cenários individuais ou execuções de cenário. Você pode usar um armazenamento de dados para armazenar novos dados de vários sistemas durante a sincronização.

Os módulos de armazenamento de dados permitem adicionar, substituir, atualizar, recuperar, excluir, pesquisar ou contar registros em seu [!DNL Adobe Workfront Fusion] armazenamento de dados.

Para obter informações sobre criação, edição e solução de problemas de armazenamentos de dados, consulte [Armazenamento de dados em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/data-stores.md)

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] para automação e integração de trabalho] </p>  <p>[!UICONTROL [!DNL Workfront Fusion] para Automação de Trabalho]</p></td> 
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

Para usar [!UICONTROL Armazenamento de dados] , primeiro você deve criar um armazenamento de dados.

Para obter informações sobre a criação de armazenamentos de dados, consulte [Armazenamento de dados em [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/modules/data-stores.md)

## [!UICONTROL Armazenamento de dados] módulos e seus campos

Ao configurar módulos do Data Store, [!DNL Workfront Fusion] exibe os campos listados abaixo. Junto a eles, campos adicionais do Data Store podem ser exibidos, dependendo de fatores como seu nível de acesso no aplicativo ou serviço. Um título em negrito em um módulo indica um campo obrigatório.

Se o botão de mapa for exibido acima de um campo ou função, é possível usá-lo para definir variáveis e funções para esse campo. Para obter mais informações, consulte [Mapear informações de um módulo para outro no [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

Todos [!UICONTROL Armazenamento de dados] são módulos do tipo Action .

* [Adicionar/Substituir um Registro](#addreplace-a-record)
* [Atualizar um registro](#update-a-record)
* [Obter um registro](#get-a-record)
* [Verificar a existência de um registro](#check-the-existence-of-a-record)
* [Excluir um registro](#delete-a-record)
* [Eliminar Todos os Registros](#delete-all-records)
* [Pesquisar registros](#search-records)
* [Registros de Contagem](#count-records)

### [!UICONTROL Adicionar/Substituir um Registro]

Esse módulo de ação adiciona ou substitui um registro.

Especifique o armazenamento de dados e a chave do registro.

O módulo retorna a ID do registro e quaisquer campos associados, juntamente com quaisquer campos e valores personalizados que a conexão acessa. Você pode mapear essas informações em módulos subsequentes do cenário.

>[!NOTE]
>
>O módulo emite um erro quando você tenta adicionar o registro que já está no armazenamento de dados com o mesmo nome e a variável [!UICONTROL Substituir um registro existente] está desativada.

Ao configurar esse módulo, os seguintes campos são exibidos.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Data store]</td> 
   <td> <p> Selecione ou adicione o armazenamento de dados onde deseja criar um registro. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Chave] </td> 
   <td> <p>Insira a chave exclusiva do registro que você deseja que o módulo adicione ou substitua. A chave pode ser usada posteriormente para recuperar o registro. Se esse campo ficar em branco, uma chave será gerada automaticamente.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Substituir um registro existente] </td> 
   <td> <p>Ative essa opção para substituir o registro. O registro que você deseja substituir deve ser especificado no campo Chave acima.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Registro] </td> 
   <td> <p>Insira os valores desejados nos campos do registro.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Atualizar um registro]

Este módulo de ação atualiza um registro.

Especifique o armazenamento de dados e a chave do registro.

O módulo retorna a ID do registro e quaisquer campos associados, juntamente com quaisquer campos e valores personalizados que a conexão acessa. Você pode mapear essas informações em módulos subsequentes do cenário.

Ao configurar esse módulo, os seguintes campos são exibidos.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Data store]</td> 
   <td> <p> Selecione ou adicione o armazenamento de dados onde deseja criar um registro. </p> </td> 
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
   <td> <p> Insira os valores desejados nos campos do registro que você deseja atualizar.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Obter um registro]

Esse módulo de ação recupera um registro.

Especifique o armazenamento de dados e a chave do registro.

O módulo retorna a ID do registro e quaisquer campos associados, juntamente com quaisquer campos e valores personalizados que a conexão acessa. Você pode mapear essas informações em módulos subsequentes do cenário.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Data store]</td> 
   <td> <p> Selecione o armazenamento de dados do qual deseja recuperar um registro</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Chave] </td> 
   <td> <p>Insira a chave exclusiva do registro que você deseja que o módulo recupere.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Verificar a existência de um registro]

Este módulo de ação especifica se existe um registro específico.

Especifique o armazenamento de dados e a chave do registro.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Data store] </td> 
   <td> <p>Selecione o armazenamento de dados que deseja verificar a existência do registro.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Chave] </td> 
   <td> <p>Insira a chave exclusiva do registro que você deseja que o módulo verifique a existência.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Excluir um registro]

Esse módulo de ação exclui um registro.

Especifique o armazenamento de dados e a chave do registro.

O módulo retorna a ID do registro e quaisquer campos associados, juntamente com quaisquer campos e valores personalizados que a conexão acessa. Você pode mapear essas informações em módulos subsequentes do cenário.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Data store] </td> 
   <td> <p>Selecione o armazenamento de dados que deseja verificar a existência do registro.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Chave] </td> 
   <td> <p>Insira a chave exclusiva do registro que você deseja que o módulo exclua.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Eliminar Todos os Registros]

Esse módulo de ação exclui todos os registros de um determinado armazenamento de dados.

Especifique o armazenamento de dados.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Data store] </td> 
   <td> <p>Selecione o armazenamento de dados do qual deseja excluir todos os registros.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Pesquisar registros]

Este módulo de pesquisa procura registros em um objeto no Data Store que correspondam à consulta de pesquisa especificada.

Você pode mapear essas informações em módulos subsequentes do cenário.

Ao configurar esse módulo, os seguintes campos são exibidos.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Data store]</td> 
   <td> <p> Selecione o armazenamento de dados que deseja pesquisar.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Filtro]</p> </td> 
   <td> <p>Defina o filtro para a pesquisa.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Classificar]</p> </td> 
   <td> <p style="font-weight: normal;">Para cada campo que deseja classificar, preencha os seguintes campos:</p> <p style="font-weight: bold;">[!UICONTROL Chave]</p> <p>Selecione o nome da coluna para a qual deseja classificar os resultados.</p> <p style="font-weight: bold;">[!UICONTROL Order]</p> <p>Selecione se deseja classificar os resultados na ordem crescente ou decrescente.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Limite]</td> 
   <td> <p> Definir o número máximo de resultados da pesquisa [!DNL Workfront Fusion] retorna durante um ciclo de execução.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Continuar a execução da rota mesmo se o módulo não retornar nenhum resultado]</td> 
   <td> <p> Se estiver habilitado, a rota em que esse módulo faz parte continuará o processamento, mesmo que esse módulo não retorne nenhum resultado.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Registros de Contagem]

Esse módulo de ação numera os registros em um armazenamento de dados.

Especifique o armazenamento de dados.

Ao configurar esse módulo, os seguintes campos são exibidos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Data store] </td> 
   <td> <p>Selecione o armazenamento de dados que contém os registros que deseja contar.</p> </td> 
  </tr> 
 </tbody> 
</table>
