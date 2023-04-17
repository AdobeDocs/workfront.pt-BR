---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Cenários de depuração com a Adobe Workfront Fusion DevTool
description: A Adobe Workfront Fusion DevTool permite compreender e solucionar problemas de cenários. A DevTool adiciona um painel extra às Ferramentas de desenvolvedor do Chrome. Com esse painel do depurador, você pode verificar todas as execuções manuais do seu cenário, analisar todas as operações executadas e ver os detalhes de cada chamada da API executada. Você pode ver qual módulo, operação ou resposta única causou o erro e usar esse conhecimento para refinar seu cenário.
author: Becky
feature: Workfront Fusion
exl-id: f7557214-3615-4797-b4cb-4af70e4797ac
source-git-commit: c7946e975c82f54c1a20e716f73d0cf8053ee1a6
workflow-type: tm+mt
source-wordcount: '1622'
ht-degree: 0%

---

# Depurar cenários com o [!DNL Adobe Workfront Fusion] DevTool

O [!DNL Adobe Workfront Fusion] O DevTool permite entender e solucionar problemas de cenários. O DevTool adiciona um painel extra ao [!DNL Chrome Developer Tools]. Com esse painel do depurador, você pode verificar todas as execuções manuais do seu cenário, analisar todas as operações executadas e ver os detalhes de cada chamada da API executada. Você pode ver qual módulo, operação ou resposta única causou o erro e usar esse conhecimento para refinar seu cenário.

## Requisitos de acesso

Você deve ter o seguinte acesso para usar a funcionalidade neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] plano*</td> 
   <td> <p>[!DNL Pro] ou superior</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licença*</td> 
   <td> <p>[!UICONTROL Plano], [!UICONTROL Trabalho]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da [!UICONTROL Adobe Workfront Fusion]**</td> 
  <td> <p>[!UICONTROL [!DNL Workfront Fusion] para automação e integração de trabalho] </p><p>[!UICONTROL [!DNL Workfront Fusion] para Automação de Trabalho] </p>  </td>    </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">Produto</td> 
   <td>Sua organização deve comprar [!DNL Adobe Workfront Fusion] bem como [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo.</td> 
  </tr> 
 </tbody> 
</table>

Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com seu [!DNL Workfront] administrador.

Para obter informações sobre [!DNL Adobe Workfront Fusion] licenças, consulte [[!DNL Adobe Workfront Fusion] licenças](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Instale o [!DNL Chrome] Extensão DevTool

<!--
To use the [!DNL Workfront Fusion] DevTool, you first need to install it.

1. Click [this link](assets/workfront-fusion-devtool-2023-feb.zip) to download the extension.
1. When the files have downloaded, extract them to a folder of your choice.
1. Open a tab in [!DNL Chrome]
1. In the search bar of the tab, enter `chrome://extensions`.
1. Click the **[!UICONTROL Developer mode]** toggle at the upper-right of the screen to enable Developer mode. If the toggle to the right, developer mode is enabled.
1. Click **[!UICONTROL Load unpacked]**.
1. Select the folder containing the DevTool (where you extracted the files in step 2).

   Once unpacked, the DevTool appears among your other Chrome extensions.
   -->

Você pode adicionar o [!DNL Workfront Fusion] DevTool para [!DNL Chrome] através da [!UICONTROL [!DNL Chrome] Loja da Web].

1. Clique em [este link](https://chrome.google.com/webstore/detail/workfront-fusion-devtool/hkimbmkkmmejdnhbhoaefggkpkndfjnn/related) para acessar o [!DNL Workfront Fusion] DevTool no [!UICONTROL [!DNL Chrome] Loja da Web].
1. Clique em [!UICONTROL Adicionar a [!DNL Chrome]].
1. Na janela que abre, examine as permissões. Se você concordar com as permissões, clique em [!UICONTROL Adicionar extensão].

O [!DNL Workfront Fusion] A extensão DevTool é adicionada a seu [!DNL Chrome] extensões.


## Localize a variável [!DNL Workfront Fusion] DevTool

Para usar o [!DNL Workfront Fusion] DevTool, você deve adicionar o [!DNL Workfront Fusion] Extensão DevTool para seu [!DNL Chrome] conforme descrito em [Instalar a extensão Chrome DevTool](#install-the-chrome-devtool-extension).

1. Abra seu [!DNL Workfront Fusion] .
1. Aberto [!DNL Chrome Developer Tools]:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!DNL Mac]</td> 
      <td>Comando + Opção + I</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!DNL Windows]</td> 
      <td> <p>Ctrl + Shift + I</p> <p> Ou </p> <p>F12</p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >Recomendamos ancorar o [!DNL Chrome Developer Console] na parte inferior para manter uma melhor visualização dos módulos.

1. Clique no botão **[!DNL Workfront Fusion]** em [!DNL Chrome Dev Tools].

## Use o [!DNL Workfront Fusion] DevTool

A Workfront Fusion DevTool é dividida em três seções principais. Você pode encontrá-los no painel esquerdo da janela DevTool.

* [Live Stream](#live-stream)
* [Depurador de Cenários](#scenario-debugger)
* [Ferramentas](#tools)

### Live Stream

O Live Stream exibe o que está acontecendo em segundo plano quando você clica em Executar uma vez em seu cenário.

1. Clique no botão **[!UICONTROL Live Stream]** ícone ![](assets/live-stream-icon.png) para abrir a seção Live Stream .
1. Siga um destes procedimentos:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>Ação</th> 
      <th>Instruções</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td role="rowheader">Exibir informações de solicitação</td> 
      <td> <p>Você pode exibir as seguintes informações para cada módulo em seu cenário</p> 
       <ul> 
        <li> <p>Cabeçalhos da solicitação (URL do ponto de extremidade da API, método http, hora e data em que a solicitação foi chamada, cabeçalhos da solicitação e sequência de consulta)</p> </li> 
        <li> <p>Corpo da solicitação</p> </li> 
        <li> <p>Cabeçalhos de resposta</p> </li> 
        <li> <p>Corpo da resposta</p> </li> 
       </ul> <p>Para exibir essas informações, clique na guia apropriada no painel direito do [!DNL Workfront Fusion] DevTool.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Pesquisar solicitações e respostas</p> </td> 
      <td> <p>Insira o termo de pesquisa no campo de pesquisa no painel esquerdo do [!DNL Workfront Fusion] DevTool para exibir somente solicitações que contenham o termo de pesquisa.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Remover lista de solicitações </p> </td> 
      <td> <p>Clique no ícone da lixeira no canto superior direito do painel esquerdo do DevTool para limpar a lista de solicitações registradas pelo [!DNL Workfront Fusion] DevTool. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Ativar o registro do console</p> </td> 
      <td> <p>Clique no ícone do computador <img src="assets/console-computer-icon.png"> no canto superior direito do painel esquerdo do DevTool.</p> <p>O logon no console é ativado quando o ícone do computador é verde.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Recuperar a solicitação no formato JSON bruto ou cURL</p> </td> 
      <td> 
       <ul> 
        <li> <p><strong>JSON bruto</strong> </p> <p>Clique em <strong>[!UICONTROL Copiar RAW]</strong> no canto superior direito do painel direito do DevTool.</p> </li> 
        <li> <p><strong>cURL</strong> </p> <p>Clique em <strong>[!UICONTROL Copiar cURL]</strong> no canto superior direito do painel direito do DevTool.</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

### Depurador de Cenários

O Depurador de cenário é útil para cenários mais complexos. Ele exibe o histórico das execuções do cenário e permite pesquisar módulos pelo nome ou ID.

1. Clique no botão **[!UICONTROL Depurador de Cenários]** ícone ![](assets/scenario-debugger-icon.png) para abrir o depurador de cenário.
1. (Opcional) Insira o termo de pesquisa (nome ou ID do módulo) no campo de pesquisa no painel esquerdo de [!DNL Workfront Fusion] DevTool no [!UICONTROL Depurador de Cenários] seção.
1. Clique duas vezes no nome do módulo para abrir suas configurações no editor de cenários.
1. Visualize os detalhes da solicitação clicando na operação desejada.

### Ferramentas

O [!DNL Workfront Fusion] O DevTool possui ferramentas que facilitam a configuração do seu cenário.

1. Clique no botão **[!UICONTROL Ferramentas]** ícone ![](assets/console-tools-icon.png) para abrir as Ferramentas.
1. Selecione a ferramenta que deseja usar
1. Configure os campos conforme detalhado abaixo.
1. Clique em **[!UICONTROL Executar]**.

Ferramentas e seus campos:

* [Focar um módulo](#focus-a-module)
* [Localizar Módulos por Mapeamento](#find-modules-by-mapping)
* [Obter metadados do aplicativo](#get-app-metadata)
* [Copiar mapeamento](#copy-mapping)
* [Copiar Filtro](#copy-filter)
* [Trocar conexão](#swap-connection)
* [Variável de troca](#swap-variable)
* [Trocar aplicativo](#swap-app)
* [Base 64](#base-64)
* [Copiar nome do módulo](#copy-module-name)
* [Remover Origem](#remap-source)
* [Destacar aplicativo](#highlight-app)
* [Migrar GS](#migrate-gs)

#### [!UICONTROL Focar um módulo]

Abre as configurações do módulo especificado por ID.

<table style="table-layout:auto">
    <tr>
        <td>[!UICONTROL ID do módulo]</td>
        <td>Insira a ID do módulo para o qual você deseja abrir as configurações.</td>
    </tr>
</table>

#### [!UICONTROL Localizar Módulos por Mapeamento]

Permite pesquisar os valores dos módulos para um termo especificado. A saída contém IDs de módulos que contêm o termo que você pesquisou.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Palavra-chave]</td> 
   <td> <p> Insira o termo que deseja pesquisar. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Usar apenas valores]</p> </td> 
   <td> <p>Ative essa opção para pesquisar apenas nos valores dos campos do módulo.</p> <p>Desative essa opção para pesquisar também nos nomes dos campos do módulo.</p> <p>A pesquisa é realizada por meio dos parâmetros de nome e rótulo.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obter metadados do aplicativo]

Recupera metadados do aplicativo pelo nome ou ID do módulo do aplicativo. Isso é útil, por exemplo, quando você precisa saber a versão do aplicativo usada em seu cenário.

<table style="table-layout:auto">
    <tr>
        <td>[!UICONTROL Módulo de origem]</td>
        <td>Selecione o módulo para o qual deseja recuperar metadados.</td>
    </tr>
</table>

#### [!UICONTROL Copiar mapeamento]

Copia valores do módulo de origem para o módulo de destino.

>[!CAUTION]
>
>Certifique-se de definir os módulos de origem e de destino corretos. Se você selecionar um tipo diferente de módulo, os valores no módulo de destino serão excluídos.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Módulo de origem]</td> 
   <td> <p> Selecione o módulo ou insira a ID do módulo a partir do qual você deseja copiar valores de campo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Módulo de destino]</p> </td> 
   <td> <p>Selecione o módulo ou insira a ID do módulo no qual deseja inserir os valores do módulo de origem.</p> <p>Importante: Os valores no módulo de destino serão substituídos.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Copiar Filtro]

Copia as configurações de filtro do módulo de origem para o módulo de destino.

>[!NOTE]
>
>A ação de cópia é executada no filtro colocado no lado esquerdo do módulo selecionado.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Módulo de origem]</td> 
   <td> <p> Selecione o módulo ou insira a ID do módulo a partir do qual deseja copiar os valores do filtro.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Módulo de destino]</p> </td> 
   <td> <p>Selecione o módulo ou insira a ID do módulo no qual deseja inserir os valores de filtro do módulo de origem.</p> <p>Importante: Os valores no módulo de destino serão substituídos.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Preservar configuração da rota de fallback]</p> </td> 
   <td> <p>O filtro de origem é definido como a rota de fallback. Ative essa opção para também definir o filtro de destino que é definido como a rota de fallback.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Trocar conexão]

Duplica uma conexão do módulo de origem a cada módulo no cenário do mesmo aplicativo.

<table style="table-layout:auto">
    <tr>
        <td>[!UICONTROL Módulo de origem]</td>
        <td>Selecione o módulo ou insira a ID do módulo a partir do qual você deseja duplicar a conexão.</td>
    </tr>
</table>

#### [!UICONTROL Variável de troca]

Pesquisa variáveis especificadas no cenário e as substitui por uma nova variável.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Variável a ser encontrada]</td> 
   <td> <p> Localize o comprimido da variável que você deseja substituir do módulo em seu cenário e copie-o para este campo ([!UICONTROL Variable to Find]). No campo , ele é exibido com colchetes duplos. Exemplo: <code>&#123;&#123;5.value&#125;&#125;</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Substituir por]</p> </td> 
   <td> <p>Localize o comprimido da variável com a qual você deseja substituir a variável do módulo em seu cenário e copie-o para este campo ([!UICONTROL Variável para localizar]). No campo , ele é exibido com colchetes duplos. Exemplo: <code>&#123;&#123;5.value&#125;&#125;</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Módulo]</p> </td> 
   <td> <p>Selecione o módulo no qual deseja substituir a variável . Se nenhum módulo for selecionado, a variável será substituída em todo o cenário.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Trocar aplicativo]

Substitui a versão do aplicativo selecionada no seu cenário por outra versão do aplicativo.

Isso pode ser usado, por exemplo, para atualizar os módulos dos aplicativos Gmail e Email para a versão mais recente.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Aplicativo a ser substituído]</td> 
   <td> <p> Selecione o aplicativo que deseja substituir.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Substituir por]</p> </td> 
   <td> <p>Selecione o aplicativo com o qual deseja substituí-lo.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Base 64]

Permite codificar os dados inseridos em Base64 ou para decodificar Base64. Algumas solicitações são codificadas em Base64. Essa ferramenta pode ser útil quando você deseja pesquisar dados específicos na solicitação codificada.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Operação] </td> 
   <td> <p>Selecione se deseja codificar os dados do campo [!UICONTROL Dados brutos] para Base64 ou decodificar Base64 para Dados brutos.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Dados brutos]</p> </td> 
   <td> <p> Insira os dados que deseja codificar para Base64 ou Base64 se quiser decodificar para dados brutos, dependendo da opção selecionada no campo [!UICONTROL Operation] acima.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Copiar nome do módulo]

Copia o nome do módulo selecionado para a área de transferência.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Módulo] </td> 
   <td> <p>Selecione o módulo do qual deseja copiar o nome.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Remover Origem]

Permite alterar a origem do mapeamento de um módulo para outro.

Primeiro, você deve adicionar o módulo que deseja usar como um módulo de origem à rota em seu cenário.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Módulo de origem] </td> 
   <td> <p> Selecione o módulo que deseja substituir como a fonte de mapeamento para outros módulos no seu cenário.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Módulo de destino]</p> </td> 
   <td> <p>Selecione o módulo que deseja usar como uma nova fonte de mapeamento.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Módulo a ser editado]</p> </td> 
   <td> <p>Selecione o módulo para o qual deseja alterar o mapeamento se não quiser alterar o mapeamento no cenário inteiro. </p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Destacar aplicativo]

Destaca os módulos do aplicativo especificado no seu cenário.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Aplicativo a ser destacado] </td> 
   <td> <p> Selecione o aplicativo que deseja destacar no seu cenário.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Versão] </p> </td> 
   <td> <p>Selecione a versão do aplicativo que deseja destacar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Cor de realce]</p> </td> 
   <td> <p> Insira o índice de cores que deseja usar nos módulos de realce.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Migrar GS]

Essa ferramenta é feita especialmente para atualizar [!DNL Google Sheets] (herdado) aos módulos mais recentes [!DNL Google Sheets] versão. Ele adiciona uma nova versão do módulo logo após a versão herdada do módulo na rota de cenário.

Esse módulo não requer a definição de parâmetros.
