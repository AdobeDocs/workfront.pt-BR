---
title: Personalizar páginas fixadas usando um modelo de layout
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: Em um modelo de layout, você pode fixar as páginas que deseja que os usuários sempre tenham disponíveis na parte superior do Adobe Workfront. Elas podem ser páginas acessadas pelo menu principal ou pelos painéis.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 55cc75c5-8b8c-48e7-b114-b41fe3d545d8
source-git-commit: 96028446d76f32daf512adf77d3b1c53021821ec
workflow-type: tm+mt
source-wordcount: '574'
ht-degree: 4%

---

# Personalizar páginas fixadas usando um modelo de layout

{{preview-fast-release-general}}

Em um modelo de layout, você pode fixar as páginas que deseja que os usuários sempre tenham disponíveis na parte superior do Adobe Workfront. Podem ser páginas acessadas por meio do ![ícone do menu principal](assets/main-menu-icon.png) ou do ![ícone do menu principal](assets/main-menu-icon-left-nav.png) do Menu principal quando disponíveis, ou painéis.

Quaisquer pins adicionados por seus usuários são exibidos à direita dos pinos adicionados no modelo de layout.

Para obter mais informações sobre como fixar páginas, consulte [Fixar páginas para personalizar seu espaço de trabalho](../../../workfront-basics/the-new-workfront-experience/pin-pages.md).

Para obter mais informações sobre modelos de layout, consulte [Criar e gerenciar modelos de layout](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

Para obter informações sobre modelos de layout para grupos, consulte [Criar e modificar modelos de layout de um grupo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

Após configurar um modelo de layout, você deve atribuí-lo aos usuários para que as alterações feitas fiquem visíveis para outros usuários. Para obter informações sobre como atribuir um modelo de layout aos usuários, consulte [Atribuir usuários a um modelo de layout](../use-layout-templates/assign-users-to-layout-template.md).

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Pacote do Adobe Workfront</td> 
   <td><p>Qualquer</p></td> 
  </tr> 
  <tr> 
   <td>Licença do Adobe Workfront</td> 
   <td><p>Standard</p>
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

## Fixar páginas usando um modelo de layout

1. Comece a trabalhar em um modelo de layout, conforme descrito em [Criar e gerenciar modelos de layout](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
1. Em **Área de navegação superior**, clique em **Adicionar novo pino**.

1. No menu suspenso exibido, siga um destes procedimentos:

   * Selecione entre as seguintes áreas:

      * Calendários
      * Painéis
      * Documentos
      * Metas
      * Início
      * Minhas atualizações
      * Portfólios
      * Programas
      * Projetos
      * Relatórios
      * Solicitações
      * Recursos
      * Cenários
      * Equipes
      * Modelos
      * Planilhas de horas
      * Usuários
      * Blueprints
      * Em Planejamento

     >[!IMPORTANT]
     >
     >Para exibir as áreas Metas, Cenários e Planejamento, são necessárias licenças adicionais.
     >
     >* Para obter informações sobre as Metas do Workfront, consulte [Visão geral das Metas do Adobe Workfront](../../../workfront-goals/goal-management/wf-goals-overview.md).
     >
     >* Para obter informações sobre o Planejador de cenários do Workfront, consulte [A visão geral do Planejador de cenários](../../../scenario-planner/scenario-planner-overview.md).
     >
     >* Para obter informações sobre o Workfront Planning, consulte [Introdução ao Adobe Workfront Planning](/help/quicksilver/planning/general/planning-overview.md).

   * Clique em **Adicionar um painel**
      * Digite um nome descritivo no campo <!--**Quick link name**-->**Nome personalizado**
      * Selecione um painel no **Adicionar um painel** campo <!-- dropdown for existing or canvas dashboard, called "Choose a dashboard" now -->
      * Clique em **Adicionar**.

1. Repita a etapa anterior para fixar quaisquer outras páginas.

1. (Opcional) Para mover um pino, passe o mouse sobre o pino e clique no ícone do menu Mais ![ícone Mais](assets/more-icon.png) ao lado do nome do pino e clique em **Mover para a esquerda** ou **Mover para a direita** para deslocar o pino na direção escolhida ou clique em **Mover para a frente** para deslocar o pino para a posição mais à esquerda.

1. (Opcional) Para renomear um pino, passe o mouse sobre o pino e clique no ícone do menu Mais ![ícone Mais](assets/more-icon.png) ao lado do nome do pino e clique em **Renomear pino**. Digite um novo nome e clique em **Salvar**.

1. (Opcional) Para excluir um pino, passe o mouse sobre o pino e clique no ícone de menu Mais ![ícone Mais](assets/more-icon.png) ao lado do nome do pino e clique em **Remover pino**.

1. <span class="preview">No ambiente de Pré-visualização: Continue personalizando o modelo de layout. Você pode clicar em **Aplicar** a qualquer momento para salvar seu progresso.</span>

   <span class="preview">Ou</span>

   <span class="preview">Se tiver terminado de personalizar, clique em **Salvar e Fechar**.</span>

1. No ambiente de Produção: Continue personalizando o modelo de layout.

   Ou

   Se tiver terminado de personalizar, clique em **Salvar**.

   >[!TIP]
   >
   >Você pode clicar em **Salvar** a qualquer momento para salvar seu progresso e, em seguida, continuar modificando o modelo mais tarde.
