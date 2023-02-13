---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Criar um cenário de integração de prática no Adobe Workfront Fusion
description: Este artigo descreve como criar um cenário de integração com o Adobe Workfront Fusion. Os cenários de integração conectam aplicativos separados, permitindo que seus dados fluam por diferentes aplicativos.
author: Becky
feature: Workfront Fusion
exl-id: 643bb1d5-d7bc-402b-8ed1-9ca9a30e4560
source-git-commit: c57a796ccbfb36bce58d49345e7515dd524604c5
workflow-type: tm+mt
source-wordcount: '2076'
ht-degree: 0%

---

# Criar um cenário de integração de prática no Adobe Workfront Fusion

Este artigo descreve como criar um cenário de integração com o Adobe Workfront Fusion. Os cenários de integração conectam aplicativos separados, permitindo que seus dados fluam por diferentes aplicativos.

Para criar um cenário de integração, sua organização deve ter um [!DNL Workfront Fusion for Work Automation and Integration] licença.

Para obter instruções sobre como criar um cenário de automação somente Workfront, consulte [Criar um cenário de automação de práticas no Adobe Workfront Fusion](../../workfront-fusion/get-started/create-a-practice-automation-scenario.md)

Para obter mais informações sobre licenças do Workfront Fusion, consulte [Licenças do Adobe Workfront Fusion](../../workfront-fusion/get-started/license-automation-vs-integration.md).

>[!NOTE]
>
>Sua organização pode não permitir o acesso às planilhas Google. Se esse for o caso, você não poderá configurar essa integração, mas as informações apresentadas aqui podem ser usadas como um exemplo geral de como os cenários de integração funcionam.

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

## Criar um cenário de prática

O papel do [!DNL Adobe Workfront Fusion] O é automatizar seus processos para que você possa se concentrar em novas tarefas em vez de repetir as mesmas tarefas várias vezes. Funciona vinculando ações dentro e entre aplicativos e serviços para criar um cenário que transfere e transforma seus dados automaticamente. O cenário criado busca dados em um aplicativo ou serviço e processa esses dados para fornecer o resultado desejado.

Um cenário é composto por uma série de módulos que indicam como os dados devem ser transformados em um aplicativo ou transferidos entre aplicativos e serviços da Web.

Para explicar como criar um cenário e reforçar as práticas recomendadas conforme você aprende a usar [!DNL Workfront Fusion], este artigo o orienta pelo processo passo a passo. Criaremos um cenário que cria um novo registro em [!DNL Workfront] para cada linha em uma [!DNL Google Sheets] planilha.

![](assets/finished-scenario-1-350x180.png)

>[!TIP]
>
>Um cenário como esse seria útil se você tivesse uma planilha listando projetos que precisam ser trabalhados no uso de projetos na [!DNL Workfront]. O cenário poderia &quot;observar&quot; a planilha de novas linhas e adicionar um novo projeto em [!DNL Workfront] para cada um.

A criação de um cenário consiste em várias tarefas principais:

## Escolha os aplicativos e nomeie o cenário

1. Baixe isto [planilha](https://cdn.experience.workfront.com/Documentation/Workfront+Fusion/Fusion+Practice+Scenario+Sample+Sheet.xlsx)e, em seguida, faça o upload para seu [!DNL Google Drive] para utilização durante este exercício.

   Ou

   Crie ou encontre seu próprio [!DNL Google Sheets] planilha semelhante a esta:

   ![](assets/spreadsheet-headers-350x55.png)

1. Faça logon em seu [!DNL Workfront Fusion] conta.
1. Clique em **[!UICONTROL Cenários]** ![](assets/scenarios-icon.png) no painel esquerdo.

   No painel esquerdo exibido, você pode organizar os cenários em pastas.

   Na parte superior da área principal à direita, é possível visualizar **[!UICONTROL Todos]** cenários que você criou, **[!UICONTROL Cenários ativos]** e **[!UICONTROL Cenários inativos]** e **[!UICONTROL Conceitos]**, que são cenários que precisam de mais trabalho antes [!DNL Workfront Fusion] podem classificá-los como ativos ou inativos.

   ![](assets/scenarios-left-panel-350x215.png)

1. No painel esquerdo, clique no botão **[!UICONTROL Adicionar pasta]** ícone ![](assets/add-folder-icon.png)e digite um nome como &quot;Cenários de prática&quot; para a primeira pasta.

1. Abra a pasta e clique em **[!UICONTROL Criar um novo cenário]** no canto superior direito da página.

   A landing page exibida permite pré-carregar os aplicativos que deseja usar na situação que você vai criar.

1. Para este exercício, pesquise e selecione a variável **[!UICONTROL Google Sheets]** aplicativo.
1. Clique em **[!UICONTROL Continuar]** no canto superior direito.

   O editor de cenário é exibido, contendo um módulo vazio no centro, o [!DNL Google Sheets] aplicativo pré-carregado e algumas opções na barra de ferramentas na parte inferior.

   ![](assets/scenario-editor-350x235.png)

   Quando você começa a criar um novo cenário, é uma boa ideia começar criando um nome para ele.

1. Selecione o **[!UICONTROL Novo cenário]** nome do espaço reservado no canto superior esquerdo e, em seguida, digite um nome como &quot;Cenário de prática 1&quot;.
1. Continue com [Adicionar e configurar o primeiro módulo](#add-and-configure-the-first-module) abaixo.

## Adicionar e configurar o primeiro módulo

O módulo vazio com um ponto de interrogação representa o módulo de acionador que você precisa adicionar. Esse módulo iniciará o cenário sempre que for executado. O ícone de relógio no módulo vazio indica que é um módulo agendado.

![](assets/empty-module.png)

Esse módulo conterá os dados que o cenário deve ser observado.

1. Clique no módulo vazio para escolher o aplicativo do qual você selecionará um módulo.

   O aplicativo pré-carregado anteriormente é exibido ao lado do módulo vazio. Você pode adicionar outros aplicativos que tenham módulos usando o [!UICONTROL Pesquisar] caixa.

   ![](assets/pre-loaded-apps-350x139.png)

1. Clique em **[!DNL Google Sheets]**.

   A lista muda para exibir todas as [!DNL Google Sheets] módulos que você pode usar como um módulo de acionador.

1. Clique no módulo de acionador **[!UICONTROL Assistir aos registros]**.

   Agora é necessário estabelecer uma conexão autenticada com sua conta Google. Cada módulo adicionado a um cenário deve ter uma conexão com seu aplicativo.

1. No **[!DNL Google Sheets]** caixa , abaixo **[!UICONTROL Conexão]**, clique em **[!UICONTROL Adicionar]** e digite um nome para a conexão, como &quot;Conta Google de Olivia&quot;, em seguida, clique em **[!UICONTROL Continuar]**.
1. Autentique a conexão na janela exibida.

   O processo de autenticação de conexão pode variar um pouco entre aplicativos. Talvez seja necessário fazer logon no aplicativo. Geralmente, é necessário clicar em um **[!UICONTROL Permitir]** botão. Se precisar de ajuda, consulte [Sobre a conexão [!DNL Adobe Workfront Fusion] para um aplicativo ou serviço](../../workfront-fusion/connections/about-connecting-wf-fusion-to-app-or-service.md).

## Configurar o primeiro módulo

Depois de se conectar [!DNL Workfront Fusion] para [!DNL Google Sheets] você pode especificar uma [!DNL Google Sheets] planilha à qual você tem acesso e os dados lá que você deseja que o primeiro módulo processe.

1. Clique no botão **[!UICONTROL Planilha]** , em seguida, selecione a **[!UICONTROL Cenário de prática do Workfront Fusion] #1** planilha na lista exibida.

   Esta planilha contém 2 planilhas (guias), portanto, precisamos especificar qual planilha contém os dados desejados:

1. No **[!UICONTROL Folha]** , selecione **[!UICONTROL Projetos]**.

   Nossa planilha contém cabeçalhos e queremos que o módulo os use para identificar os dados que queremos processar:

   ![](assets/spreadsheet-headers-350x55.png)

1. Sair **[!UICONTROL Sim]** selecionado para **[!UICONTROL A tabela contém cabeçalhos]**.

1. No **[!UICONTROL Linha com cabeçalhos]** , você pode especificar um intervalo de linhas que deseja incluir, mas vamos deixar o padrão A1:Z1 lá para este exercício.
1. No **[!UICONTROL Limite]** , digite 1.

   Dessa forma, toda vez que você executar o cenário, o módulo processará apenas uma linha na planilha. Isso é útil para simplificar suas execuções de teste enquanto você cria o cenário.

1. Clique em **[!UICONTROL OK]**.

   O **[!UICONTROL Escolha onde começar]** solicita que você especifique onde deseja que o módulo inicie o processamento na planilha na planilha.

1. Clique em **[!UICONTROL Escolher manualmente]**, selecione a opção superior na lista exibida e clique em **[!UICONTROL OK]**.
1. Clique com o botão direito do mouse no módulo e clique em **[!UICONTROL Renomear]** e digite um nome para a descrição do que deseja que o módulo faça (como &quot;Assista à lista de projetos&quot;) e clique em **[!UICONTROL OK]**.

   O nome aparece logo abaixo do módulo . Abaixo disso, [!DNL Workfront Fusion] inclui uma breve descrição do tipo de ação executada pelo módulo.

   ![](assets/module-renamed-350x388.png)

1. Continue com [Adicionar e configurar o segundo módulo](#add-and-configure-the-second-module).

## Adicionar e configurar o segundo módulo

1. Clique no círculo parcial à direita do do módulo para **[!UICONTROL Adicionar outro módulo]**.

   Esse segundo módulo precisa ser um [!DNL Workfront] , mas não pré-carregamos o [!DNL Workfront] aplicativo.

1. Para encontrar o [!DNL Workfront] aplicativo, comece a digitar &quot;[!DNL Workfront]&quot; e clique no aplicativo quando ele for exibido.
1. Na lista de [!DNL Workfront] módulos exibidos, clique em **[!UICONTROL Criar registro]**.

1. Como você fez antes com o aplicativo Google Sheets, clique em **[!UICONTROL Adicionar]** no [!DNL Workfront] para adicionar uma conexão entre o Workfront Fusion e o Workfront.

   Agora, começaremos a especificar o que queremos fazer com os dados da planilha.

1. Clique em **[!UICONTROL Tipo de registro]**, em seguida selecione **[!UICONTROL Projeto]** porque queremos criar um projeto no [!DNL Workfront] usando uma linha da planilha.

   >[!TIP]
   >
   >Você pode encontrar **[!UICONTROL Projeto]** na lista, se você começar a digitar a palavra &quot;[!UICONTROL projeto].&quot;

   A caixa se expande para exibir todas as [!DNL Workfront] campos do projeto, onde é possível colocar as informações encontradas pelo primeiro módulo.

   Vamos usar o **[!UICONTROL Nome]** campo : queremos que este módulo nomeie cada projeto no [!DNL Workfront] usando o texto no [!UICONTROL Google Sheets] linha.

1. Localize e clique no botão **[!UICONTROL Nome]** campo.

   >[!TIP]
   >
   >Você pode usar **Cmd+F** ([!DNL Mac] OS) ou **Ctrl-F**([!DNL Windows] SO) para localizar um campo rapidamente.

   Essa ação abre a lista de variáveis que podem ser usadas no **[!UICONTROL Nome]** para definir o nome de cada projeto criado no Workfront.

   ![](assets/list-of-available-variables-350x261.png)

   Observe que as variáveis perto do topo da lista correspondem aos cabeçalhos das colunas na planilha.

   ![](assets/spreadsheet-headers-marked-350x55.png)

   ![](assets/list-of-available-variables-marked-350x320.png)

1. Clique na variável **[!UICONTROL Nome do projeto (A)]** para adicioná-lo ao **[!UICONTROL Nome]** campo.

   Você acabou de mapear a primeira parte dos dados para este cenário.

   Vamos mapear mais um dado da planilha para [!DNL Workfront]: a data de início de cada projeto.

1. Localize e clique no botão **[!UICONTROL Data de início planejada]** , em seguida, clique no botão **[!UICONTROL Data Inicial Planejada (E)]** , para extrair dados dessa coluna na planilha.

1. Clique em **[!UICONTROL OK]**.

   Agora você tem um cenário de trabalho.

1. Dê um nome ao segundo módulo, como &quot;Criar projeto do Workfront&quot; e continue com [Testar o cenário](#test-the-scenario).

## Testar o cenário

Antes de ativar seu cenário, é importante testá-lo executando-o pelo menos uma vez e visualizando os resultados. Isso ajuda você a entender como os dados fluem pelo cenário e encontrar erros.

Optamos por ter uma linha da planilha processada para criar um projeto no Workfront. Se você executar o cenário, é isso que deve acontecer.

1. Clique em **[!UICONTROL Executar uma vez]** no canto inferior esquerdo do editor de cenário.
1. Depois que o cenário terminar de ser executado, clique na bolha acima do [!DNL Google Sheets] módulo.

   ![](assets/click-bubble.png)

   Na caixa exibida, é possível exibir informações sobre o pacote de dados processados pelo módulo, incluindo os dados reais que foram obtidos da planilha para a linha com a qual você começou.

   ![](assets/execution-inspector-g-sheets-350x637.png)

1. Clique na bolha do inspetor de execução acima de [!DNL Workfront] para ver a entrada de informações e a saída, que é a ID do projeto agora criado em [!DNL Workfront]

   ![](assets/execution-inspector-wf-350x384.png)

   Você pode saber mais sobre como ler as informações de execução do cenário nos seguintes artigos:

   * Para obter informações gerais, consulte [Fluxo de execução do cenário em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-flow.md).
   * Para obter informações sobre pacotes processados, consulte [Execução do cenário, ciclos e fases em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

1. Ir para [!DNL Workfront] e procure por &quot;soho downtown loft&quot; para ver o projeto criado pelo cenário. Esta foi a última linha na planilha.
1. Em [!DNL Workfront Fusion], clique em **[!UICONTROL Salvar]** ![](assets/save-icon.png) próximo ao canto inferior esquerdo para salvar o progresso no cenário.

   >[!IMPORTANT]
   >
   >Salve sempre que você tocar e testar um cenário.

## Finalize o cenário e teste-o novamente

Ainda precisamos configurar o cenário para criar projetos para todas as outras linhas na planilha.

1. Clique no botão **[!UICONTROL Linhas de observação]** módulo que você criou para Google Sheets.
1. Altere o **[!UICONTROL Limite]** para 100.

   Especificar um número superior ao número de linhas que você sabe que estão na planilha garante que o cenário irá capturar todas elas.

1. Clique com o botão direito do mouse no **[!UICONTROL Linhas de observação]** módulo, clique em **[!UICONTROL Escolha onde começar]**, clique em **[!UICONTROL Todos]**, depois clique em **[!UICONTROL OK]**.

1. Clique em **[!UICONTROL Executar uma vez]** e observe o que acontece nas bolhas do inspetor de execução.

   O [!DNL Google] Folhas **[!UICONTROL Linhas de observação]** O módulo é executado uma vez para ler todas as linhas. Em seguida, a Workfront **[!UICONTROL Criar registro]** O módulo é executado 20 vezes para criar um projeto para cada uma das 20 linhas restantes na planilha.

1. Clique na bolha do inspetor de execução para [!DNL Workfront] para visualizar todas as 20 operações, clique em uma das operações para visualizar as informações sobre o projeto criado.
1. Clique em **[!UICONTROL Salvar]** ![](assets/save-icon.png) próximo ao canto inferior esquerdo.
1. Ir para [!DNL Workfront] para ver os projetos criados pelo cenário.

>[!TIP]
>
>Recomendamos a prática opcional, mas útil, de adicionar observações sobre cada módulo.
>
>1. Clique com o botão direito do mouse no [!DNL Workfront] e clique em **[!UICONTROL Adicionar uma nota]**.
>1. Na nota que é exibida, digite uma visão geral para o módulo.

>
>   Isso é útil porque você não precisará abrir continuamente o módulo para ver o que ele faz. Você pode digitar algo como &quot;Cria um projeto com Nome, Data de início planejada e Prioridade mapeada da planilha&quot;.
>
>   Para o [!UICONTROL Google Sheets] , você pode digitar algo como &quot;Assistir à lista de projetos para novas linhas/projetos adicionados&quot;.
>
>   É possível adicionar várias observações para um módulo.
>
>1. Feche o **[!UICONTROL Notas]** área.
>
>   Depois de adicionar uma observação a um cenário, um ponto laranja é exibido no cenário **[!UICONTROL Notas]** ícone ![](assets/notes-icon-w-dot.png) na parte inferior do editor de cenário.
>
>1. Clique no botão **[!UICONTROL Notas]** ícone ![](assets/notes-icon-w-dot.png) para visualizar suas notas.

>




## Ativar o cenário

Se esse fosse um cenário que você usaria para dados reais, a última coisa que você faria seria ativá-lo. Após ativar um cenário, por padrão, ele é executado a cada 15 minutos. Você pode alterar isso definindo quando e com que frequência deseja que seja executado.

Para obter mais informações sobre como ativar cenários, consulte [Ativar ou desativar um cenário no Adobe Workfront Fusion](../../workfront-fusion/scenarios/activate-or-inactivate-scenario.md).

Para obter informações sobre programações, consulte [Programar um cenário no Adobe Workfront Fusion](../../workfront-fusion/scenarios/schedule-a-scenario.md).
