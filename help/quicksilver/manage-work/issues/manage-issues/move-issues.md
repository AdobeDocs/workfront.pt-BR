---
product-area: projects
navigation-topic: manage-issues
title: Mover problemas
description: Você pode mover problemas entre projetos e tarefas.
author: Alina
feature: Work Management
exl-id: 8ab9be3e-0412-43d9-ad1e-75c43613fa82
source-git-commit: 6c82c585376b41cff0e57b253b6a214fb00309de
workflow-type: tm+mt
source-wordcount: '881'
ht-degree: 1%

---

# Mover problemas

Você pode mover problemas entre os seguintes objetos:

* De um projeto para outro projeto
* De uma tarefa para outra tarefa no mesmo projeto ou em outro projeto
* De uma tarefa para um projeto ou para outro projeto
* De um projeto para uma tarefa no mesmo projeto ou uma tarefa em outro projeto

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront*</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Solicitação ou superior</p> <p>Licença de revisão ou superior para mover problemas na seção Problemas de um projeto.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a ocorrências</p> <p>Acesso de visualização ou superior a projetos e tarefas</p> <p>Observação: se você ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre acesso a problemas em seu Nível de Acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">Conceder acesso a problemas</a>. Para obter informações sobre como um administrador do Workfront pode alterar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões do problema</p> <p>Permissões do Contribute para o item no qual você está movendo o problema com a capacidade de Adicionar problemas.</p> <p> Para obter informações sobre a concessão de permissões para problemas, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Compartilhar um problema </a></p> <p>Para obter informações sobre como solicitar permissões adicionais, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso aos objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Para descobrir que plano, tipo de licença ou acesso você tem, entre em contato com o administrador do Workfront.

## Considerações sobre a movimentação de problemas

Considere o seguinte ao mover problemas que contêm documentos ou estão associados a uma fila de solicitações:

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

   ![](assets/copy-and-move-to-links-for-issue-in-a-list-nwe-350x119.png)

1. Continue com a movimentação do problema, conforme descrito na seção [Mover um único problema](#move-a-single-issue) começando na Etapa 2.

   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   (NOTE: ensure step stays accurate)
   </MadCap:conditionalText>
   -->

## Mover um único problema {#move-a-single-issue}

Você pode mover um problema ao visualizá-lo.

### Mover um único problema no ambiente de Pré-visualização

1. Vá para um problema que você deseja copiar, clique no menu **Mais** ![](assets/more-icon.png)à direita do nome do problema e selecione **Mover** para.

   ![](assets/nwe-move-at-issue-level-highlighted-350x579.png)

   A caixa **Mover Problema** é exibida.

   ![](assets/move-issue-box-nwe-350x280.png)

1. Na seção **Selecionar projeto de destino**, especifique o nome do projeto para o qual deseja mover os problemas. O nome do projeto atual é exibido por padrão.

   >[!TIP]
   >
   >Somente 100 projetos são exibidos na lista.

1. (Condicional) Clique em **solicitar acesso** se você não tiver acesso para mover problemas para o projeto.
1. (Condicional) Continue a mover o problema no projeto de destino selecionado sem solicitar acesso se tiver acesso para adicionar problemas a uma das tarefas no projeto de destino.

   ![](assets/move-issue-request-access-from-project-nwe-350x118.png)

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




