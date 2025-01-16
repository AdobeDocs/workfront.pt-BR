---
title: Módulos do MariaDB
description: A documentação do Adobe Workfront Fusion foi movida para um novo local. Este artigo foi descontinuado, mas contém um link para o novo artigo que aborda essa funcionalidade.
author: Becky
draft: Probably
feature: Workfront Fusion
exl-id: 45d4d7fe-a70c-4906-adb4-f913a870fe47
source-git-commit: efbe888d370e20c895dc40f18f999f2d01ec6337
workflow-type: tm+mt
source-wordcount: '647'
ht-degree: 0%

---

# [!DNL MariaDB] módulos

>[!IMPORTANT]
>
>A documentação do Adobe Workfront Fusion foi movida para um novo local.
>
>As informações neste artigo agora podem ser encontradas no artigo:
>
>* [Módulos do MariaDB](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/mariadb-modules.html)
>
>Atualize todos os marcadores.
>
>Este artigo não está mais sendo atualizado e será removido em breve.

Em um cenário [!DNL Adobe Workfront Fusion], você pode automatizar fluxos de trabalho que usam [!DNL MariaDB], bem como conectá-los a vários aplicativos e serviços de terceiros.

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

Para usar módulos [!DNL MariaDB], você deve ter uma conta [!DNL MariaDB].

## Conectar [!DNL MariaDB] a [!DNL Workfront Fusion]

Você pode criar uma conexão com sua conta do [!DNL MariaDB] diretamente de dentro de um módulo do [!DNL MariaDB].

1. Em qualquer módulo [!DNL MariaDB], clique em **[!UICONTROL Adicionar]** ao lado do campo [!UICONTROL Conexão].
1. Configure os seguintes campos:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Nome da Conexão]</p> </td> 
      <td> <p>Insira um nome para a nova conexão.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Host]</td> 
      <td> <p>Informe o endereço IP ou o nome do host da instância do banco de dados. Esse host deve ser acessível de fora da rede.</p> <p>Exemplo: <code>[!DNL mariadb.hwoh2j5h.us-east-1.rds.amazon.com]</code></p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Porta]</td> 
      <td>A porta padrão é 3306. Se você estiver usando uma porta não padrão, defina esse número para sua porta. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Nome do Banco de Dados]</td> 
      <td>Insira o nome do banco de dados com o qual você deseja interagir.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Nome de Usuário]</td> 
      <td>Insira seu nome de usuário.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Senha]</td> 
      <td>Digite sua senha.</td> 
     </tr> 
    </tbody> 
   </table>

1. Clique em **[!UICONTROL Continuar]** para criar a conexão e voltar para o módulo.

## [!DNL MariaDB] Módulos e seus campos

Ao configurar módulos do [!DNL MariaDB], o [!DNL Workfront Fusion] exibe os campos listados abaixo. Junto com esses, campos [!DNL MariaDB] adicionais podem ser exibidos, dependendo de fatores como seu nível de acesso no aplicativo ou serviço. Um título em negrito em um módulo indica um campo obrigatório.

Se você vir o botão de mapa acima de um campo ou função, poderá usá-lo para definir variáveis e funções para esse campo. Para obter mais informações, consulte [Mapear informações de um módulo para outro em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### Executar uma consulta (avançado)

Este módulo de ação recupera informações do banco de dados, com base em uma consulta fornecida por você.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão]</td> 
   <td>Para obter instruções sobre como conectar sua conta do [!DNL MariaDB] ao [!DNL Workfront Fusion], consulte <a href="#connect-mariadb-to-workfront-fusion" class="MCXref xref">Conectar [!DNL MariaDB] ao [!DNL Workfront Fusion]</a> neste artigo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Consulta]</td> 
   <td> <p>Insira a consulta SQL que você deseja que o módulo use para recuperar dados.</p> <p>Importante: as variáveis usadas na consulta não são limpas. Certifique-se de limpar as variáveis corretamente para impedir a injeção de SQL.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Selecionar linhas de uma tabela (avançado)]

Esse módulo lê registros do banco de dados.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexão]</td> 
   <td>Para obter instruções sobre como conectar sua conta do [!DNL MariaDB] ao [!DNL Workfront Fusion], consulte <a href="#connect-mariadb-to-workfront-fusion" class="MCXref xref">Conectar [!DNL MariaDB] ao [!DNL Workfront Fusion]</a> neste artigo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tabela]</td> 
   <td> <p>Selecione a tabela que contém os registros que você deseja ler.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filtro]</td> 
   <td> <p>Configure o filtro pelo qual deseja selecionar linhas</p> 
    <ul> 
     <li> <p>Selecione o campo pelo qual deseja pesquisar</p> </li> 
     <li> <p>Selecione o operador que deseja usar na pesquisa</p> </li> 
     <li> <p>Insira ou mapeie o valor que você deseja pesquisar.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Classificar] </td> 
   <td> <p>Para cada nível pelo qual você deseja classificar os resultados, clique em <strong>[!UICONTROL Adicionar item]</strong> e selecione o campo pelo qual deseja classificar os resultados e se deseja classificar em ordem crescente ou decrescente</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limite]</td> 
   <td> <p>Insira ou mapeie o número máximo de registros que deseja que o módulo retorne durante cada ciclo de execução de cenário.</p> </td> 
  </tr> 
 </tbody> 
</table>
