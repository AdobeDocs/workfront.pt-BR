---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: O editor de cenários no [!DNL Adobe] Workfront Fusion
description: O editor de cenários permite criar e editar cenários em uma interface visual.
author: Becky
feature: Workfront Fusion
exl-id: 4377303d-7615-41eb-b0cc-4bf884899361
source-git-commit: 28ca9bab8d6a5aed395dc3297eb62912ebb506c7
workflow-type: tm+mt
source-wordcount: '867'
ht-degree: 0%

---

# O editor de cenários no [!DNL Adobe Workfront Fusion]

O editor de cenários permite criar e editar cenários em uma interface visual.

![](assets/scenario-editor-350x228.jpg)

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
   <p>Requisito de licença herdada: [!UICONTROL [!DNL Workfront Fusion] para Automação e integração do trabalho] </p>
   </td> 
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

## Abra o editor de cenários:

1. Clique em **[!UICONTROL Cenários]** ![](assets/scenarios-icon.png) no painel esquerdo.

1. Para criar um cenário, clique em **[!UICONTROL Criar um novo cenário]** no canto superior direito da página.

   Ou

   Se quiser editar um cenário existente, clique nele.

   No editor de cenários exibido, é possível executar todas as ações listadas na tabela abaixo. Para obter mais informações, consulte [Criar um cenário no [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

1. Quando terminar de editar um cenário (ou a qualquer momento enquanto estiver editando), clique no link [!UICONTROL Salvar] ícone. ![](assets/save-icon.gif)

   >[!NOTE]
   >
   >Depois de salvar o cenário, uma nova versão estará disponível no menu de três pontos, caso você precise acessá-lo no futuro. As versões de cenários salvas anteriormente só estão disponíveis por 60 dias.

## Ações disponíveis do editor de cenário

As seguintes ações estão disponíveis no Editor de cenários:

<table style="table-layout:auto"> 
<tbody>
  <tr>
     <td role="rowheader">Adicionar o primeiro módulo</td>
     <td> <p>Clique no ícone de ponto de interrogação. <img src="assets/question-mark-full-size.png"></p> <p> Em seguida, localize e clique no aplicativo ou serviço com o qual deseja começar. Se você selecionou algum aplicativo na etapa 2, ele aparecerá aqui para fácil acesso (e no <strong>[!UICONTROL Favoritos]</strong> na parte inferior da tela).</p> </td>
  </tr>
  <tr>
     <td role="rowheader">Adicionar um módulo</td>
     <td>Passe o mouse sobre um módulo, clique no ícone de adição exibido à direita e, em seguida, clique no módulo desejado no menu exibido.</td>
  </tr>  
  <tr>   
     <td role="rowheader">Especificar quando e com que frequência o cenário será executado</td>  
      <td> <p>Clique no ícone do relógio. </p> <p> <img src="assets/clock-icon.gif"> </p> <p>Para obter mais informações, consulte <a href="../../workfront-fusion/scenarios/schedule-a-scenario.md" class="MCXref xref">Agendar um cenário no [!DNL Adobe Workfront Fusion]</a>.</p> </td>
  </tr>  
  <tr>
     <td role="rowheader">Configurar um roteiro</td>   
     <td> <p>Clique no ícone da chave inglesa [!UICONTROL] <img src="assets/wrench-icon.gif"> entre os dois módulos e use uma das seguintes opções:</p>    
       <ul>
         <li><strong>[!UICONTROL Configurar um filtro]</strong>: controle quais pacotes são usados em determinados pontos do cenário. Para obter mais informações, consulte <a href="../../workfront-fusion/scenarios/add-a-filter-to-a-scenario.md" class="MCXref xref">Adicionar um filtro a um cenário no [!DNL Adobe Workfront Fusion]</a>.</li>     
         <li><strong>[!UICONTROL Desvincular]</strong>: remove uma rota.</li>     
         <li><strong>[!UICONTROL Adicionar um roteador]</strong>: adiciona um roteador entre módulos. </li>     
         <li><strong>[!UICONTROL Adicionar um módulo]</strong>: adiciona um novo módulo entre módulos.</li>     
         <li><strong>[!UICONTROL Adicionar uma observação]</strong>: adiciona uma observação à rota.</li>   
       </ul> 
     </td>  
  </tr>  
  <tr>  
     <td role="rowheader">Remover um módulo</td>   
     <td>Clique com o botão direito do mouse no módulo e clique em <strong>[!UICONTROL Excluir módulo]</strong>.</td>  
   </tr>  
   <tr> 
     <td role="rowheader">Exibir um log de eventos que ocorre em um cenário</td>     
     <td> 
       <p>Execute um cenário. Quando o cenário terminar de ser executado, o log aparecerá no canto inferior direito do [!UICONTROL Editor de Cenário]. </p> <p> <img src="assets/log-350x189.png" style="width: 350;height: 189;"> </p> <p>Dependendo do cenário, o log pode conter informações sobre a dificuldade de cada fase e os erros encontrados durante a execução do cenário.</p> 
     </td>  
   </tr>  
   <tr>   
     <td role="rowheader">Definir as configurações do cenário</td>   
     <td>Clique no ícone [!UICONTROL Configurações de cenário]. <img src="assets/gear-icon-settings.png"> Essas configurações são destinadas principalmente a usuários avançados.</td>  
   </tr>  
   <tr>   
     <td role="rowheader">Digite ou exiba observações sobre o cenário</td>   
     <td>Clique no ícone [!UICONTROL Notes]. <img src="assets/notes-icon.gif"></td>  
   </tr>  
   <tr> 
     <td role="rowheader">Alinhar automaticamente o layout dos módulos </td>   
     <td>Clique no ícone [!UICONTROL Alinhamento automático]. <img src="assets/auto-align-icon.gif"></td>  </tr>  <tr>   <td role="rowheader">Exibir uma animação que mostra como os dados fluem pelo cenário</td>   <td>Clique no ícone [!UICONTROL Explicar Fluxo]. <img src="assets/explain-flow-airplane-icon.gif"></td>  
   </tr>  
   <tr> 
     <td role="rowheader">Exportar o cenário para seu computador como um blueprint</td>   
     <td>Clique no menu [!UICONTROL Mais] <img src="assets/more-icon.png">e clique em [!UICONTROL Exportar blueprint].</td>  
   </tr>  
   <tr>   
     <td role="rowheader">Importar um blueprint de cenário do seu computador</td>   
     <td>Clique no menu [!UICONTROL Mais] <img src="assets/more-icon.png">, em seguida, clique em [!UICONTROL Importar Blueprint].</td>  
   </tr>  
   <tr>   
     <td role="rowheader">Restaurar uma versão anterior do cenário</td>   
     <td>Consulte o artigo <a href="../../workfront-fusion/scenarios/restore-a-scenario-version.md" class="MCXref xref">Restaurar uma versão do cenário no [!DNL Adobe Workfront Fusion]</a>.</td>  
   </tr>  
   <tr> 
     <td role="rowheader">Definir configurações de [!UICONTROL Controle de Fluxo]</td>   
     <td> <p>Clique no ícone [!UICONTROL Controle de Fluxo]. <img src="assets/flow-control-icon.gif"> Você pode configurar uma tarefa para repetir um determinado número de vezes, converter uma matriz em uma série de pacotes e mesclar vários pacotes em um único pacote. Para obter mais informações, consulte <a href="../../workfront-fusion/apps-and-their-modules/flow-control.md" class="MCXref xref">Controle de fluxo em [!DNL Adobe Workfront Fusion]</a>.</p> </td>  
   </tr>  
   <tr> 
     <td role="rowheader">Aprimorar o cenário usando ferramentas avançadas</td>   
     <td>Clique no ícone [!UICONTROL Ferramentas]. <img src="assets/tools-icon.gif"> Você pode criar acionadores, ações, agregadores e transformadores. Para obter mais informações, consulte <a href="../../workfront-fusion/apps-and-their-modules/tools-modules.md" class="MCXref xref">Ferramentas</a>.</td>  
   </tr>  
   <tr> 
     <td role="rowheader">Usar ferramentas de análise de texto</td>   
     <td>Clique no ícone [!UICONTROL Analisador de texto]. <img src="assets/text-parser-icon.gif"> Você pode recuperar elementos do código HTML, localizar e extrair elementos de string que correspondam a um padrão de pesquisa, pesquisar e substituir texto e "extrair" dados de um site. Para obter mais informações, consulte <a href="../../workfront-fusion/apps-and-their-modules/tools-modules.md" class="MCXref xref">Ferramentas</a>.</td>  
   </tr>  
   <tr> 
     <td role="rowheader">Acesse os aplicativos e serviços mais usados</td>   
     <td> Clique em um ícone na <strong>[!UICONTROL Favoritos]</strong> na parte inferior da tela. Os ícones são exibidos nesta seção automaticamente à medida que você adiciona aplicativos e serviços ao seu cenário. Também é possível clicar no ícone Add <img src="assets/add-icon.gif"> para adicionar aplicativos e serviços a esta área manualmente.</td>  
   </tr>  
   <tr> 
     <td role="rowheader">Testar o cenário</td>   
     <td>Clique em <strong>[!UICONTROL Executar uma vez]</strong> para verificar se o cenário é executado como esperado antes de ativá-lo. Uma vez ativado, o cenário será executado de acordo com seu cronograma. Se tudo não for executado conforme o esperado, visite nossa seção de tratamento de erros para saber como lidar com erros.</td> 
   </tr> 
   <tr> 
     <td role="rowheader">Use Devtool para depurar o cenário</td>   
     <td>Para obter mais informações, consulte <a href="../../workfront-fusion/scenarios/debug-scenarios-with-dev-tool.md" class="MCXref xref">Depurar cenários com o [!DNL Adobe Workfront Fusion] Devtool</a>.
</td> 
   </tr> 
</tbody>
</table>
