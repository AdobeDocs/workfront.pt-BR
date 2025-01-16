---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Criar um cenário de automação de prática em  [!DNL Adobe Workfront Fusion]
description: A documentação do Adobe Workfront Fusion foi movida para um novo local. Este artigo foi descontinuado, mas contém um link para o novo artigo que aborda essa funcionalidade.
author: Becky
feature: Workfront Fusion
exl-id: f6a6eb28-9b0b-48ea-af11-f55009a01178
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '1562'
ht-degree: 0%

---

# Criar um cenário de automação de prática em [!DNL Adobe Workfront Fusion]

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

Cenários de automação automatizam processos do Workfront, incluindo manipulação e transformação de dados. Este artigo orienta você pelo processo de criação de um cenário que pesquisa um projeto e retorna todas as tarefas associadas a esse projeto.

<!-- not sure why these are here?
For instructions on building an integration scenario that connects separate apps, see [Create a practice integration scenario in Adobe Workfront Fusion](../../workfront-fusion/get-started/create-a-practice-scenario.md).

For more information on functionality available with each Workfront Fusion license, see [Adobe Workfront Fusion licenses](../../workfront-fusion/get-started/license-automation-vs-integration.md).

-->

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte acesso para usar a funcionalidade neste artigo:

<table style="table-layout:auto"> 
  <tbody>  
    <tr>  
      <td>plano do Adobe Workfront</td>  
      <td>Qualquer</td>  
    </tr>  
    <tr>  
      <td>Licença do Adobe Workfront</td>  
      <td>
        Novo: Padrão<br>
        Ou<br>
        Atual: trabalho ou superior
      </td>  
    </tr>  
    <tr>  
      <td>Licença do Adobe Workfront Fusion</td>  
      <td> 
        Atual: nenhum requisito de licença do Workfront Fusion.<br>
        Ou<br>
        Herdados: Qualquer um
      </td>  
    </tr>  
    <tr>  
      <td>Produto</td>  
      <td> 
        Novo: Selecione ou Prime Workfront Plan: sua organização deve comprar o Adobe Workfront Fusion.<br>
        Plano do Ultimate Workfront: o Workfront Fusion está incluído.<br>
        Ou<br>
        Atual: sua organização deve comprar o Adobe Workfront Fusion.
      </td>  
    </tr> 
  </tbody>  
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

Para obter informações sobre [!DNL Adobe Workfront Fusion] licenças, consulte [[!DNL Adobe Workfront Fusion] licenças](../../workfront-fusion/get-started/license-automation-vs-integration.md).

+++

## Criar um cenário de prática de automação

O [!DNL Adobe Workfront Fusion] ajuda você a se concentrar em tarefas importantes, automatizando as repetitivas. Ele cria cenários que gerenciam automaticamente seus dados em vários aplicativos e serviços.

Cada cenário consiste em módulos, que orientam como os dados são processados em um aplicativo ou transferidos entre diferentes aplicativos e serviços. Por exemplo, é possível criar um cenário no Fusion para localizar automaticamente um projeto [!DNL Workfront] e listar suas tarefas. Dessa forma, o Fusion economiza tempo e esforço ao manipular tarefas de rotina.

Este cenário de prática orienta você pelo processo de criação de um cenário que procura por um projeto [!DNL Workfront] e retorna as tarefas no projeto.

![](assets/create-practice-scenario-wf-only-350x157.png)

### Antes de começar

Crie um projeto com tarefas no Workfront que você pode usar neste exercício. Não é necessário fazer nenhuma configuração adicional além de adicionar tarefas ao projeto.

Para obter informações sobre como criar um projeto no Workfront, consulte xxx.

### 1. Criar e nomear o cenário

1. Entre na sua conta [!DNL Workfront Fusion].
1. Clique em **[!UICONTROL Cenários]** ![](assets/scenarios-icon.png) no painel esquerdo.

   >[!NOTE]
   >
   >Se você não vir o painel de navegação esquerdo ou seus ícones, clique no ícone Menu ![Menu](assets/main-menu-icon-left-nav.png).

1. No painel [!UICONTROL **Pastas**], clique no ícone ![](assets/add-folder-icon.png) de **[!UICONTROL Adicionar pasta]** e digite um nome como &quot;Cenários de prática&quot; para a sua primeira pasta.

1. Abra a pasta e clique em **[!UICONTROL Criar um novo cenário]** no canto superior direito da página.

1. Para este exercício, selecione o aplicativo **[!DNL Adobe Workfront]** e clique em **Pesquisar** próximo à parte inferior.


1. Selecione o nome do espaço reservado **[!UICONTROL Novo cenário]** no canto superior esquerdo e digite um nome como &quot;Praticar cenário 1&quot;.

   ![](assets/name-the-scenario.png)

1. Continue com [Conecte o primeiro módulo](#2-connect-the-first-module) abaixo.

### 2. Conecte o primeiro módulo

Agora, é necessário estabelecer uma conexão autenticada com a conta do [!DNL Workfront]. Cada módulo adicionado a um cenário deve ter uma conexão com seu aplicativo.

1. Na caixa **[!DNL Workfront]**, em **[!UICONTROL Conexão]**, clique em **[!UICONTROL Adicionar]** e digite um nome para a conexão, como &quot;Conta da Workfront de Olivia&quot;, e clique em **[!UICONTROL Continuar]**.
1. Autentique a conexão na janela que é exibida.

   O processo para autenticar uma conexão pode variar um pouco entre os aplicativos. O processo a seguir é específico de [!DNL Workfront], mas é semelhante a vários aplicativos:

   1. Digite o domínio [!DNL Workfront] e clique em **[!UICONTROL Continuar]**.
   1. Faça logon em [!DNL Workfront].
   1. Examine o acesso que [!DNL Workfront Fusion] está solicitando e clique em **[!UICONTROL Permitir Acesso]**.

   Se precisar de ajuda, consulte [Visão geral das conexões](../../workfront-fusion/connections/about-connecting-wf-fusion-to-app-or-service.md).

### 3. Configure o primeiro módulo

Após conectar o [!DNL Workfront Fusion] à sua conta do [!DNL Workfront], você pode especificar um projeto do [!DNL Workfront] ao qual tenha acesso e os dados que deseja que o primeiro módulo processe.

1. Na caixa [!UICONTROL Tipo de Registro], selecione **[!UICONTROL Projeto]**. Isso define o módulo para pesquisar somente projetos.

   >[!TIP]
   >
   >Você pode encontrar **[!UICONTROL Projeto]** na lista se começar a digitar a palavra &quot;[!UICONTROL projeto].&quot;

1. Na caixa **[!UICONTROL Conjunto de Resultados]**, selecione **[!UICONTROL Primeiro Registro Correspondente]**. Isso define o módulo para retornar somente o primeiro registro encontrado que atenda aos critérios. Neste exemplo, precisamos apenas de um registro retornado.
1. Na área **[!UICONTROL Critérios de pesquisa]**, vamos configurar um filtro para retornar o projeto específico:

   | Campo | Ação |
   |--------|-------------|
   | Campos de critérios de pesquisa | Selecione o campo no qual deseja pesquisar os valores. Para este exemplo, selecione **[!UICONTROL Nome]**. |
   | Critérios de pesquisa | No primeiro menu suspenso, selecione **[!UICONTROL Nome]**. |
   | Operadores básicos | Na segunda lista suspensa, selecione [!UICONTROL Contém (não diferencia maiúsculas de minúsculas)]. Isso permite que o módulo encontre projetos com as palavras escolhidas em seu nome, mesmo se você não inserir o nome inteiro ou inserir o nome com a caixa incorreta (como todas em maiúsculas). |
   | Caixa de texto | Digite uma palavra ou frase que você sabe que está no nome do projeto que você está procurando. |

+++ Expanda para visualizar um exemplo na tela.
   ![](assets/search-name.png)
+++

1. Na lista **[!UICONTROL Saídas]**, selecione os campos nos quais deseja que o módulo faça a saída. Para este exemplo, selecione os campos **[!UICONTROL ID]** e **[!UICONTROL Name]**.

   >[!TIP]
   >
   >Você pode usar **Cmd+F** (SO [!DNL Mac]) ou **Ctrl-F** (SO [!DNL Windows]) para localizar um campo rapidamente.

1. Clique em **[!UICONTROL OK]**.

   >[!NOTE]
   >
   >Como esse não é um módulo acionador, você não escolhe onde iniciá-lo. Ao usar um módulo de acionador, você agora selecionaria onde iniciá-lo.
   >
   >
   >Para obter mais informações, consulte [Escolher onde um módulo de acionador começa em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/choose-where-trigger-module-starts.md).

1. Clique com o botão direito do mouse no módulo, clique em **[!UICONTROL Renomear]**, digite um nome que descreva o que você deseja que o módulo faça (como &quot;Procurar projeto&quot;) e clique em **[!UICONTROL OK]**.

   O nome aparece logo abaixo do módulo. Abaixo disso, [!DNL Workfront Fusion] inclui uma breve descrição do tipo de ação executada pelo módulo.

   ![](assets/module-renamed-wf.png)

1. Continue com [Adicionar e configurar o segundo módulo](#add-and-configure-the-second-module).

### 4. Adicionar e configurar o segundo módulo

1. Clique no círculo parcial à direita do do módulo para **[!UICONTROL Adicionar outro módulo]**.
1. Selecione [!DNL Workfront] na lista de aplicativos e escolha o módulo de pesquisa **[!UICONTROL Ler Registros Relacionados]**.
1. Na caixa **[!UICONTROL Conexão]**, selecione a conexão criada para o módulo anterior. Você deve verificar se esse módulo está usando a mesma conexão que o módulo anterior.
1. Clique em **[!UICONTROL Tipo de registro]** e selecione **[!UICONTROL Projeto]**, pois queremos ler registros relacionados a um projeto.

   >[!TIP]
   >
   >Você pode encontrar **[!UICONTROL Projeto]** na lista se começar a digitar a palavra &quot;projeto&quot;.

1. Clique no campo **[!UICONTROL ID do Registro Pai]**. Este campo requer a Workfront ID do projeto do qual você deseja retornar tarefas.

   Clicar no campo abre a lista de variáveis que podem ser usadas no campo **[!UICONTROL ID do Registro Pai]** para identificar o projeto no Workfront.

   ![](assets/list-of-available-variables-wf-350x368.png)

1. Clique na variável **[!UICONTROL ID]** para adicioná-la ao campo **[!UICONTROL ID do Registro Pai]**. Isso permite que a ID retornada do primeiro módulo seja usada como o identificador do projeto com o qual você deseja trabalhar no segundo módulo, o que garante que as tarefas retornadas pertençam a esse projeto.
1. No campo **[!UICONTROL Coleções]**, selecione **[!UICONTROL Tarefas]**. Isso indica que o módulo retornará tarefas associadas ao projeto escolhido.
1. No campo **[!UICONTROL Saídas]**, selecione **[!UICONTROL Id]** e **[!UICONTROL Nome]**.
1. Clique em **[!UICONTROL OK]**

   Agora você tem um cenário de trabalho.

1. Dê um nome ao segundo módulo, como &quot;Retornar tarefas associadas ao projeto&quot;, e continue com [Testar o cenário](#test-the-scenario).

## Testar o cenário

Antes de ativar o cenário, é importante testá-lo executando-o pelo menos uma vez e visualizando os resultados. Isso ajuda você a entender como os dados fluem pelo cenário e encontrar erros.

Escolhemos ter 1 projeto retornado, bem como as tarefas associadas a esse projeto. Se você executar o cenário, isso é o que deve acontecer.

1. Clique em **[!UICONTROL Executar uma vez]** no canto inferior esquerdo do editor de cenários.
1. Depois que o cenário terminar de ser executado, clique no balão acima do primeiro módulo.

   ![](assets/click-bubble.png)

   Na caixa que aparece, você pode visualizar informações sobre o pacote de dados que o módulo processou, incluindo os dados reais que foram obtidos do projeto que o módulo retornou.

   ![](assets/execution-inspector-wf-only-first-350x423.png)

1. Clique na bolha do inspetor de execução acima do Segundo módulo para ver a entrada de informações e a saída, que é uma coleção de tarefas contidas no projeto.

   ![](assets/execution-inspector-wf-only-second-350x738.png)

   Você pode saber mais sobre como ler as informações de execução do cenário nos seguintes artigos:

   * Para obter informações gerais, consulte [Fluxo de execução do cenário em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-flow.md).
   * Para obter informações sobre pacotes processados, consulte [Execução do cenário, ciclos e fases em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

1. Em [!DNL Workfront Fusion], clique em **[!UICONTROL Salvar]** ![](assets/save-icon.png) próximo ao canto inferior esquerdo para salvar seu progresso no cenário.

   >[!IMPORTANT]
   >
   >Salve com frequência à medida que você aprimora e testa um cenário.

>[!TIP]
>
>Recomendamos a prática opcional, mas útil, de adicionar observações sobre cada módulo.
>
>1. Clique com o botão direito do mouse em um módulo [!DNL Workfront] e clique em **[!UICONTROL Adicionar uma observação]**.
>1. Na nota exibida, digite uma visão geral do módulo.
>
>    Você pode adicionar várias notas para um módulo.
>
>1. Feche a área **[!UICONTROL Notas]**.
>
>     Depois de adicionar uma observação a um cenário, um ponto laranja é exibido no ícone ![](assets/notes-icon-w-dot.png) das **[!UICONTROL Notas]**, na parte inferior do editor de cenários.
>
>1. Clique no ícone **[!UICONTROL Notas]** ![](assets/notes-icon-w-dot.png) para exibir suas notas.
>

## Ativar o cenário

Este cenário de exemplo não tem um módulo acionador. Se esse fosse um cenário usado para dados reais, ele começaria com um módulo de acionamento e a última coisa que você faria é ativá-lo. Após ativar um cenário, por padrão, ele é executado a cada 15 minutos. Você pode alterar isso definindo quando e com que frequência deseja que ele seja executado.

Para obter mais informações sobre como ativar cenários, consulte [Ativar ou desativar um cenário no [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/activate-or-inactivate-scenario.md).

Para obter informações sobre agendamentos, consulte [Agendar um cenário no [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/schedule-a-scenario.md).
