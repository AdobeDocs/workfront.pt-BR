---
product-area: agile-and-teams;projects
navigation-topic: scrum-board
title: Exibir e editar informações da história no quadro de Soma
description: Ao visualizar um bloco de história no quadro Kanban, determinadas informações estão disponíveis para edição em linha, diretamente do bloco de história.
author: Lisa
feature: Agile
exl-id: 88d156ea-0913-425e-b3eb-6ae81d2d2336
source-git-commit: 6f817ca39c7489b85673ff601faf440fe51ab72c
workflow-type: tm+mt
source-wordcount: '495'
ht-degree: 0%

---

# Exibir e editar informações da história no [!UICONTROL Scrum] quadro

## Entender quais informações podem ser visualizadas e editadas

Ao visualizar um bloco de matérias no quadro de matérias, as informações na tabela a seguir estão disponíveis. Você pode editar a maioria das informações em linha, diretamente do bloco de história.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Informações</strong> </th> 
   <th><strong>Visível</strong> </th> 
   <th><strong>Editável em linha</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>O nome da história com um link diretamente para a tarefa ou edição</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>O nome do projeto com um link diretamente para o projeto<br>Esse link é exibido somente em histórias (tarefas principais, não subtarefas) ao usar a visualização ágil em uma iteração; não é exibido ao usar uma visualização ágil em um projeto.</p> </td> 
   <td>✓ </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>O número de pontos ou horas concluídas da história e o número de pontos ou horas atribuídas à história<br>Esses números são usados para calcular e exibir a [!UICONTROL Porcentagem concluída] para cada história.</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>A [!UICONTROL Porcentagem concluída] para cada história e edição.<br>A [!UICONTROL Porcentagem concluída] da iteração é calculada com base na [!UICONTROL Porcentagem concluída] de cada história.</p> <p>Ao atualizar a [!UICONTROL Porcentagem concluída] para uma história ou problema, você pode escolher qualquer número entre 0 e 100.</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>A quem a história está atribuída</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>A cor ou categoria do bloco</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>Quaisquer campos adicionais (incluindo campos personalizados) que possam ter sido adicionados à exibição ágil modificando a exibição ágil, conforme descrito em "Criação e personalização de uma exibição [!UICONTROL Ágil]" em <a href="../../../reports-and-dashboards/reports/reporting-elements/views-overview.md" class="MCXref xref">Visão geral das exibições na [!UICONTROL Adobe Workfront]</a>.</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] plano*</strong></td> 
   <td> <p>Qualquer Um</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licença*</strong></td> 
   <td> <p>[!UICONTROL Trabalho] ou superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurações de nível de acesso*</strong></td> 
   <td> <p>[!UICONTROL Worker] ou superior</p> <p>Observação: Se ainda não tiver acesso, pergunte ao seu [!DNL Workfront] administrador se eles definirem restrições adicionais em seu nível de acesso. Para obter informações sobre como uma [!DNL Workfront] administrador pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Permissões de objeto</strong></td> 
   <td> <p>Editar acesso à tarefa ou ocorrência</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com seu [!DNL Workfront] administrador.

## Exibir e editar informações em um bloco de história

1. Clique no botão **[!UICONTROL Menu principal]** ícone ![](assets/main-menu-icon.png) no canto superior direito de [!DNL Adobe Workfront], depois clique em **[!UICONTROL Equipes]**.

1. (Opcional) Clique no botão **[!UICONTROL Alterar equipe]** ícone ![Ícone Alternar equipe](assets/switch-team-icon.png)e, em seguida, selecione uma nova equipe de Soma no menu suspenso ou procure por uma equipe na barra de pesquisa.

1. No painel esquerdo, selecione **[!UICONTROL Iterações]** para escolher uma iteração específica, ou selecione **[!UICONTROL Iteração atual]**.

1. Vá para o [!UICONTROL Scrum] quadro de histórias ágeis.
1. Expanda o [!UICONTROL história] bloco para exibir todos os campos associados à história.

   ![](assets/agile-storycard-scrum-2021-350x333.png)

1. (Opcional) Para editar um campo, clique no campo e faça as alterações.

   Você deve ter [!UICONTROL Editar] direitos à tarefa ou edição para editar o bloco de história.

>[!NOTE]
>
>Para alterar o [!UICONTROL Porcentagem concluída], você deve digitar um número entre 0 e 100. O campo não é um controle deslizante que você pode mover.
