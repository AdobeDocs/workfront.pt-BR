---
content-type: overview
product-previous: workfront-goals
product-area: projects
navigation-topic: results-and-activities
title: Adicionar projetos às metas no Adobe Workfront Goals
description: Você pode conectar projetos a metas para indicar como a meta avança, com base no progresso real do projeto. O projeto se torna um indicador de progresso para a meta.
author: Alina
feature: Workfront Goals
exl-id: 683c9cd9-6c7b-4d50-b326-b4000c9863e8
source-git-commit: 4ef71db5d93e314b746e8acdbf90fd041c6e71ae
workflow-type: tm+mt
source-wordcount: '865'
ht-degree: 1%

---

# Adicionar projetos às metas no Adobe Workfront Goals

<!--Audited for P&P only: 10/2025-->

Você pode conectar projetos a metas para indicar como a meta avança, com base no progresso real do projeto. O projeto se torna um indicador de progresso para a meta.

Conectando projetos a metas, você pode vincular o planejamento estratégico de sua organização (metas) ao trabalho real que sua equipe está realizando e concluindo todos os dias (projetos).

>[!IMPORTANT]
>
>As metas a nível de projeto criadas na área Business Case de um projeto não estão conectadas às metas estratégicas criadas no Workfront Goals. Para obter informações sobre as metas do projeto de Business Case, consulte [Criar metas de Business Case](../../manage-work/projects/define-a-business-case/create-business-case-goals.md).


## Requisitos de acesso

>[!NOTE]
>
>Sua empresa pode optar por continuar usando o Adobe Workfront Goals se ele comprou esse pacote no passado. Você precisa falar com o seu representante de conta para obter mais detalhes.
>
>O Adobe Workfront Goals não está mais disponível para compra.

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo. 

<table style="table-layout:auto">
<col>
</col>
<col>
</col>
<tbody>
 <tr>
  <td> <p>Pacote do Adobe Workfront</p> </td> 
   <td> 
   <p>Adobe Workfront Ultimate</p>
   </td> 
  </tr>
 <tr>
 <td role="rowheader">Licença do Adobe Workfront</td>
 <td>
 <p>Colaborador ou superior</p>
<p>Solicitação ou superior</p></td>
 </tr>
  <tr>
 <td role="rowheader">Configuração do nível de acesso</td>
 <td> <p>Editar acesso às Metas</p> </td>
 </tr>
 <tr data-mc-conditions="">
 <td role="rowheader">Permissões de objeto</td>
 <td>
  <div>
  <p>Exibir permissões ou mais altas para a meta para exibi-la</p>
  <p>Gerenciar permissões para a meta para editá-la</p>
  </div> </td>
 </tr>
<tr>
   <td role="rowheader"><p>Modelo de layout</p></td>
   <td> <p>Todos os usuários, incluindo Administradores do sistema, devem receber um modelo de layout que inclua a área Metas no Menu principal. </p>  
</td>
  </tr>
</tbody>
</table>

Para obter mais informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:
<table style="table-layout:auto">
<col>
</col>
<col>
</col>
<tbody>
 <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> 
   <p>For the new plan and license structure:
  <ul><li>An Ultimate plan </li></ul>
   </p>
<p>For the current plan and license structure: 
<ul><li> A Pro or higher </li>
  <li>An Adobe Workfront Goals license in addition to a Workfront license.</li></ul></p>
   </td> 
  </tr>
 <tr>
 <td role="rowheader">Adobe Workfront license*</td>
 <td>
 <p>New license: Contributor or higher</p>
 Or
 <p>Current license: Request or higher</p> <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p> </td>
 </tr>
 <tr>
 <td role="rowheader">Product*</td>
 <td>
 <p> New product requirement, one of the following: </p>
<ul>
<li>A Select or Prime Adobe Workfront plan and an additional Adobe Workfront Goals license.</li>
<li>An Ultimate Workfront plan which includes Workfront Goals by default. </li></ul>
 <p>Or</p>
 <p>Current product requirement: A Workfront plan and an additional license for Adobe Workfront Goals. </p> <p>For information, see <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requirements to use Workfront Goals</a>. </p> </td>
 </tr>
 <tr>
 <td role="rowheader">Access level</td>
 <td> <p>Edit access to Goals</p> </td>
 </tr>
 <tr data-mc-conditions="">
 <td role="rowheader">Object permissions</td>
 <td>
  <div>
  <p>View or higher permissions to the goal to view it</p>
  <p>Manage permissions to the goal to edit it</p>
  <p>For information about sharing goals, see <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Share a goal in Workfront Goals</a>. </p>
  </div> </td>
 </tr>
 <tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>All users, including Workfront administrators,  must be assigned a layout template that includes the Goals area in the Main Menu. </p>  
</td>
  </tr>
</tbody>
</table>-->

## Considerações sobre a conexão de projetos às metas

* Você pode adicionar um projeto que atenda aos seguintes critérios a uma meta:

   * Você deve ter pelo menos permissões para Visualizá-lo.

     >[!NOTE]
     >
     >Se você perder as permissões para visualizar o projeto depois de anexar o projeto à meta, ainda poderá ver as informações do projeto sobre a meta, mas não poderá mais acessar o projeto.

   * O projeto não deve ter o status de Desativado.

* É possível associar vários projetos a uma meta.
* Você pode associar o mesmo projeto a várias metas.
* Não é possível atualizar manualmente o progresso de um projeto da meta à qual o projeto está anexado. Em vez disso, o Workfront calcula o percentual concluído do projeto e o Workfront Goals calcula o progresso da meta usando esse percentual concluído. Isso atualiza a meta em tempo real após as atualizações de porcentagem do projeto.
* A duração do projeto pode estar fora do período de uma meta. Se um projeto durar mais do que o prazo da meta, você ainda poderá fechar a meta e considerá-la concluída, mas a porcentagem concluída da meta não será 100%. A porcentagem concluída do projeto não é mais atualizada na meta.

<!--this is no longer visible in the new redesigned interface for goals: logged a bug for this: https://experience.adobe.com/#/@adobeinternalworkfront/so:hub-Hub/workfront/issue/63ceb049000080d30022aab9a359f6f1/updates - but confirmed that this will not be brought back at least for now - Jan 2023. 

There is an indication on the goal list that the project no longer updates progress for the goal.

  ![Goal closed](assets/goal-closed-project-active-warning-goal-list-350x94.png)
-->

* Quando você exclui um projeto anexado a uma meta, o projeto também é excluído da meta.

  >[!CAUTION]
  >
  >Se a meta estava ativa antes de você excluir o projeto e não há outros indicadores de progresso na meta, a meta se torna Inativa.


## Adicionar projetos às metas

1. Clique no **Ícone do** ![Menu Principal](assets/main-menu-icon.png) (faça o rascunho deste para o Shell: ou clique no **Menu Principal** ![Linhas do Menu Principal](assets/three-line-main-menu-icon.png) no canto superior esquerdo, se estiver disponível.) e em **Metas**.
1. Na Lista de Metas, clique no nome de uma meta para abrir a página de metas.
1. Clique em **Indicadores de progresso** no painel esquerdo.
1. No menu suspenso **Novo indicador de progresso**, clique em **Adicionar projeto existente**.

   A caixa Adicionar projetos à meta é exibida.
1. (Opcional) Atualize o **Modo de Exibição**, **Filtro** ou **Agrupamento** clicando nos respectivos ícones no canto superior direito da lista para modificar o modo como a lista de projetos é exibida.
1. (Opcional) Clique no ícone **Pesquisar** ![Ícone Pesquisar](assets/search-icon.png) e comece a digitar o nome de um projeto para localizá-lo rapidamente na lista.
1. Selecione os projetos que deseja adicionar à meta e clique em **Adicionar**.

   Os projetos selecionados são adicionados à meta e são exibidos na seção Indicadores de progresso da página de meta, no agrupamento **Projeto**.

   Após ativar a meta, o progresso da meta é atualizado automaticamente quando o progresso de um projeto é atualizado. Para obter informações sobre como ativar uma meta, consulte [Ativar metas no Adobe Workfront Goals](../goal-management/activate-goals.md).

## Localizar informações do projeto sobre metas

<p>
As seguintes informações do projeto estão visíveis no nível da meta na seção Indicadores de progresso da página de uma meta:

</p>

<table>
  <tr>
   <td>Nome do Projeto
   </td>
   <td>Quaisquer alterações no nome do projeto também serão refletidas no projeto conectado.
   </td>
  </tr>
  <tr>
   <td>Proprietário do projeto
   </td>
   <td>Quaisquer alterações no proprietário do projeto também serão refletidas no projeto conectado.
   </td>
  </tr>
    <tr>
   <td>Progresso real
   </td>
   <td> <p>O percentual concluído do projeto. Não é possível atualizar manualmente a porcentagem concluída do projeto a partir da meta. O Workfront a calcula automaticamente com base no percentual concluído das tarefas. </p>
   </td>
  </tr>
  <tr>
   <td>Progresso
   </td>
   <td>A porcentagem concluída do projeto representada por uma barra. Qualquer alteração na porcentagem concluída do projeto atualiza automaticamente o progresso da meta, a menos que a meta esteja fechada.
   </td>
  </tr>

</table>

## Localizar informações de meta em projetos

As seguintes informações de meta estão visíveis em uma lista de projetos ou relatório:

| Informações da meta | Descrição |
|---|---|
| Metas | Uma lista de todas as metas que têm um projeto associado a elas. |
| Hierarquia de metas | A hierarquia à qual uma meta pertence. Somente os pais da meta e a meta são exibidos neste campo. As metas secundárias não são exibidas. |
| Número de metas vinculadas | O número de metas vinculadas a um projeto. |
