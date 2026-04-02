---
title: Personalizar o menu principal usando um modelo de layout
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: Como administrador do Adobe Workfront ou administrador de grupo, você pode usar um modelo de layout para configurar as opções que os usuários veem quando abrem o menu principal no Workfront.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: d4f02102-0378-472f-9ebb-753502ec048b
source-git-commit: 4ce13e7d46efb026c1d42a61f4fce4bf1a37bb5f
workflow-type: tm+mt
source-wordcount: '777'
ht-degree: 10%

---

# Personalizar o menu principal usando um modelo de layout

{{highlighted-preview}}

<!--Audited: 01/2024-->

Como administrador do Adobe Workfront ou administrador de grupo, você pode usar um modelo de layout para configurar as opções que os usuários veem quando abrem o menu principal no Workfront.

>[!NOTE]
>
>As opções do Menu principal que os usuários veem dependem do tipo de licença e das configurações definidas no nível de acesso. Alguns usuários que utilizarão este modelo de layout talvez não vejam todas as opções escolhidas aqui. Para obter mais informações, consulte [Como os níveis de acesso e as permissões funcionam juntos](../../../administration-and-setup/add-users/access-levels-and-object-permissions/how-access-levels-permissions-work-together.md) e [Acesso configurável à funcionalidade para cada tipo de objeto](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).
>
>Você poderá ver diferentes opções no Menu principal se sua organização tiver sido integrada à Experiência unificada do Adobe Workfront. Para obter informações, consulte [Experiência unificada da Adobe para Workfront](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md).

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
   <td><p>Qualquer</p>
       <p>Adicionar aplicativos personalizados ao menu principal só está disponível para organizações licenciadas para o Adobe App Builder.</p></td> 
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

## Personalizar o menu principal

1. Comece a trabalhar em um modelo de layout, conforme descrito em [Criar e gerenciar modelos de layout](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
1. Clique em **Definir menu principal** no canto superior direito do modelo.

   A caixa Menu principal é aberta e você pode ver as áreas exibidas atualmente no Menu principal do modelo, bem como os itens disponíveis para adição. A seguir estão todos os itens possíveis que você pode adicionar:
   * Página inicial

     >[!TIP]
     >
     >Por padrão, o ícone Início no Menu principal exibe a área Minhas atualizações para usuários com licença de revisão (no plano de licença atual), a menos que eles tenham um modelo de layout associado ao seu perfil que inclua a área Minhas atualizações no Menu principal, além da área Início.

   * Prioridades
   * Portfólios
   * Programas
   * Projetos
   * Relatórios
   * Painéis
   * Calendários
   * Recursos
   * Cenários

     >[!NOTE]
     >
     >O planejador de cenários requer uma licença adicional. Para obter informações sobre o planejador de cenários do Workfront, consulte [Visão geral do planejador de cenários](../../../scenario-planner/scenario-planner-overview.md).

   * Equipes
   * Usuários

     >[!NOTE]
     >
     >Somente os usuários com uma licença de Plano (no modelo de licença atual) ou os usuários com uma licença Padrão (no novo modelo de licença) podem ver o ![ícone Usuários](assets/users-icon-in-main-menu.png) da área Usuários no Menu Principal.

   * Solicitações
   * Planilhas de horas
   * Documentos
   * Modelos
   * Metas

     >[!NOTE]
     >
     >As metas exigem uma licença adicional. Para obter informações sobre as Metas do Workfront, consulte [Visão geral das Metas do Adobe Workfront](../../../workfront-goals/goal-management/wf-goals-overview.md).

   * Minhas atualizações
   * Quadros
   * Blueprints
   * Em Planejamento

     >[!NOTE]
     >
     >O Planning exige uma licença adicional. Para obter informações sobre o Workfront Planning, consulte [Introdução ao Adobe Workfront Planning](/help/quicksilver/planning/general/planning-overview.md).

   * Aplicativo personalizado

     >[!NOTE]
     >
     > Os aplicativos personalizados devem ser criados separadamente antes de serem disponibilizados como opções do Menu principal. Para obter mais informações, consulte [Criar um aplicativo personalizado para o Workfront com o Adobe App Builder](/help/quicksilver/app-builder/app-builder.md).

<div class="preview">

No ambiente de Pré-visualização:

1. Siga qualquer um destes procedimentos para os itens **Nativos**:

   * Ocultar ![Ícone Ocultar](assets/remove-icon---x-in-circle.png) itens que você não deseja exibir no Menu Principal.
   * Mostrar ![ícone Mostrar](assets/add-icon-plus-in-circle.png) itens que você deseja exibir no Menu Principal.
   * Arraste ![ícone Arrastar](assets/move-icon---dots.png) itens para alterar sua ordem de exibição no Menu Principal.

1. Siga um destes procedimentos para os itens do **Sistema**:

   * Ocultar ![Ícone Ocultar](assets/remove-icon---x-in-circle.png) itens que você não deseja exibir no Menu Principal.
   * Mostrar ![ícone Mostrar](assets/add-icon-plus-in-circle.png) itens que você deseja exibir no Menu Principal.

</div>

>[!NOTE]
>
><span class="preview">Não é possível alterar a ordem dos itens do sistema. Esses itens sempre são exibidos na parte inferior do Menu Principal quando estão ativos.</span>

1. No ambiente de Produção, execute um dos procedimentos a seguir:

   * Ocultar ![Ícone Ocultar](assets/remove-icon---x-in-circle.png) **Itens ativos** que você não deseja exibir
   * Mostrar ![ícone Mostrar](assets/add-icon-plus-in-circle.png) **Itens disponíveis** que você deseja exibir no Menu Principal.
   * Arraste ![ícone Arrastar](assets/move-icon---dots.png) **Itens ativos** para alterar sua ordem de exibição no Menu Principal.

1. Clique em **Concluído**.

   Você também pode clicar em **Cancelar** a qualquer momento se desejar descartar as alterações.

1. Continue personalizando o modelo de layout. Você pode clicar em **Aplicar** a qualquer momento para salvar seu progresso.

   Ou

   Se tiver terminado de personalizar, clique em **Salvar e Fechar**.

Para obter mais informações sobre modelos de layout, consulte [Criar e gerenciar modelos de layout](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
