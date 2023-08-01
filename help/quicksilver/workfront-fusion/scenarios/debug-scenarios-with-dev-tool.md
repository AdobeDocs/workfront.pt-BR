---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Cenários de depuração com a Ferramenta de Desenvolvimento Adobe Workfront Fusion
description: A Ferramenta de Desenvolvimento Adobe Workfront Fusion permite compreender e solucionar problemas de cenários. A DevTool adiciona um painel extra às Ferramentas do desenvolvedor do Chrome. Usando esse painel do depurador, você pode verificar todas as execuções manuais do cenário, revisar todas as operações executadas e ver os detalhes de cada chamada de API realizada. Você pode ver qual módulo, operação ou única resposta causou o erro e usar esse conhecimento para refinar seu cenário.
author: Becky
feature: Workfront Fusion
exl-id: f7557214-3615-4797-b4cb-4af70e4797ac
source-git-commit: 19de44559be7b5bd7584012f1d6f7e12523f12be
workflow-type: tm+mt
source-wordcount: '1687'
ht-degree: 0%

---

# Depurar cenários com o [!DNL Adobe Workfront Fusion] DevTool

A variável [!DNL Adobe Workfront Fusion] O DevTool permite compreender e solucionar problemas de cenários. A DevTool adiciona um painel extra à [!DNL Chrome Developer Tools]. Usando esse painel do depurador, você pode verificar todas as execuções manuais do cenário, revisar todas as operações executadas e ver os detalhes de cada chamada de API realizada. Você pode ver qual módulo, operação ou única resposta causou o erro e usar esse conhecimento para refinar seu cenário.

>[!NOTE]
>
>A Ferramenta de Desenvolvimento Workfront Fusion não está disponível para organizações que acessam o Fusion por meio do Unified Shell Adobe.

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
   <td role="rowheader">Licença [!UICONTROL Adobe Workfront Fusion]**</td> 
  <td>
   <p>Requisito de licença atual: Não [!DNL Workfront Fusion] requisito de licença.</p>
   <p>Ou</p>
   <p>Requisito de licença herdada: [!UICONTROL [!DNL Workfront Fusion] para Automação e Integração do Trabalho], [!UICONTROL [!DNL Workfront Fusion] para automação de trabalho]</p>
   </td>    </tr> 
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

Você pode adicionar o [!DNL Workfront Fusion] DevTool para [!DNL Chrome] por meio da [!UICONTROL [!DNL Chrome] Loja na Web].

1. Clique em [este link](https://chrome.google.com/webstore/detail/workfront-fusion-devtool/hkimbmkkmmejdnhbhoaefggkpkndfjnn/related) para acessar o [!DNL Workfront Fusion] DevTool no [!UICONTROL [!DNL Chrome] Loja na Web].
1. Clique em **[!UICONTROL Adicionar a[!DNL Chrome]]**.
1. Na janela que abre, examine as permissões. Se você concordar com as permissões, clique em **[!UICONTROL Adicionar extensão]**.

A variável [!DNL Workfront Fusion] A extensão DevTool é adicionada ao [!DNL Chrome] extensões.


## Localize o [!DNL Workfront Fusion] DevTool

Para usar o [!DNL Workfront Fusion] DevTool, você deve adicionar o [!DNL Workfront Fusion] Extensão DevTool para o [!DNL Chrome] navegador, conforme descrito em [Instalar a extensão DevTool do Chrome](#install-the-chrome-devtool-extension).

1. Abra o [!DNL Workfront Fusion] cenário.
1. Aberto [!DNL Chrome Developer Tools]:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!DNL Mac]</td> 
      <td>Command+Option+I</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!DNL Windows]</td> 
      <td> <p>Ctrl + Shift + I</p> <p> Ou </p> <p>F12</p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >Recomendamos encaixar o [!DNL Chrome Developer Console] na parte inferior para manter uma melhor visualização dos módulos.

1. Clique em **[!DNL Workfront Fusion]** guia em [!DNL Chrome Dev Tools].

## Use o [!DNL Workfront Fusion] DevTool

O Workfront Fusion DevTool é dividido em três seções principais. Você pode encontrá-los no painel esquerdo da janela DevTool.

* [Live Stream](#live-stream)
* [Depurador de cenários](#scenario-debugger)
* [Ferramentas](#tools)

### Live Stream

O Live Stream exibe o que está acontecendo em segundo plano quando você clica em Executar uma vez no seu cenário.

1. Clique em **[!UICONTROL Live Stream]** ícone ![](assets/live-stream-icon.png) para abrir a seção Live Stream.
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
      <td role="rowheader">Exibir informações da solicitação</td> 
      <td> <p>Você pode exibir as seguintes informações para cada módulo em seu cenário</p> 
       <ul> 
        <li> <p>Cabeçalhos de solicitação (URL do endpoint da API, método http, hora e data em que a solicitação foi chamada, cabeçalhos de solicitação e sequência de consulta)</p> </li> 
        <li> <p>Corpo da solicitação</p> </li> 
        <li> <p>Cabeçalhos de resposta</p> </li> 
        <li> <p>Corpo da resposta</p> </li> 
       </ul> <p>Para exibir essas informações, clique na guia apropriada no painel direito do [!DNL Workfront Fusion] DevTool</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Pesquisar solicitações e respostas</p> </td> 
      <td> <p>Insira o termo de pesquisa no campo de pesquisa no painel esquerdo do [!DNL Workfront Fusion] DevTool para exibir somente solicitações que contenham o termo de pesquisa.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Remover lista de solicitações </p> </td> 
      <td> <p>Clique no ícone de lixeira no canto superior direito do painel esquerdo da DevTool para limpar a lista de solicitações registradas pela [!DNL Workfront Fusion] DevTool </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Ativar o registro do console</p> </td> 
      <td> <p>Clique no ícone do computador <img src="assets/console-computer-icon.png"> no canto superior direito do painel esquerdo da DevTool.</p> <p>O login no console é ativado quando o ícone do computador está verde.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Recuperar a solicitação no formato JSON bruto ou cURL</p> </td> 
      <td> 
       <ul> 
        <li> <p><strong>JSON bruto</strong> </p> <p>Clique em <strong>[!UICONTROL Copiar BRUTO]</strong> no canto superior direito do painel direito da DevTool.</p> </li> 
        <li> <p><strong>cURL</strong> </p> <p>Clique em <strong>[!UICONTROL Copiar cURL]</strong> no canto superior direito do painel direito da DevTool.</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

### Depurador de cenários

O Depurador de cenários é útil para cenários mais complexos. Ele exibe o histórico das execuções de cenário e permite pesquisar módulos pelo nome ou ID.

1. Clique em **[!UICONTROL Depurador de cenários]** ícone ![](assets/scenario-debugger-icon.png) para abrir o Depurador de cenários.
1. (Opcional) Insira o termo de pesquisa (nome ou ID do módulo) no campo de pesquisa no painel esquerdo de [!DNL Workfront Fusion] DevTool no [!UICONTROL Depurador de cenários] seção.
1. Clique duas vezes no nome do módulo para abrir suas configurações no editor de cenários.
1. Exibir detalhes da solicitação clicando na operação desejada.

### Ferramentas

A variável [!DNL Workfront Fusion] O DevTool apresenta ferramentas que facilitam a configuração do seu cenário.

1. Clique em **[!UICONTROL Ferramentas]** ícone ![](assets/console-tools-icon.png) para abrir as Ferramentas.
1. Selecione a ferramenta que deseja usar
1. Configure os campos conforme detalhado abaixo.
1. Clique em **[!UICONTROL Executar]**.

Ferramentas e seus campos:

* [Foco em um módulo](#focus-a-module)
* [Localizar Módulos por Mapeamento](#find-modules-by-mapping)
* [Obter metadados do aplicativo](#get-app-metadata)
* [Copiar mapeamento](#copy-mapping)
* [Copiar Filtro](#copy-filter)
* [Trocar conexão](#swap-connection)
* [Variável de troca](#swap-variable)
* [Trocar aplicativo](#swap-app)
* [Base 64](#base-64)
* [Copiar nome do módulo](#copy-module-name)
* [Remapear origem](#remap-source)
* [Realçar aplicativo](#highlight-app)
* [Migrar GS](#migrate-gs)

#### [!UICONTROL Foco em um módulo]

Abre as configurações do módulo especificado por ID.

<table style="table-layout:auto">
    <tr>
        <td>[!UICONTROL ID de Módulo]</td>
        <td>Insira a ID do módulo para o qual deseja abrir as configurações.</td>
    </tr>
</table>

#### [!UICONTROL Localizar Módulos por Mapeamento]

Permite pesquisar valores de módulos para um termo especificado. A saída contém IDs de módulos que contêm o termo que você pesquisou.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Palavra-chave]</td> 
   <td> <p> Insira o termo que deseja pesquisar. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Usar Somente Valores]</p> </td> 
   <td> <p>Habilite esta opção para pesquisar apenas nos valores dos campos do módulo.</p> <p>Desative essa opção para pesquisar também nos nomes dos campos do módulo.</p> <p>A pesquisa é realizada por meio dos parâmetros name e label.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obter metadados do aplicativo]

Recupera metadados do aplicativo pelo nome do módulo ou ID do aplicativo. Isso é útil, por exemplo, quando você precisa saber a versão do aplicativo usada em seu cenário.

<table style="table-layout:auto">
    <tr>
        <td>[!UICONTROL Módulo de Origem]</td>
        <td>Selecione o módulo para o qual deseja recuperar metadados.</td>
    </tr>
</table>

#### [!UICONTROL Copiar mapeamento]

Copia valores do módulo de origem para o módulo de destino.

>[!CAUTION]
>
>Defina os módulos de origem e de destino corretos. Se você selecionar um tipo diferente de módulo, os valores no módulo de destino serão excluídos.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Módulo de Origem]</td> 
   <td> <p> Selecione o módulo ou insira a ID do módulo do qual deseja copiar valores de campo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Módulo de Destino]</p> </td> 
   <td> <p>Selecione o módulo ou insira a ID do módulo no qual deseja inserir os valores do módulo de origem.</p> <p>Importante: os valores no módulo de destino serão substituídos.</p> </td> 
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
   <td role="rowheader">[!UICONTROL Módulo de Origem]</td> 
   <td> <p> Selecione o módulo ou insira a ID do módulo do qual deseja copiar valores de filtro.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Módulo de Destino]</p> </td> 
   <td> <p>Selecione o módulo ou insira a ID do módulo no qual deseja inserir os valores de filtro do módulo de origem.</p> <p>Importante: os valores no módulo de destino serão substituídos.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Preservar Configuração de Rota de Fallback]</p> </td> 
   <td> <p>O filtro de origem é definido como a rota de fallback. Habilite esta opção para também definir o filtro de destino como a rota de fallback.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Trocar conexão]

Duplica uma conexão do módulo de origem para cada módulo no cenário do mesmo aplicativo.

<table style="table-layout:auto">
    <tr>
        <td>[!UICONTROL Módulo de Origem]</td>
        <td>Selecione o módulo ou insira a ID do módulo do qual deseja duplicar a conexão.</td>
    </tr>
</table>

#### [!UICONTROL Variável de troca]

Pesquisa variáveis especificadas no cenário e as substitui por uma nova variável.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Variável a ser Localizada]</td> 
   <td> <p> Localize o preenchimento de variável que deseja substituir do módulo no seu cenário e copie-o para este campo ([!UICONTROL Variável para Localizar]). No campo, ele é exibido com chaves duplas. Exemplo: <code>&#123;&#123;5.value&#125;&#125;</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Substituir Por]</p> </td> 
   <td> <p>Localize o preenchimento de variável que deseja substituir a variável no módulo do seu cenário e copie-o para este campo ([!UICONTROL Variável a Ser Localizada]). No campo, ele é exibido com chaves duplas. Exemplo: <code>&#123;&#123;5.value&#125;&#125;</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Módulo]</p> </td> 
   <td> <p>Selecione o módulo no qual deseja substituir a variável. Se nenhum módulo for selecionado, a variável será substituída em todo o cenário.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Trocar aplicativo]

Substitui a versão do aplicativo selecionado no seu cenário por outra versão do aplicativo.

Isso pode ser usado, por exemplo, para atualizar os módulos dos aplicativos Gmail e Email para a versão mais recente.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Aplicativo a ser Substituído]</td> 
   <td> <p> Selecione o aplicativo que deseja substituir.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Substituir por]</p> </td> 
   <td> <p>Selecione o aplicativo com o qual deseja substituí-lo.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Base 64]

Permite codificar os dados inseridos em Base64 ou decodificar Base64. Algumas solicitações estão codificadas em Base64. Essa ferramenta pode ser útil quando você deseja pesquisar dados específicos na solicitação codificada.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Operação] </td> 
   <td> <p>Selecione se deseja codificar os dados do campo [!UICONTROL Dados Brutos] em Base64 ou decodificar Base64 em Dados Brutos.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Dados Brutos]</p> </td> 
   <td> <p> Insira os dados que deseja codificar em Base64 ou Base64 se quiser decodificar em dados brutos, dependendo da opção selecionada no campo [!UICONTROL Operation] acima.</p> </td> 
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

#### [!UICONTROL Remapear origem]

Permite alterar a origem do mapeamento de um módulo para outro.

Primeiro, você deve adicionar o módulo que deseja usar como módulo de origem à rota em seu cenário.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Módulo de Origem] </td> 
   <td> <p> Selecione o módulo que você deseja substituir como a origem de mapeamento para outros módulos em seu cenário.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Módulo de Destino]</p> </td> 
   <td> <p>Selecione o módulo que deseja usar como uma nova origem de mapeamento.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Módulo a ser Editado]</p> </td> 
   <td> <p>Selecione o módulo para o qual deseja alterar o mapeamento se não quiser alterar o mapeamento em todo o cenário. </p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Realçar aplicativo]

Realça os módulos do aplicativo especificado no seu cenário.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Aplicativo a ser Destacado] </td> 
   <td> <p> Selecione o aplicativo que deseja realçar em seu cenário.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Versão] </p> </td> 
   <td> <p>Selecione a versão do aplicativo que deseja realçar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Cor de Realce]</p> </td> 
   <td> <p> Insira o hexadecimal de cor que deseja usar para os módulos de realce.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Migrar GS]

Essa ferramenta é feita especialmente para atualizar [!DNL Google Sheets] módulos (herdados) para a mais recente [!DNL Google Sheets] versão. Ele adiciona uma nova versão do módulo logo após a versão herdada do módulo na rota do cenário.

Esse módulo não requer a definição de nenhum parâmetro.
