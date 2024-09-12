---
title: Personalizar o menu principal usando um modelo de layout
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: Como administrador do Adobe Workfront ou administrador de grupo, você pode usar um modelo de layout para configurar as opções que os usuários veem quando abrem o menu principal no Workfront.
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: d4f02102-0378-472f-9ebb-753502ec048b
source-git-commit: a79e4146ce6d076ef0e3707416a9c21d643b96e1
workflow-type: tm+mt
source-wordcount: '630'
ht-degree: 3%

---

# Personalizar o menu principal usando um modelo de layout

<!--Audited: 01/2024-->

Como administrador do Adobe Workfront ou administrador de grupo, você pode usar um modelo de layout para configurar as opções que os usuários veem quando abrem o menu principal no Workfront.

![Opções do menu principal](assets/main-menu-with-blueprints-no-branding.png)

>[!NOTE]
>
>As opções do Menu principal que os usuários veem dependem do tipo de licença e das configurações definidas no nível de acesso. Alguns usuários que utilizarão este modelo de layout talvez não vejam todas as opções escolhidas aqui. Para obter mais informações, consulte [Como os níveis de acesso e as permissões funcionam juntos](../../../administration-and-setup/add-users/access-levels-and-object-permissions/how-access-levels-permissions-work-together.md) e [Acesso configurável à funcionalidade para cada tipo de objeto](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).
>
>Você poderá ver diferentes opções no Menu principal se sua organização tiver sido integrada à Experiência unificada do Adobe Workfront. Para obter informações, consulte [Experiência unificada Adobe para Workfront](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md).

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
   <td role="rowheader"><strong>plano do Adobe Workfront</strong></td> 
   <td>Qualquer</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Licença da Adobe Workfront*</strong></td> 
   <td><p>Atual:Plano</p>
   Ou
   <p>Novo: Padrão</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configuração do nível de acesso</strong></td> 
   <td> <p>Para executar essas etapas no nível do sistema, você precisa do nível de acesso Administrador do sistema.</p>
    <p>Para executá-las para um grupo, você deve ser um gerente desse grupo.</p> 
     </td> 
  </tr> 
 </tbody> 
</table>

*Para obter mais informações sobre requisitos de acesso, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Personalizar o menu principal

1. Comece a trabalhar em um modelo de layout, conforme descrito em [Criar e gerenciar modelos de layout](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
1. Clique em **Definir menu principal** no canto superior direito do modelo.

   A caixa Menu principal é aberta e você pode ver as áreas exibidas atualmente no Menu principal do modelo, bem como os itens disponíveis para adição. A seguir estão todos os itens possíveis que você pode adicionar:
   * Início

     >[!TIP]
     >
     >Por padrão, o ícone Início no Menu principal exibe a área Minhas atualizações para usuários com licença de revisão (no plano de licença atual), a menos que eles tenham um modelo de layout associado ao seu perfil que inclua a área Minhas atualizações no Menu principal, além da área Início.

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
     >O Planejador de cenários requer uma licença adicional. Para obter informações sobre o Planejador de cenários do Workfront, consulte [A visão geral do Planejador de cenários](../../../scenario-planner/scenario-planner-overview.md).

   * Equipes
   * Usuários

     >[!NOTE]
     >
     >Somente os usuários com uma licença de Plano (no modelo de licença atual) ou os usuários com uma licença Padrão (no novo modelo de licença) podem ver a área de Usuários ![](assets/users-icon-in-main-menu.png) no Menu Principal.

   * Solicitações
   * Planilhas de horas
   * Documentos
   * Modelos
   * Análise
   * Prova
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
     >O Planning exige uma licença adicional. Para obter informações sobre o Workfront Planning, consulte [Visão geral do Adobe Workfront Planning](/help/quicksilver/planning/general/planning-overview.md)

1. Siga um destes procedimentos:

   * Ocultar ![](assets/remove-icon---x-in-circle.png) **itens ativos** que você não deseja exibir
   * Mostrar ![](assets/add-icon-plus-in-circle.png) **Itens disponíveis** que você deseja exibir no Menu Principal.
   * Arraste ![](assets/move-icon---dots.png) **Itens ativos** para alterar sua ordem de exibição no menu principal.

1. Clique em **Concluído**.

   Você também pode clicar em **Cancelar** a qualquer momento se desejar descartar as alterações.

1. Continue personalizando o modelo de layout.

   Ou

   Se tiver terminado de personalizar, clique em **Salvar**.

   >[!TIP]
   >
   >Você pode clicar em Salvar a qualquer momento para salvar seu progresso e, em seguida, continuar modificando o modelo posteriormente.

Para obter mais informações sobre modelos de layout, consulte [Criar e gerenciar modelos de layout](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
