---
title: Personalizar a exibição de Detalhes usando um modelo de layout
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: Como administrador do Workfront, você pode usar um modelo de layout para determinar quais informações aparecem quando um usuário seleciona a seção Detalhes no painel esquerdo enquanto visualiza uma tarefa, problema, documento, programa ou portfólio.
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: 1474e1dd-9b10-476e-9526-6577efa8d1c2
source-git-commit: 7c624eff8931d206285b6c4d91083f4bf09a88b0
workflow-type: tm+mt
source-wordcount: '558'
ht-degree: 0%

---

# Personalizar a exibição de Detalhes usando um modelo de layout

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available for all customers in the Preview environment and for a select group of customers in the Production environment.</span>-->

Como administrador do Adobe Workfront, você pode usar um modelo de layout para determinar quais informações aparecem quando um usuário clica no ícone Detalhes ![](assets/project-details-icon.png) no painel esquerdo enquanto visualiza uma tarefa, problema, documento, programa ou portfólio.

<!--
or billing record
-->

Você também pode alterar a ordem das informações nas quais essas informações aparecem. Por exemplo, para todas as tarefas que os usuários veem, é possível mover as informações do Forms personalizado para a parte superior da exibição Detalhes para todas as tarefas que os usuários veem.

Para obter informações sobre como criar modelos de layout, consulte [Criar e gerenciar modelos de layout](../use-layout-templates/create-and-manage-layout-templates.md).

Para obter informações sobre modelos de layout para grupos, consulte [Criar e modificar modelos de layout de um grupo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

Após configurar um modelo de layout, você deve atribuí-lo aos usuários para que as alterações feitas fiquem visíveis para outros usuários. Para obter informações sobre como atribuir um modelo de layout aos usuários, consulte [Atribuir usuários a um modelo de layout](../use-layout-templates/assign-users-to-layout-template.md).

As alterações feitas na view Detalhes de um objeto também determinam a disponibilidade e a ordem dos campos que os usuários veem nas seguintes áreas:


* Caixas &quot;Criar objeto&quot;, como Criar tarefa

  ![](assets/new-task-dialog.png)


* Telas &quot;Editar objeto&quot; ao editar um objeto, como Editar tarefa, Editar problema e Editar projeto

  ![](assets/edit-task-screen.png)


* As telas &quot;Editar objetos&quot; são exibidas ao editar objetos em massa. Atualmente, isso é compatível com a edição de projetos em massa.

  ![](assets/customize-edit-projects-in-bulk-box-with-layout-template.png)


* Painel ![](assets/summary-panel-icon.png) de resumo para listas de tarefas e problemas

  ![](assets/summary-area.png)

  >[!NOTE]
  >
  >As alterações nos modelos de layout afetam a ordem e a disponibilidade dos campos no painel Resumo somente para as tarefas e problemas atribuídos ao usuário conectado.

* Caixas de conversão, como as caixas Converter problema em tarefa ou Converter problema em projeto.

  ![Converter problema em caixa de tarefa](assets/convert-issue-to-task-box.png)

Para obter informações sobre modelos de layout para grupos, consulte [Criar e modificar modelos de layout de um grupo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront</td> 
   <td>Qualquer</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td>Plano</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Para executar essas etapas no nível do sistema, você precisa do nível de acesso Administrador do sistema.
Para executá-las para um grupo, você deve ser um gerente desse grupo</p> <p><b>OBSERVAÇÃO</b>: se você ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais no seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Personalize o que os usuários veem na visualização de Detalhes

1. Comece a trabalhar em um modelo de layout, conforme descrito em [Criar e gerenciar modelos de layout](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
1. Clique na seta para baixo ![](assets/dropdown-arrow-12x12.png) em **Personalizar o que os usuários veem** e em **Projeto**, **Tarefa**, **Problema**, **Programa** ou **Portfolio.**
<!--
, or billing record
-->

1. Na seção **Detalhes**, siga um destes procedimentos para personalizar o que os usuários veem na exibição Detalhes:

   * Arraste qualquer cabeçalho de seção ![](assets/move-icon---dots.png) para alterar sua ordem.
   * Habilite ou desabilite opções em **Visão geral** e **Forms Personalizado** para exibi-las ou ocultá-las.

     Se você ocultar todos os campos em uma dessas seções, a seção inteira será ocultada.

     Todos os campos são ativados por padrão.

1. Continue personalizando o modelo de layout.

   Ou

   Se tiver terminado de personalizar, clique em **Salvar**.

   >[!TIP]
   >
   >Você pode clicar em Salvar a qualquer momento para salvar seu progresso e, em seguida, continuar modificando o modelo posteriormente.
