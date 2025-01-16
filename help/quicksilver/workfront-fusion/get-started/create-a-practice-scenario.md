---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Criar um cenário de integração de prática no Adobe Workfront Fusion
description: A documentação do Adobe Workfront Fusion foi movida para um novo local. Este artigo foi descontinuado, mas contém um link para o novo artigo que aborda essa funcionalidade.
author: Becky
feature: Workfront Fusion
exl-id: 643bb1d5-d7bc-402b-8ed1-9ca9a30e4560
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '2188'
ht-degree: 0%

---

# Criar um cenário de integração de prática no Adobe Workfront Fusion

>[!IMPORTANT]
>
>A documentação do Adobe Workfront Fusion foi movida para um novo local.
>
>As informações neste artigo agora podem ser encontradas no artigo:
>
>* [Fluxo de trabalho para criar um cenário](https://experienceleague.adobe.com/docs/workfront-fusion/using/create-scenarios/plan-a-scenario/create-a-scenario-workflow.html)
>
>Atualize todos os marcadores.
>
>Este artigo não está mais sendo atualizado e será removido em breve.

Este artigo descreve como criar um cenário de integração com o Adobe Workfront Fusion. Os cenários de integração conectam aplicativos separados, permitindo que seus dados fluam por diferentes aplicativos.

Para criar um cenário de integração, sua organização deve ter uma licença do [!DNL Workfront Fusion for Work Automation and Integration].

Para obter instruções sobre como criar um cenário de automação somente com o Workfront, consulte [Criar um cenário de automação de prática no Adobe Workfront Fusion](../../workfront-fusion/get-started/create-a-practice-automation-scenario.md)

Para obter mais informações sobre licenças do Workfront Fusion, consulte [licenças do Adobe Workfront Fusion](../../workfront-fusion/get-started/license-automation-vs-integration.md).

>[!NOTE]
>
>Sua organização pode não permitir o acesso às Planilhas do Google. Se esse for o caso, você não poderá configurar essa integração, mas as informações apresentadas aqui podem ser usadas como um exemplo geral de como os cenários de integração funcionam.

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
   <p>Requisito de licença atual: nenhum requisito de licença [!DNL Workfront Fusion].</p>
   <p>Ou</p>
   <p>Requisito de licença herdada: [!UICONTROL [!DNL Workfront Fusion] para Automação e Integração do Trabalho] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produto</td> 
   <td>
   <p>Requisito atual do produto: se você tiver o Plano [!DNL Adobe Workfront] da [!UICONTROL Select] ou da [!UICONTROL Prime], sua organização deve comprar o [!DNL Adobe Workfront Fusion] e o [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo. [!DNL Workfront Fusion] está incluído no plano [!DNL Workfront] da [!UICONTROL Ultimate].</p>
   <p>Ou</p>
   <p>Requisito de produto herdado: sua organização deve comprar o [!DNL Adobe Workfront Fusion] e o [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Para saber que plano, tipo de licença ou acesso você tem, contate o administrador do [!DNL Workfront].

Para obter informações sobre [!DNL Adobe Workfront Fusion] licenças, consulte [[!DNL Adobe Workfront Fusion] licenças](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Criar um cenário de prática

O papel de [!DNL Adobe Workfront Fusion] é automatizar seus processos para que você possa se concentrar em novas tarefas em vez de repetir as mesmas tarefas repetidamente. Ele funciona vinculando ações em e entre aplicativos e serviços para criar um cenário que transfere e transforma seus dados automaticamente. O cenário que você cria observa dados em um aplicativo ou serviço e processa esses dados para fornecer o resultado desejado.

Um cenário é composto de uma série de módulos que indicam como os dados devem ser transformados em um aplicativo ou transferidos entre aplicativos e serviços da Web.

Para explicar como criar um cenário e reforçar as práticas recomendadas à medida que você aprende a usar o [!DNL Workfront Fusion], este artigo o orienta pelo processo passo a passo. Criaremos um cenário que cria um novo registro em [!DNL Workfront] para cada linha em uma planilha [!DNL Google Sheets].

![](assets/finished-scenario-1-350x180.png)

>[!TIP]
>
>Um cenário como esse seria útil se você tivesse uma planilha listando projetos que precisam ser trabalhados usando os projetos em [!DNL Workfront]. O cenário pode &quot;observar&quot; a planilha em busca de novas linhas e adicionar um novo projeto em [!DNL Workfront] para cada uma.

A criação de um cenário consiste em várias tarefas principais:

## Escolha os aplicativos e nomeie o cenário

1. Baixe esta [planilha](https://cdn.experience.workfront.com/Documentation/Workfront+Fusion/Fusion+Practice+Scenario+Sample+Sheet.xlsx) e carregue-a no seu [!DNL Google Drive] para usar durante este exercício.

   Ou

   Crie ou encontre sua própria planilha simples do [!DNL Google Sheets] semelhante a esta:

   ![](assets/spreadsheet-headers-350x55.png)

1. Entre na sua conta [!DNL Workfront Fusion].
1. Clique em **[!UICONTROL Cenários]** ![](assets/scenarios-icon.png) no painel esquerdo.

   >[!NOTE]
   >
   >Se você não vir o painel de navegação esquerdo ou seus ícones, clique no ícone Menu ![Menu](assets/main-menu-icon-left-nav.png).

   No painel cinza [!UICONTROL Pastas] que é exibido, você pode organizar seus cenários em pastas.

   Na parte superior da área principal à direita, você pode ver **[!UICONTROL Todos]** os cenários que criou, os **[!UICONTROL Cenários Ativos]** e os **[!UICONTROL Cenários Inativos]** e os **[!UICONTROL Conceitos]**, que são cenários que precisam de mais trabalho para que o [!DNL Workfront Fusion] possa classificá-los como ativos ou inativos.

<!--
   ![](assets/scenarios-left-panel-350x215.png)
-->

1. No painel [!UICONTROL Pastas], clique no ícone ![](assets/add-folder-icon.png) de **[!UICONTROL Adicionar pasta]** e digite um nome como &quot;Cenários de prática&quot; para a sua primeira pasta.

1. Abra a pasta e clique em **[!UICONTROL Criar um novo cenário]** no canto superior direito da página.

   A landing page que é exibida permite pré-carregar todos os aplicativos que você deseja usar no cenário que você vai criar.

1. Neste exercício, pesquise e selecione o aplicativo **[!UICONTROL Google Sheets]**.
1. Clique em **[!UICONTROL Continuar]** no canto superior direito.

   O editor de cenários exibe, contendo um módulo vazio no centro, o aplicativo [!DNL Google Sheets] pré-carregado e algumas opções na barra de ferramentas na parte inferior.

<!--
   ![](assets/scenario-editor.png)
-->

Quando você começar a criar um novo cenário, é uma boa ideia começar criando um nome para ele.

1. Selecione o nome do espaço reservado **[!UICONTROL Novo cenário]** no canto superior esquerdo e digite um nome como &quot;Praticar cenário 1&quot;.
1. Continue com [Adicione e configure o primeiro módulo](#add-and-configure-the-first-module) abaixo.

## Adicionar e configurar o primeiro módulo

O módulo vazio com um ponto de interrogação representa o módulo acionador que você precisa adicionar. Esse módulo iniciará o cenário sempre que for executado. O ícone de relógio no módulo vazio indica que é um módulo agendado.

![](assets/empty-module.png)

Este módulo conterá os dados que você deseja que o cenário observe.

1. Clique no módulo vazio para escolher o aplicativo do qual você selecionará um módulo.

   O aplicativo pré-carregado anteriormente é exibido ao lado do módulo vazio. Você pode adicionar outros aplicativos que tenham módulos usando a caixa [!UICONTROL Pesquisar].

   ![](assets/pre-loaded-apps-350x139.png)

1. Clique em **[!DNL Google Sheets]**.

   A lista é alterada para exibir todos os [!DNL Google Sheets] módulos que você pode usar como um módulo de gatilho.

1. Clique no módulo do acionador **[!UICONTROL Observar Registros]**.

   Agora é necessário estabelecer uma conexão autenticada com sua conta do Google. Cada módulo adicionado a um cenário deve ter uma conexão com seu aplicativo.

1. Na caixa **[!DNL Google Sheets]**, em **[!UICONTROL Conexão]**, clique em **[!UICONTROL Adicionar]** e digite um nome para a conexão, como &quot;Conta da Google de Olivia&quot;, e clique em **[!UICONTROL Continuar]**.
1. Autentique a conexão na janela que é exibida.

   O processo para autenticar uma conexão pode variar um pouco entre os aplicativos. Talvez seja necessário fazer logon no aplicativo. Normalmente, você precisará clicar no botão **[!UICONTROL Permitir]**. Se precisar de ajuda, consulte [Visão geral das conexões](../../workfront-fusion/connections/about-connecting-wf-fusion-to-app-or-service.md).

## Configurar o primeiro módulo

Após conectar o [!DNL Workfront Fusion] à sua conta [!DNL Google Sheets], você pode especificar uma planilha [!DNL Google Sheets] à qual tem acesso e os dados que deseja que o primeiro módulo processe.

1. Clique na caixa **[!UICONTROL Planilha]** e selecione a planilha **[!UICONTROL cenário de prática do Workfront Fusion] #1** na lista exibida.

   Esta planilha contém 2 planilhas (guias), portanto, precisamos especificar qual planilha contém os dados desejados:

1. Na lista suspensa **[!UICONTROL Planilha]**, selecione **[!UICONTROL Projetos]**.

   Nossa planilha contém cabeçalhos e queremos que o módulo os use para identificar os dados que queremos processar:

   ![](assets/spreadsheet-headers-350x55.png)

1. Deixe **[!UICONTROL Sim]** selecionado para **[!UICONTROL A tabela contém cabeçalhos]**.

1. Na caixa **[!UICONTROL Linha com cabeçalhos]**, você pode especificar um intervalo de linhas que deseja incluir, mas deixe o padrão A1:Z1 aqui para este exercício.
1. Na caixa **[!UICONTROL Limite]**, digite 1.

   Dessa forma, sempre que você executar o cenário, o módulo processará apenas uma linha na planilha. Isso é útil para simplificar suas execuções de teste enquanto você está criando o cenário.

1. Clique em **[!UICONTROL OK]**.

   A caixa **[!UICONTROL Escolher onde começar]** solicita que você especifique onde deseja que o módulo inicie o processamento na planilha.

1. Clique em **[!UICONTROL Escolher manualmente]**, selecione a opção superior na lista exibida e clique em **[!UICONTROL OK]**.
1. Clique com o botão direito do mouse no módulo, clique em **[!UICONTROL Renomear]**, digite um nome que descreva o que você deseja que o módulo faça (como &quot;Assista à lista de projetos&quot;) e clique em **[!UICONTROL OK]**.

   O nome aparece logo abaixo do módulo. Abaixo disso, [!DNL Workfront Fusion] inclui uma breve descrição do tipo de ação executada pelo módulo.

   ![](assets/module-renamed-350x388.png)

1. Continue com [Adicionar e configurar o segundo módulo](#add-and-configure-the-second-module).

## Adicionar e configurar o segundo módulo

1. Clique no círculo parcial à direita do do módulo para **[!UICONTROL Adicionar outro módulo]**.

   Este segundo módulo precisa ser um módulo [!DNL Workfront], mas não pré-carregamos o aplicativo [!DNL Workfront].

1. Para localizar o aplicativo [!DNL Workfront], comece digitando &quot;[!DNL Workfront]&quot; e clique no aplicativo quando ele for exibido.
1. Na lista de [!DNL Workfront] módulos exibidos, clique em **[!UICONTROL Criar Registro]**.

1. Como você fez antes com o aplicativo Google Sheets, clique em **[!UICONTROL Adicionar]** na caixa [!DNL Workfront] para adicionar uma conexão entre o Workfront Fusion e o Workfront.

   Agora começaremos a especificar o que queremos fazer com os dados da planilha.

1. Clique em **[!UICONTROL Tipo de registro]** e selecione **[!UICONTROL Projeto]** porque queremos criar um projeto em [!DNL Workfront] usando uma linha da planilha.

   >[!TIP]
   >
   >Você pode encontrar **[!UICONTROL Projeto]** na lista se começar a digitar a palavra &quot;[!UICONTROL projeto].&quot;

   A caixa se expande para exibir todos os campos de projeto [!DNL Workfront] disponíveis, nos quais você pode colocar as informações encontradas pelo primeiro módulo.

   Vamos usar o campo **[!UICONTROL Nome]**: queremos que este módulo nomeie cada projeto em [!DNL Workfront] usando o texto na linha [!UICONTROL Google Sheets] correspondente.

1. Localize e clique no campo **[!UICONTROL Nome]**.

   >[!TIP]
   >
   >Você pode usar **Cmd+F** ([!DNL Mac] SO) ou **Ctrl-F**([!DNL Windows] OS) para localizar um campo rapidamente.

   Isso abre a lista de variáveis que você pode usar no campo **[!UICONTROL Nome]** para definir o nome de cada projeto criado no Workfront.

   ![](assets/list-of-available-variables-350x261.png)

   Observe que as variáveis próximas à parte superior da lista correspondem aos cabeçalhos das colunas na planilha.

   ![](assets/spreadsheet-headers-marked-350x55.png)

   ![](assets/list-of-available-variables-marked-350x320.png)

1. Clique na variável **[!UICONTROL Meu Nome de Projeto (A)]** para adicioná-la ao campo **[!UICONTROL Nome]**.

   Você acabou de mapear os primeiros dados para esse cenário.

   Vamos mapear mais um dado da planilha para [!DNL Workfront]: a data de início de cada projeto.

1. Localize e clique no campo **[!UICONTROL Data de Início Planejada]** e clique na variável **[!UICONTROL Data de Início Planejada (E)]** para extrair dados dessa coluna na planilha.

1. Clique em **[!UICONTROL OK]**.

   Agora você tem um cenário de trabalho.

1. Dê um nome ao segundo módulo, como &quot;Criar projeto Workfront&quot;, e continue com [Testar o cenário](#test-the-scenario).

## Testar o cenário

Antes de ativar o cenário, é importante testá-lo executando-o pelo menos uma vez e visualizando os resultados. Isso ajuda você a entender como os dados fluem pelo cenário e encontrar erros.

Escolhemos ter uma linha da planilha processada para criar um projeto no Workfront. Se você executar o cenário, isso é o que deve acontecer.

1. Clique em **[!UICONTROL Executar uma vez]** no canto inferior esquerdo do editor de cenários.
1. Depois que o cenário terminar de ser executado, clique no balão acima do módulo [!DNL Google Sheets].

   ![](assets/click-bubble.png)

   Na caixa que aparece, você pode exibir informações sobre o pacote de dados que o módulo processou, incluindo os dados reais que foram extraídos da planilha para a linha com a qual você começou.

   ![](assets/execution-inspector-g-sheets-350x637.png)

1. Clique na bolha do inspetor de execução acima do módulo [!DNL Workfront] para ver a entrada de informações e a saída, que é a ID do projeto agora criado em [!DNL Workfront]

   ![](assets/execution-inspector-wf-350x384.png)

   Você pode saber mais sobre como ler as informações de execução do cenário nos seguintes artigos:

   * Para obter informações gerais, consulte [Fluxo de execução do cenário em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-flow.md).
   * Para obter informações sobre pacotes processados, consulte [Execução do cenário, ciclos e fases em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

1. Acesse [!DNL Workfront] e procure por &quot;soho center loft&quot; para ver o projeto que o cenário criou. Esta foi a última linha da planilha.
1. Em [!DNL Workfront Fusion], clique em **[!UICONTROL Salvar]** ![](assets/save-icon.png) próximo ao canto inferior esquerdo para salvar seu progresso no cenário.

   >[!IMPORTANT]
   >
   >Salve com frequência à medida que você aprimora e testa um cenário.

## Finalize o cenário e teste-o novamente

Ainda precisamos configurar o cenário para criar projetos para todas as outras linhas na planilha.

1. Clique no módulo **[!UICONTROL Linhas de observação]** que você criou para o Google Sheets.
1. Altere o **[!UICONTROL Limite]** para 100.

   Especificar um número maior do que o número de linhas que você sabe que estão na planilha garante que o cenário capturará todas elas.

1. Clique com o botão direito do mouse no módulo **[!UICONTROL Linhas de observação]**, clique em **[!UICONTROL Escolher onde começar]**, clique em **[!UICONTROL Todas]** e em **[!UICONTROL OK]**.

1. Clique em **[!UICONTROL Executar uma vez]** e observe o que acontece nos balões do inspetor de execução.

   O módulo [!DNL Google] Planilhas **[!UICONTROL Linhas de observação]** é executado uma vez para ler todas as linhas. Em seguida, o módulo **[!UICONTROL Criar registro]** do Workfront é executado 20 vezes para criar um projeto para cada uma das 20 linhas restantes na planilha.

1. Clique na bolha do inspetor de execução para o módulo [!DNL Workfront] para exibir todas as 20 operações, em seguida, clique em uma das operações para exibir as informações sobre o projeto criado.
1. Clique em **[!UICONTROL Salvar]** ![](assets/save-icon.png) próximo ao canto inferior esquerdo.
1. Vá para [!DNL Workfront] para ver os projetos criados pelo cenário.

>[!TIP]
>
>Recomendamos a prática opcional, mas útil, de adicionar observações sobre cada módulo.
>
>1. Clique com o botão direito do mouse no módulo [!DNL Workfront] e clique em **[!UICONTROL Adicionar uma observação]**.
>1. Na nota exibida, digite uma visão geral do módulo.
>
>    Isso é útil porque você não precisará abrir o módulo continuamente para ver o que ele faz. Você pode digitar algo como &quot;Cria um projeto com Nome, Data de início planejada e Prioridade mapeada da planilha&quot;.
>
>    Para o módulo [!UICONTROL Google Sheets], você pode digitar algo como &quot;Assista à Lista de Projetos para novas linhas/projetos adicionados&quot;.
>
>    Você pode adicionar várias notas para um módulo.
>
>1. Feche a área **[!UICONTROL Notas]**.
>
>    Depois de adicionar uma observação a um cenário, um ponto laranja é exibido no ícone ![](assets/notes-icon-w-dot.png) das **[!UICONTROL Notas]**, na parte inferior do editor de cenários.
>
>1. Clique no ícone **[!UICONTROL Notas]** ![](assets/notes-icon-w-dot.png) para exibir suas notas.
>



## Ativar o cenário

Se esse fosse um cenário que você usaria para dados reais, a última coisa que faria seria ativá-lo. Após ativar um cenário, por padrão, ele é executado a cada 15 minutos. Você pode alterar isso definindo quando e com que frequência deseja que ele seja executado.

Para obter mais informações sobre como ativar cenários, consulte [Ativar ou desativar um cenário no Adobe Workfront Fusion](../../workfront-fusion/scenarios/activate-or-inactivate-scenario.md).

Para obter informações sobre agendamentos, consulte [Agendar um cenário no Adobe Workfront Fusion](../../workfront-fusion/scenarios/schedule-a-scenario.md).
