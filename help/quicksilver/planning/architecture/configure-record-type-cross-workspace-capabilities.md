---
title: Configurar recursos entre espaços de trabalho para tipos de registro
description: Você pode ativar um tipo de registro para ser adicionado a outro espaço de trabalho ou estar conectado de outro espaço de trabalho no Adobe Workfront Planning.
hidefromtoc: true
hide: true
exl-id: d36ab9fb-0275-483d-97be-0a88e170f8e0
source-git-commit: 7d37481fc5b468f6f8ea1fce6ccd7ae064f00251
workflow-type: tm+mt
source-wordcount: '1329'
ht-degree: 0%

---

<!-- add these to the metadata, when making this public: 

feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog

-->

<!--*******************REPLACE THE "ADVANCED SETTINGS" SECTION IN THE "EDIT RECORD TYPES" ARTICLE WITH A LINK TO THIS ARTICLE INSTEAD AND REMOVE THE STEPS FROM THE "EDIT RECORD TYPES" ARTICLE ON HOW TO ALLOW CROSS-WORKSPACE SETTINGS FOR RECORD TYPES*************-->


<!--this article is linked to the UI - do not delete or change the URL-->

<!--THIS MIGHT ALREADY BE ADDED TO THE "OVERVIEW" ARTICLE, BUT CHECK: add more info here about permissions, how users gain permissions from the original record type, per Lilit: users who add this to another space gain View permissions on that space when they add records to this added record type.

-->

# Configurar recursos entre espaços de trabalho para tipos de registro

{{planning-important-intro}}

<!--this is linked to the UI in the info icon when you enable a record to be either global or connectable-->

<span class="preview">As informações nesta página se referem a funcionalidades que ainda não estão disponíveis. Ela está disponível somente no ambiente de Pré-visualização para todos os clientes. Depois das versões mensais para produção, os mesmos recursos também ficam disponíveis no ambiente de produção para clientes que ativaram versões rápidas. </span>

<span class="preview">Para obter informações sobre versões rápidas, consulte [Habilitar ou desabilitar versões rápidas para sua organização](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

Você pode configurar tipos de registro para trabalhar em vários espaços de trabalho no Adobe Workfront Planning.

Você pode designar um tipo de registro como um dos seguintes:

* **Um tipo de registro global**: os usuários podem adicionar tipos de registro global a outros espaços de trabalho que eles podem gerenciar.
* **Um tipo de registro conectável**: os usuários podem se conectar a este tipo de registro a partir de outros espaços de trabalho.

Primeiro, você deve definir os recursos entre espaços de trabalho de um tipo de registro para que os gerentes de espaços de trabalho possam adicioná-lo ou conectá-lo a outros espaços de trabalho.

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
<p>E</p>
<li><p>Qualquer pacote do Planning para criar tipos de registro conectáveis</p></li>
<li><p>Um pacote do Planning Plus para criar tipos de registros globais</p></li>
</ul>
Ou:
<ul><li><p>Um pacote de fluxo de trabalho Prime ou Ultimate</p> </li>
E
<li><p>Um pacote do Planning Prime ou Ultimate</p></li></ul>
<p>Para obter mais informações sobre o que está incluído em cada pacote do Workfront Planning, entre em contato com seu gerente de conta da Workfront. </p> 
   </td> 
  <tr> 
   <td role="rowheader"><p>Licença do Adobe Workfront</p></td> 
   <td><p>Standard</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Permissões de objeto</p></td> 
   <td>   <p>Gerenciar permissões para um espaço de trabalho e para o tipo de registro </a> </p>  
   <p>Os administradores do sistema têm permissões para todos os espaços de trabalho, incluindo aqueles que não criaram</p>  </td> 
  </tr>  
</tbody> 
</table>

Para obter mais informações sobre requisitos de acesso do Workfront, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++   

## Configurar tipos de registro global

<!--this is a UI term; don't change the title of this section-->

Como gerenciador de espaço de trabalho, você pode configurar um tipo de registro para ser um tipo de registro global. Um tipo de registro global pode ser adicionado a outros espaços de trabalho.

Um gerenciador de espaço de trabalho pode adicionar um tipo de registro global a um espaço de trabalho gerenciado por ele. Os campos originais do tipo de registro também são adicionados ao espaço de trabalho secundário.

Os usuários podem adicionar registros a um tipo de registro global de qualquer espaço de trabalho ao qual tenham permissões do Contribute e ao qual o tipo de registro global seja adicionado, incluindo seu espaço de trabalho original. Eles podem exibir registros de espaços de trabalho para os quais têm somente permissões de Exibição.

Para obter mais informações, consulte [Visão geral dos tipos de registro entre espaços de trabalho](/help/quicksilver/planning/architecture/cross-workspace-record-types-overview.md).

Para configurar um tipo de registro como global:

{{step1-to-planning}}

1. Clique no espaço de trabalho cujos tipos de registro você deseja configurar como global.

   A página do espaço de trabalho é aberta e os tipos de registro são exibidos.
1. Siga um destes procedimentos:

   * Passe o mouse sobre o cartão de um tipo de registro e clique no menu **Mais** ![Mais menu](assets/more-menu.png) no canto superior direito do cartão de tipo de registro

     ![Mais opções de menu do cartão de tipo de registro](assets/more-menu-options-from-record-type-card.png)

   * Clique em um cartão de tipo de registro para abrir a página de tipo de registro e clique no menu **Mais** ![Mais menu](assets/more-menu.png) à direita do nome do tipo de registro.
1. Clique em **Editar** ou **Configurações**.

   >[!TIP]
   >
   >Quando um tipo de registro é adicionado a outro espaço de trabalho, ele é exibido como um tipo de registro global nesse espaço de trabalho. Nesse caso, as opções Edit e Settings ficam esmaecidas.

1. (Condicional) Se você clicou em **Editar**, na caixa **Editar tipo de registro**, clique na guia **Configurações entre espaços de trabalho**

   Ou, se você clicou em **Configurações**, clique na seção **Configurações entre espaços de trabalho** no painel esquerdo.
1. Habilitar a configuração **Permitir a adição deste tipo de registro a outros espaços de trabalho**.

   ![Editar tipo de registro Configurações entre espaços de trabalho com Adicionar a outros espaços de trabalho habilitado](assets/edit-record-type-advanced-settings-add-to-other-workspaces-enabled.png)

   >[!TIP]
   >
   >Após adicionar um tipo de registro global a outro espaço de trabalho, essa configuração não poderá mais ser desativada.

1. No campo **Selecione quem pode adicionar este tipo de registro a espaços de trabalho que eles gerenciam**, adicione entidades que você deseja permitir para adicionar este tipo de registro a espaços de trabalho que eles gerenciam.

   Seu nome é adicionado automaticamente ao campo.

   É possível adicionar usuários individuais, grupos, equipes, funções de trabalho ou empresas cujos usuários você deseja permitir que adicionem esse tipo de registro aos espaços de trabalho que eles gerenciam.

   É possível editar esse campo depois de salvar o tipo de registro.

1. (Opcional) Remova seu nome do campo **Selecione quem pode adicionar este tipo de registro ao espaço de trabalho que eles gerenciam**.

   >[!TIP]
   >
   >Você deve designar pelo menos uma entidade (usuário, equipe, grupo, função ou empresa) para habilitar essa configuração.

1. (Condicional) Clique em **Salvar** na caixa **Editar tipo de registro** ou clique na seta para trás à esquerda de **Configurações** no cabeçalho da página para salvar suas alterações.

   As seguintes situações ocorrem:

   * O tipo de registro e seus campos agora estão disponíveis para serem adicionados a outro espaço de trabalho pelas pessoas designadas.

   >[!NOTE]
   >
   >É possível editar a aparência e as configurações do tipo de registro e seus campos originais somente a partir de seu espaço de trabalho original.

   * O cartão de tipo de registro exibe um **ícone de tipo de registro global** ![ícone de tipo de registro global](assets/global-icon.png) para indicar que o tipo de registro está disponível para ser adicionado a outros espaços de trabalho.
   * Um campo **Workspace** gerado pelo sistema é adicionado à exibição de tabela do tipo de registro e seus detalhes de registros.

     O campo Workspace exibe o espaço de trabalho de onde cada registro é criado.

     Este campo é somente leitura e não pode ser excluído.
1. (Opcional) Vá para outro espaço de trabalho e crie um tipo de registro usando um tipo de registro existente. Selecione o tipo de registro que você ativou nas etapas acima.

   Para obter informações, consulte [Adicionar tipos de registro existentes de outro espaço de trabalho](/help/quicksilver/planning/architecture/add-existing-record-types-from-another-workspace.md).

   O tipo de registro adicionado de um tipo de registro global no espaço de trabalho secundário também exibe um **ícone de tipo de registro global** ![ícone de tipo de registro global](assets/global-icon.png).
1. (Opcional) Retorne ao espaço de trabalho original onde você criou o tipo de registro global e edite o tipo de registro seguindo as etapas de 1 a 4 acima <!--ensure this stays accurate-->
1. (Opcional) Revise a lista de espaços de trabalho em que o registro global foi adicionado na **seção Espaços de trabalho em que esse tipo de registro é usado**.

   ![Espaços de trabalho onde este tipo de registro é usado](assets/workspaces-where-this-record-type-is-used.png)


## Configurar tipos de registro conectáveis

<!--this is a UI term; don't change the title of this section-->

É possível configurar um tipo de registro para ser conectado a partir de outros espaços de trabalho ao criar ou editar o tipo de registro.

Para configurar um tipo de registro como conectável:

{{step1-to-planning}}

1. Clique no espaço de trabalho cujos tipos de registro você deseja configurar como conectáveis.

   A página do espaço de trabalho é aberta e os tipos de registro são exibidos.
1. Siga um destes procedimentos:

   * Passe o mouse sobre o cartão de um tipo de registro e clique no menu **Mais** ![Mais menu](assets/more-menu.png) no canto superior direito do cartão de tipo de registro

     ![Mais opções de menu do cartão de tipo de registro](assets/more-menu-options-from-record-type-card.png)

   * Clique em um cartão de tipo de registro para abrir a página de tipo de registro e clique no menu **Mais** ![Mais menu](assets/more-menu.png) à direita do nome do tipo de registro.
1. Clique em **Editar** ou **Configurações**.

1. (Condicional) Se você clicou em **Editar**, na caixa **Editar tipo de registro**, clique na guia **Configurações entre espaços de trabalho**

   Ou, se você clicou em **Configurações**, clique na seção **Configurações entre espaços de trabalho** no painel esquerdo.

1. Habilitar a configuração **Permitir conexão com este tipo de registro em outros espaços de trabalho**. <!-- check the setting name, I sent this to Lilit to say FROM instead of IN-->

   <!-- add new screen shot with new tab name-->

   ![Editar tipo de registro na guia de configurações entre espaços de trabalho com conexão de outros espaços de trabalho habilitada](assets/edit-record-type-advanced-settings-connect-from-other-workspaces-enabled.png)

   Quando ativado, o tipo de registro é acessível e pode ser conectado a partir de outros espaços de trabalho.

1. Escolha a partir de quais espaços de trabalho o tipo de registro pode ser acessado. Escolha entre as seguintes opções:

   <!--check names of the setting: System wide?? OR All workspaces??-->

   * **Todos os espaços de trabalho**: os usuários podem se conectar a este tipo de registro de todos os espaços de trabalho onde têm permissões de Gerenciamento.
   * **Espaços de trabalho específicos**: no menu suspenso, adicione os nomes dos espaços de trabalho onde os gerentes de espaço de trabalho podem se conectar a este tipo de registro.
1. (Condicional) Clique em **Salvar** na caixa **Editar tipo de registro** ou clique na seta para trás à esquerda de **Configurações** no cabeçalho da página para salvar suas alterações.

   As seguintes situações ocorrem:

   * O tipo de registro e seus campos agora estão disponíveis para conexão a partir dos espaços de trabalho designados.
   * O cartão de tipo de registro exibe um ícone de tipo de registro conectável ![ícone de tipo de registro conectável](assets/connect-from-other-workspaces-icon.png) para indicar que o tipo de registro está disponível para conexão a partir de qualquer espaço de trabalho designado na sua configuração.

1. (Opcional) Vá para outro espaço de trabalho e adicione uma conexão ao tipo de registro que você ativou para conectividade entre espaços de trabalho nas etapas acima.

   Para obter informações, consulte [Tipos de registro de conexão](/help/quicksilver/planning/architecture/connect-record-types.md).









