---
title: Personalizar cabeçalhos de objetos usando um modelo de layout
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: Como administrador do Adobe Workfront ou administrador de grupo , você pode usar um modelo de layout para configurar os campos que os usuários veem no cabeçalho do objeto quando abrem a página de um objeto.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: cbeaa0d7-a61a-4806-a871-96663d9ce124
source-git-commit: a1ffec0d8a50ff7f025ff23370afa746cf0d6d3f
workflow-type: tm+mt
source-wordcount: '464'
ht-degree: 0%

---

# Personalizar cabeçalhos de objetos usando um modelo de layout

Como administrador do Adobe Workfront ou administrador de grupo, você pode usar um modelo de layout para configurar os campos que os usuários veem no cabeçalho do objeto quando abrem a página de um objeto.

>[!IMPORTANT]
>
>A personalização de cabeçalhos de objetos está disponível atualmente para projetos, tarefas e problemas.


Para obter informações sobre modelos de layout para grupos, consulte [Criar e modificar modelos de layout de um grupo](../../manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

![](assets/object-header-fields.png)

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:


<table>
  <tr>
   <td><strong>Plano Adobe Workfront</strong>
   </td>
   <td>Qualquer Um
   </td>
  </tr>
  <tr>
   <td><strong>Licença Adobe Workfront</strong>
   </td>
   <td>Plano
   </td>
  </tr>
  <tr>
   <td><strong>Configurações de nível de acesso</strong>
   </td>
   <td>Você deve ser um administrador do Workfront ou de grupo.
<p>
   </td>
  </tr>
</table>

Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte [Criar ou modificar níveis de acesso personalizados](../../add-users/configure-and-grant-access/create-modify-access-levels.md).

## Personalizar cabeçalhos de objetos

1. Comece a trabalhar em um modelo de layout, conforme descrito em [Criar e gerenciar modelos de layout](../../customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
1. No **Personalize o que os usuários veem** , selecione **Projetos**, **Tarefas** ou **Problemas**.

   <!--when this will be possible for more than 3 objects, at production, make this more general: update the sentence above to say "select an object you want to customize in the Customize what users see drop-down menu). -->

1. No [!UICONTROL Campos de cabeçalho] passe o mouse sobre os campos exibidos e execute um dos seguintes procedimentos:
   * Clique no botão **x** ícone para remover um campo

      Ou

   * Clique e segure a **agarrar** ícone para arrastar e soltar o campo em um novo local.

   <!--(NOTE: make sure the default names of these fields have not changed; otherwise, update screen shot)-->

   ![](assets/object-header-field-x-and-grab-icons-in-lt.png)

1. É possível ter até cinco campos no cabeçalho de um objeto.
Se você já tiver cinco campos selecionados, remova um campo antes de adicionar um novo.
1. No **Adicionar campo** , comece digitando o nome de um campo Workfront não editável que deseja adicionar e, em seguida, selecione-o quando for exibido na lista. O campo é adicionado à direita imediata da caixa Add field e será exibido como o primeiro campo no canto superior esquerdo do cabeçalho do objeto.

   >[!TIP]
   >
   >* Você só pode adicionar campos que são exibidos na área Visão geral da seção Detalhes do objeto e que não são editáveis. Campos não editáveis são campos que não podem ser editados manualmente pelos usuários. Eles são calculados automaticamente pelo Workfront.
   >
   >* Você pode adicionar campos editáveis que já fazem parte dos cabeçalhos padrão (por exemplo, Proprietário do projeto, Status, Porcentagem concluída, Atribuições).
   >
   >* Quando você adiciona o campo &quot;Resolvido por&quot; ao cabeçalho de um problema, o campo muda para &quot;Resolvendo problema, tarefa ou projeto&quot;, quando há um objeto de resolução associado ao problema.



   ![](assets/add-field-to-header-in-lt-list.png)


1. (Opcional) Arraste e solte os campos adicionados em uma ordem diferente.

1. Continue personalizando o modelo de layout.

   Ou

   Se tiver terminado de personalizar, clique em **Salvar**.

   >[!TIP]
   >
   >Você pode clicar em Salvar a qualquer momento para salvar seu progresso e continuar modificando o modelo posteriormente.
