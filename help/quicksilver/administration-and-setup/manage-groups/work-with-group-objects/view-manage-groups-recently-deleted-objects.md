---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: work-with-a-groups-objects
title: Visualizar e gerenciar os itens excluídos recentemente de um grupo
description: Ao visualizar um grupo gerenciado na área Grupos, você pode visualizar, filtrar, restaurar e exportar os itens de trabalho, documentos e modelos excluídos recentemente.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: d5fbc71b-3b22-48d1-a056-f2c4b32c220c
source-git-commit: 7eaff1c74cd880bde062e6fdf169c73d6eeb7f75
workflow-type: tm+mt
source-wordcount: '414'
ht-degree: 1%

---

# Exibir e gerenciar os itens excluídos recentemente de um grupo

Ao visualizar um grupo gerenciado na área Grupos, você pode visualizar e trabalhar com projetos, tarefas, problemas, documentos e modelos excluídos recentemente das seguintes maneiras:

* Exibir, filtrar e agrupar uma lista de itens excluídos recentemente
* Restaurar itens excluídos recentemente selecionados
* Exportar uma lista de itens excluídos recentemente

Se houver algum grupo acima do seu, os administradores também poderão fazer essas coisas pelo seu grupo. O mesmo se aplica aos administradores do Workfront (para qualquer grupo).

Para obter mais informações sobre itens excluídos, consulte [Gerenciar itens excluídos](../../../administration-and-setup/manage-workfront/manage-deleted-items/manage-deleted-items.md).

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Pacote do Adobe Workfront</td> 
   <td><p>Qualquer</p></td> 
  </tr> 
  <tr> 
   <td>Licença do Adobe Workfront</td> 
   <td><p>Standard</p>
       <p>Plano</p></td>
  </tr> 
  <tr>
   <td>Configurações de nível de acesso</td> 
   <td>Você deve ser um administrador de grupo do grupo ou um administrador do sistema.</td>
  </tr>
  <tr> 
   <td>Permissões de objeto</td>
   <td>Os itens excluídos devem ser associados ao grupo ou a qualquer um de seus subgrupos.</td> 
  </tr> 
 </tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Exibir e gerenciar os itens excluídos recentemente de um grupo

{{step-1-to-setup}}

1. No painel esquerdo, clique em **Grupos** ![Grupos](assets/groups-icon.png).

1. Clique no nome do grupo.
1. No painel esquerdo, clique em **Excluídos recentemente**.
1. Abra uma das seguintes guias onde deseja visualizar e gerenciar os itens excluídos recentemente do grupo:

   * Projetos
   * Tarefas
   * Problemas
   * Documentos
   * Modelos

   Cada guia lista itens do tipo de objeto correspondente que pertencem ao grupo atual ou a seus subgrupos e que foram excluídos nos últimos 30 dias.

   >[!NOTE]
   >
   >Se alguém excluísse um projeto, todas as suas tarefas individuais, problemas e documentos fossem excluídos com ele. Elas não são exibidas individualmente nas guias Tarefas, Ocorrências, Documentos ou Modelos. No entanto, restaurar o projeto também restaura todos esses objetos filho no projeto.
   >
   >
   >Se alguém tiver excluído uma tarefa, problema, documento ou modelo individualmente, você poderá exibi-lo e gerenciá-lo na guia apropriada.

1. Conclua qualquer uma das seguintes ações:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>Restaurar objetos</p> </td> 
      <td> <p>Selecione até 10 objetos e clique em <strong>Restaurar</strong>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Exportar a lista inteira de objetos na guia</p> </td> 
      <td> <p>Clique em <strong>Exportar</strong>.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"> <p>Alterar a exibição de informações na lista</p> </td> 
      <td> <p>No canto superior direito acima da lista, use <strong>Filtro</strong> para definir o que é exibido com base nos critérios fornecidos. Use <strong>Exibir</strong> para definir quais campos são exibidos como colunas. Use o <strong>Agrupamento</strong> para agrupar os itens em categorias.</p> </td> 
     </tr> 
    </tbody> 
   </table>
