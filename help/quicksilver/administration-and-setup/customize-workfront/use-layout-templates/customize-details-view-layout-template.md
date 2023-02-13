---
title: Personalizar a visualização de Detalhes usando um modelo de layout
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: Como administrador do Workfront, você pode usar um modelo de layout para determinar quais informações serão exibidas quando um usuário selecionar a seção Detalhes no painel esquerdo enquanto exibe uma tarefa, problema, documento, programa ou portfólio.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 1474e1dd-9b10-476e-9526-6577efa8d1c2
source-git-commit: 6580fec18982215dbc2535d5f2ab159fc32ac3f5
workflow-type: tm+mt
source-wordcount: '477'
ht-degree: 0%

---

# Personalizar a visualização de Detalhes usando um modelo de layout

<!-- drafted for bulk editing proejcts: 
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment.</span> -->

Como administrador do Adobe Workfront, você pode usar um modelo de layout para determinar quais informações serão exibidas quando um usuário clicar no ícone Detalhes ![](assets/project-details-icon.png) no painel esquerdo, ao visualizar uma tarefa, problema, documento, programa ou portfólio.

<!--
or billing record
-->

Você também pode alterar a ordem das informações em que essas informações são exibidas. Por exemplo, para todas as tarefas que seus usuários veem, você pode mover informações personalizadas do Forms para a parte superior da exibição Detalhes para todas as tarefas que seus usuários veem.

As alterações feitas na exibição Detalhes de um objeto também determinam a disponibilidade e a ordem dos campos que os usuários veem nas seguintes áreas:

* Caixas &quot;Novo objeto&quot;, como Nova tarefa e Nova ocorrência

   ![](assets/new-task-dialog.png)

* Telas &quot;Editar objeto&quot;, como Editar tarefa, Editar ocorrência e Editar projeto

   ![](assets/edit-task-screen.png)

<!--drafted for bulk editing proejcts - make this bullet live and in yellow at Preview: 

* <span class="preview">"Edit objects" screens, such as Edit Projects, when editing projects in bulk</span>

  <span>![](assets/customize-edit-projects-in-bulk-box-with-layout-template.png)</span>
  -->

* Resumo ![](assets/summary-panel-icon.png) painel para listas de tarefas e problemas

   ![](assets/summary-area.png)

   >[!NOTE]
   >
   >As alterações nos modelos de layout afetam a ordem e a disponibilidade dos campos no painel Resumo somente para as tarefas e problemas atribuídos ao usuário conectado.

* Caixas de conversão, como o problema Converter em tarefa ou Converter edição em caixas de projeto.

   ![Caixa Converter problema em tarefa](assets/convert-issue-to-task-box.png)

Para obter informações sobre modelos de layout para grupos, consulte [Criar e modificar modelos de layout de um grupo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plano Adobe Workfront</td> 
   <td>Qualquer Um</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença Adobe Workfront</td> 
   <td>Plano</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Para executar essas etapas no nível do sistema, é necessário o nível de acesso Administrador do sistema.
Para executá-los para um grupo, você deve ser um gerente desse grupo</p> <p><b>OBSERVAÇÃO</b>: Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Personalizar o que os usuários veem na exibição Detalhes

1. Comece a trabalhar em um modelo de layout, conforme descrito em [Criar e gerenciar modelos de layout](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
1. Clique na seta para baixo ![](assets/dropdown-arrow-12x12.png) under **Personalize o que os usuários veem**, depois clique em **Projeto**, **Tarefa**, **Problema**, **Programa** ou **Portfolio.**
<!--
, or billing record
-->

1. No **Detalhes** siga um destes procedimentos para personalizar o que os usuários veem na exibição Detalhes:

   * Arraste qualquer cabeçalho de seção ![](assets/move-icon---dots.png) para alterar sua ordem.
   * Ative ou desative as opções em **Visão geral** e **Forms personalizada** para exibi-los ou ocultá-los.

      Se você ocultar todos os campos em uma dessas seções, a seção inteira ficará oculta.

      Todos os campos são ativados por padrão.

1. Continue personalizando o modelo de layout.

   Ou

   Se tiver terminado de personalizar, clique em **Salvar**.

   >[!TIP]
   >
   >Você pode clicar em Salvar a qualquer momento para salvar seu progresso e continuar modificando o modelo posteriormente.
