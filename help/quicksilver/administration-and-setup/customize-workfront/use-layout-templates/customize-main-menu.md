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
source-git-commit: 7ee96045e5673c51c3ce348f395226857686a923
workflow-type: tm+mt
source-wordcount: '570'
ht-degree: 4%

---

# Personalizar o menu principal usando um modelo de layout

Como administrador do Adobe Workfront ou administrador de grupo, você pode usar um modelo de layout para configurar as opções que os usuários veem quando abrem o menu principal no Workfront:

![Opções do menu principal](assets/main-menu-with-blueprints-no-branding.png)

>[!NOTE]
>
>As opções do Menu principal que os usuários veem dependem do tipo de licença e das configurações definidas no nível de acesso. Alguns usuários que utilizarão este modelo de layout talvez não vejam todas as opções escolhidas aqui. Para obter mais informações, consulte [Como os níveis de acesso e as permissões funcionam juntos](../../../administration-and-setup/add-users/access-levels-and-object-permissions/how-access-levels-permissions-work-together.md) e [Acesso configurável à funcionalidade para cada tipo de objeto](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

Para obter informações sobre como criar modelos de layout, consulte [Criar e gerenciar modelos de layout](../use-layout-templates/create-and-manage-layout-templates.md).

Para obter informações sobre modelos de layout para grupos, consulte [Criar e modificar os modelos de layout de um grupo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

Após configurar um modelo de layout, você deve atribuí-lo aos usuários para que as alterações feitas fiquem visíveis para outros usuários. Para obter informações sobre como atribuir um modelo de layout aos usuários, consulte [Atribuir usuários a um modelo de layout](../use-layout-templates/assign-users-to-layout-template.md).

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>plano do Adobe Workfront</strong></td> 
   <td>Qualquer Um</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Licença do Adobe Workfront</strong></td> 
   <td>Plano</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurações de nível de acesso</strong></td> 
   <td> <p>Para executar essas etapas no nível do sistema, você precisa do nível de acesso Administrador do sistema.
Para executá-las para um grupo, você deve ser um gerente desse grupo.</p> <p><b>NOTA</b>: se você ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Personalizar o menu principal

1. Comece a trabalhar em um modelo de layout, conforme descrito em [Criar e gerenciar modelos de layout](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
1. Clique em **Definir menu principal** próximo ao canto superior direito.

   Na caixa Menu principal exibida, é possível ver os itens que estão ativos no momento no Menu principal do modelo, bem como os itens que estão disponíveis para adição. A seguir estão todos os itens possíveis que podem ser adicionados:

   * Página inicial

     >[!TIP]
     >
     >Por padrão, a Página inicial é exibida como Minhas atualizações para usuários com licença de revisão, a menos que eles tenham um modelo de layout associado ao perfil que inclui a área Minhas atualizações no Menu principal.

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
     >O Planejador de cenários está disponível somente na nova experiência do Adobe Workfront e requer uma licença adicional. Para obter informações sobre o Planejador de cenários do Workfront, consulte [A visão geral do Planejador de cenários](../../../scenario-planner/scenario-planner-overview.md).

   * Equipes
   * Usuários

     >[!NOTE]
     >
     >Somente os usuários com uma licença do Plano podem ver os Usuários ![](assets/users-icon-in-main-menu.png) no menu principal.

   * Solicitações
   * Folhas de horas
   * Documentos
   * Modelos
   * Análise
   * Prova
   * Metas

     >[!NOTE]
     >
     >Isso requer uma licença adicional. Para obter informações sobre o Workfront Goals, consulte [Visão geral dos objetivos do Adobe Workfront](../../../workfront-goals/goal-management/wf-goals-overview.md).

   * Minhas atualizações
   * Quadros
   * Blueprints

1. Siga um destes procedimentos:

   * Ocultar ![](assets/remove-icon---x-in-circle.png) **Itens ativos** que você não deseja exibir
   * Mostrar ![](assets/add-icon-plus-in-circle.png) **Itens disponíveis** que você deseja exibir no menu principal.
   * Arrastar ![](assets/move-icon---dots.png) **Itens ativos** para alterar a ordem de exibição no Menu principal.

1. Clique em **Concluído**.

   Você também pode clicar em **Cancelar** a qualquer momento se desejar descartar suas alterações.

1. Continue personalizando o modelo de layout.

   Ou

   Se tiver terminado de personalizar, clique em **Salvar**.

   >[!TIP]
   >
   >Você pode clicar em Salvar a qualquer momento para salvar seu progresso e, em seguida, continuar modificando o modelo posteriormente.

Para obter mais informações sobre modelos de layout, consulte [Criar e gerenciar modelos de layout](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
