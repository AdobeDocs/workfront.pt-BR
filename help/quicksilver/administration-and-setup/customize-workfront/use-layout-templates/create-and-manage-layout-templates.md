---
title: Criar e gerenciar modelos de layout
user-type: administrator
content-type: overview
product-area: system-administration;templates
navigation-topic: layout-templates
description: Como administrador do Workfront ou administrador de grupo, você pode criar e modificar modelos de layout para personalizar elementos de layout no Workfront para seus usuários.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 53076920-3b13-4b65-85cb-38096cf2d04d
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: b9e0747a58618353caf3ce1c7e8521d22d2b412d
workflow-type: tm+mt
source-wordcount: '507'
ht-degree: 10%

---

# Criar e gerenciar modelos de layout

<!--Audited: 12/2023-->

<!--
**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.
-->

{{highlighted-preview}}

Como administrador do Adobe Workfront ou administrador de grupo, você pode criar e modificar modelos de layout para personalizar os seguintes elementos de layout no Workfront para seus usuários:

* Menu principal
* Painel de navegação esquerdo
* Área inicial
* Painel de resumo
* Visualizações, filtros e agrupamentos que as pessoas usam com listas e relatórios.
* Terminologia na tela
* <span class="preview">Cabeçalhos de objetos</span>
* <span class="preview">Menu Mais (menu de três pontos) para um objeto</span>

Depois de criar ou modificar um modelo de layout, você pode atribuí-lo a usuários individuais, equipes, grupos ou funções de trabalho.

O layout padrão do Workfront de cada usuário depende do nível de acesso e do tipo de licença. Por exemplo, alguns usuários podem não ver algumas áreas no menu principal. Para obter mais informações, consulte [Sobre o layout padrão do Adobe Workfront](../../../administration-and-setup/customize-workfront/use-layout-templates/about-the-default-wf-layout.md).

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo.

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

## Considerações para a criação e o gerenciamento de modelos de layout

* Os usuários podem personalizar algumas áreas de seu próprio layout. Ao alterar um modelo de layout, as alterações são mescladas com qualquer personalização feita, sem substituí-las ou redefini-las. Isso também é verdadeiro se você atribuir usuários a um novo modelo de layout.
* Administradores de grupo e usuários com uma licença de plano que podem editar outros usuários podem adicionar modelos de layout em nível de sistema e em nível de grupo aos usuários que eles podem gerenciar ao editar seus perfis.
* Os administradores de grupo não podem atribuir modelos de layout a funções de trabalho ou equipes.

Para obter mais informações sobre modelos de layout, consulte [Modelos de layout](../../../administration-and-setup/customize-workfront/use-layout-templates/use-layout-templates-customize-ui.md).

## Criar ou modificar um modelo de layout

{{step-1-to-setup}}

1. No painel esquerdo, clique em **Interface** > **Modelos de layout**.

1. Clique em **Novo Modelo de Layout**.

   Ou

   Clique no nome do modelo de layout que deseja modificar.

1. Se você estiver criando um novo modelo de layout, digite um **Nome do modelo de layout** e (opcional) uma **Descrição** para ele.

1. Personalize áreas da interface do usuário, conforme descrito nos seguintes artigos:

   * [Personalizar o menu principal usando um modelo de layout](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md)
   * [Personalizar o painel esquerdo usando um modelo de layout](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-left-panel.md)
   * [Personalizar o menu Mais usando um modelo de layout](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-more-menu.md)
   * [Personalizar páginas fixadas usando um modelo de layout](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-pinned-pages.md)
   * [Personalizar a exibição de Detalhes usando um modelo de layout](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md)
   * [Personalizar o painel Resumo usando um modelo de layout](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-home-summary-layout-template.md)
   * [Personalizar página inicial usando um modelo de layout](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-new-home-layout-template.md)
   * [Personalizar a página de aterrissagem usando um modelo de layout](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-landing-page.md)
   * [Personalizar filtros, visualizações e agrupamentos usando um modelo de layout](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)
   * [Personalizar a terminologia da interface de usuário usando um modelo de layout](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-terminology.md)

1. Continue a testar seu modelo de layout e disponibilize-o para os usuários conforme descrito nos artigos abaixo:

   * [Testar um novo modelo de layout](../../../administration-and-setup/customize-workfront/use-layout-templates/test-a-layout-template.md)
   * [Conceder acesso administrativo a um modelo de layout](../../../administration-and-setup/customize-workfront/use-layout-templates/grant-admin-access-layout-template.md)
   * [Atribuir usuários a um modelo de layout](../../../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md)

>[!TIP]
>
>Você também pode criar um modelo de layout copiando-o e alterando a versão copiada. Para obter mais informações, consulte [Copiar um modelo de layout](../../../administration-and-setup/customize-workfront/use-layout-templates/copy-a-layout-template.md).

