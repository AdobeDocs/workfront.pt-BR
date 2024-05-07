---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Criar um cenário básico no [!DNL Adobe Workfront Fusion]
description: Saiba como criar um cenário de automação simples com o Adobe Workfront Fusion. Cenários de automação automatizam processos do Workfront, incluindo manipulação e transformação de dados. Este exemplo orienta você no processo de criação de um cenário que procura por um [!DNL Workfront] no Workfront e o a converte em um projeto.
author: Becky
feature: Workfront Fusion
source-git-commit: 91d3dcde8eda416286c6781f6eef85404fd382c2
workflow-type: tm+mt
source-wordcount: '1300'
ht-degree: 0%

---

# Criar um cenário básico no [!DNL Adobe Workfront Fusion]

O papel da [!DNL Adobe Workfront Fusion] O é automatizar seus processos para que você possa se concentrar em novas tarefas, em vez de repetir as mesmas tarefas repetidamente. Ele funciona vinculando ações em e entre aplicativos e serviços para criar um cenário que transfere e transforma seus dados automaticamente. O cenário que você cria observa dados em um aplicativo ou serviço e processa esses dados para fornecer o resultado desejado.

Este exemplo orienta você no processo de criação de um cenário que procura por um [!DNL Workfront] no Workfront e o a converte em um projeto.

<!--# Access requirements

You must have the following access to use the functionality in this article:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!DNL Pro] or higher</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion] license**</td> 
   <td>
   <p>Current license requirement: No [!DNL Workfront Fusion] license requirement.</p>
   <p>Or</p>
   <p>Legacy license requirement: [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>
   <p>Current product requirement: If you have the [!UICONTROL Select] or [!UICONTROL Prime] [!DNL Adobe Workfront] Plan, your organization must purchase [!DNL Adobe Workfront Fusion] as well as [!DNL Adobe Workfront] to use functionality described in this article. [!DNL Workfront Fusion] is included in the [!UICONTROL Ultimate] [!DNL Workfront] plan.</p>
   <p>Or</p>
   <p>Legacy product requirement: Your organization must purchase [!DNL Adobe Workfront Fusion] as well as [!DNL Adobe Workfront] to use functionality described in this article.</p>
   </td> 
  </tr> 
 </tbody> 
</table>
To find out what plan, license type, or access you have, contact your [!DNL Workfront] administrator.

For information on [!DNL Adobe Workfront Fusion] licenses, see [[!DNL Adobe Workfront Fusion] licenses](../../workfront-fusion/get-started/license-automation-vs-integration.md).

-->

## Criar um cenário de prática

### Começar a criar o cenário

1. No **Cenários** clique em **Criar um novo cenário**.

   <!--To locate the Scenarios area, see navigation article-->

   O editor de cenários é exibido, contendo um módulo vazio no centro.

   <!--picture?-->

1. Selecione o **[!UICONTROL Novo cenário]** nome do espaço reservado no canto superior esquerdo e digite um nome.
1. Continuar com [Adicionar e configurar o primeiro módulo](#add-and-configure-the-first-module) abaixo.

### Adicionar e configurar o primeiro módulo

1. Clique no módulo vazio para escolher o aplicativo do qual você selecionará um módulo.

   Uma lista de aplicativos é exibida à direita do módulo.

1. Selecionar **[!DNL Adobe Workfront]**. Se não estiver visível, clique na barra de pesquisa na parte inferior da lista, digite &quot;Workfront&quot; e selecione-a quando ela aparecer na lista.

   A lista muda para exibir tudo [!DNL Workfront] módulos que você pode usar.

1. Clique em **[!UICONTROL Pesquisar]** módulo.

   A janela de configuração do módulo é aberta.

1. No [!UICONTROL Conexão] selecione a conexão Workfront.

   Se você não tiver uma conexão Workfront, consulte [Criar uma conexão com o [!DNL Adobe Workfront Fusion]](/help/quicksilver/workfront-fusion/connections/connect-to-fusion-general.md)
1. No [!UICONTROL Tipo de registro] , selecione **[!UICONTROL Tarefa]**. Isso define o módulo para pesquisar somente tarefas.

   Você pode encontrar **[!UICONTROL Tarefa]** na lista se você começar a digitar a palavra &quot;[!UICONTROL tarefa].&quot;

1. No **[!UICONTROL Conjunto de resultados]** , selecione **[!UICONTROL Primeiro registro correspondente]**.

   Isso define o módulo para retornar somente o primeiro registro encontrado que atenda aos critérios.
1. No **[!UICONTROL Critérios de pesquisa]** configure os critérios para retornar a tarefa específica.

   1. Na primeira caixa, em [!UICONTROL Critérios de pesquisa], selecione o campo que deseja incluir na pesquisa. Para este exemplo, selecione **[!UICONTROL Nome]**.

      Você pode encontrar **[!UICONTROL Nome]** na lista se você começar a digitar a palavra &quot;[!UICONTROL name].&quot;
   1. Para o operador, clique na seta suspensa ao lado de **Existe** e altere para [!UICONTROL **Contém (não diferencia maiúsculas de minúsculas)**].

      Isso permite que o módulo encontre projetos com as palavras escolhidas em seu nome, mesmo se você não inserir o nome inteiro ou inserir o nome com a caixa incorreta (como todas em maiúsculas).
   1. No último campo em [!UICONTROL Critérios de pesquisa], digite uma palavra ou frase que você sabe que está no nome da tarefa que está procurando.

1. No **[!UICONTROL Saídas]** selecione os campos que deseja que o módulo exporte. Para este exemplo, selecione a variável **[!UICONTROL ID]** e **[!UICONTROL Nome]** campos.

   >[!TIP]
   >
   >Você pode usar **Cmd+F** ([!DNL Mac] OS) ou **Ctrl-F** ([!DNL Windows] OS) para localizar um campo rapidamente.

1. Clique em **[!UICONTROL OK]** para salvar a configuração do módulo.

1. Clique com o botão direito do mouse no módulo e clique em **[!UICONTROL Renomear]**, em seguida, digite um nome que descreva o que você deseja que o módulo faça (como &quot;Procurar tarefa&quot;) e, em seguida, clique em **[!UICONTROL OK]**.

   O nome aparece logo abaixo do módulo. Abaixo disso, [!DNL Workfront Fusion] O inclui uma breve descrição do tipo de ação executada pelo módulo.

   ![](assets/module-renamed-wf.png)

1. Continuar com [Adicionar e configurar o segundo módulo](#add-and-configure-the-second-module).

## Adicionar e configurar o segundo módulo

1. Passe o mouse sobre o círculo parcial à direita do do módulo e clique em **[!UICONTROL Adicionar outro módulo]**.
1. Selecionar [!DNL Adobe Workfront] na lista de aplicativos, escolha o módulo **[!UICONTROL Converter objeto]**.
1. No [!UICONTROL Conexão] , selecione a mesma conexão Workfront usada no módulo anterior.
1. No **[!UICONTROL Tipo de registro]** selecione **[!UICONTROL Tarefa]**, pois o módulo converterá uma tarefa.
1. No **[!UICONTROL Converter para]** selecione **Projeto**.
1. Ao lado do campo ID de tarefa, clique no botão de alternância do mapa para ativá-lo.

   O botão fica azul quando é ativado. Isso permite mapear a ID da tarefa do módulo anterior.

   ![Alternância do mapa](assets/map-toggle.png)
1. Clique em **[!UICONTROL ID da tarefa]** campo.

   É aberto um painel que permite selecionar o que será usado como a ID da tarefa que você deseja converter em um projeto. Como você ativou o mapeamento, o painel inclui a saída de qualquer módulo anterior. Você selecionou ID como uma saída do módulo anterior, de modo que ele agora está disponível no painel.

   Esse painel é chamado de painel de mapeamento. Para obter mais informações sobre o painel de mapeamento, consulte [Mapear informações de um módulo para outro](/help/quicksilver/workfront-fusion/mapping/map-information-between-modules.md).
1. Selecionar **ID** no painel de mapeamento.

   Um bloco ID é exibido no campo ID. Ela mostra o número do módulo do qual é mapeado e o campo que é mapeado.

   ![ID do mapa](assets/map-id.png)

1. Clique em **ID do modelo** comece digitando o nome do modelo Workfront que deseja usar para este projeto e, em seguida, selecione-o quando ele aparecer na lista.
1. Clique em **[!UICONTROL OK]** para salvar a configuração do módulo.

1. Clique com o botão direito do mouse no módulo e clique em **[!UICONTROL Renomear]**, digite um nome que descreva o que você deseja que o módulo faça (como &quot;Converter em projeto&quot;) e clique em **[!UICONTROL OK]**.

1. Continue para [Testar o cenário](#test-the-scenario).

## Testar o cenário

Antes de ativar o cenário, é importante testá-lo executando-o pelo menos uma vez e visualizando os resultados. Isso ajuda você a entender como os dados fluem pelo cenário e encontrar erros.

Para este cenário, um teste bem-sucedido resultaria na localização da nova tarefa e sua conversão em um projeto.

1. Clique em **[!UICONTROL Executar uma vez]** no canto inferior esquerdo do editor de cenários.
1. Depois que o cenário terminar de ser executado, clique no balão acima do primeiro módulo para exibir informações sobre o pacote de dados que o módulo processou, incluindo dados obtidos da tarefa que o módulo retornou.

1. Clique na bolha do inspetor de execução acima do segundo módulo para ver a entrada (a tarefa) e a saída (o projeto convertido).

   Para obter mais informações sobre os dados nas bolhas de inspeção, consulte:

   * Para obter informações gerais, consulte [Fluxo de execução de cenário em [!DNL Adobe Workfront Fusion]](/help/quicksilver/workfront-fusion/scenarios/scenario-execution-flow.md).
   * Para obter informações sobre pacotes processados, consulte [Execução de cenário, ciclos e fases em [!DNL Adobe Workfront Fusion]](/help/quicksilver/workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

1. Entrada [!DNL Workfront Fusion], clique em **[!UICONTROL Salvar]** próximo ao canto inferior esquerdo para salvar seu progresso no cenário.

   >[!IMPORTANT]
   >
   >Salve com frequência à medida que você aprimora e testa um cenário.

>[!TIP]
>
>Recomendamos a prática opcional, mas útil, de adicionar observações sobre cada módulo.
>
>1. Clique com o botão direito do mouse em uma [!DNL Workfront] e clique em **[!UICONTROL Adicionar uma observação]**.
>1. Na nota exibida, digite uma visão geral do módulo.
>
>    Você pode adicionar várias notas para um módulo.
>
>1. Feche o **[!UICONTROL Notas]** área.
>
>     Depois de adicionar uma nota a um cenário, um ponto laranja é exibido no **[!UICONTROL Notas]** ícone ![](assets/notes-icon-w-dot.png) na parte inferior do editor de cenários.
>
>1. Clique em **[!UICONTROL Notas]** ícone ![](assets/notes-icon-w-dot.png) para exibir suas notas.
>

## Ativar o cenário

A última etapa na criação de um cenário é ativá-lo.

Como esse cenário está procurando uma tarefa específica, não há necessidade de ativá-la. Ativar um cenário faz com que ele seja executado de acordo com um agendamento ou quando uma ação específica ocorre em um aplicativo. Após ativar um cenário, por padrão, ele é executado a cada 15 minutos. Você pode alterar isso definindo quando e com que frequência deseja que ele seja executado.

Para obter mais informações sobre a ativação de cenários, consulte [Ativar ou desativar um cenário no [!UICONTROL Adobe Workfront Fusion]](/help/quicksilver/workfront-fusion/scenarios/activate-or-inactivate-scenario.md).

Para obter informações sobre programações, consulte [Agendar um cenário no [!UICONTROL Adobe Workfront Fusion]](/help/quicksilver/workfront-fusion/scenarios/schedule-a-scenario.md).

## Próximas etapas

* [Adicionar um módulo de acionamento](/help/quicksilver/workfront-fusion/get-started/build-practice-scenarios/add-trigger-to-simple-scenario.md) para permitir que o cenário procure novas solicitações periodicamente e as converta em projetos.
* Adicione um webhook para permitir que o cenário seja executado sempre que uma solicitação for inserida.
* Adicione um filtro para garantir que somente determinadas solicitações sejam convertidas em projetos.
* Adicione uma função que personalize o nome do novo projeto.
* Adicione o tratamento de erros para garantir que o cenário seja resiliente contra erros.

