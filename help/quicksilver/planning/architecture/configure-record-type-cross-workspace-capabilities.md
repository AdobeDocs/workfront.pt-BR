---
title: Configurar Recursos entre Espaços de Trabalho para o Tipo de Registro
description: Você pode habilitar um tipo de registro para ser adicionado a outro espaço de trabalho ou ser conectado de outro espaço de trabalho.
hidefromtoc: true
hide: true
exl-id: d36ab9fb-0275-483d-97be-0a88e170f8e0
source-git-commit: ff5bc262a5ed2a22099c058ebdb61bc32485b201
workflow-type: tm+mt
source-wordcount: '1134'
ht-degree: 1%

---

<!-- add these to the metadata, when making this public: 

feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog

-->

<!--*******************THIS TITLE MIGHT NEED TO CHANGE WHEN WE HAVE THE FINAL NAME FOR THE "GLOBAL" RECORD TYPE - NOT SURE IF WE ARE GOING TO USE "GLOBAL" OR "DYNAMIC", OR ???? ***************; also update TOC file, the miniTOC,  etc when this is finalized-->



<!--this article is linked to the UI - do not delete or change the URL-->
<!--add more info here about permissions, how users gain permissions from the original record type, per Lilit: users who add this to another space gain View permissions on that space when they add records to this added record type - this info is in the UI - this is what she sent in figma:

Hey, Alina, Lusine. As this page contains not only the "global record types" but also cross-workspace connectivity setting, we shouldn't have this message that's highlighting only the global rt features. I think we should have explanation for each setting both in enabled and disabled states. 

So we'd have the "Allow adding this record type to other workspaces" setting in enabled or disabled state, and display an explanation text below it explaining the capability, as well as a link to help articles for more context. I'd like to include the following key points in the message:  

Once enabled, this record type can be added in other workspaces by designated people 

Members of those workspaces can create and manage records in scope of their workspace 

Any records added by other workspace members will be rolled up to this workspace with view access so members of the current workspace can create views for cross-workspace records.  

Then for the second setting for cross-workspace connections, we'll need a similar explanation text would highlight that the other workspaces can create connections and gain view access to the records in this record type, but will not see the record type in their workspace. (not sure what she means by this last bit, asking in figma also)

-->

# Configurar recursos entre espaços de trabalho para tipos de registro

<!--this is linked to the UI in the info icon when you enable a record to be either centralized or connectable-->

<span class="preview">As informações nesta página se referem a funcionalidades que ainda não estão disponíveis. Ela está disponível somente no ambiente de Pré-visualização para todos os clientes. Depois das versões mensais para produção, os mesmos recursos também ficam disponíveis no ambiente de produção para clientes que ativaram versões rápidas. </span>

<span class="preview">Para obter informações sobre versões rápidas, consulte [Habilitar ou desabilitar versões rápidas para sua organização](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

A seguir estão os recursos entre espaços de trabalho dos tipos de registro:

* Você pode designar um tipo de registro como centralizado. Os usuários podem adicionar tipos de registro centralizados a outros espaços de trabalho que eles podem gerenciar.
* Você pode designar um tipo de registro como conectável. Os usuários podem se conectar a esse tipo de registro a partir de outros espaços de trabalho.

Primeiro, você deve definir os recursos entre espaços de trabalho de um tipo de registro para que os gerentes de espaços de trabalho possam conectá-lo ou adicioná-lo a outros espaços de trabalho.

Você define os recursos entre espaços de trabalho de um tipo de registro ao criar ou editar um tipo de registro.

Para obter informações, consulte um dos seguintes artigos:

* [Criar tipos de registro](/help/quicksilver/planning/architecture/create-record-types.md)
* [Editar tipos de registro](/help/quicksilver/planning/architecture/edit-record-types.md)

## Requisitos de acesso

+++ Expanda para exibir os requisitos de acesso para a funcionalidade neste artigo.

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr>

</tr>   
<tr> 
   <td role="rowheader"><p>Pacote do Adobe Workfront</p></td> 
   <td> 
<ul><li><p>Qualquer pacote do Workfront</p></li>
E
<li><p>Pacote do Planning Plus</p></li></ul>
Ou:
<ul><li><p>Qualquer pacote de fluxo de trabalho</p> </li>
E
<li><p>Planejamento do pacote Prime ou Ultimate</p></li></ul>
<p>Para obter mais informações sobre o que está incluído em cada plano do Workfront Planning, entre em contato com seu gerente de conta da Workfront. </p> 
   </td>

<tr> 
   <td role="rowheader"><p>Licença do Adobe Workfront</p></td> 
   <td><p>Standard</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Permissões de objeto</p></td> 
   <td>   <p>Gerenciar permissões para um espaço de trabalho</a> </p>  
   <p>Os administradores do sistema têm permissões para todos os espaços de trabalho, incluindo aqueles que não criaram</p>  </td> 
  </tr>  
</tbody> 
</table>

Para obter mais informações sobre requisitos de acesso do Workfront, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++   

## Configurar tipos de registros centralizados

<!--this is a UI term; don't change the title of this section-->
<!--IMPORTANT: not sure if we can call these centralized yet - checking with Lilit as of Sept 2; you might need to revert this to what the screen shot shows below?????-->

Como gerenciador de espaço de trabalho, você pode configurar um tipo de registro para ser um tipo de registro centralizado. Um tipo de registro centralizado pode ser adicionado a outros espaços de trabalho.

Um gerenciador de espaço de trabalho pode adicionar um tipo de registro centralizado a um espaço de trabalho gerenciado por ele. Os campos originais do tipo de registro também são adicionados.

Os usuários podem adicionar registros a um tipo de registro centralizado a partir de qualquer espaço de trabalho ao qual tenham permissões do Contribute e ao qual o tipo de registro centralizado seja adicionado, incluindo seu espaço de trabalho original. Eles podem exibir registros do espaço de trabalho para o qual têm somente permissões de Exibição.

Para obter mais informações, consulte [Visão geral dos tipos de registro entre espaços de trabalho](/help/quicksilver/planning/architecture/cross-workspace-record-types-overview.md)

Para configurar a adição de um tipo de registro como um tipo de registro centralizado:

{{step1-to-planning}}

1. Clique no espaço de trabalho cujos tipos de registro você deseja editar.

   A página do espaço de trabalho é aberta e os tipos de registro são exibidos.
1. Siga um destes procedimentos:

   * Passe o mouse sobre o cartão de um tipo de registro e clique no menu **Mais** ![Mais menu](assets/more-menu.png) no canto superior direito do cartão de tipo de registro
Ou
   * Clique em um cartão de tipo de registro para abrir a página de tipo de registro e clique no menu **Mais** ![Mais menu](assets/more-menu.png) à direita do nome do tipo de registro.
1. Clique em **Editar**.

   ![Mais opções de menu do cartão de tipo de registro](assets/more-menu-options-from-record-type-card.png)

   >[!TIP]
   >
   >Se um tipo de registro já tiver sido designado como um tipo de registro centralizado e ele tiver sido adicionado a outros espaços de trabalho, a opção Editar ficará esmaecida.

1. Na caixa **Editar tipo de registro**, selecione a guia **Configurações avançadas**.
1. Habilitar a configuração **Permitir a adição deste tipo de registro a outros espaços de trabalho**.

   ![Editar configurações avançadas do tipo de registro com Adicionar a outros espaços de trabalho habilita](assets/edit-record-type-advanced-settings-add-to-other-workspaces-enabled.png)

   >[!TIP]
   >
   >Após adicionar um tipo de registro centralizado a outro espaço de trabalho, essa configuração não poderá mais ser desativada.

1. No campo **Selecione quem pode adicionar este tipo de registro a espaços de trabalho que eles gerenciam**, adicione entidades que você deseja permitir para adicionar este tipo de registro a espaços de trabalho que eles gerenciam.

   Seu nome é adicionado automaticamente ao campo.

   É possível adicionar usuários individuais, ou grupos, equipes, funções de trabalho ou empresas cujos usuários você deseja permitir que adicionem esse tipo de registro aos espaços de trabalho que eles gerenciam.

   Você deve designar pelo menos uma entidade (usuário, equipe, grupo, função ou empresa) para habilitar essa configuração.

   É possível editar esse campo depois de salvar o tipo de registro.

1. (Opcional) Remova seu nome do campo **Selecione quem pode adicionar este tipo de registro ao espaço de trabalho que eles gerenciam**.

1. Clique em **Salvar**.

   As seguintes situações ocorrem:

   * O tipo de registro e seus campos agora estão disponíveis para serem adicionados a outro espaço de trabalho pelas pessoas designadas.

   >[!NOTE]
   >
   >É possível editar a aparência e as configurações do tipo de registro e seus campos originais somente a partir de seu espaço de trabalho original.

   * O cartão de tipo de registro exibe um ícone centralizado ![ícone de tipo de registro centralizado](assets/global-icon.png) para indicar que o tipo de registro está disponível para ser adicionado a outros espaços de trabalho.
   * Um campo **Workspace** gerado pelo sistema é adicionado à exibição de tabela do tipo de registro e seus detalhes de registros.

     O campo Workspace exibe o espaço de trabalho de onde cada registro é criado.

     Este campo é somente leitura e não pode ser excluído.
1. (Opcional) Vá para outro espaço de trabalho e crie um tipo de registro usando um tipo de registro existente. Selecione o tipo de registro que você ativou nas etapas acima.

   Para obter informações, consulte [Adicionar tipos de registro existentes de outro espaço de trabalho](/help/quicksilver/planning/architecture/add-existing-record-types-from-another-workspace.md).

## Configurar tipos de registro conectáveis

<!--this is a UI term; don't change the title of this section-->

É possível configurar um tipo de registro para ser conectado a partir de outros espaços de trabalho ao criar ou editar o tipo de registro.

Para configurar um tipo de registro para conexão a partir de outros espaços de trabalho ao editar o tipo de registro:

{{step1-to-planning}}

1. Clique no espaço de trabalho cujos tipos de registro você deseja editar.

   A página do espaço de trabalho é aberta e os tipos de registro são exibidos.
1. Siga um destes procedimentos:

   * Passe o mouse sobre o cartão de um tipo de registro e clique no menu **Mais** ![Mais menu](assets/more-menu.png) no canto superior direito do cartão de tipo de registro e clique em **Editar**
Ou
   * Clique em um cartão de tipo de registro para abrir a página de tipo de registro, clique no menu **Mais** ![Mais menu](assets/more-menu.png) à direita do nome do tipo de registro e clique em **Editar**.

   ![Mais opções de menu do cartão de tipo de registro](assets/more-menu-options-from-record-type-card.png)

1. Na caixa **Editar tipo de registro**, selecione a guia **Configurações avançadas**.
1. Habilitar a configuração **Permitir conexão com este tipo de registro em outros espaços de trabalho**. <!-- check the setting name, I sent this to Lilit to say FROM instead of IN-->

   ![Editar a guia Configurações avançadas do tipo de registro com conexão de outros espaços de trabalho habilitada](assets/edit-record-type-advanced-settings-connect-from-other-workspaces-enabled.png)

   Quando ativado, o tipo de registro é acessível e pode ser conectado a partir de outros espaços de trabalho.

1. Escolha a partir de quais espaços de trabalho o tipo de registro pode ser acessado. Escolha entre as seguintes opções:

   * **Em todo o sistema**: os usuários podem se conectar a este tipo de registro de todos os espaços de trabalho onde têm permissões de Gerenciamento.
   * **Espaços de trabalho específicos**: adicione os nomes dos espaços de trabalho nos quais os gerentes de espaço de trabalho podem se conectar a este tipo de registro.
1. Clique em **Salvar**.

   As seguintes situações ocorrem:

   * O tipo de registro e seus campos agora estão disponíveis para conexão a partir dos espaços de trabalho designados.
   * O cartão de tipo de registro exibe um ícone de conexão entre espaços de trabalho ![ícone de conexão entre espaços de trabalho](assets/connect-from-other-workspaces-icon.png) para indicar que o tipo de registro está disponível para conexão a partir de qualquer espaço de trabalho designado na sua configuração.

   O tipo de registro fica disponível para conexão a partir dos espaços de trabalho designados.
1. (Opcional) Vá para outro espaço de trabalho e adicione uma conexão ao tipo de registro que você ativou para conectividade entre espaços de trabalho nas etapas acima.

   Para obter informações, consulte [Tipos de registro de conexão](/help/quicksilver/planning/architecture/connect-record-types.md).









