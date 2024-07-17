---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Criar um cenário no Adobe Workfront Fusion
description: As tarefas a seguir explicam como criar um cenário  [!DNL Adobe Workfront Fusion] .
author: Becky
feature: Workfront Fusion
exl-id: adf66cfc-ccaf-4b29-9199-c13260695569
source-git-commit: ee2283ac159ca26ca473cac28ec4bed85d1dea04
workflow-type: tm+mt
source-wordcount: '1406'
ht-degree: 0%

---

# Criar um cenário em [!DNL Adobe Workfront Fusion]

As tarefas a seguir explicam como criar um cenário [!DNL Adobe Workfront Fusion].

Para um exercício de prática que orienta você na criação de um cenário de automação, consulte [Criar um cenário de automação de prática [!DNL Adobe Workfront Fusion]](../../workfront-fusion/get-started/create-a-practice-automation-scenario.md).

Para um exercício de prática que orienta você na criação de um cenário de integração usando os dados que fornecemos, consulte [Criar um cenário de integração de prática no Adobe Workfront Fusion](../../workfront-fusion/get-started/create-a-practice-scenario.md).

>[!NOTE]
>
>Para criar um cenário a partir de um modelo, consulte [Criar cenários com [!DNL Adobe Workfront Fusion] modelos](../../workfront-fusion/scenarios/templates/create-scenarios-with-fusion-templates.md).

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
        Novo: plano Select ou Prime do Workfront: sua organização deve comprar o Adobe Workfront Fusion.<br>
        Plano Ultimate do Workfront: o Workfront Fusion está incluído.<br>
        Ou<br>
        Atual: sua organização deve comprar o Adobe Workfront Fusion.
      </td>  
    </tr> 
  </tbody>  
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

Para obter informações sobre [!DNL Adobe Workfront Fusion] licenças, consulte [[!DNL Adobe Workfront Fusion] licenças](../../workfront-fusion/get-started/license-automation-vs-integration.md).

+++

## Começar a criar um cenário

1. Clique em **[!UICONTROL Cenários]** ![](assets/scenarios-icon.png) no painel esquerdo.

1. Clique em **[!UICONTROL Criar um novo cenário]** no canto superior direito da página.
1. Na tela exibida (o editor de cenários), se você estiver criando um novo cenário, clique em **[!UICONTROL Novo cenário]** no canto superior esquerdo e digite um nome para o cenário.
1. Continue em [Adicionar um módulo em um cenário](#add-a-module-in-a-scenario).

## Adicionar um módulo em um cenário

1. Para adicionar o primeiro módulo ao cenário, clique no ícone de ponto de interrogação. ![](assets/question-mark-icon.gif)

   Ou

   Para adicionar mais módulos ao cenário, clique na alça no lado direito do módulo que você deseja que ele siga.

1. Na caixa exibida, localize e clique no aplicativo ou serviço com o qual deseja começar.

   Todos os aplicativos selecionados anteriormente são exibidos na caixa para facilitar o acesso e na seção **[!UICONTROL Favoritos]**, na parte inferior da tela.

   Se você clicar em **[!UICONTROL Adicionar outro módulo]**, os módulos exibidos dependerão de onde, no cenário, você está adicionando o módulo. Alguns módulos podem ser colocados somente entre outros módulos e outros somente no início do cenário.

   >[!TIP]
   >
   >Os dois tipos mais comuns de módulos são ações e acionadores. Para obter mais informações, consulte [Tipos de módulos](../../workfront-fusion/modules/module-types.md).

1. Na lista de módulos que é exibida, clique no primeiro módulo que deseja adicionar ao cenário.

   Os módulos exibidos dependem de onde você deseja adicionar um módulo em seu cenário. Alguns módulos podem ser colocados somente entre outros módulos e outros somente no início do cenário.

   Os dois tipos mais comuns de módulos são ações e acionadores. Para obter mais informações, consulte [Tipos de módulos](../../workfront-fusion/modules/module-types.md).

1. Continue em [Conectar o aplicativo ou serviço Web do módulo a [!DNL Workfront Fusion]](#connect-the-modules-app-or-web-service-to-workfront-fusion).

## Conectar o aplicativo ou serviço Web do módulo a [!DNL Workfront Fusion] {#connect-the-modules-app-or-web-service-to-workfront-fusion}

Os módulos do Workfront Fusion que se conectam a um aplicativo (como [!DNL Workfront], [!DNL Salesforce] ou [!DNL Jira)]) apresentam o campo [!UICONTROL Conexão]. Aqui, você pode especificar a conexão que deseja que esse módulo use para se conectar ao aplicativo. Você pode selecionar uma conexão existente na lista suspensa ou criar uma nova conexão.

Quando você seleciona ou cria uma conexão para um aplicativo em um cenário, outros módulos para esse aplicativo usam automaticamente a mesma conexão, a menos que você selecione um diferente ao configurar os módulos posteriores.

Para obter mais informações, consulte [Visão geral das conexões](../../workfront-fusion/connections/about-connecting-wf-fusion-to-app-or-service.md).

![](assets/connection-field-350x169.png)

Para criar uma conexão dentro de um módulo [!DNL Workfront Fusion]:

1. Clique em **[!UICONTROL Adicionar]** para abrir a caixa **[!UICONTROL Criar uma conexão]**.
1. (Opcional) Altere o **[!UICONTROL Nome da conexão]** padrão.
1. (Condicional) Se o aplicativo exigir configurações de conexão avançadas, como ID, chave ou [!UICONTROL segredo], insira essas informações.

   Talvez seja necessário clicar em **[!UICONTROL Mostrar configurações avançadas]** para exibir os campos nos quais você pode inserir esse tipo de informação.

1. Clique em **[!UICONTROL Continuar]**.
1. Na janela de logon que é exibida, digite suas credenciais para fazer logon no aplicativo, se ainda não tiver feito.
1. (Condicional) Se um botão **[!UICONTROL Permitir]** for exibido, examine as ações que o conector poderá realizar e clique no botão para conectar o aplicativo ao [!DNL Workfront Fusion].
1. Continue em [Configurar o módulo](#configure-the-module).


## Configurar o módulo

1. Nos campos abaixo do campo Conexão, defina as configurações do módulo e clique em **[!UICONTROL OK]**.

   ![](assets/conf-settigs-mod-350x547.png)

   Essas configurações são diferentes para cada módulo. Um título em negrito indica uma configuração necessária.

   >[!TIP]
   >
   >Conforme você trabalha no cenário, pode clicar no módulo para exibir essa caixa de configurações a qualquer momento.
   >
   >
   >Se você vir um círculo preto em um módulo, você ainda não terminou de definir suas configurações. Clique no módulo para abri-lo e continuar a configuração.
   >
   >
   >![](assets/black-error-circle-on-module.png)

1. Se estiver adicionando o primeiro módulo do em um cenário, selecione uma opção para indicar onde deseja que o cenário comece sempre que for executado.

   ![](assets/choose-where-start-350x194.png)

1. Repita as etapas nas seções [Adicionar um módulo em um cenário](#add-a-module-in-a-scenario) e [Configurar o módulo](#configure-the-module) para adicionar outros módulos ao cenário.

1. (Opcional) Copie e cole um módulo ou grupo de módulos.

   Para obter mais informações, consulte [Copiar módulos ou cenários no Adobe Workfront Fusion](../../workfront-fusion/scenarios/copy-modules-or-scenarios.md).

1. Continue para [Configurar e trabalhar com seu cenário](#configure-and-work-with-your-scenario).

## Configurar e trabalhar com seu cenário

1. Siga qualquer um destes procedimentos para configurar seu cenário:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Especificar quando e com que frequência o cenário será executado</td> 
      <td> <p>Clique no ícone do relógio. </p> <p> <img src="assets/clock-icon.gif"> </p> <p>Para obter mais informações, consulte <a href="../../workfront-fusion/scenarios/schedule-a-scenario.md" class="MCXref xref">Agendar um cenário em [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Configurar um roteiro</td> 
      <td> <p>Clique na chave inglesa <img src="assets/wrench-icon.gif"> entre os dois módulos e use uma das opções a seguir. Para obter mais informações, consulte <a href="../../workfront-fusion/scenarios/add-a-filter-to-a-scenario.md" class="MCXref xref">Adicionar um filtro a um cenário em [!DNL Adobe Workfront Fusion]</a>.</p> 
       <ul> 
        <li><strong>[!UICONTROL Configurar um filtro]</strong>: controla quais conjuntos são usados em determinados pontos do cenário.</li> 
        <li><strong>[!UICONTROL Desvincular]</strong>: Remove uma rota.</li> 
        <li><strong>[!UICONTROL Adicionar um roteador]</strong>: Adiciona um roteador entre módulos. </li> 
        <li><strong>[!UICONTROL Adicionar um módulo]</strong>: Adiciona um novo módulo entre módulos.</li> 
        <li><strong>[!UICONTROL Adicionar uma observação]</strong>: adiciona uma observação à rota.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Definir as configurações do cenário</td> 
      <td>Clique no ícone [!UICONTROL Configurações de cenário]. <img src="assets/gear-icon-settings.png"> Estas configurações destinam-se principalmente a usuários avançados. Para obter mais informações, consulte <a href="../../workfront-fusion/scenarios/scenario-settings-panel.md" class="MCXref xref">O painel de configurações do cenário em [!DNL Adobe Workfront Fusion]</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Definir configurações de Controle de Fluxo</td> 
      <td> <p>Clique no ícone [!UICONTROL Controle de Fluxo]. <img src="assets/flow-control-icon.gif"> Você pode configurar uma tarefa para repetir um determinado número de vezes, converter uma matriz em uma série de pacotes e mesclar vários pacotes em um único pacote. Para obter mais informações, consulte <a href="../../workfront-fusion/apps-and-their-modules/flow-control.md" class="MCXref xref">Controle de fluxo em [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Aprimorar o cenário usando ferramentas avançadas</td> 
      <td>Clique no ícone [!DNL Tools]. <img src="assets/tools-icon.gif"> Você pode criar acionadores, ações, agregadores e transformadores. Para obter mais informações, consulte <a href="../../workfront-fusion/apps-and-their-modules/tools-modules.md" class="MCXref xref">Ferramentas</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ferramentas de análise de texto do usuário</td> 
      <td>Clique no ícone [!DNL Text parser] <img src="assets/text-parser-icon.gif">. Você pode recuperar elementos do código HTML, localizar e extrair elementos de string que correspondam a um padrão de pesquisa, pesquisar e substituir texto e "extrair" dados de um site. Para obter mais informações, consulte <a href="../../workfront-fusion/apps-and-their-modules/tools-modules.md" class="MCXref xref">Ferramentas</a>.</td> 
     </tr> 
    </tbody> 
   </table>

1. Siga qualquer um destes procedimentos para trabalhar com seu cenário:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Exibir um log dos eventos que ocorrem quando o cenário é executado</td> 
      <td> <p>Clique na seta [!UICONTROL Sair editando] <img src="assets/exit-editing-arrow.png"> no editor de cenários para exibir a página Detalhes do cenário. O registro é exibido na parte inferior da janela ou no canto inferior direito. Ele contém informações sobre cada fase e os erros encontrados durante a execução do cenário.</p> <p>Para voltar a trabalhar com seu cenário no [!DNL scenario editor], clique em qualquer lugar na página Detalhes do cenário.</p> <p>Para obter mais informações sobre a página de detalhes do cenário, consulte <a href="../../workfront-fusion/scenarios/scenario-detail.md" class="MCXref xref">Detalhes do cenário em [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Acesse os aplicativos e serviços mais usados</td> 
      <td> Clique em um ícone na seção <strong>[!UICONTROL Favoritos]</strong>, na parte inferior da tela. Os ícones são exibidos nesta seção automaticamente à medida que você adiciona aplicativos e serviços ao seu cenário. Você também pode clicar no ícone [!UICONTROL Adicionar] <img src="assets/add-icon.gif"> para adicionar aplicativos e serviços a esta área manualmente.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Exibir uma animação que mostra como os dados fluem pelo cenário</td> 
      <td>Clique no ícone [!UICONTROL Explicar fluxo] <img src="assets/explain-flow-airplane-icon.gif">.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Alinhar automaticamente o layout dos módulos </td> 
      <td>Clique no ícone [!UICONTROL Alinhamento Automático] <img src="assets/auto-align-icon.gif">.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Digite ou exiba observações sobre o cenário</td> 
      <td>Clique no ícone [!UICONTROL Notes] <img src="assets/notes-icon.gif">.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Remover um módulo</td> 
      <td>Clique com o botão direito do mouse no módulo e clique em <strong>[!UICONTROL Excluir módulo]</strong>.</td> 
     </tr> 
    </tbody> 
   </table>

1. Para testar o cenário, clique em **[!UICONTROL Executar uma vez]**.

   É importante verificar se o cenário é executado como esperado antes de ativá-lo. Uma vez ativado, o cenário será executado de acordo com seu cronograma. Se tudo não funcionar conforme o esperado, consulte [Tratamento de erros [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-handling.md).

1. Ao terminar de editar o cenário (ou a qualquer momento enquanto estiver editando), clique no ícone [!UICONTROL Salvar] na parte inferior da janela ![](assets/save-icon.gif).

Para obter informações sobre como ativar um cenário, consulte [Ativar ou desativar um cenário [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/activate-or-inactivate-scenario.md).

## Atalhos de teclado do cenário do Workfront Fusion

Você pode usar os seguintes atalhos de teclado ao criar ou editar um cenário:

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <thead> 
  <tr> 
   <th> <p>Ação</p> </th> 
   <th>[!DNL Windows]</th> 
   <th> <p>[!DNL MacOS]</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Salvar] </td> 
   <td>Ctrl+Shift+S</td> 
   <td><span style="font-weight: normal;">Cmd+Shift+S</span> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Executar Uma Vez]</td> 
   <td>Ctrl+Shift+Enter</td> 
   <td><span style="font-weight: normal;">Cmd+Shift+Enter</span> </td> 
  </tr> 
 </tbody> 
</table>
