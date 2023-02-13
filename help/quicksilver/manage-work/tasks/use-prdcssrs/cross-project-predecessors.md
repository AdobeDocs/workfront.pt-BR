---
product-area: projects
navigation-topic: use-predecessors
title: Criar antecessores entre projetos
description: Um Predecessor entre projetos é uma tarefa da qual depende outra tarefa (chamada de tarefa sucessora) em outro projeto. O antecessor é a tarefa que tem prioridade sobre a tarefa dependente (sucessor). Por exemplo, você pode criar uma dependência que requer que a tarefa antecessora seja marcada como Concluída antes que a tarefa dependente possa iniciar.
author: Alina
feature: Work Management
exl-id: 7e29e589-e0a5-437e-935d-d5bc1b268594
source-git-commit: 7b61f6d9380365daa614c597ee7755d6d01d915d
workflow-type: tm+mt
source-wordcount: '734'
ht-degree: 0%

---

# Criar antecessores entre projetos

Um antecessor entre projetos é uma tarefa da qual depende outra tarefa (chamada de tarefa sucessora) em outro projeto. O antecessor é a tarefa que tem prioridade sobre a tarefa dependente (sucessor). Por exemplo, você pode criar uma dependência que requer que a tarefa antecessora seja marcada como Concluída antes que a tarefa dependente possa iniciar.

Assim como os antecessores em um único projeto, o Adobe Workfront permite que as tarefas sejam dependentes de tarefas em outros projetos.

**EXEMPLO**

Se uma empresa escavadora tiver apenas um backhoe e dois projetos simultâneos tiverem tarefas que exigem o uso do backhoe, o gerente de projeto poderá tornar a tarefa no primeiro projeto dependente da tarefa no segundo projeto para ilustrar que a escavação pode iniciar quando o projeto anterior abdicar do backhoe.
Ao vincular projetos por meio de predecessores entre projetos, as datas do projeto principal (aquele que tem a tarefa predecessora) afetarão o projeto secundário (aquele que tem a tarefa sucessora).

>[!TIP]
>
>Você deve recalcular as linhas do tempo dos projetos para ver as datas atualizadas para o projeto secundário. Para obter mais informações sobre o recálculo de linhas do tempo, consulte [Configurar recálculos de linha do tempo para projetos](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-timeline-recalculations-projects.md).

Para obter mais informações sobre os relacionamentos do antecessor, consulte [Visão geral dos antecessores de tarefas](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

## Requisitos de acesso

<!--drafted - replace table for P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Standard </p> 
   Or
   <p>Legacy license: Plan </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Tasks and Projects</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the tasks and the projects</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plano Adobe Workfront*</td> 
   <td> <p>Qualquer Um</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Plano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a Tarefas e Projetos</p> <p><b>Nota</b>

Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões para as tarefas e os projetos</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

## Criar um antecessor entre projetos

1. Vá para a tarefa que será seu sucessor.
1. Clique em **Predecessores** no painel esquerdo.
1. Clique em **Adicionar antecessor.**
1. No **Projeto pai** , comece a digitar o nome do projeto que contém a tarefa que você deseja que dependa da tarefa atual.
1. Clique no nome quando ele aparecer na lista suspensa.
1. No **Tarefas** , comece a digitar o nome da tarefa que deseja que dependa da tarefa atual.
1. Especifique as seguintes informações para definir a relação entre o antecessor e a tarefa dependente:

   * **Tipo de dependência:** Selecione a relação que deseja que a tarefa tenha com a tarefa dependente. O relacionamento padrão é &quot;Finish-Start&quot;, o que significa que a tarefa predecessora deve ser concluída antes que a tarefa dependente possa ser iniciada. Para obter mais informações sobre os vários tipos de dependência, consulte [Visão geral dos tipos de dependência de tarefa](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md)

   * **Atraso:** Especifique a quantidade de tempo que deve decorrer após a conclusão de um antecessor imposto até que a tarefa dependente possa começar. Para obter mais informações sobre os vários tipos de atraso, consulte [Visão geral dos tipos de atraso](../../../manage-work/tasks/use-prdcssrs/lag-types.md).

   * **Forçado:** Quando essa opção é selecionada, a relação de dependência entre as duas tarefas não pode ser contornada pelos usuários que iniciam tarefas antecipadamente. Por exemplo, se você aplicar uma relação entre a Tarefa A e a Tarefa B, a Tarefa B não poderá ser iniciada até que a Tarefa A seja concluída. Para obter mais informações sobre como impor predecessores, consulte [Impor predecessores](../../../manage-work/tasks/use-prdcssrs/enforced-predecessors.md).

      Quando essa opção não está selecionada, a dependência é tratada como uma sugestão para os usuários. Por exemplo, os usuários podem iniciar a Tarefa B antes que a Tarefa A seja concluída.

1. Clique em **Salvar**.

   As tarefas que têm um predecessor entre projetos exibem o número de referência do projeto ao qual o predecessor pertence e o número da tarefa, separado por dois pontos na coluna Predecessores em uma lista de tarefas.

   ![Antecessor de vários projetos](assets/cross-project-predecessor-in-list-view.png)

   O ícone antecessor fica verde quando a tarefa antecessora é marcada como concluída. Isso indica que a tarefa dependente está pronta para o trabalho.

   Passe o mouse sobre esse valor para obter mais informações sobre o antecessor, o projeto e as datas. Clique no predecessor entre projetos na caixa de detalhes para abrir a tarefa. Clique em **Consulte Projeto** para abrir o projeto cruzado.

   ![Detalhes do antecessor entre projetos](assets/cross-project-predecessor-details.png)

   >[!TIP]
   >
   >   O **Consulte Projeto** é exibida somente ao visualizar um antecessor de projeto cruzado.

