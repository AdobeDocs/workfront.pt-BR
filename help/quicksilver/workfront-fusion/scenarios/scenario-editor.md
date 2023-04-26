---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: O editor de cenário em [!DNL Adobe] Workfront Fusion
description: O editor de cenários permite criar e editar cenários em uma interface visual.
author: Becky
feature: Workfront Fusion
exl-id: 4377303d-7615-41eb-b0cc-4bf884899361
source-git-commit: c19e8c104ac1e93d67300637437d32b6f8534e99
workflow-type: tm+mt
source-wordcount: '804'
ht-degree: 0%

---

# O editor de cenário em [!DNL Adobe Workfront Fusion]

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

## Abra o editor de cenário:

1. Clique em **[!UICONTROL Cenários]** ![](assets/scenarios-icon.png) no painel esquerdo.

1. Se quiser criar um cenário, clique em **[!UICONTROL Criar um novo cenário]** no canto superior direito da página.

   Ou

   Para editar um cenário existente, clique no cenário.

   No editor de cenário exibido, é possível fazer tudo o que está listado na tabela abaixo. Para obter mais informações, consulte [Crie um cenário em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

1. Ao terminar de editar um cenário (ou a qualquer momento durante a edição), clique no link [!UICONTROL Salvar] ícone . ![](assets/save-icon.gif)

   >[!NOTE]
   >
   >Depois de salvar o cenário, uma nova versão estará disponível no menu de três pontos, caso você precise acessá-la no futuro. As versões de cenário salvas anteriormente só estão disponíveis por 60 dias.

## Ações disponíveis do editor de cenário

As seguintes ações estão disponíveis no Editor de cenário:

<table style="table-layout:auto"> 
<tbody>
  <tr>
     <td role="rowheader">Adicionar o primeiro módulo</td>
     <td> <p>Clique no ícone de ponto de interrogação. <img src="assets/question-mark-full-size.png"></p> <p> Em seguida, localize e clique no aplicativo ou serviço com o qual deseja começar. Se você selecionou aplicativos na etapa 2, eles são exibidos aqui para fácil acesso (e no <strong>[!UICONTROL Favoritos]</strong> na parte inferior da tela).</p> </td>
  </tr>
  <tr>
     <td role="rowheader">Adicionar um módulo</td>
     <td>Passe o mouse sobre um módulo, clique no ícone de adição exibido à direita e clique no módulo desejado no menu exibido.</td>
  </tr>  
  <tr>   
     <td role="rowheader">Especifique quando e com que frequência o cenário será executado</td>  
      <td> <p>Clique no ícone do relógio. </p> <p> <img src="assets/clock-icon.gif"> </p> <p>Para obter mais informações, consulte <a href="../../workfront-fusion/scenarios/schedule-a-scenario.md" class="MCXref xref">Programe um cenário em [!DNL Adobe Workfront Fusion]</a>.</p> </td>
  </tr>  
  <tr>
     <td role="rowheader">Configurar uma rota</td>   
     <td> <p>Clique no ícone [!UICONTROL chave] <img src="assets/wrench-icon.gif"> entre os dois módulos e use qualquer uma das seguintes opções:</p>    
       <ul>
         <li><strong>[!UICONTROL Configurar um filtro]</strong>: Controlar quais pacotes são usados em determinados pontos do cenário. Para obter mais informações, consulte <a href="../../workfront-fusion/scenarios/add-a-filter-to-a-scenario.md" class="MCXref xref">Adicione um filtro a um cenário em [!DNL Adobe Workfront Fusion]</a>.</li>     
         <li><strong>[!UICONTROL Desvincular]</strong>: Remove uma rota.</li>     
         <li><strong>[!UICONTROL Adicionar um roteador]</strong>: Adiciona um roteador entre módulos. </li>     
         <li><strong>[!UICONTROL Adicionar um módulo]</strong>: Adiciona um novo módulo entre módulos.</li>     
         <li><strong>[!UICONTROL Adicionar uma observação]</strong>: Adiciona uma nota à rota.</li>   
       </ul> 
     </td>  
  </tr>  
  <tr>  
     <td role="rowheader">Remover um módulo</td>   
     <td>Clique com o botão direito do mouse no módulo e depois clique em <strong>[!UICONTROL Excluir módulo]</strong>.</td>  
   </tr>  
   <tr> 
     <td role="rowheader">Exibir um log de eventos que ocorre em um cenário</td>     
     <td> 
       <p>Execute um cenário. Quando o cenário terminar de ser executado, o log será exibido no canto inferior direito do [!UICONTROL Scenario Editor]. </p> <p> <img src="assets/log-350x189.png" style="width: 350;height: 189;"> </p> <p>Dependendo do cenário, o log pode conter informações sobre a dificuldade de cada fase e quaisquer erros encontrados durante a execução do cenário.</p> 
     </td>  
   </tr>  
   <tr>   
     <td role="rowheader">Definir as configurações de cenário</td>   
     <td>Clique no ícone [!UICONTROL Configurações do cenário] . <img src="assets/gear-icon-settings.png"> Essas configurações destinam-se principalmente a usuários avançados.</td>  
   </tr>  
   <tr>   
     <td role="rowheader">Digite ou exiba observações sobre o cenário</td>   
     <td>Clique no ícone [!UICONTROL Notas]. <img src="assets/notes-icon.gif"></td>  
   </tr>  
   <tr> 
     <td role="rowheader">Alinhar automaticamente o layout dos módulos </td>   
     <td>Clique no ícone [!UICONTROL Autoalinhamento]. <img src="assets/auto-align-icon.gif"></td>  </tr>  <tr>   <td role="rowheader">Exibir uma animação que mostra como os dados fluem pelo cenário</td>   <td>Clique no ícone [!UICONTROL Explicar Fluxo]. <img src="assets/explain-flow-airplane-icon.gif"></td>  
   </tr>  
   <tr> 
     <td role="rowheader">Exporte o cenário para o seu computador como um blueprint</td>   
     <td>Clique no menu [!UICONTROL Mais] <img src="assets/more-icon.png">e clique em [!UICONTROL Exportar blueprint].</td>  
   </tr>  
   <tr>   
     <td role="rowheader">Importe um blueprint de cenário do seu computador</td>   
     <td>Clique no menu [!UICONTROL Mais] <img src="assets/more-icon.png">e clique em [!UICONTROL Importar blueprint].</td>  
   </tr>  
   <tr>   
     <td role="rowheader">Restaurar uma versão anterior do cenário</td>   
     <td>Veja o artigo <a href="../../workfront-fusion/scenarios/restore-a-scenario-version.md" class="MCXref xref">Restaure uma versão de cenário em [!DNL Adobe Workfront Fusion]</a>.</td>  
   </tr>  
   <tr> 
     <td role="rowheader">Definir configurações do [!UICONTROL Flow Control]</td>   
     <td> <p>Clique no ícone [!UICONTROL Flow Control]. <img src="assets/flow-control-icon.gif"> Você pode definir uma tarefa para repetir um determinado número de vezes, converter uma matriz em uma série de pacotes e mesclar vários pacotes em um único pacote. Para obter mais informações, consulte <a href="../../workfront-fusion/apps-and-their-modules/flow-control.md" class="MCXref xref">Controle de fluxo em [!DNL Adobe Workfront Fusion]</a>.</p> </td>  
   </tr>  
   <tr> 
     <td role="rowheader">Aprimorar o cenário usando ferramentas avançadas</td>   
     <td>Clique no ícone [!UICONTROL Ferramentas]. <img src="assets/tools-icon.gif"> Você pode criar acionadores, ações, agregadores e transformadores. Para obter mais informações, consulte <a href="../../workfront-fusion/apps-and-their-modules/tools-modules.md" class="MCXref xref">Ferramentas</a>.</td>  
   </tr>  
   <tr> 
     <td role="rowheader">Usar ferramentas de análise de texto</td>   
     <td>Clique no ícone [!UICONTROL Text parser]. <img src="assets/text-parser-icon.gif"> Você pode recuperar elementos do código HTML, localizar e extrair elementos da string correspondentes a um padrão de pesquisa, pesquisar e substituir texto e dados de "rascunho" de um site. Para obter mais informações, consulte <a href="../../workfront-fusion/apps-and-their-modules/tools-modules.md" class="MCXref xref">Ferramentas</a>.</td>  
   </tr>  
   <tr> 
     <td role="rowheader">Acesse os aplicativos e serviços mais usados</td>   
     <td> Clique em um ícone na <strong>[!UICONTROL Favoritos]</strong> na parte inferior da tela. Os ícones são exibidos nesta seção automaticamente à medida que você adiciona aplicativos e serviços ao seu cenário. Você também pode clicar no ícone Adicionar <img src="assets/add-icon.gif"> para adicionar aplicativos e serviços a essa área manualmente.</td>  
   </tr>  
   <tr> 
     <td role="rowheader">Testar o cenário</td>   
     <td>Clique em <strong>[!UICONTROL Executar uma vez]</strong> para verificar se o cenário é executado conforme o esperado antes de ativá-lo. Depois de ativado, o cenário será executado de acordo com seu agendamento. Se tudo não for executado conforme o esperado, visite nossa seção de tratamento de erros para saber como lidar com erros.</td> 
   </tr> 
</tbody>
</table>
