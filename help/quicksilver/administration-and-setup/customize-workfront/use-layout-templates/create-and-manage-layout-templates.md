---
title: Criar e gerenciar modelos de layout
user-type: administrator
content-type: overview
product-area: system-administration;templates
navigation-topic: layout-templates
description: Como administrador do Workfront ou administrador de grupo, você pode criar e modificar modelos de layout para personalizar elementos de layout no Workfront para seus usuários.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 53076920-3b13-4b65-85cb-38096cf2d04d
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
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
* Exibições, filtros e agrupamentos que as pessoas usam com listas e relatórios.
* Terminologia na tela

Após criar ou modificar um modelo de layout, é possível atribuí-lo a usuários individuais, equipes, grupos ou funções de trabalho.

O layout padrão do Workfront de cada usuário depende do nível de acesso e do tipo de licença. Por exemplo, alguns usuários podem não ver algumas áreas no Menu principal. Para obter mais informações, consulte [Sobre o layout padrão do Adobe Workfront](../../../administration-and-setup/customize-workfront/use-layout-templates/about-the-default-wf-layout.md).

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
Para executá-los para um grupo, você deve ser um gerente desse grupo.</p> <p><b>OBSERVAÇÃO</b>: Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Considerações para a criação e o gerenciamento de modelos de layout

* Os usuários podem personalizar algumas áreas de seu próprio layout. Ao alterar um modelo de layout, suas alterações se mesclam com as personalizações feitas, sem substituí-las ou redefini-las. Isso também é verdadeiro se você atribuir usuários a um novo modelo de layout.
* Seus modelos de layout mais antigos criados no Adobe Workfront Classic foram automaticamente disponibilizados na sua instância da nova experiência do Adobe Workfront desde que foram migrados no início do último trimestre de 2019. Os modelos de layout criados no Adobe Workfront Classic após essa data foram migrados em abril de 2020. Recomendamos que você atualize esses modelos de layout na nova experiência do Adobe Workfront para aproveitar os novos recursos e torná-los ainda mais úteis nesse ambiente.
* Os administradores de grupo e usuários com uma licença de Plano que podem editar outros usuários podem adicionar modelos de layout de nível de sistema e de grupo aos usuários que podem gerenciar ao editar seu perfil.
* Os administradores de grupo não podem atribuir modelos de layout a funções ou equipes de trabalho.

Para obter mais informações sobre modelos de layout, consulte [Modelos de layout](../../../administration-and-setup/customize-workfront/use-layout-templates/use-layout-templates-customize-ui.md).

## Criar ou modificar um modelo de layout

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront, em seguida, clique em **Configuração** ![](assets/gear-icon-settings.png).

1. No painel esquerdo, clique em **Interface** > **Modelos de layout**.

1. Clique em **Novo modelo de layout**.

   Ou

   Clique no nome do template de layout que deseja modificar.

1. Se estiver criando um novo modelo de layout, digite um **Nome do modelo de layout** e (opcional) a **Descrição** para isso.

1. Personalize áreas da interface do usuário, conforme descrito nos seguintes artigos:

   * [Personalizar o Menu principal usando um modelo de layout](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md)
   * [Personalizar o painel esquerdo usando um modelo de layout](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-left-panel.md)
   * [Personalizar páginas fixas usando um modelo de layout](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-pinned-pages.md)
   * [Personalizar a visualização de Detalhes usando um modelo de layout](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md)
   * [Personalizar página inicial e resumo usando um modelo de layout](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-home-summary-layout-template.md)
   * [Personalizar a landing page usando um modelo de layout](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-landing-page.md)
   * [Personalizar filtros, exibições e agrupamentos usando um modelo de layout](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)
   * [Personalizar a terminologia da interface do usuário usando um modelo de layout](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-terminology.md)

1. Continue para testar seu modelo de layout e disponibilizá-lo aos usuários, conforme descrito nos artigos abaixo:

   * [Teste de um novo modelo de layout](../../../administration-and-setup/customize-workfront/use-layout-templates/test-a-layout-template.md)
   * [Conceder acesso administrativo a um modelo de layout](../../../administration-and-setup/customize-workfront/use-layout-templates/grant-admin-access-layout-template.md)
   * [Atribuir usuários a um modelo de layout](../../../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md)

Também é possível criar um novo modelo de layout copiando-o e alterando a cópia. Para obter mais informações, consulte [Copiar um modelo de layout](../../../administration-and-setup/customize-workfront/use-layout-templates/copy-a-layout-template.md).
