---
product-area: agile-and-teams;projects
navigation-topic: scrum-board
title: Adicionar uma subtarefa a uma história existente no quadro Scrum
description: Ao criar subtarefas para matérias existentes, lembre-se da configuração do Modo de conclusão do projeto, pois isso afeta a forma como as matérias são atualizadas.
author: Lisa
feature: Agile
exl-id: 264e66e9-94c7-4904-baad-f733d39b4791
source-git-commit: 6f817ca39c7489b85673ff601faf440fe51ab72c
workflow-type: tm+mt
source-wordcount: '661'
ht-degree: 0%

---

# Adicionar uma subtarefa a uma história existente no quadro [!UICONTROL Scrum]

Ao criar subtarefas para matérias existentes, lembre-se do seguinte:

**Quando a configuração [!UICONTROL Modo de Conclusão] do projeto estiver definida como [!UICONTROL Manual]:**

* Mover uma matéria pai com subtarefas para [!UICONTROL Concluído] atualiza a matéria pai para 100% e o [!UICONTROL Status] para [!UICONTROL Concluído]. As subtarefas não são atualizadas.
* Para atualizar o [!UICONTROL Percentual concluído] da matéria, atualize-o na guia [!UICONTROL Histórias] ou na página [!UICONTROL Detalhes] do objeto.

**Quando a configuração [!UICONTROL Modo de Conclusão] do projeto estiver definida como [!UICONTROL Automático]**:

* Mover uma matéria pai com subtarefas para [!UICONTROL Concluído] atualiza a matéria pai para 100% e o [!UICONTROL Status] para [!UICONTROL Concluído]. Subtarefas também são atualizadas para 100% e o [!UICONTROL Status] é atualizado para [!UICONTROL Concluído].
* Para atualizar o [!UICONTROL Percentual concluído] da matéria, você deve atualizar o [!UICONTROL Percentual concluído] para qualquer subtarefa. O [!UICONTROL Percentual concluído] da história é calculado com base no [!UICONTROL Percentual concluído] de todas as subtarefas.

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
   <td> <p>Acesso à [!UICONTROL Contribute] ou [!UICONTROL Manage] para a tarefa em que a subtarefa está</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso aos objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qual plano, tipo de licença ou acesso você tem, contate o administrador do [!DNL Workfront].

## Adicionar uma subtarefa a uma história existente no quadro Scrum

1. Clique no ícone ![](assets/main-menu-icon.png) do **[!UICONTROL Menu principal]** no canto superior direito de [!DNL Adobe Workfront] e em **[!UICONTROL Equipes]**.

1. (Opcional) Clique no ícone **[!UICONTROL Equipe do Switch]** ![Ícone da equipe do Switch](assets/switch-team-icon.png), em seguida, selecione uma nova equipe do Scrum no menu suspenso ou procure uma equipe na barra de pesquisa.

1. Vá para a iteração ágil ou para o projeto que contém a matéria em que você deseja adicionar uma subtarefa. Para obter informações sobre como navegar para uma iteração, consulte [Exibir uma iteração](../../../agile/use-scrum-in-an-agile-team/iterations/view-iteration.md).
1. Vá para o bloco de matéria no storyboard onde deseja adicionar uma subtarefa.
1. Clique em **[!UICONTROL Adicionar Subtarefa]** no cartão de história principal para criar uma subtarefa para a história.

   ![Adicionar subtarefa](assets/agile-story-addsubtask-NWE.png)

   Ou

   Clique em **[!UICONTROL Adicionar Subtarefa]** em um bloco de subtarefa para criar uma subtarefa para a subtarefa.

   O [!DNL Workfront] oferece suporte a níveis infinitos de subtarefas, mas apenas dois níveis (subtarefas de subtarefas) são exibidos no storyboard Agile.

   ![Adicionar subtarefa](assets/agile-story-addsubtask2-NWE.png)

   Ao adicionar uma subtarefa a uma história que atualmente não tem uma raia, a tarefa pai é promovida para a coluna [!UICONTROL História pai] e a subtarefa se move dentro da raia.

1. Especifique as seguintes informações:

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Nome da Subtarefa]</strong></td>
      <td> Especifique um nome para a subtarefa.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Descrição]</strong></td>
      <td>Especifique uma descrição para a subtarefa.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Estimativa]</strong></td>
      <td>Especifique a estimativa para a subtarefa.<br><p>Lembre-se do seguinte ao criar estimativas:</p>
       <ul>
        <li>Se a sua equipe ágil estiver configurada para estimar histórias em pontos, por padrão, 1 ponto é igual a 8 horas. As estimativas são adicionadas como [!UICONTROL Horas planejadas] na história.</li>
        <li>As estimativas combinadas de todas as subtarefas determinam a estimativa da matéria-prima. Para obter mais informações, consulte <a href="../../../agile/use-scrum-in-an-agile-team/scrum-board/update-status-of-stories-and-subtasks.md" class="MCXref xref">Atualizar o status de histórias e subtarefas no quadro Scrum</a>.</li>
        <li>Quando você cria uma nova subtarefa, o campo [!UICONTROL Estimativa] já está definido. Se você redefinir a estimativa na subtarefa, estará redefinindo a estimativa na matéria pai (porque a matéria pai é a soma de todas as suas subtarefas).</li>
       </ul><br></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Horas Planejadas]</strong></td>
      <td> (Disponível somente em projetos) Especifique o número de horas planejadas para a tarefa.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Atribuição]</strong></td>
      <td>Comece digitando o nome da equipe à qual deseja atribuir a subtarefa e clique nela quando ela aparecer na lista suspensa.</td>
     </tr>
    </tbody>
   </table>

1. Clique em **[!UICONTROL Criar]**.
