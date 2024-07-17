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
source-git-commit: e896d156854c6729e5ea0a82dcbc641fbfa9415e
workflow-type: tm+mt
source-wordcount: '532'
ht-degree: 0%

---

# Criar e gerenciar modelos de layout

<!--Audited: 12/2023-->

<!--
**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.
-->

Como administrador do Adobe Workfront ou administrador de grupo, você pode criar e modificar modelos de layout para personalizar os seguintes elementos de layout no Workfront para seus usuários:

* Menu principal
* Painel de navegação esquerdo
* Área inicial
* Visualizações, filtros e agrupamentos que as pessoas usam com listas e relatórios.
* Terminologia na tela
* Cabeçalhos de projeto, tarefa e problema

Depois de criar ou modificar um modelo de layout, você pode atribuí-lo a usuários individuais, equipes, grupos ou funções de trabalho.

O layout padrão do Workfront de cada usuário depende do nível de acesso e do tipo de licença. Por exemplo, alguns usuários podem não ver algumas áreas no menu principal. Para obter mais informações, consulte [Sobre o layout padrão do Adobe Workfront](../../../administration-and-setup/customize-workfront/use-layout-templates/about-the-default-wf-layout.md).

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
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td><p>Novo: Padrão</p>
   Ou
   <p>Atual: Plano</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Para executar essas etapas no nível do sistema, você precisa do nível de acesso Administrador do sistema.</p>
<p>Para executá-las para um grupo, você deve ser um gerente desse grupo.</p> <p><b>NOTA</b>:</p> <p>Se você não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso.

Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td>
</tr> 
 </tbody> 
</table>

+++

## Considerações para a criação e o gerenciamento de modelos de layout

* Os usuários podem personalizar algumas áreas de seu próprio layout. Ao alterar um modelo de layout, as alterações são mescladas com qualquer personalização feita, sem substituí-las ou redefini-las. Isso também é verdadeiro se você atribuir usuários a um novo modelo de layout.
* Administradores de grupo e usuários com uma licença de plano que podem editar outros usuários podem adicionar modelos de layout em nível de sistema e em nível de grupo aos usuários que eles podem gerenciar ao editar seus perfis.
* Os administradores de grupo não podem atribuir modelos de layout a funções de trabalho ou equipes.

Para obter mais informações sobre modelos de layout, consulte [Modelos de layout](../../../administration-and-setup/customize-workfront/use-layout-templates/use-layout-templates-customize-ui.md).

<!--removed this from above, but keeping it for a bit, in case it will be needed - known issue around old templates still visible at time:
* Your older layout templates created in Adobe Workfront Classic have been automatically available in your instance of the new Adobe Workfront experience since they were migrated in early Fall 2019. Layout templates created in Adobe Workfront Classic after that time were migrated in April 2020. We recommend that you update these layout templates in the new Adobe Workfront experience to take advantage of new functionality and to make them even more useful in that environment.
-->

## Criar ou modificar um modelo de layout

{{step-1-to-setup}}

1. No painel esquerdo, clique em **Interface** > **Modelos de layout**.

1. Clique em **Novo Modelo de Layout**.

   Ou

   Clique no nome do modelo de layout que deseja modificar.

1. Se você estiver criando um novo modelo de layout, digite um **Nome do modelo de layout** e (opcional) uma **Descrição** para ele.

1. Personalize áreas da interface do usuário, conforme descrito nos seguintes artigos:

   * [Personalizar o Menu Principal usando um modelo de layout](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md)
   * [Personalizar o painel esquerdo usando um modelo de layout](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-left-panel.md)
   * [Personalizar páginas fixadas usando um modelo de layout](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-pinned-pages.md)
   * [Personalizar o modo de exibição de Detalhes usando um modelo de layout](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md)
   * [Personalizar Início e Resumo usando um modelo de layout](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-home-summary-layout-template.md)
   * [Personalizar a página de aterrissagem usando um modelo de layout](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-landing-page.md)
   * [Personalizar Filtros, Modos de Exibição e Agrupamentos usando um modelo de layout](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)
   * [Personalizar a terminologia da interface de usuário usando um modelo de layout](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-terminology.md)

1. Continue a testar seu modelo de layout e disponibilize-o para os usuários conforme descrito nos artigos abaixo:

   * [Testando um novo modelo de layout](../../../administration-and-setup/customize-workfront/use-layout-templates/test-a-layout-template.md)
   * [Conceder acesso administrativo a um modelo de layout](../../../administration-and-setup/customize-workfront/use-layout-templates/grant-admin-access-layout-template.md)
   * [Atribuir usuários a um modelo de layout](../../../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md)

>[!TIP]
>
>Você também pode criar um modelo de layout copiando-o e alterando a cópia. Para obter mais informações, consulte [Copiar um modelo de layout](../../../administration-and-setup/customize-workfront/use-layout-templates/copy-a-layout-template.md).

