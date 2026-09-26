---
title: Personalizar o menu Mais usando um modelo de layout
user-type: administrator
content-type: overview
product-area: system-administration;templates
navigation-topic: layout-templates
description: 'Você pode usar um modelo de layout para determinar as opções que aparecem quando um usuário clica no menu Mais (o menu de três pontos) ao visualizar os seguintes objetos na Adobe Workfront: projetos, tarefas, problemas, portfólios e programas.'
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: bee0117d-a15b-494a-833a-179a42ae4f74
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d5896d07-2812-5418-8b18-8957a0d7f0fb
    internal-label: System Setup and Administration
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
source-git-commit: 4c642a8ef31f3b9a03288f2d74e704be6ee86c55
workflow-type: tm+mt
source-wordcount: '352'
ht-degree: 9%
---
# Personalizar o menu Mais usando um modelo de layout

Você pode usar um modelo de layout para determinar as opções que aparecem quando um usuário clica no menu Mais (o menu de três pontos) ao visualizar os seguintes objetos na Adobe Workfront: projetos, tarefas, problemas, portfólios e programas.

![Amostra do menu Mais de um projeto](assets/more-menu-display-for-project.png)

Para obter informações sobre como criar modelos de layout, consulte [Criar e gerenciar modelos de layout](../use-layout-templates/create-and-manage-layout-templates.md).

Para obter informações sobre modelos de layout para grupos, consulte [Criar e modificar modelos de layout de um grupo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

Após configurar um modelo de layout, você deve atribuí-lo aos usuários para que as alterações feitas fiquem visíveis para outros usuários. Para obter informações sobre como atribuir um modelo de layout aos usuários, consulte [Atribuir usuários a um modelo de layout](../use-layout-templates/assign-users-to-layout-template.md).

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Pacote do Adobe Workfront</td> 
   <td>Qualquer</td> 
  </tr> 
  <tr> 
   <td>Licença do Adobe Workfront</td> 
   <td><p>Padrão</p>
       <p>Plano</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td>Configurações de nível de acesso</td> 
   <td> <p>Para executar essas etapas no nível do sistema, você precisa do nível de acesso Administrador do sistema.</p>
        <p>Para executá-las para um grupo, você deve ser um gerente desse grupo.</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Personalizar o menu Mais para uma área no Workfront

1. Comece a trabalhar em um modelo de layout, conforme descrito em [Criar e gerenciar modelos de layout](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
1. No menu suspenso **Personalizar o que os usuários veem**, clique no nome de um tipo de objeto ou de uma área do Workfront cujo menu Mais você deseja personalizar.
1. Clique em **Selecionar opções de menu**.
1. Na caixa **Selecionar opções de menu**, siga um destes procedimentos para determinar o que os usuários verão no menu Mais da área do Workfront ou do tipo de objeto selecionado:

   * Clique nos ícones **Mostrar** ![Mostrar ícone](assets/add-secondary-nav-item.png) ou **Ocultar** ![Ocultar ícone](assets/delete-secondary-nav-item.png) para exibir ou ocultar seções no painel esquerdo. Você não pode ocultar itens que não tenham um ícone **Mostrar** ou **Ocultar**.

   * Arraste os itens ![ícone Mover](assets/move-icon---dots.png) para alterar sua ordem no painel esquerdo.

1. Clique em **Concluído**.
