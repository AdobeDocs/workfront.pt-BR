---
product-area: agile-and-teams;projects
navigation-topic: use-kanban-in-an-agile-team
title: Editar informações da história
description: Ao visualizar um bloco de matéria no quadro Kanban, determinadas informações estão disponíveis para edição em linha, diretamente do bloco de matéria.
author: Jenny
feature: Agile
exl-id: a22a7b61-b331-4c98-9421-e7fccedcd096
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '396'
ht-degree: 2%

---

# Editar informações da história

## Entenda quais informações podem ser visualizadas e editadas {#understand-what-information-can-be-viewed-and-edited}

Ao visualizar um bloco de história no quadro [!UICONTROL Kanban], as informações na tabela a seguir estão disponíveis. É possível editar a maioria das informações em linha, diretamente no bloco de matéria.

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
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>O nome do projeto com um link direto para o projeto</p> </td> 
   <td>✓ </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>O número de pontos ou horas concluídos na matéria e o número de pontos ou horas atribuídos à matéria<br>Esses números são usados para calcular e exibir o Percentual concluído de cada matéria.</p> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>A [!UICONTROL Porcentagem concluída] para cada história e problema.<br>[!UICONTROL Porcentagem Concluída] para a iteração é calculada com base na [!UICONTROL Porcentagem Concluída] para cada matéria.<br></p> <p>Ao atualizar a [!UICONTROL Porcentagem concluída] para uma história ou problema, você pode escolher qualquer número entre 0 e 100.</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>A quem a história é atribuída</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>A cor ou categoria do bloco</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>Quaisquer campos adicionais (incluindo campos personalizados) que possam ter sido adicionados à exibição Agile modificando a exibição Agile, conforme descrito em "Criando e Personalizando uma Exibição Agile" na <a href="../../reports-and-dashboards/reports/reporting-elements/views-overview.md" class="MCXref xref">Visão geral das Exibições em [!DNL Adobe Workfront]</a></p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacote do Adobe Workfront</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td> <p>Standard</p> 
   <p>Trabalhar ou superior</p> </td> 
  </tr>
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Exibir e editar informações em um bloco de história

{{step1-to-team}}

1. (Opcional) Clique no ícone **[!UICONTROL Equipe do Switch]** ![Ícone Equipe do Switch](assets/switch-team-icon.png), em seguida, selecione uma nova equipe Kanban no menu suspenso ou procure uma equipe na barra de pesquisa.

1. Vá para o quadro [!UICONTROL Kanban].
1. Expanda o bloco da matéria para exibir todos os campos associados à matéria.

   ![Cartão de história](assets/story-expanded-on-kanban-board-2021-350x405.png)

1. (Opcional) Para editar um campo, clique nele e, em seguida, faça as alterações.
Você deve ter direitos de [!UICONTROL Editar] à tarefa ou problema para editar o bloco de história.
Para obter mais informações sobre cada campo e se ele pode ser editado, consulte [Entender quais informações podem ser visualizadas e editadas](#understand-what-information-can-be-viewed-and-edited).

>[!NOTE]
>
>Para alterar o [!UICONTROL Percentual concluído], você deve digitar um número entre 0 e 100. O campo não é um controle deslizante que você pode mover.
