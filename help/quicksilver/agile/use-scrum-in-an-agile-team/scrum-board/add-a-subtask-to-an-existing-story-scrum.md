---
product-area: agile-and-teams;projects
navigation-topic: scrum-board
title: Adicionar uma subtarefa a uma história existente no Quadro de crum
description: Ao criar subtarefas para histórias existentes, lembre-se da configuração Modo de conclusão do projeto, pois isso afeta a forma como as histórias são atualizadas.
author: Lisa
feature: Agile
exl-id: 264e66e9-94c7-4904-baad-f733d39b4791
source-git-commit: 6f817ca39c7489b85673ff601faf440fe51ab72c
workflow-type: tm+mt
source-wordcount: '656'
ht-degree: 0%

---

# Adicionar uma subtarefa a uma história existente no [!UICONTROL Scrum] quadro

Ao criar subtarefas para histórias existentes, lembre-se do seguinte:

**Quando a variável [!UICONTROL Modo de conclusão] a configuração do projeto está definida como [!UICONTROL Manual]:**

* Mover uma história pai com subtarefas para [!UICONTROL Concluído] atualiza a história pai para 100% e a variável [!UICONTROL Status] para [!UICONTROL Concluído]. Subtarefas não são atualizadas.
* Para atualizar o [!UICONTROL Porcentagem concluída] para a história, você deve atualizá-la do [!UICONTROL Histórias] ou da guia [!UICONTROL Detalhes] página do objeto.

**Quando a variável [!UICONTROL Modo de conclusão] a configuração do projeto está definida como [!UICONTROL Automático]**:

* Mover uma história pai com subtarefas para [!UICONTROL Concluído] atualiza a história pai para 100% e a variável [!UICONTROL Status] para [!UICONTROL Concluído]. As subtarefas também são atualizadas para 100% e a variável [!UICONTROL Status] é atualizado para [!UICONTROL Concluído].
* Para atualizar o [!UICONTROL Porcentagem concluída] para a história, você deve atualizar o [!UICONTROL Porcentagem concluída] para quaisquer subtarefas. O [!UICONTROL Porcentagem concluída] para a história é calculada com base na variável [!UICONTROL Porcentagem concluída] de todas as subtarefas.

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
   <td> <p>Acesso ao [!UICONTROL Contribute] ou [!UICONTROL Gerenciar] para a tarefa na qual a subtarefa está</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com seu [!DNL Workfront] administrador.

## Adicionar uma subtarefa a uma história existente no Quadro de crum

1. Clique no botão **[!UICONTROL Menu principal]** ícone ![](assets/main-menu-icon.png) no canto superior direito de [!DNL Adobe Workfront], depois clique em **[!UICONTROL Equipes]**.

1. (Opcional) Clique no botão **[!UICONTROL Alterar equipe]** ícone ![Ícone Alternar equipe](assets/switch-team-icon.png)e, em seguida, selecione uma nova equipe de Soma no menu suspenso ou procure por uma equipe na barra de pesquisa.

1. Vá para a iteração ágil ou o projeto que contém a história à qual deseja adicionar uma subtarefa. Para obter informações sobre como navegar para uma iteração, consulte [Exibir uma iteração](../../../agile/use-scrum-in-an-agile-team/iterations/view-iteration.md).
1. Vá para o bloco de história no quadro onde deseja adicionar uma subtarefa.
1. Clique em **[!UICONTROL Adicionar Subtarefa]** no cartão da história principal para criar uma subtarefa para a história.

   ![Adicionar subtarefa](assets/agile-story-addsubtask-NWE.png)

   Ou

   Clique em **[!UICONTROL Adicionar Subtarefa]** em um bloco de subtarefa para criar uma subtarefa para a subtarefa.

   [!DNL Workfront] O suporta níveis infinitos de subtarefas, mas apenas dois níveis (subtarefas de subtarefas) são exibidos no quadro de história ágil.

   ![Adicionar subtarefa](assets/agile-story-addsubtask2-NWE.png)

   Ao adicionar uma subtarefa a uma história que atualmente não tem uma linha de expansão, a tarefa pai é promovida para o [!UICONTROL História principal] e a subtarefa se move dentro da faixa.

1. Especifique as seguintes informações:

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Nome da subtarefa]</strong></td>
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
        <li>Se sua equipe ágil estiver configurada para estimar histórias em pontos, então por padrão 1 ponto é igual a 8 horas. As estimativas são adicionadas como [!UICONTROL Horas planejadas] na história.</li>
        <li>As estimativas combinadas para todas as subtarefas determinam a estimativa da história principal. Para obter mais informações, consulte <a href="../../../agile/use-scrum-in-an-agile-team/scrum-board/update-status-of-stories-and-subtasks.md" class="MCXref xref">Atualize o status de histórias e subtarefas no quadro Soma</a>.</li>
        <li>Ao criar uma nova subtarefa, o campo [!UICONTROL Estimativa] já está definido. Se você redefinir a estimativa na subtarefa, estará redefinindo a estimativa na história pai (porque a história pai é a soma de todas as suas subtarefas).</li>
       </ul><br></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Horas planejadas]</strong></td>
      <td> (Disponível somente em projetos) Especifique o número de horas planejadas para a tarefa.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Atribuição]</strong></td>
      <td>Comece digitando o nome da equipe à qual deseja atribuir a subtarefa e clique nele quando ele for exibido na lista suspensa.</td>
     </tr>
    </tbody>
   </table>

1. Clique em **[!UICONTROL Criar]**.
