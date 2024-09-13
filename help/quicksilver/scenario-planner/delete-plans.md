---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Excluir planos no Planejador de cenários
description: Você pode excluir os planos que criou. Não é possível excluir planos compartilhados com você.
author: Alina
feature: Workfront Scenario Planner
exl-id: 74515723-3822-425a-aa9e-970af63f9189
source-git-commit: bbc3ac852dae3d9a503b4585dfc229d43c9aed28
workflow-type: tm+mt
source-wordcount: '508'
ht-degree: 1%

---

# Excluir planos no [!DNL Scenario Planner]

Você pode excluir os planos que criou. Não é possível excluir planos compartilhados com você.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] plano*</p> </td> 
   <td> <ul></li>
   <li><p>Novo: Ultimate </p></li>
   <p>O Planejador de cenários não está disponível para os novos planos do Workfront Select ou do Workfront Prime. </p>
   <li><p>Atual: [!UICONTROL Business] ou superior</p></ul>
   </td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] licença*</p> </td> 
   <td> <p>Novo: Claro ou superior</p> 
   <p>Atual: [!UICONTROL Review] ou posterior</p> </td> 
  </tr> 
  <tr> 
   <td>Produto* </td> 
   <td> <ul><li><p>Para os novos planos do Workfront:</p><p> Adobe Workfront</li></p>
   <li><p>Para os planos atuais do Workfront: </p>
   <p>Adobe Workfront</p> <p>Planejador de cenários do Adobe Workfront</p></li></ul>

<p>Para obter mais informações, consulte <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">Acesso necessário para usar o [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Nível de acesso </td> 
   <td> <p>[!UICONTROL Editar] acesso à [!DNL Scenario Planner]</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>Permissões de objeto </p> </td> 
   <td> <p>[!UICONTROL Gerenciar] permissões para um plano</p> <p>Para obter informações sobre como solicitar acesso adicional a um plano, consulte <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">Solicitar acesso a um plano no [!DNL Scenario Planner]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Para obter informações, consulte [Requisitos de acesso à documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Excluir planos

>[!IMPORTANT]
>
>Não é possível recuperar planos excluídos.

É possível excluir um plano ou excluir um cenário em um plano.

* [Excluir planos](#delete-plans)
* [Excluir cenários](#delete-scenarios)

### Excluir planos

>[!IMPORTANT]
>
>Considere o seguinte ao excluir planos:
>
>* Todas as informações relacionadas ao plano também são excluídas. Isso inclui todos os cenários e iniciativas associados ao plano, incluindo informações sobre funções de trabalho e custos. Essas informações não podem ser recuperadas.
>* Se o plano contiver um cenário publicado, os projetos vinculados às iniciativas excluídas serão preservados e a área [!DNL Scenario Planner] permanecerá na seção [!UICONTROL Detalhes do projeto].
>
>  Para obter informações sobre como publicar iniciativas em projetos, consulte [Atualizar ou criar projetos publicando iniciativas em [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md).

Para deletar um plano:

{{step1-to-scenario-planner}}

Uma lista de planos é exibida.

1. Clique no nome de um plano para abri-lo.
1. Clique no **[!UICONTROL Mais menu]** ![](assets/more-menu.png) à direita do nome do plano e em **[!UICONTROL Excluir]** > **[!UICONTROL Sim, exclua-o]**.

   O plano é excluído e você retorna à lista de planos.

### Excluir cenários {#delete-scenarios}

>[!IMPORTANT]
>
>Considere o seguinte ao excluir um cenário:
>
>* A exclusão de um cenário exclui todas as iniciativas e suas informações do cenário. Se forem copiadas para outros cenários, as iniciativas permanecerão nos outros cenários.
>* Ao excluir um cenário, o cenário subsequente assume o número do cenário excluído e a ordem de contagem é preservada. Por exemplo, se você excluir o cenário 4, o cenário 5 se tornará o cenário 4.
>* Se algumas iniciativas no cenário forem publicadas, o projeto vinculado à iniciativa será preservado e a área Planejador de cenários permanecerá nos projetos vinculados
>* Se as iniciativas publicadas existirem em outro cenário, elas permanecerão nesse cenário, incluindo o link para o projeto. A publicação dessas iniciativas a partir de outros cenários atualiza os projetos vinculados com novas informações desses cenários.
>
>  Para obter informações sobre como publicar iniciativas em projetos, consulte [Atualizar ou criar projetos publicando iniciativas em [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md).

Para excluir um cenário:

1. Vá para o plano para o qual deseja deletar um cenário.

   Por padrão, o cenário Inicial é exibido.

1. Clique em **[!UICONTROL Comparar cenários]**.
1. No canto superior direito do cartão de cenário, clique no menu **[!UICONTROL Mais]** ![](assets/more-menu.png) e em **[!UICONTROL Excluir]**.

   O cenário é excluído.

1. Clique em **[!UICONTROL Salvar plano]** para salvar suas alterações.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Delete initiatives</h2>
<p>(NOTE: moved this section to its own article about deleting initiatives) </p> <note type="important">
<p>Consider the following when deleting initiatives:</p>
<ul>
<li>Deleting an initiative deletes the job roles and cost information from the initiative.</li>
<li><span>When you delete an initiative that is published to a project, the initiative is removed from the scenario but the Scenario Planner area remains in the Project Details section.</span> </li>
<li> <p>If the initiative you delete is the only published initiative on the scenario, the indicator that the plan has been published is also removed. </p> <p>For information about publishing initiatives to projects, see <a href="../scenario-planner/publish-scenarios-update-projects.md" class="MCXref xref">Update or create projects by publishing initiatives in the Scenario Planner</a>.</p> </li>
</ul>
</note>
<p>To delete an initiative:</p>
<ol>
<li value="1"> <p> <p>Click the <strong>Main Menu</strong> icon <img src="assets/main-menu-icon.png">, then click Scenarios.</p> </p> <p>A list of plans displays. </p> </li>
<li value="2">Click the name of a plan to open it, then locate the initiative you want to delete.</li>
<li value="3"> <p>Click the <strong>More menu</strong> <img src="assets/more-menu.png"> to the right of the initiative name, then click <strong>Delete</strong> > <strong>Yes, delete it</strong>. </p> <p>The initiative is deleted. </p> </li>
<li value="4">Click <strong>Save Plan</strong> to save your changes. </li>
</ol>
</div>
-->


