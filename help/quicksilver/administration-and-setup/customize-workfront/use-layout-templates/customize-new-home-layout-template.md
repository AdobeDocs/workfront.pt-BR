---
title: Personalizar nova página inicial usando um modelo de layout
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: Você pode usar um Modelo de layout para configurar o que os usuários veem quando abrem a Página inicial.
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: b9997e79-a893-49dd-8c90-290399b2d2f7
source-git-commit: 0a19683e2311b1acc57423f5cb5a7dd141c8b79c
workflow-type: tm+mt
source-wordcount: '841'
ht-degree: 1%

---

# Personalizar página inicial usando um modelo de layout

Você pode usar um Modelo de layout para configurar o que os usuários veem quando abrem a Página inicial pela primeira vez.

Você pode configurar:

* Quais widgets são exibidos no espaço de trabalho por padrão
* Qual plano de fundo está selecionado
* Configurações específicas do widget, incluindo quais filtros e grupos estão disponíveis para os widgets Meus projetos, Minhas tarefas e Meus problemas, bem como seus padrões

>[!IMPORTANT]
>
>Os usuários finais podem alterar seu plano de fundo e reordenar widgets na página após a aplicação do Modelo de layout. Eles não podem remover widgets incluídos por um Administrador do Workfront.
> <br>
>Os administradores têm a capacidade de adicionar novos widgets para os usuários. No entanto, se um usuário final já tiver personalizado a ordem do widget ou a seleção do plano de fundo, essas personalizações específicas não serão alteradas.



Para obter informações sobre a página inicial, consulte [Introdução à Página Inicial](/help/quicksilver/workfront-basics/using-home/using-the-home-area/get-started-with-home.md).

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
   <td role="rowheader">plano do Adobe Workfront</td> 
   <td>Qualquer</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td><p>Novo: Padrão</p>
  <p> Atual: Plano</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Para executar essas etapas no nível do sistema, você precisa do nível de acesso Administrador do sistema.
Para executá-las para um grupo, você deve ser um gerente desse grupo.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Para obter mais informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Personalizar página inicial usando um modelo de layout

Para personalizar a Página inicial usando um modelo de layout:

1. Comece a trabalhar em um modelo de layout, conforme descrito em [Criar e gerenciar modelos de layout](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

1. Clique na seta para baixo ![](assets/dropdown-arrow.png) em **Personalize o que os usuários veem** e clique em **Workspace Residencial**.

1. Nas guias à direita, clique em **Design e layout** para escolher e organizar widgets e o plano de fundo, ou em **Configurações de widget** para gerenciar configurações de widgets individuais, como filtros e grupos disponíveis.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Design e layout</td> 
      <td>
      <p>Selecione quais widgets estarão presentes nos espaços de trabalho dos usuários, suas posições e escolha um plano de fundo. Observe que, embora os usuários não possam remover os widgets selecionados, eles podem movê-los e redimensioná-los livremente, bem como adicionar widgets adicionais.</p>
      <p>Esta guia funciona essencialmente como um pequeno espaço de trabalho na Página Inicial; dessa forma, ela pode ser personalizada de acordo com as etapas descritas em <a href="/help/quicksilver/workfront-basics/using-home/using-the-home-area/add-edit-remove-widgets-in-new-home.md" class="MCXref xref">Adicionar, editar ou remover widgets na Página Inicial</a>. Selecione widgets e organize o espaço de trabalho da maneira que você desejar que ele seja exibido para os usuários.</p>
      <p>Para alterar o plano de fundo, siga as etapas em <b>Personalização do plano de fundo</b> em <a href="/help/quicksilver/workfront-basics/using-home/using-the-home-area/get-started-with-home.md" class="MCXref xref">Introdução à Página Inicial</a>.</p>
      <p>

>[!NOTE]
>
>Somente mover ou redimensionar widgets no Modelo de layout não fará com que as Home pages dos usuários atualizem seu layout. No entanto, adicionar ou remover um widget acionará uma atualização nas páginas dos usuários.

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
      <p>Depois de selecionar o widget que deseja editar, as opções disponíveis serão exibidas à direita. Estas opções incluem <b>Filtros</b>, <b>Colunas</b> e <b>Grupos</b>. Você pode:</p>
      <ul>
      <li><p><b>Selecione e ordene Filtros, Colunas ou Grupos disponíveis para os usuários:</b></p>
      <p>Marque a caixa ao lado de todas as opções na lista que você deseja que os usuários possam usar. Essas opções não se estendem ao painel Resumo. Você deve configurar essa área na guia Resumo do Modelo de layout. Opções desmarcadas não serão exibidas para usuários. Arraste e solte opções na lista para definir uma ordem.</li></p>
      <p>

>[!IMPORTANT]
>
>* As opções Filtro, Colunas e Grupo são vinculadas às opções de personalização da lista no Modelo de layout. As alterações feitas aqui também serão aplicadas a essas configurações.
>* Os usuários devem ter pelo menos o acesso de Criação a Exibições para que a configuração da coluna do administrador seja aplicada corretamente a suas Páginas iniciais.

</p>
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

>[!IMPORTANT]
>
>Você deve atualizar a página inicial para ver as personalizações do Modelo de layout.
