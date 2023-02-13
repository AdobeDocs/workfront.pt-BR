---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Excluir planos no Planejador de Cenário
description: Você pode excluir os planos criados. Não é possível excluir planos compartilhados com você.
author: Alina
feature: Workfront Scenario Planner
exl-id: 74515723-3822-425a-aa9e-970af63f9189
source-git-commit: 6c5be4dccff46abbed104f1f1b3c958aaf74d629
workflow-type: tm+mt
source-wordcount: '530'
ht-degree: 1%

---

# Excluir planos na [!DNL Scenario Planner]

Você pode excluir os planos criados. Não é possível excluir planos compartilhados com você.

## Requisitos de acesso

Você deve ter o seguinte:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront]<b> plano*</b> </p> </td> 
   <td>[!UICONTROL Business] ou superior</td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront]<b> licença*</b> </p> </td> 
   <td> <p>[!UICONTROL Review] ou superior</p> </td> 
  </tr> 
  <tr> 
   <td><b>Produto</b> </td> 
   <td> <p>Você deve comprar uma licença adicional para a [!DNL Adobe Workfront Scenario Planner] para acessar a funcionalidade descrita neste artigo.</p> <p>Para obter informações sobre como obter o [!DNL Workfront Scenario Planner], consulte <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">O acesso necessário para usar o [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><strong>Configurações de nível de acesso*</strong> </td> 
   <td> <p>Acesso à [!UICONTROL Editar] ou superior à [!DNL Scenario Planner]</p> <p>Observação: Se ainda não tiver acesso, pergunte ao seu [!DNL Workfront] administrador se eles definirem restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode alterar seu nível de acesso, consulte <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><strong>Permissões de objeto</strong> </p> </td> 
   <td> <p>Permissões do [!UICONTROL Manager] para um plano</p> <p>Para obter informações sobre como solicitar acesso adicional a um plano, consulte <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">Solicitar acesso a um plano na [!DNL Scenario Planner]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com seu [!DNL Workfront] administrador.

## Excluir planos

>[!IMPORTANT]
>
>Não é possível recuperar planos excluídos.

Você pode deletar um plano ou pode deletar um cenário em um plano.

* [Excluir planos](#delete-plans)
* [Excluir cenários](#delete-scenarios)

### Excluir planos

>[!IMPORTANT]
>
>Considere o seguinte ao excluir planos:
>
>* Todas as informações relacionadas ao plano também são excluídas. Inclui todos os cenários e iniciativas associados ao plano, incluindo informações sobre funções e custos do emprego. Essas informações não podem ser recuperadas.
>* Se o plano contiver um cenário publicado, os projetos vinculados às iniciativas excluídas serão preservados e a variável [!DNL Scenario Planner] a área permanece no [!UICONTROL Detalhes do projeto] seção.
>
>  Para obter informações sobre como publicar iniciativas em projetos, consulte [Atualize ou crie projetos publicando iniciativas no [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md).

Para deletar um plano:

1. Clique no botão **[!UICONTROL Menu principal]** ícone ![](assets/main-menu-icon.png), depois clique em [!UICONTROL Cenários].

   Uma lista de planos é exibida.

1. Clique no nome de um plano para abri-lo.
1. Clique no botão **[!UICONTROL Menu Mais]** ![](assets/more-menu.png) à direita do nome do plano e clique em **[!UICONTROL Excluir]** > **[!UICONTROL Sim, exclua]**.

   O plano é excluído e você retorna à lista de planos.

### Excluir cenários {#delete-scenarios}

>[!IMPORTANT]
>
>Considere o seguinte ao excluir um cenário:
>
>* A exclusão de um cenário exclui todas as iniciativas e suas informações do cenário. Se forem copiadas para outros cenários, as iniciativas permanecerão em outros cenários.
>* Ao excluir um cenário, o cenário subsequente assume o número do cenário excluído e a ordem de contagem é preservada. Por exemplo, se você excluir o Cenário 4, o Cenário 5 se torna o Cenário 4.
>* Se algumas iniciativas no cenário forem publicadas, o projeto vinculado à iniciativa será preservado e a área do Planejador de Cenário permanecerá nos projetos vinculados
>* Se as iniciativas publicadas existirem em outro cenário, elas permanecerão nesse cenário, incluindo seu link para o projeto. Publicar essas iniciativas de outros cenários atualiza os projetos vinculados com novas informações desses cenários.
>
>  Para obter informações sobre como publicar iniciativas em projetos, consulte [Atualize ou crie projetos publicando iniciativas no [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md).

Para excluir um cenário:

1. Vá para o plano para o qual deseja excluir um cenário.

   Por padrão, o cenário inicial é exibido.

1. Clique em **[!UICONTROL Comparar cenários]**.
1. No canto superior direito do cartão de cenário, clique no botão **[!UICONTROL Mais]** menu ![](assets/more-menu.png), depois clique em **[!UICONTROL Excluir]**.

   O cenário é excluído.

1. Clique em **[!UICONTROL Salvar plano]** para salvar as alterações.

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


