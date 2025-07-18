---
title: Editar Tipos de Registro
description: Você poderá editar os tipos de registro depois que eles forem salvos. Os tipos de registro são os tipos de objeto do Adobe Workfront Planning.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 7d6de742-9657-4286-968c-1fc78ebbb94e
source-git-commit: 298c542afea902d9fc14ef6a4470c0bc1d9bd33c
workflow-type: tm+mt
source-wordcount: '633'
ht-degree: 2%

---


# Editar tipos de registro

<!--<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>
-->

{{planning-important-intro}}

Os tipos de registro são os tipos de objeto do Adobe Workfront Planning. É possível editar a aparência dos tipos de registros criados por você ou por qualquer outra pessoa. Para obter informações sobre como criar tipos de registro do Workfront Planning, consulte [Criar tipos de registro](/help/quicksilver/planning/architecture/create-record-types.md).

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso.

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Produtos</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Planejamento do Adobe Workfront<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>plano do Adobe Workfront*</p></td> 
   <td> 
<p>Qualquer um dos seguintes planos da Workfront:</p> 
<ul><li>Selecionar</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>O Workfront Planning não está disponível para planos herdados do Workfront</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Pacote de planejamento do Adobe Workfront*</p></td> 
   <td> 
<p>Qualquer </p> 
<p>Para obter mais informações sobre o que está incluído em cada plano do Workfront Planning, entre em contato com seu gerente de conta da Workfront. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>plataforma Adobe Workfront</p></td> 
   <td> 
<p>A instância da Workfront de sua organização deve ser integrada à Adobe Unified Experience para acessar o Workfront Planning.</p> 
<p>Para obter mais informações, consulte <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Experiência unificada da Adobe para Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Licença da Adobe Workfront*</p></td> 
   <td><p> Padrão </p>
   <p>O Workfront Planning não está disponível para licenças herdadas do Workfront</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Configuração do nível de acesso</p></td> 
   <td> <p>Não há controles de nível de acesso para o Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Permissões de objeto</p></td> 
   <td>   <p>Gerenciar permissões para um espaço de trabalho e tipo de registro </p>  
   <p>Os administradores do sistema têm permissões para todos os espaços de trabalho, incluindo aqueles que não criaram</p>
   <p>Somente administradores do sistema podem habilitar tipos de registro para se conectar de outros espaços de trabalho</p> </td> 
  </tr>

</tbody> 
</table>

*Para obter mais informações sobre requisitos de acesso do Workfront, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Editar tipos de registro

{{step1-to-planning}}

1. Clique no espaço de trabalho cujos tipos de registro você deseja editar,

   A página do espaço de trabalho é aberta e os tipos de registro são exibidos.
1. Siga um destes procedimentos:

   * Passe o mouse sobre o cartão de um tipo de registro e clique no menu **Mais** ![Mais menu](assets/more-menu.png) no canto superior direito do cartão de tipo de registro e clique em **Editar**
Ou
   * Clique em um cartão de tipo de registro para abrir a página de tipo de registro, clique no menu **Mais** ![Mais menu](assets/more-menu.png) à direita do nome do tipo de registro e clique em **Editar**.

   ![Mais opções de menu do cartão de tipo de registro](assets/more-menu-options-from-record-type-card.png)

1. Na caixa **Editar tipo de registro**, a guia **Aparência** é aberta por padrão.

   ![Guia de aparência da caixa Editar tipo de registro ](assets/edit-record-type-box-appearance-tab.png)

   Atualize as seguintes informações na guia **Aparência**:

   * Edite o nome do tipo de registro, se necessário. <!--did they add a field label for this?-->
   * **Descrição**: edite ou adicione uma descrição para o tipo de registro com mais informações sobre ele.
   * Editar a cor e a forma do ícone associado ao tipo de registro. Faça o seguinte:
      * Selecione uma cor para identificar o tipo de registro. Esta é a cor do ícone do tipo de registro.
      * Selecione um ícone na lista ou comece a digitar o nome de um ícone para descrever o que ele representa e, em seguida, selecione-o quando ele for exibido. Este é o ícone do tipo de registro. Um ícone de arquivo é selecionado por padrão.

   <!--old info: 
   1. (Conditional) If you are a system administrator, click the **Advanced settings** tab in the **Edit record type** box. 
      ![Edit record type box advanced settings tab](assets/edit-record-type-box-advanced-settings-tab.png)
   1. (Conditional) Update the following information in the **Advanced settings** tab: 
      * Enable the **Connect from other workspace** setting. When enabled, the record type is accessible and can be connected from other workspaces. 
      * Choose from which workspaces the record type can be accessed. Choose from the following options:
         * **System wide**: Users can connect to this record type from all workspaces where they have manage permissions. 
         * **Specific workspaces**: Add the names of the workspaces where workspace managers can connect to this record type.-->


1. (Opcional e condicional) Se você for um administrador do sistema, clique em **Configurações avançadas** e atualize as seguintes informações na seção **Recurso entre espaços de trabalho**: <!--the info here is duplicated in the Create record types article-->
   * Habilitar a configuração **Permitir conexão com este tipo de registro em outros espaços de trabalho**: isso permite que os gerentes de espaço de trabalho se conectem a este tipo de registro a partir de outros espaços de trabalho.\
     Você pode designar de quais espaços de trabalho esse tipo de registro pode ser conectado. Você pode disponibilizá-lo para todos os espaços de trabalho ou designar outros específicos para que possa importá-lo.
Para obter mais informações, consulte [Configurar recursos entre espaços de trabalho para tipos de registro](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md).

   ![Guia de configurações avançadas da caixa Editar tipo de registro](assets/edit-record-type-box-advanced-settings-tab.png)

   <!--replace last point with this when we release dynamic record types:
      1. (Optional and conditional) If you are a system administrator, click **Advanced settings** and update the following information in the **Cross-workspace capability** section: **** the info here is duplicated in the Edit record types article ***
         * Enable the **Allow adding this record type to other workspaces** setting: This allows workspace managers to add this record type to other workspaces. 
               You can designate specific users who can add this record type to other workspaces. 
         * Enable the **Allow connecting to this record type in other workspaces** setting: This allows workspace managers to connect to this record type from other workspaces.  
               You can designate which workspaces this record type can be connected from. You can make it available for all workspaces or designate specific ones where you can import it.
         For more information, see [Configure cross-workspace capabilities for record types](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md).  
         ******** replace screen shot below **********
         ![Create record type box on advanced settings tab](assets/create-record-type-box-advanced-settings-tab.png) 
      -->

1. Clique em **Salvar**.

   O cartão de tipo de registro no espaço de trabalho exibe um ícone de conectividade ![Conectar-se de outros espaços de trabalho](assets/connect-from-other-workspaces-icon.png) no canto superior direito para indicar que o registro agora pode ser acessado de outros espaços de trabalho.

1. (Opcional) Clique no cartão de tipo de registro na área do espaço de trabalho para abrir a página do tipo de registro e, em seguida, renomeie o tipo de registro no cabeçalho.

1. (Opcional) Para editar outro tipo de registro, na página Tipo de registro, expanda a seta apontando para baixo à direita do nome de um tipo de registro, procure um tipo de registro e selecione-o quando ele for exibido na lista.

   ![Menu suspenso de tipo de registro na página de tipo de registro com caixa de pesquisa](assets/record-type-drop-down-on-record-type-page-with-search-box.png)
