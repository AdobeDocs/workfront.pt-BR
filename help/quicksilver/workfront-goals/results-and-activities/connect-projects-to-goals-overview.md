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
source-git-commit: 024c612d46848c55529e902a00d481588d261584
workflow-type: tm+mt
source-wordcount: '939'
ht-degree: 2%

---

# Adicionar projetos às metas no Adobe Workfront Goals

<!--
THIS MIGHT NEED TO BE RENAMED BECAUSE THERE WILL BE OTHER OBJECTS CONNECTED TO GOALS IN THE FUTURE
-->

Você pode conectar projetos a metas para indicar como a meta avança, com base no progresso real do projeto. O projeto se torna um indicador de progresso para a meta.

Conectando projetos a metas, você pode vincular o planejamento estratégico de sua organização (metas) ao trabalho real que sua equipe está realizando e concluindo todos os dias (projetos).

>[!IMPORTANT]
>
>As metas a nível de projeto criadas na área Business Case de um projeto não estão conectadas às metas estratégicas criadas no Workfront Goals. Para obter informações sobre as metas do projeto de Business Case, consulte [Criar metas de Business Case](../../manage-work/projects/define-a-business-case/create-business-case-goals.md).


## Requisitos de acesso

Você deve ter o seguinte:

<table style="table-layout:auto">
<col>
</col>
<col>
</col>
<tbody>
 <tr> 
   <td role="rowheader">plano do Adobe Workfront*</td> 
   <td> 
   <p>Para o novo plano e estrutura de licença:
  <ul><li>Um plano Ultimate </li>
  Ou
  <li>Uma licença adicional para o Adobe Workfront Goals para os planos Prime ou Select Adobe Workfront. </li></ul> </p>
<p>Para o plano e a estrutura de licença atuais: 
<ul><li> A Pro ou superior </li>
  <li>Uma licença do Adobe Workfront Goals, além de uma licença da Workfront.</li></ul></p>
   </td> 
  </tr>
 <tr>
 <td role="rowheader">Licença da Adobe Workfront*</td>
 <td>
 <p>Nova licença: Contributor ou superior</p>
 Ou
 <p>Licença atual: Solicitação ou superior</p> <p>Para obter mais informações, consulte <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">visão geral das licenças da Adobe Workfront</a>.</p> </td>
 </tr>
 <tr>
 <td role="rowheader">Produto*</td>
 <td>
 <p> Novo requisito de produto, um dos seguintes: </p>
<ul>
<li>Um plano Select ou Prime do Adobe Workfront e uma licença adicional do Adobe Workfront Goals.</li>
<li>Um plano do Ultimate Workfront que inclui o Workfront Goals por padrão. </li></ul>
 <p>Ou</p>
 <p>Requisito atual do produto: um plano do Workfront e uma licença adicional para o Adobe Workfront Goals. </p> <p>Para obter informações, consulte <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requisitos para usar as Metas do Workfront</a>. </p> </td>
 </tr>
 <tr>
 <td role="rowheader">Nível de acesso</td>
 <td> <p>Editar acesso às Metas</p> </td>
 </tr>
 <tr data-mc-conditions="">
 <td role="rowheader">Permissões de objeto</td>
 <td>
  <div>
  <p>Exibir permissões ou mais altas para a meta para exibi-la</p>
  <p>Gerenciar permissões para a meta para editá-la</p>
  <p>Para obter informações sobre como compartilhar metas, consulte <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Compartilhar uma meta no Workfront Goals</a>. </p>
  </div> </td>
 </tr>
 <tr>
   <td role="rowheader"><p>Modelo de layout</p></td>
   <td> <p>Todos os usuários, incluindo administradores do Workfront, devem receber um modelo de layout que inclui a área Metas no Menu principal. </p>  
</td>
  </tr>
</tbody>
</table>

*Para obter mais informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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

  ![](assets/goal-closed-project-active-warning-goal-list-350x94.png)
-->

* Quando você exclui um projeto anexado a uma meta, o projeto também é excluído da meta.

  >[!CAUTION]
  >
  >Se a meta estava ativa antes de você excluir o projeto e não há outros indicadores de progresso na meta, a meta se torna Inativa.


## Adicionar projetos às metas

1. Clique no **Menu Principal** ![](assets/main-menu-icon.png) (faça o rascunho deste para o Shell: ou clique no **Menu Principal** ![](assets/three-line-main-menu-icon.png) no canto superior esquerdo, se estiver disponível.) e depois em **Metas**.
1. Na Lista de Metas, clique no nome de uma meta para abrir a página de metas.
1. Clique em **Indicadores de progresso** no painel esquerdo.
1. No menu suspenso **Novo indicador de progresso**, clique em **Adicionar projeto existente**.

   A caixa Adicionar projetos à meta é exibida.
1. (Opcional) Atualize o **Modo de Exibição**, **Filtro** ou **Agrupamento** clicando nos respectivos ícones no canto superior direito da lista para modificar o modo como a lista de projetos é exibida.
1. (Opcional) Clique no ícone ![](assets/search-icon.png) da **Pesquisa** e comece a digitar o nome de um projeto para localizá-lo rapidamente na lista.
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
