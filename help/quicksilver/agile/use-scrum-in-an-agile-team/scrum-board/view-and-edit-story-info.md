---
product-area: agile-and-teams;projects
navigation-topic: scrum-board
title: Exibir e editar informações de história no quadro Scrum
description: Ao visualizar um bloco de matéria no quadro Kanban, determinadas informações estão disponíveis para edição em linha, diretamente do bloco de matéria.
author: Lisa
feature: Agile
exl-id: 88d156ea-0913-425e-b3eb-6ae81d2d2336
source-git-commit: 6f817ca39c7489b85673ff601faf440fe51ab72c
workflow-type: tm+mt
source-wordcount: '511'
ht-degree: 0%

---

# Exibir e editar informações de história no quadro [!UICONTROL Scrum]

## Entenda quais informações podem ser visualizadas e editadas

Ao exibir um bloco de matéria no storyboard, as informações na tabela a seguir estão disponíveis. É possível editar a maioria das informações em linha, diretamente no bloco de matéria.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Informações</strong> </th> 
   <th><strong>Visível</strong> </th> 
   <th><strong>Editável Embutido</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>O nome da história com um link diretamente para a tarefa ou problema</td> 
   <td>✓ µ</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>O nome do projeto com um link diretamente para o projeto<br>Este link é exibido somente em histórias (tarefas pai, não subtarefas) ao usar a exibição ágil em uma iteração; ele não é exibido ao usar uma exibição ágil em um projeto.</p> </td> 
   <td>✓ µ </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>O número de pontos ou horas concluídas na matéria e o número de pontos ou horas atribuídas à matéria<br>Esses números são usados para calcular e exibir a [!UICONTROL Percentual concluído] para cada matéria.</p> </td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
  </tr> 
  <tr> 
   <td> <p>A [!UICONTROL Porcentagem concluída] para cada história e problema.<br>A [!UICONTROL Porcentagem Concluída] para a iteração é calculada com base na [!UICONTROL Porcentagem Concluída] para cada matéria.</p> <p>Ao atualizar a [!UICONTROL Porcentagem concluída] para uma história ou problema, você pode escolher qualquer número entre 0 e 100.</p> </td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
  </tr> 
  <tr> 
   <td> <p>A quem a história é atribuída</p> </td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
  </tr> 
  <tr> 
   <td> <p>A cor ou categoria do bloco</p> </td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
  </tr> 
  <tr> 
   <td> <p>Quaisquer campos adicionais (incluindo campos personalizados) que possam ter sido adicionados à exibição ágil por meio da modificação da exibição ágil, conforme descrito em "Criação e Personalização de uma Exibição do [!UICONTROL Agile]" na <a href="../../../reports-and-dashboards/reports/reporting-elements/views-overview.md" class="MCXref xref">Visão geral das Exibições no [!UICONTROL Adobe Workfront]</a>.</p> </td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
  </tr> 
 </tbody> 
</table>

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] plano*</strong></td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licença*</strong></td> 
   <td> <p>[!UICONTROL Work] ou superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurações de nível de acesso*</strong></td> 
   <td> <p>[!UICONTROL Worker] ou superior</p> <p>Observação: se você ainda não tiver acesso, pergunte ao administrador do [!DNL Workfront] se ele definiu restrições adicionais no seu nível de acesso. Para obter informações sobre como um administrador do [!DNL Workfront] pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Permissões de objeto</strong></td> 
   <td> <p>Editar acesso à tarefa ou problema</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso aos objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qual plano, tipo de licença ou acesso você tem, contate o administrador do [!DNL Workfront].

## Exibir e editar informações em um bloco de história

1. Clique no ícone ![](assets/main-menu-icon.png) do **[!UICONTROL Menu principal]** no canto superior direito de [!DNL Adobe Workfront] e em **[!UICONTROL Equipes]**.

1. (Opcional) Clique no ícone **[!UICONTROL Equipe do Switch]** ![Ícone da equipe do Switch](assets/switch-team-icon.png), em seguida, selecione uma nova equipe do Scrum no menu suspenso ou procure uma equipe na barra de pesquisa.

1. No painel esquerdo, selecione **[!UICONTROL Iterações]** para escolher uma iteração específica, ou selecione **[!UICONTROL Iteração atual]**.

1. Vá para o storyboard ágil [!UICONTROL Scrum].
1. Expanda o bloco [!UICONTROL história] para exibir todos os campos associados à história.

   ![](assets/agile-storycard-scrum-2021-350x333.png)

1. (Opcional) Para editar um campo, clique nele e, em seguida, faça as alterações.

   Você deve ter direitos de [!UICONTROL Editar] à tarefa ou problema para editar o bloco de história.

>[!NOTE]
>
>Para alterar o [!UICONTROL Percentual concluído], você deve digitar um número entre 0 e 100. O campo não é um controle deslizante que você pode mover.
