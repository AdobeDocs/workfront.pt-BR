---
product-area: agile-and-teams;projects
navigation-topic: use-kanban-in-an-agile-team
title: Editar informações da história
description: Ao visualizar um bloco de história no quadro Kanban, determinadas informações estão disponíveis para edição em linha, diretamente do bloco de história.
author: Lisa
feature: Agile
exl-id: a22a7b61-b331-4c98-9421-e7fccedcd096
source-git-commit: 9da0c8234f563a0202cd15017b37a341476f7406
workflow-type: tm+mt
source-wordcount: '433'
ht-degree: 0%

---

# Editar informações da história

## Entender quais informações podem ser visualizadas e editadas {#understand-what-information-can-be-viewed-and-edited}

Ao visualizar um bloco de história na [!UICONTROL Kanban] quadro, as informações na tabela a seguir estão disponíveis. Você pode editar a maioria das informações em linha, diretamente do bloco de história.

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
   <td> <p>O nome do projeto com um link diretamente para o projeto</p> </td> 
   <td>✓ </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>O número de pontos ou horas concluídas da história e o número de pontos ou horas atribuídas à história<br>Esses números são usados para calcular e exibir a porcentagem concluída de cada história.</p> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>A [!UICONTROL Porcentagem concluída] para cada história e edição.<br>[!UICONTROL A porcentagem concluída] da iteração é calculada com base na [!UICONTROL porcentagem concluída] de cada história.<br></p> <p>Ao atualizar a [!UICONTROL Porcentagem concluída] para uma história ou problema, você pode escolher qualquer número entre 0 e 100.</p> </td> 
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
   <td> <p>Quaisquer campos adicionais (incluindo campos personalizados) que possam ter sido adicionados à exibição ágil modificando a exibição ágil, conforme descrito em "Criação e personalização de uma exibição ágil" em <a href="../../reports-and-dashboards/reports/reporting-elements/views-overview.md" class="MCXref xref">Visão geral das exibições em [!DNL Adobe Workfront]</a></p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
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
   <td> <p>[!UICONTROL Worker] ou superior</p> <p>Observação: Se ainda não tiver acesso, pergunte ao seu [!DNL Workfront] administrador se eles definirem restrições adicionais em seu nível de acesso. Para obter informações sobre como uma [!DNL Workfront] administrador pode alterar seu nível de acesso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com seu [!DNL Workfront] administrador.

## Exibir e editar informações em um bloco de história

1. Clique no botão *[!UICONTROL *Menu principal]** ícone ![](assets/main-menu-icon.png) no canto superior direito de [!DNL Adobe Workfront], depois clique em **[!UICONTROL Equipes]**.

1. (Opcional) Clique no botão **[!UICONTROL Alterar equipe]** ícone ![Ícone Alternar equipe](assets/switch-team-icon.png), em seguida, selecione uma nova equipe de Kanban no menu suspenso ou procure por uma equipe na barra de pesquisa.

1. Vá para o [!UICONTROL Kanban] quadro.
1. Expanda o bloco de história para exibir todos os campos associados à história.

   ![](assets/story-expanded-on-kanban-board-2021-350x405.png)

1. (Opcional) Para editar um campo, clique no campo e faça as alterações.\
   Você deve ter [!UICONTROL Editar] direitos à tarefa ou edição para editar o bloco de história.\
   Para obter mais informações sobre cada campo e se ele pode ser editado, consulte [Entender quais informações podem ser visualizadas e editadas](#understand-what-information-can-be-viewed-and-edited).

>[!NOTE]
>
>Para alterar o [!UICONTROL Porcentagem concluída], você deve digitar um número entre 0 e 100. O campo não é um controle deslizante que você pode mover.
