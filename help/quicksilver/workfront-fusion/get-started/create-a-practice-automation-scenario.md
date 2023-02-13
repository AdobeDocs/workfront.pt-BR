---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Crie um cenário de automação de práticas em [!DNL Adobe Workfront Fusion]
description: Este artigo descreve como criar um cenário de automação com o Adobe Workfront Fusion. Os cenários de automação automatizam os processos do Workfront, incluindo a manipulação e transformação de dados. Este exemplo o orienta pelo processo de criação de um cenário que pesquisa por um projeto e retorna todas as tarefas associadas a esse projeto.
author: Becky
feature: Workfront Fusion
exl-id: f6a6eb28-9b0b-48ea-af11-f55009a01178
source-git-commit: 97f91d663df86341a079894cff04d07c18b7bf08
workflow-type: tm+mt
source-wordcount: '1782'
ht-degree: 0%

---

# Crie um cenário de automação de práticas em [!DNL Adobe Workfront Fusion]

Este artigo descreve como criar um cenário de automação com o Adobe Workfront Fusion. Os cenários de automação automatizam os processos do Workfront, incluindo a manipulação e transformação de dados. Este exemplo o orienta pelo processo de criação de um cenário que pesquisa por um projeto e retorna todas as tarefas associadas a esse projeto.

Para obter instruções sobre como criar um cenário de integração que conecta aplicativos separados, consulte [Criar um cenário de integração de prática no Adobe Workfront Fusion](../../workfront-fusion/get-started/create-a-practice-scenario.md).

Para obter mais informações sobre a funcionalidade disponível com cada licença do Workfront Fusion, consulte [Licenças do Adobe Workfront Fusion](../../workfront-fusion/get-started/license-automation-vs-integration.md).

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] para automação e integração de trabalho] </p><p>[!UICONTROL [!DNL Workfront Fusion] para Automação de Trabalho]</p>  </td> 
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
Este exemplo o orienta pelo processo de criação de um cenário que pesquisa por um [!DNL Workfront] e retorna as tarefas no projeto.

![](assets/create-practice-scenario-wf-only-350x157.png)

A criação de um cenário consiste em várias tarefas principais:

## Escolha os aplicativos e nomeie o cenário

1. Faça logon em seu [!DNL Workfront Fusion] conta.
1. Clique em **[!UICONTROL Cenários]** ![](assets/scenarios-icon.png) no painel esquerdo.

   No painel esquerdo exibido, você pode organizar os cenários em pastas.

   Na parte superior da área principal à direita, é possível visualizar **[!UICONTROL Todos]** cenários que você criou, **[!UICONTROL Cenários ativos]**, **[!UICONTROL Cenários inativos]** e **[!UICONTROL Conceitos]**. Os conceitos são cenários que precisam de mais trabalho antes [!DNL Workfront Fusion] podem classificá-los como ativos ou inativos.

   ![](assets/scenarios-left-panel-350x215.png)

1. No painel esquerdo, clique no botão **[!UICONTROL Adicionar pasta]** ícone ![](assets/add-folder-icon.png)e digite um nome como &quot;Cenários de prática&quot; para a primeira pasta.

1. Abra a pasta e clique em **[!UICONTROL Criar um novo cenário]** no canto superior direito da página.

   A landing page exibida permite pré-carregar os aplicativos que deseja usar na situação que você vai criar.

1. Para este exercício, pesquise e selecione a variável **[!DNL Workfront]** aplicativo.
1. Clique em **[!UICONTROL Continuar]** no canto superior direito.

   O editor de cenário é exibido, contendo um módulo vazio no centro, o [!DNL Workfront] aplicativo pré-carregado e algumas opções na barra de ferramentas na parte inferior.

   ![](assets/scenario-editor-350x235.png)

   Quando você começa a criar um novo cenário, é uma boa ideia começar criando um nome para ele.

1. Selecione o **[!UICONTROL Novo cenário]** nome do espaço reservado no canto superior esquerdo e, em seguida, digite um nome como &quot;Cenário de prática 1&quot;.
1. Continue com [Adicionar e configurar o primeiro módulo](#add-and-configure-the-first-module) abaixo.

## Adicionar e configurar o primeiro módulo

O módulo vazio com um ponto de interrogação representa o módulo de acionador que você precisa adicionar. Esse módulo iniciará o cenário sempre que for executado. O ícone de relógio no módulo vazio indica que é um módulo agendado.

![](assets/empty-module.png)

Esse módulo conterá os dados que o cenário deve ser observado.

Neste exemplo, não estamos usando um módulo de acionador. Em vez disso, esse cenário começa com uma pesquisa.

1. Clique no módulo vazio para escolher o aplicativo do qual você selecionará um módulo.

   O aplicativo pré-carregado anteriormente é exibido ao lado do módulo vazio. Você pode adicionar outros aplicativos que tenham módulos usando o [!UICONTROL Pesquisar] caixa.

   ![](assets/pre-loaded-app-wf-350x172.png)

1. Clique em **[!DNL Workfront]**.

   A lista muda para exibir todas as [!DNL Workfront] módulos que você pode usar como um módulo de acionador.

1. Clique no módulo Pesquisar **[!UICONTROL Pesquisar]**.

   Agora é necessário estabelecer uma conexão autenticada com o [!DNL Workfront] conta. Cada módulo adicionado a um cenário deve ter uma conexão com seu aplicativo.

1. No **[!DNL Workfront]** caixa , abaixo **[!UICONTROL Conexão]**, clique em **[!UICONTROL Adicionar]** e digite um nome para a conexão, como &quot;Conta Workfront de Olivia&quot;, em seguida, clique em **[!UICONTROL Continuar]**.
1. Autentique a conexão na janela exibida.

   O processo de autenticação de conexão pode variar um pouco entre aplicativos. O processo a seguir é específico para [!DNL Workfront], mas o processo é semelhante a muitos aplicativos.

   1. Insira seu [!DNL Workfront] domínio e, em seguida, clique em **[!UICONTROL Continuar]**.
   1. Faça logon [!DNL Workfront].
   1. Examine o acesso que [!DNL Workfront Fusion] está solicitando, em seguida, clique em **[!UICONTROL Permitir acesso]**.

   Se precisar de ajuda, consulte [Sobre a conexão [!DNL Adobe Workfront Fusion] para um aplicativo ou serviço](../../workfront-fusion/connections/about-connecting-wf-fusion-to-app-or-service.md).

## Configurar o primeiro módulo

Depois de se conectar [!DNL Workfront Fusion] para [!DNL Workfront] você pode especificar uma [!DNL Workfront] fila de solicitações à qual você tem acesso e os dados lá que você deseja que o primeiro módulo processe.

1. No [!UICONTROL Tipo de registro] , selecione **[!UICONTROL Projeto]**. Isso define o módulo para pesquisar somente projetos.

   >[!TIP]
   >
   >Você pode encontrar **[!UICONTROL Projeto]** na lista, se você começar a digitar a palavra &quot;[!UICONTROL projeto].&quot;

1. No **[!UICONTROL Conjunto de resultados]** , selecione **[!UICONTROL Registro da Primeira Correspondência]**. Isso define o módulo para retornar somente o primeiro registro que ele encontrar que atenda aos critérios. Neste exemplo, precisamos de apenas um registro retornado.
1. No **[!UICONTROL Critérios de pesquisa]** , vamos configurar um filtro para retornar o projeto específico.

   1. Na primeira caixa em [!UICONTROL Critérios de pesquisa], selecione o campo no qual deseja pesquisar os valores. Para este exemplo, selecione **[!UICONTROL Nome]**.
   1. Para o operador , selecione [!UICONTROL Contém (não diferencia maiúsculas de minúsculas)]. Isso permite que o módulo encontre projetos com as palavras escolhidas em seu nome, mesmo que você não digite o nome inteiro ou insira o nome com as letras maiúsculas e minúsculas incorretas (como todas as maiúsculas).
   1. No último campo, em [!UICONTROL Critérios de pesquisa], digite uma palavra ou frase que você sabe que está no nome do projeto que está procurando.

1. No **[!UICONTROL Saídas]** selecione os campos que o problema deve exibir. Para este exemplo, selecione o **[!UICONTROL ID]** e **[!UICONTROL Nome]** campos.

   >[!TIP]
   >
   >Você pode usar **Cmd+F** ([!DNL Mac] OS) ou **Ctrl-F** ([!DNL Windows] SO) para localizar um campo rapidamente.

1. Clique em **[!UICONTROL OK]**.

   >[!NOTE]
   >
   >(Somente informações) Como esse não é um módulo acionador, você não escolhe onde iniciá-lo. Ao usar um módulo de acionador, agora você selecionaria onde iniciá-lo.
   >
   >
   >Para obter mais informações, consulte [Escolha onde um módulo de acionador começa em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/choose-where-trigger-module-starts.md).

1. Clique com o botão direito do mouse no módulo e clique em **[!UICONTROL Renomear]**, em seguida, digite um nome para a descrição do que deseja que o módulo faça (como &quot;Pesquisar projeto&quot;) e clique em **[!UICONTROL OK]**.

   O nome aparece logo abaixo do módulo . Abaixo disso, [!DNL Workfront Fusion] inclui uma breve descrição do tipo de ação executada pelo módulo.

   ![](assets/module-renamed-wf.png)

1. Continue com [Adicionar e configurar o segundo módulo](#add-and-configure-the-second-module).

## Adicionar e configurar o segundo módulo

1. Clique no círculo parcial à direita do do módulo para **[!UICONTROL Adicionar outro módulo]**.
1. Selecionar [!DNL Workfront] na lista de aplicativos, escolha o módulo de pesquisa **[!UICONTROL Ler registros relacionados]**.
1. Você já criou uma conexão com [!DNL Workfront] para o módulo anterior. Não é necessário criá-lo novamente aqui, mas certifique-se de que esse módulo esteja usando a mesma conexão do módulo anterior.\
   No **[!UICONTROL Conexão]** selecione a conexão criada para o módulo anterior.
1. Clique em **[!UICONTROL Tipo de registro]**, em seguida selecione **[!UICONTROL Projeto]**, pois queremos ler registros relacionados a um projeto.

   >[!TIP]
   >
   >Você pode encontrar **[!UICONTROL Projeto]** na lista, se você começar a digitar a palavra &quot;projeto&quot;.

1. Clique no botão **[!UICONTROL ID de registro pai]** campo. Este campo requer a Workfront ID do projeto do qual você deseja retornar tarefas.

   Clicar no campo abre a lista de variáveis que podem ser usadas no **[!UICONTROL ID de registro pai]** para identificar o projeto no Workfront.

   ![](assets/list-of-available-variables-wf-350x368.png)

1. Clique na variável **[!UICONTROL ID]** para adicioná-lo ao **[!UICONTROL ID de registro pai]** campo. Isso permite que a ID retornada do primeiro módulo seja usada como o identificador do projeto com o qual você deseja trabalhar no segundo módulo, o que garante que as tarefas retornadas pertençam a esse projeto.
1. No **[!UICONTROL Coleções]** , selecione **[!UICONTROL Tarefas]**. Isso indica que o módulo deve retornar tarefas associadas ao projeto escolhido.
1. Clique em **[!UICONTROL OK]**

   Agora você tem um cenário de trabalho.

1. Dê um nome ao segundo módulo, como &quot;Tarefas de retorno associadas ao projeto&quot; e continue com [Testar o cenário](#test-the-scenario).

## Testar o cenário

Antes de ativar seu cenário, é importante testá-lo executando-o pelo menos uma vez e visualizando os resultados. Isso ajuda você a entender como os dados fluem pelo cenário e encontrar erros.

Optamos por retornar 1 projeto, bem como as tarefas associadas a esse projeto. Se você executar o cenário, é isso que deve acontecer.

1. Clique em **[!UICONTROL Executar uma vez]** no canto inferior esquerdo do editor de cenário.
1. Depois que o cenário terminar de ser executado, clique na bolha acima do primeiro módulo.

   ![](assets/click-bubble.png)

   Na caixa exibida, é possível exibir informações sobre o pacote de dados que o módulo processou, incluindo os dados reais que foram obtidos do projeto retornado pelo módulo.

   ![](assets/execution-inspector-wf-only-first-350x423.png)

1. Clique na bolha do inspetor de execução acima do segundo módulo para ver a entrada de informações e a saída, que é uma coleção de tarefas contidas no projeto.

   ![](assets/execution-inspector-wf-only-second-350x738.png)

   Você pode saber mais sobre como ler as informações de execução do cenário nos seguintes artigos:

   * Para obter informações gerais, consulte [Fluxo de execução do cenário em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-flow.md).
   * Para obter informações sobre pacotes processados, consulte [Execução do cenário, ciclos e fases em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

1. Em [!DNL Workfront Fusion], clique em **[!UICONTROL Salvar]** ![](assets/save-icon.png) próximo ao canto inferior esquerdo para salvar o progresso no cenário.

   >[!IMPORTANT]
   >
   >Salve sempre que você tocar e testar um cenário.

>[!TIP]
>
>Recomendamos a prática opcional, mas útil, de adicionar observações sobre cada módulo.
>
>1. Clique com o botão direito do mouse em um [!DNL Workfront] e clique em **[!UICONTROL Adicionar uma nota]**.
>1. Na nota que é exibida, digite uma visão geral para o módulo.

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

Este exemplo de cenário não tem um módulo de acionador. Se esse fosse um cenário que você estaria usando para dados reais, ele começaria com um módulo de acionador e a última coisa que você faria seria ativá-lo. Após ativar um cenário, por padrão, ele é executado a cada 15 minutos. Você pode alterar isso definindo quando e com que frequência deseja que seja executado.

Para obter mais informações sobre como ativar cenários, consulte [Ativar ou desativar um cenário em [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/activate-or-inactivate-scenario.md).

Para obter informações sobre programações, consulte [Programe um cenário em [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/schedule-a-scenario.md).
