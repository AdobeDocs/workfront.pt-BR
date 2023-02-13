---
title: Módulos Intacct
description: Módulos Intacct
author: Becky
draft: Probably
feature: Workfront Fusion
exl-id: fa1aa943-fbda-4eb4-bfa1-ab94a56785a7
source-git-commit: 9a4a847b542783845a3f896ec4e35d5efc7c122b
workflow-type: tm+mt
source-wordcount: '571'
ht-degree: 1%

---

# Módulos Intacct

Em um [!DNL Adobe Workfront Fusion] você pode automatizar workflows que usam o Intacct, bem como conectá-lo a vários aplicativos e serviços de terceiros.

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

Para usar os módulos Intacct, você deve ter uma conta Intacct.

## Conecte-se à Workfront Fusion

### Autorizar [!DNL Workfront Fusion] para fazer alterações no Intacct

Antes [!DNL Workfront Fusion] pode se conectar a [!DNL Intacct], você deve autorizá-lo.

Na sua conta do Intacct, navegue até o **[!UICONTROL Empresa]** guia .

1. Clique em **Informações da empresa**.
1. Navegue até o **Segurança** guia .
1. Clique em [!UICONTROL Editar] no canto superior direito
1. Selecione Autorizações de Serviços Web.
1. Clique no ícone de mais
1. Insira AzuquaMPP como sender_id.
1. (Opcional) Insira uma descrição para a conexão

### Configure uma conexão em [!DNL Workfront Fusion] {#set-up-a-connection-in-workfront-fusion}

Você pode criar uma conexão com o [!DNL Intacct] conta diretamente de dentro de uma [!DNL Intacct] módulo.

1. Em qualquer módulo do Intacct, clique em **[!UICONTROL Adicionar]** ao lado do campo Connection .
1. Insira suas credenciais do Intacct

   * ID da Empresa
   * ID do Usuário
   * Senha

1. Clique em **[!UICONTROL Continuar]** para criar a conexão e retornar ao módulo .

## Módulos de interação e seus campos

Ao configurar [!DNL Intacct] módulos, [!DNL Workfront Fusion] exibe os campos listados abaixo. Juntamente com eles, campos Intact adicionais podem ser exibidos, dependendo de fatores como seu nível de acesso no aplicativo ou serviço. Um título em negrito em um módulo indica um campo obrigatório.

Se o botão de mapa for exibido acima de um campo ou função, é possível usá-lo para definir variáveis e funções para esse campo. Para obter mais informações, consulte [Mapear informações de um módulo para outro no [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [[!UICONTROL Efetuar uma chamada de API personalizada]](#make-a-custom-api-call)
* [[!UICONTROL Pesquisar registros]](#search-records)

### [!UICONTROL Efetuar uma chamada de API personalizada] {#make-a-custom-api-call}

Esse módulo de ação permite que você faça uma chamada autenticada personalizada para o [!DNL Intacct] API. Dessa forma, você pode criar uma automação de fluxo de dados que não pode ser realizada pela outra [!DNL Intacct] módulos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Conexão</p> </td> 
   <td> <p>Para obter instruções sobre como conectar sua conta da Intel a [!DNL Workfront Fusion] 2.0, consulte <a href="#set-up-a-connection-in-workfront-fusion" class="MCXref xref">Configurar uma conexão no Workfront Fusion</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Corpo XML</td> 
   <td> <p>Inclua somente o XML no corpo. A solicitação inclui automaticamente cabeçalhos de autenticação.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Pesquisar registros]

Esse módulo de pesquisa recupera uma lista de registros que correspondem a critérios de pesquisa específicos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Conexão</p> </td> 
   <td> <p>Para obter instruções sobre como conectar sua conta da Intel a [!DNL Workfront Fusion] 2.0, consulte <a href="#set-up-a-connection-in-workfront-fusion" class="MCXref xref">Configurar uma conexão no Workfront Fusion</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de registro]</td> 
   <td> <p>Selecione o tipo de registro que deseja pesquisar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Critérios de pesquisa</p> </td> 
   <td> 
    <ul> 
     <li> <p>Selecione o campo pelo qual deseja pesquisar</p> </li> 
     <li> <p>Selecione o operador que deseja usar na pesquisa</p> </li> 
     <li> <p>Insira o valor que deseja pesquisar</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Conjunto de resultados</td> 
   <td>Selecione se deseja retornar todos os registros correspondentes ou somente o primeiro registro correspondente.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Limite</td> 
   <td> <p>Insira ou mapeie o número máximo de registros que você deseja que o módulo retorne durante cada ciclo de execução de cenário.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Ordenar por</td> 
   <td>Selecione o campo no qual deseja classificar os resultados. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Ordem</td> 
   <td>Selecione se deseja classificar crescente ou decrescente.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Saídas</td> 
   <td> <p>Selecione as informações que deseja incluir no pacote de saída deste módulo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Diferenciação de maiúsculas e minúsculas</td> 
   <td>Ative essa opção para tornar sua consulta diferencia maiúsculas de minúsculas.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Consulta em entidades privadas</td> 
   <td>Ative essa opção para permitir que o módulo pesquise entidades privadas.</td> 
  </tr> 
 </tbody> 
</table>
