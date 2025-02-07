---
title: Personalizar cabeçalhos de objetos usando um modelo de layout
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: Como administrador do Adobe Workfront ou administrador de grupo , você pode usar um modelo de layout para configurar os campos que os usuários veem no cabeçalho do objeto quando abrem a página de um objeto.
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: cbeaa0d7-a61a-4806-a871-96663d9ce124
source-git-commit: d2ca099e78d5adb707a0a5a53ccb2e6dd06698f8
workflow-type: tm+mt
source-wordcount: '531'
ht-degree: 0%

---

# Personalizar cabeçalhos de objetos usando um modelo de layout

Como administrador do Adobe Workfront ou administrador de grupo, você pode usar um modelo de layout para configurar os campos que os usuários veem no cabeçalho do objeto quando abrem a página de um objeto.

>[!IMPORTANT]
>
>A personalização de cabeçalhos de objetos está disponível atualmente para projetos, tarefas e problemas.

![Campos do cabeçalho do objeto](assets/object-header-fields.png)

Para obter informações sobre como criar modelos de layout, consulte [Criar e gerenciar modelos de layout](../use-layout-templates/create-and-manage-layout-templates.md).

Para obter informações sobre modelos de layout para grupos, consulte [Criar e modificar modelos de layout de um grupo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

Após configurar um modelo de layout, você deve atribuí-lo aos usuários para que as alterações feitas fiquem visíveis para outros usuários. Para obter informações sobre como atribuir um modelo de layout aos usuários, consulte [Atribuir usuários a um modelo de layout](../use-layout-templates/assign-users-to-layout-template.md).

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

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
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td><p>Novo: Padrão</p>
  <p> Atual: Plano</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Para executar essas etapas no nível do sistema, você precisa do nível de acesso Administrador do sistema.
Para executá-las para um grupo, você deve ser um gerente desse grupo.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Para obter mais informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Personalizar cabeçalhos de objetos

1. Comece a trabalhar em um modelo de layout, conforme descrito em [Criar e gerenciar modelos de layout](../../customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
1. No menu suspenso **Personalizar o que os usuários veem**, selecione **Projetos**, **Tarefas** ou **Problemas**.

   <!--when this will be possible for more than 3 objects, at production, make this more general: update the sentence above to say "select an object you want to customize in the Customize what users see drop-down menu). -->

1. Na seção [!UICONTROL Campos de cabeçalho], passe o mouse sobre os campos exibidos e siga um destes procedimentos:
   * Clique no ícone **x** para remover um campo

     Ou

   * Clique e segure o ícone de **captura** para arrastar e soltar o campo em um novo local.

   <!--(NOTE: make sure the default names of these fields have not changed; otherwise, update screen shot)-->

   ![Campos do cabeçalho do objeto ocultam e movem ícones](assets/object-header-field-x-and-grab-icons-in-lt.png)

1. Você pode ter até cinco campos no cabeçalho de um objeto.
Se você já tiver cinco campos selecionados, remova um campo antes de adicionar um novo.
1. Na caixa **Adicionar campo**, comece digitando o nome de um campo do Workfront não editável que você deseja adicionar e, em seguida, selecione-o quando ele for exibido na lista. O campo é adicionado imediatamente à direita da caixa Adicionar campo e será exibido como o primeiro campo no canto superior esquerdo do cabeçalho do objeto.

   >[!TIP]
   >
   >* Você só pode adicionar campos exibidos na área Visão geral da seção Detalhes do objeto e que não sejam editáveis. Campos não editáveis são campos que os usuários não podem editar manualmente. Eles são automaticamente calculados pela Workfront.
   >
   >* Você pode adicionar campos editáveis que já fazem parte dos cabeçalhos padrão (por exemplo, Proprietário do projeto, Status, Percentual concluído, Atribuições).
   >
   >* Ao adicionar o campo &quot;Resolvido por&quot; ao cabeçalho de um problema, o campo é alterado para &quot;Resolvendo problema, tarefa ou projeto&quot; quando há um objeto de resolução associado ao problema.


   ![Adicionar campo ao cabeçalho](assets/add-field-to-header-in-lt-list.png)


1. (Opcional) Arraste e solte os campos adicionados em uma ordem diferente.

1. Continue personalizando o modelo de layout.

   Ou

   Se tiver terminado de personalizar, clique em **Salvar**.

   >[!TIP]
   >
   >Você pode clicar em Salvar a qualquer momento para salvar seu progresso e, em seguida, continuar modificando o modelo posteriormente.
