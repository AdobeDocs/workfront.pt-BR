---
product-area: projects
navigation-topic: manage-issues
title: Mover problemas
description: Você pode mover problemas entre projetos e tarefas.
author: Alina
feature: Work Management
exl-id: 8ab9be3e-0412-43d9-ad1e-75c43613fa82
source-git-commit: 0542587bb3254dec5664de493c1c321528cf7f3e
workflow-type: tm+mt
source-wordcount: '873'
ht-degree: 1%

---

# Mover problemas

<!--Audited: 12/2024-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

Você pode mover problemas entre os seguintes objetos:

* De um projeto para outro projeto
* De uma tarefa para outra tarefa no mesmo projeto ou em outro projeto
* De uma tarefa para um projeto ou para outro projeto
* De um projeto para uma tarefa no mesmo projeto ou uma tarefa em outro projeto

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacote do Adobe Workfront</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td> 
   <ul><li>Colaborador ou superior</li>
   <li>Leve ou superior para mover problemas na seção Problemas de um projeto</li></ul>
   Ou:
   <ul>   <li><p>Solicitação ou superior</p></li>
   <li><p>Licença de revisão ou superior para mover problemas na seção Problemas de um projeto.</p></li></ul>   
     </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Editar acesso a ocorrências</p> <p>Acesso de visualização ou superior a projetos e tarefas</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões do problema</p> <p>Contribua com permissões para o item em que você está movendo o problema com a capacidade de Adicionar problemas.</td> 
  </tr> 
 </tbody> 
</table>

*Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>New:</p> 
   <ul><li>Contributor or higher</li>
   <li>Light or higher to move issues in the Issues section of a project</li></ul>
   <p>Current:</p>
   <ul>
   <li><p>Request or higher</p></li>
   <li><p>Review or higher license to move issues in the Issues section of a project.</p></li></ul>   
     </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to Issues</p> <p>View or higher access to Projects and Tasks</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the issue</p> <p>Contribute permissions to the item where you are moving the issue with the ability to Add Issues.</td> 
  </tr> 
 </tbody> 
</table>-->

## Considerações sobre a movimentação de problemas

Considere o seguinte ao mover problemas que contêm documentos ou estão associados a uma fila de solicitações:

* O administrador do sistema ou do grupo pode impedir que você mova problemas que têm horas reportadas, dependendo de como ele configura a preferência Permitir que os usuários movam tarefas e problemas com horas reportadas na área Configuração. Para obter informações, consulte [Configurar preferências de tarefas e problemas do sistema](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

* **Quando um problema está associado a uma fila de solicitações:** Quando você move um problema para outro objeto e o problema está associado a uma fila de solicitações, o problema movido não está mais associado à fila original da qual o primeiro problema se originou.
* **Quando um documento é anexado ao problema:** Quando você move um problema para outro objeto e o problema tem um documento anexado a ele, o documento, suas versões e provas também são movidos para o novo problema. As aprovações associadas ao documento não são movidas.
* **Quando um problema está vinculado a um documento ou a uma pasta:** Quando você move um problema que tem documentos ou pastas vinculados a um serviço de terceiros, como o Google Drive, os links para os documentos são movidos com o problema.

## Mover problemas em uma lista

Você pode mover um ou vários problemas de uma lista de problemas ou de um relatório de problemas.

1. Vá para o projeto que contém o problema ou problemas que você deseja mover.

   Ou

   Ir para um relatório de problemas.

1. Se você optou por ir para um projeto, clique em **Problemas** no painel esquerdo.
1. Selecione o(s) problema(s) que deseja mover e clique no **menu Mais** na parte superior da lista de problemas, em seguida, clique em **Mover para**.

   ![Copiar e Mover para links](assets/copy-and-move-to-links-for-issue-in-a-list-nwe-350x119.png)

1. Continue com a movimentação dos problemas, conforme descrito na seção [Mover um único problema](#move-a-single-issue) começando na Etapa 2.

## Mover um único problema {#move-a-single-issue}

Você pode mover um problema ao visualizá-lo.

### Mover um único problema

1. Vá para um problema que você deseja mover, clique no menu **Mais** ![Mais menu](assets/more-icon.png) à direita do nome do problema e clique em **Mover para**.

   ![Mover no nível do problema](assets/nwe-move-at-issue-level-highlighted-350x579.png)

   A caixa **Mover Problema** é exibida.

   ![Mover caixa de problemas](assets/move-issue-box-nwe-350x280.png)

1. Na seção **Selecionar projeto de destino**, especifique o nome do projeto para o qual deseja mover os problemas. O nome do projeto atual é exibido por padrão.

   >[!TIP]
   >
   >Somente 100 projetos são exibidos na lista.

1. (Condicional) Clique em **solicitar acesso** se você não tiver acesso para mover problemas para o projeto.
1. (Condicional) Continue a mover o problema no projeto de destino selecionado sem solicitar acesso se tiver acesso para adicionar problemas a uma das tarefas no projeto de destino.

   ![Mover problema e solicitar acesso](assets/move-issue-request-access-from-project-nwe-350x118.png)

   >[!TIP]
   >
   >Mensagens semelhantes serão exibidas se o projeto selecionado estiver com aprovação pendente, concluído ou inativo, quando o administrador do Workfront impedir a adição de problemas a esses projetos. Para obter mais informações, consulte [Configurar preferências de projeto do sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

1. (Opcional) Na seção **Opções**, desmarque qualquer um dos itens listados na tabela abaixo para removê-los do problema movido. Todas as opções são selecionadas por padrão.

   >[!IMPORTANT]
   >
   >Desmarcar itens na lista Opções resulta em perda de dados. As informações do problema existente serão removidas e não poderão ser recuperadas.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Selecionar tudo</td> 
      <td>Desmarque esta opção para remover todas as informações do problema ao movê-lo para seu novo local. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Atribuições</td> 
      <td>Remove usuários, funções de trabalho ou equipes atribuídos ao problema.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Progresso</td> 
      <td>Remove o percentual concluído, se houver, do problema. </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><p>Documentos</p></td> 
      <td> <p>Remove tudo na guia documentos, incluindo versões de documentos, documentos vinculados e pastas.

   <b>OBSERVAÇÃO</b>

   Se você optar por não mover os documentos com o problema, eles serão excluídos e colocados na Lixeira por 30 dias. Um administrador pode restaurá-los e eles serão restaurados quando o problema for movido.

   Se o problema for excluído depois de movido, os documentos restaurados serão colocados na área Documentos da página do usuário do administrador que os restaura.
   <br> </p> </td>
   </tr> 
     <tr> 
      <td role="rowheader">Permissões</td> 
      <td>Remove as entidades com as quais o problema é compartilhado. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Atualizações</td> 
      <td>Remove comentários da seção Atualizações do problema.</td> 
     </tr> 
    </tbody> 
   </table>


1. (Opcional) Na seção **Selecionar tarefa**, selecione a tarefa para onde deseja mover o problema.
1. Clique em **Mover problema** ou **Mover problemas**, se tiver selecionado vários problemas em uma lista.

   Os problemas movidos são adicionados ao projeto especificado.




