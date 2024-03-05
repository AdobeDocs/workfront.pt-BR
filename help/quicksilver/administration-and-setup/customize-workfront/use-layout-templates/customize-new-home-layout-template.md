---
title: Personalizar a nova página inicial usando um modelo de layout
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: Você pode usar um modelo de layout para configurar o que os usuários veem quando abrem uma nova página inicial.
author: Nolan
feature: System Setup and Administration
role: Admin
source-git-commit: 2551089a20d3301ff1cf7dd633114dbb5235e959
workflow-type: tm+mt
source-wordcount: '779'
ht-degree: 1%

---

# Personalizar a nova página inicial usando um modelo de layout

Você pode usar um modelo de layout para configurar o que os usuários veem quando abrem uma nova página inicial.

Você pode configurar:

* Quais widgets são exibidos no espaço de trabalho por padrão e seu layout na página
* Qual plano de fundo está selecionado
* Configurações específicas do widget, incluindo quais filtros e grupos estão disponíveis para os widgets Meus projetos, Minhas tarefas e Meus problemas, bem como seus padrões

>[!IMPORTANT]
>
>As opções do modelo de layout do administrador descritas nesta página substituem as opções de personalização de usuários individuais.
>
>Quando as alterações em um modelo de layout forem salvas, os usuários desse modelo de layout terão sua nova página inicial alterada para corresponder ao modelo de layout. As seleções de widget existentes serão enviadas para a parte inferior da página. Embora os widgets selecionados pelo administrador possam ser reposicionados e redimensionados por um usuário, eles não podem ser removidos.

Para obter informações sobre a nova Página inicial, consulte [Introdução à nova página inicial](/help/quicksilver/workfront-basics/using-home/new-home/get-started-with-new-home.md).

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
   <td role="rowheader">plano do Adobe Workfront</td> 
   <td>Qualquer</td> 
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

## Personalizar a nova página inicial usando um modelo de layout

1. Comece a trabalhar em um modelo de layout, conforme descrito em [Criar e gerenciar modelos de layout](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

1. Clique na seta para baixo ![](assets/dropdown-arrow.png) em **Personalize o que os usuários veem** e, em seguida, clique em **Espaço de trabalho inicial**.

1. Nas guias exibidas à direita, clique em **Design e layout** para escolher e organizar widgets e o fundo, ou **Configurações do widget** para gerenciar configurações de widgets individuais, como filtros e grupos disponíveis.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Design e layout</td> 
      <td>
      <p>Selecione quais widgets estarão presentes nos espaços de trabalho dos usuários, suas posições e escolha um plano de fundo. Observe que, embora os usuários não possam remover os widgets selecionados, eles podem movê-los e redimensioná-los livremente, bem como adicionar widgets adicionais.</p>
      <p>Essa guia funciona essencialmente como um pequeno espaço de trabalho novo da Página inicial; dessa forma, ela pode ser personalizada de acordo com as etapas descritas em <a href="/help/quicksilver/workfront-basics/using-home/new-home/add-edit-remove-widgets-in-new-home.md" class="MCXref xref">Adicionar, editar ou remover widgets em nova Página inicial</a>. Selecione widgets e organize o espaço de trabalho da maneira que você desejar que ele seja exibido para os usuários.</p>
      <p>Para alterar o plano de fundo, siga as etapas em <b>Personalização de plano de fundo</b> in <a href="/help/quicksilver/workfront-basics/using-home/new-home/get-started-with-new-home.md" class="MCXref xref">Introdução à nova página inicial</a>.</p>
      <p>

>[!NOTE]
>
>Somente mover ou redimensionar widgets no Modelo de layout não fará com que as novas Home pages dos usuários atualizem seu layout. No entanto, adicionar ou remover um widget acionará uma atualização nas páginas dos usuários.

</p>
     </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Configurações do dispositivo</td> 
      <td>
      <p>Alterar configurações de widgets individuais. Atualmente, somente três widgets são suportados:</p>
      <ul>
        <li>Meus projetos</li>
        <li>Minhas tarefas</li>
        <li>Meus problemas</li>
      </ul>
      <p>Depois de selecionar o widget que deseja editar, as opções disponíveis serão exibidas à direita. Essas opções incluem <b>Filtros</b>, <b>Colunas</b>, e <b>Grupos</b>. Você pode:</p>
      <ul>
      <li><p><b>Selecione quais Filtros, Colunas ou Grupos estarão disponíveis para os usuários:</b></p>
      <p>Marque a caixa ao lado de todas as opções na lista que você deseja que os usuários possam usar. Opções desmarcadas não serão exibidas para usuários.</li></p>
      <li><p><b>Defina um Filtro ou Grupo padrão para o widget:</b></p>
      <p>Passe o mouse sobre uma opção e um botão aparecerá, permitindo que você defina essa opção como padrão para os usuários. O padrão atual terá um emblema Padrão azul à direita.</li></p>
      <li><p><b>Adicione um Filtro, Coluna ou Grupo existente à lista de opções disponíveis:</b></p>
      <p>Clique no botão de adição na parte inferior de cada lista para adicionar uma opção a ela. Observe que somente Filtros, Campos (para Colunas) ou Grupos existentes podem ser adicionados dessa maneira.</p></li>
      </ul>
      <p>

>[!NOTE]
>
>Se você definir um filtro ou agrupamento padrão para um widget específico usando um modelo de layout, ele pode não entrar em vigor imediatamente devido às preferências do usuário existentes. Para aplicar o novo filtro ou agrupamento imediatamente, você ou o usuário podem precisar redefinir suas preferências de usuário anexando &quot;/resetUser&quot; ao final de seu URL.

</p>
  </td> 
  </tr>
  </tbody> 
  </table>

1. Continue personalizando o modelo de layout.

   Ou

   Se tiver terminado de personalizar, clique em **Salvar** no canto inferior esquerdo.

