---
title: Editar tipos de registro
description: Você poderá editar os tipos de registro depois que eles forem salvos. Os tipos de registro são os tipos de objeto do Adobe Workfront Planning.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 7d6de742-9657-4286-968c-1fc78ebbb94e
source-git-commit: ded6db27fa3fba9195e2133134f60bcadb0f897a
workflow-type: tm+mt
source-wordcount: '628'
ht-degree: 1%

---

<!--update the metadata with real information when making this available in TOC and in the left nav
---
title: Edit record types
description: You can edit record types after they have been saved. Record types are the object types of Adobe Workfront Planning.
author: Alina
role: User
feature: Work Management 
topic: Architecture
hidefromtoc: yes
hide: yes
---

-->

# Editar tipos de registro

{{planning-important-intro}}

Os tipos de registro são os tipos de objeto do Adobe Workfront Planning. É possível editar a aparência dos tipos de registros criados por você ou por qualquer outra pessoa. Para obter informações sobre como criar tipos de registro do Workfront Planning, consulte [Criar tipos de registro](/help/quicksilver/planning/architecture/create-record-types.md).

## Requisitos de acesso

+++ Expanda para exibir os requisitos de acesso do Workfront Planning.

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Produto</p> </td>
   <td>
   <p> Adobe Workfront</p> <p>Para conectar tipos de registro do Adobe Workfront Planning com o Experience Manager Assets, você deve ter uma licença do Adobe Experience Manager Assets e a instância da Workfront de sua organização deve ser integrada à Adobe Business Platform ou à Adobe Admin Console.</p> </td>
  </tr>  
 <td role="rowheader"><p>contrato do Adobe Workfront</p></td>
   <td>
<p>Sua organização deve estar inscrita no estágio de acesso antecipado do Workfront Planning </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>plano do Adobe Workfront</p></td>
   <td>
<p>Qualquer</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Licença da Adobe Workfront*</p></td>
   <td>
   <p>Novo: Padrão</p>
   <p>Atual: Plano</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>Configurações de nível de acesso</p></td>
   <td> <p>Não há controles de nível de acesso para o Workfront Planning</p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Permissões</p></td>
   <td> <p>Gerenciar permissões para um espaço de trabalho</a> </p>  
   <p>Os administradores do sistema têm permissões para todos os espaços de trabalho, incluindo aqueles que não criaram</p>
   <p>Somente administradores do sistema podem habilitar tipos de registro para se conectar de outros espaços de trabalho</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Modelo de layout</p></td>
   <td> <p>O administrador do Workfront ou do grupo deve adicionar a área do Planning ao modelo de layout. Para obter informações, consulte <a href="/help/quicksilver/planning/access/access-overview.md">Visão geral sobre acesso</a>. </p>  
</td>
  </tr>

</tbody>
</table>

*Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Maybe enable this at GA - but Planning is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

## Editar tipos de registro

{{step1-to-planning}}

1. Clique no espaço de trabalho cujos tipos de registro você deseja editar,

   A página do espaço de trabalho é aberta e os tipos de registro são exibidos.
1. Siga um destes procedimentos:

   * Passe o mouse sobre o cartão de um tipo de registro e clique no menu **Mais** ![](assets/more-menu.png) no canto superior direito do cartão de tipo de registro e clique em **Editar**
Ou
   * Clique em um cartão de tipo de registro para abrir a página de tipo de registro, clique no menu **Mais** ![](assets/more-menu.png) à direita do nome do tipo de registro e clique em **Editar**.

   ![](assets/more-menu-options-from-record-type-card.png)

1. Na caixa **Editar tipo de registro**, a guia **Aparência** é aberta por padrão.

   ![](assets/edit-record-type-box-appearance-tab.png)

   Atualize as seguintes informações na guia **Aparência**:

   * Edite o nome do tipo de registro, se necessário. <!--did they add a field label for this?-->
   * **Descrição**: edite ou adicione uma descrição para o tipo de registro com mais informações sobre ele.
   * Editar a cor e a forma do ícone associado ao tipo de registro. Faça o seguinte:
      * Selecione uma cor para identificar o tipo de registro. Esta é a cor do ícone do tipo de registro.
      * Selecione um ícone na lista ou comece a digitar o nome de um ícone para descrever o que ele representa e, em seguida, selecione-o quando ele for exibido. Este é o ícone do tipo de registro. Um ícone de arquivo é selecionado por padrão.

1. (Condicional) Se você for um administrador do sistema, clique na guia **Configurações avançadas** na caixa **Editar tipo de registro**.

   ![](assets/edit-record-type-box-advanced-settings-tab.png)

1. (Condicional) Como administrador do sistema, atualize as seguintes informações na guia **Configurações avançadas**:

   * **Conectar de outros espaços de trabalho**: selecione esta opção para permitir que os usuários se conectem a este tipo de registro de outros espaços de trabalho. Essa opção é desmarcada por padrão.
   * **Nível do sistema**: selecione esta opção para permitir que os usuários se conectem a este registro de todos os espaços de trabalho do sistema.
   * **Espaços de trabalho específicos**: selecione esta opção para restringir os espaços de trabalho dos quais os usuários podem se conectar a este tipo de registro, expanda o menu suspenso e selecione os espaços de trabalho dos quais deseja que os usuários se conectem a este tipo de registro. Você pode começar a digitar o nome de um espaço de trabalho e selecioná-lo quando ele for exibido na lista.

1. Clique em **Salvar**.

   O cartão de tipo de registro no espaço de trabalho exibe um ícone de conectividade ![](assets/connect-from-other-workspaces-icon.png) no canto superior direito para indicar que o registro agora pode ser acessado de outros espaços de trabalho.

1. (Opcional) Clique no cartão de tipo de registro na área do espaço de trabalho para abrir a página do tipo de registro e, em seguida, renomeie o tipo de registro no cabeçalho.

1. (Opcional) Para editar outro tipo de registro, na página Tipo de registro, expanda a seta apontando para baixo à direita do nome de um tipo de registro, procure um tipo de registro e selecione-o quando ele for exibido na lista.

   ![](assets/record-type-drop-down-on-record-type-page-with-search-box.png)