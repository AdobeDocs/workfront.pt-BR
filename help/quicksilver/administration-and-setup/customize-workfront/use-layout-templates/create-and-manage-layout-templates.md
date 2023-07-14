---
title: Criar e gerenciar modelos de layout
user-type: administrator
content-type: overview
product-area: system-administration;templates
navigation-topic: layout-templates
description: Como administrador do Workfront ou administrador de grupo, você pode criar e modificar modelos de layout para personalizar elementos de layout no Workfront para seus usuários.
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: 53076920-3b13-4b65-85cb-38096cf2d04d
source-git-commit: 7ee96045e5673c51c3ce348f395226857686a923
workflow-type: tm+mt
source-wordcount: '602'
ht-degree: 0%

---

# Criar e gerenciar modelos de layout

<!--
**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.
-->

Como administrador do Workfront ou administrador de grupo, você pode criar e modificar modelos de layout para personalizar os seguintes elementos de layout no Workfront para seus usuários:

* Menu principal
* Painel de navegação esquerdo
* Área inicial
* Visualizações, filtros e agrupamentos que as pessoas usam com listas e relatórios.
* Terminologia na tela

Depois de criar ou modificar um modelo de layout, você pode atribuí-lo a usuários individuais, equipes, grupos ou funções de trabalho.

O layout padrão do Workfront de cada usuário depende do nível de acesso e do tipo de licença. Por exemplo, alguns usuários podem não ver algumas áreas no menu principal. Para obter mais informações, consulte [Sobre o layout padrão do Adobe Workfront](../../../administration-and-setup/customize-workfront/use-layout-templates/about-the-default-wf-layout.md).

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront</td> 
   <td>Qualquer Um</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td>Plano</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Para executar essas etapas no nível do sistema, você precisa do nível de acesso Administrador do sistema.
Para executá-las para um grupo, você deve ser um gerente desse grupo.</p> <p><b>NOTA</b>: se você ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Considerações para a criação e o gerenciamento de modelos de layout

* Os usuários podem personalizar algumas áreas de seu próprio layout. Ao alterar um modelo de layout, as alterações são mescladas com qualquer personalização feita, sem substituí-las ou redefini-las. Isso também é verdadeiro se você atribuir usuários a um novo modelo de layout.
* Os modelos de layout mais antigos criados no Adobe Workfront Classic estão automaticamente disponíveis na sua instância da nova experiência do Adobe Workfront desde que foram migrados no início do último trimestre de 2019. Após esse período, os modelos de layout criados no Adobe Workfront Classic foram migrados em abril de 2020. Recomendamos que você atualize esses modelos de layout na nova experiência do Adobe Workfront para aproveitar os novos recursos e torná-los ainda mais úteis nesse ambiente.
* Administradores de grupo e usuários com uma licença de plano que podem editar outros usuários podem adicionar modelos de layout em nível de sistema e em nível de grupo aos usuários que eles podem gerenciar ao editar seus perfis.
* Os administradores de grupo não podem atribuir modelos de layout a funções de trabalho ou equipes.

Para obter mais informações sobre modelos de layout, consulte [Modelos de layout](../../../administration-and-setup/customize-workfront/use-layout-templates/use-layout-templates-customize-ui.md).

## Criar ou modificar um modelo de layout

1. Clique em **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront e clique em **Configuração** ![](assets/gear-icon-settings.png).

1. No painel esquerdo, clique em **Interface** > **Modelos de layout**.

1. Clique em **Novo modelo de layout**.

   Ou

   Clique no nome do modelo de layout que deseja modificar.

1. Se você estiver criando um novo modelo de layout, digite um **Nome do modelo de layout** e (opcional) uma **Descrição** para ele.

1. Personalize áreas da interface do usuário, conforme descrito nos seguintes artigos:

   * [Personalizar o menu principal usando um modelo de layout](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md)
   * [Personalizar o painel esquerdo usando um modelo de layout](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-left-panel.md)
   * [Personalizar páginas fixadas usando um modelo de layout](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-pinned-pages.md)
   * [Personalizar a exibição de Detalhes usando um modelo de layout](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md)
   * [Personalizar Início e Resumo usando um modelo de layout](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-home-summary-layout-template.md)
   * [Personalizar a página de aterrissagem usando um modelo de layout](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-landing-page.md)
   * [Personalizar filtros, visualizações e agrupamentos usando um modelo de layout](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)
   * [Personalizar a terminologia da interface de usuário usando um modelo de layout](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-terminology.md)

1. Continue testando seu modelo de layout e disponibilizando-o para os usuários conforme descrito nos artigos abaixo:

   * [Teste de um novo modelo de layout](../../../administration-and-setup/customize-workfront/use-layout-templates/test-a-layout-template.md)
   * [Conceder acesso administrativo a um modelo de layout](../../../administration-and-setup/customize-workfront/use-layout-templates/grant-admin-access-layout-template.md)
   * [Atribuir usuários a um modelo de layout](../../../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md)

Você também pode criar um novo modelo de layout copiando-o e alterando a cópia. Para obter mais informações, consulte [Copiar um modelo de layout](../../../administration-and-setup/customize-workfront/use-layout-templates/copy-a-layout-template.md).
