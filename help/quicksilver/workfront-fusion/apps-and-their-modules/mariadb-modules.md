---
title: Módulos de MariaDB
description: Em um [!DNL Adobe Workfront Fusion] , é possível automatizar workflows que usam [!DNL MariaDB], bem como conectá-lo a vários aplicativos e serviços de terceiros.
author: Becky
draft: Probably
feature: Workfront Fusion
exl-id: 45d4d7fe-a70c-4906-adb4-f913a870fe47
source-git-commit: c57a796ccbfb36bce58d49345e7515dd524604c5
workflow-type: tm+mt
source-wordcount: '545'
ht-degree: 1%

---

# [!DNL MariaDB] módulos

Em um [!DNL Adobe Workfront Fusion] , é possível automatizar workflows que usam [!DNL MariaDB], bem como conectá-lo a vários aplicativos e serviços de terceiros.

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

Para usar [!DNL MariaDB] módulos, você deve ter um [!DNL MariaDB] conta.

## Connect [!DNL MariaDB] para [!DNL Workfront Fusion]

Você pode criar uma conexão com o [!DNL MariaDB] conta diretamente de dentro de uma [!DNL MariaDB] módulo.

1. Em qualquer [!DNL MariaDB] módulo, clique em **[!UICONTROL Adicionar]** ao lado do [!UICONTROL Conexão] campo.
1. Configure os seguintes campos:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Nome da conexão]</p> </td> 
      <td> <p>Digite um nome para a nova conexão.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Host]</td> 
      <td> <p>Insira o endereço IP ou o nome do host da instância do banco de dados. Esse host deve ser acessível de fora da sua rede.</p> <p>Exemplo: <code>[!DNL mariadb.hwoh2j5h.us-east-1.rds.amazon.com]</code></p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Port]</td> 
      <td>A porta padrão é 3306. Se você estiver usando uma porta não padrão, defina esse número como sua porta. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Nome do banco de dados]</td> 
      <td>Insira o nome do banco de dados com o qual deseja interagir.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Nome de usuário]</td> 
      <td>Entre com seu nome de usuário.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Senha]</td> 
      <td>Digite sua senha.</td> 
     </tr> 
    </tbody> 
   </table>

1. Clique em **[!UICONTROL Continuar]** para criar a conexão e retornar ao módulo .

## [!DNL MariaDB] Módulos e seus campos

Ao configurar [!DNL MariaDB] módulos, [!DNL Workfront Fusion] exibe os campos listados abaixo. Junto com esses, [!DNL MariaDB] podem ser exibidos, dependendo de fatores como seu nível de acesso no aplicativo ou serviço. Um título em negrito em um módulo indica um campo obrigatório.

Se o botão de mapa for exibido acima de um campo ou função, é possível usá-lo para definir variáveis e funções para esse campo. Para obter mais informações, consulte [Mapear informações de um módulo para outro no [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### Executar um query (avançado)

Esse módulo de ação recupera informações do banco de dados, com base em uma consulta fornecida.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Para obter instruções sobre como conectar seu [!DNL MariaDB] para [!DNL Workfront Fusion], consulte <a href="#connect-mariadb-to-workfront-fusion" class="MCXref xref">Connect [!DNL MariaDB] para [!DNL Workfront Fusion]</a> neste artigo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Consulta]</td> 
   <td> <p>Insira a consulta SQL que você deseja que o módulo use para recuperar dados.</p> <p>Importante: As variáveis usadas no query não são apagadas. Certifique-se de limpar as variáveis corretamente para evitar a injeção de SQL.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Selecionar linhas de uma tabela (avançado)]

Esse módulo lê o registro do banco de dados.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Para obter instruções sobre como conectar seu [!DNL MariaDB] para [!DNL Workfront Fusion], consulte <a href="#connect-mariadb-to-workfront-fusion" class="MCXref xref">Connect [!DNL MariaDB] para [!DNL Workfront Fusion]</a> neste artigo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tabela]</td> 
   <td> <p>Selecione a tabela que contém os registros que deseja ler.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filtro]</td> 
   <td> <p>Configure o filtro pelo qual deseja selecionar as linhas</p> 
    <ul> 
     <li> <p>Selecione o campo que deseja pesquisar por</p> </li> 
     <li> <p>Selecione o operador que pretende utilizar para a pesquisa</p> </li> 
     <li> <p>Insira ou mapeie o valor que deseja pesquisar.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Classificar] </td> 
   <td> <p>Para cada nível pelo qual você deseja que os resultados sejam classificados, clique em <strong>[!UICONTROL Adicionar item]</strong>, selecione o campo no qual deseja classificar os resultados e se deseja classificar crescente ou decrescente</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limite]</td> 
   <td> <p>Insira ou mapeie o número máximo de registros que você deseja que o módulo retorne durante cada ciclo de execução de cenário.</p> </td> 
  </tr> 
 </tbody> 
</table>
