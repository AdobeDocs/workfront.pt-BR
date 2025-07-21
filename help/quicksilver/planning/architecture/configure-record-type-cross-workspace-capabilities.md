---
title: Configurar Recursos entre Espaços de Trabalho para o Tipo de Registro
description: Você pode habilitar um tipo de registro para ser adicionado a outro espaço de trabalho ou ser conectado de outro espaço de trabalho.
hidefromtoc: true
hide: true
exl-id: d36ab9fb-0275-483d-97be-0a88e170f8e0
source-git-commit: 943c26efa6f6351abf885dbc5f3aa09c0b0fab05
workflow-type: tm+mt
source-wordcount: '1006'
ht-degree: 1%

---

<!-- add these to the metadata, when making this public: 

feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog

-->

<!--*******************THIS TITLE MIGHT NEED TO CHANGE WHEN WE HAVE THE FINAL NAME FOR THE "GLOBAL" RECORD TYPE - NOT SURE IF WE ARE GOING TO USE "GLOBAL" OR "DYNAMIC", OR ???? ***************; also update TOC file, the miniTOC,  etc when this is finalized-->

<!--this is linked to the UI in the info icon of when you create a record type from a global record type-->

# Configurar recursos entre espaços de trabalho para tipos de registro

<span class="preview">As informações nesta página se referem a funcionalidades que ainda não estão disponíveis. Ela está disponível somente no ambiente de Pré-visualização para todos os clientes. Depois das versões mensais para produção, os mesmos recursos também ficam disponíveis no ambiente de produção para clientes que ativaram versões rápidas. </span>

<span class="preview">Para obter informações sobre versões rápidas, consulte [Habilitar ou desabilitar versões rápidas para sua organização](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

Você pode designar um tipo de registro para ser adicionado a outro espaço de trabalho ou estar conectado de outro espaço de trabalho, no Adobe Workfront Planning.

Primeiro, você deve definir os recursos entre espaços de trabalho de um tipo de registro para que os gerentes de espaços de trabalho possam conectá-lo ou importá-lo para outros espaços de trabalho.

Você define os recursos entre espaços de trabalho de um tipo de registro ao criar ou editar um tipo de registro.

Para obter informações, consulte um dos seguintes artigos:

* [Criar tipos de registro](/help/quicksilver/planning/architecture/create-record-types.md)
* [Editar tipos de registro](/help/quicksilver/planning/architecture/edit-record-types.md)

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
   <td><p> Padrão</p>
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
   <td>   <p>Gerenciar permissões para um espaço de trabalho</a> </p>  
   <p>Os administradores do sistema têm permissões para todos os espaços de trabalho, incluindo aqueles que não criaram</p>  </td> 
  </tr> 
</tbody> 
</table>

*Para obter mais informações sobre requisitos de acesso do Workfront, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Configurar a adição de um tipo de registro a outros espaços de trabalho

Como gerenciador de espaço de trabalho, você pode configurar um tipo de registro a ser adicionado a outros espaços de trabalho ao criar ou editar um tipo de registro.

Quando você configura a adição de um tipo de registro a outros espaços de trabalho, um gerenciador de espaço de trabalho pode importar o tipo de registro e todas as suas informações para um dos espaços de trabalho que gerenciam.

Para configurar a adição de um tipo de registro a outro espaço de trabalho ao editar o tipo de registro:

{{step1-to-planning}}

1. Clique no espaço de trabalho cujos tipos de registro você deseja editar.

   A página do espaço de trabalho é aberta e os tipos de registro são exibidos.
1. Siga um destes procedimentos:

   * Passe o mouse sobre o cartão de um tipo de registro e clique no menu **Mais** ![Mais menu](assets/more-menu.png) no canto superior direito do cartão de tipo de registro
Ou
   * Clique em um cartão de tipo de registro para abrir a página de tipo de registro e clique no menu **Mais** ![Mais menu](assets/more-menu.png) à direita do nome do tipo de registro.
1. Clique em **Editar**.

   ![Mais opções de menu do cartão de tipo de registro](assets/more-menu-options-from-record-type-card.png)

1. Na caixa **Editar tipo de registro**, selecione a guia **Configurações avançadas**.
1. Habilitar a configuração **Permitir a adição deste tipo de registro a outros espaços de trabalho**.

   ![Editar configurações avançadas do tipo de registro com Adicionar a outros espaços de trabalho habilita](assets/edit-record-type-advanced-settings-add-to-other-workspaces-enabled.png)

1. No campo **Selecione quem pode adicionar este tipo de registro a espaços de trabalho que eles gerenciam**, adicione os usuários que você deseja permitir que adicionem este tipo de registro a espaços de trabalho que eles gerenciam.

   Seu nome é adicionado automaticamente ao campo.

   É possível adicionar usuários individuais, ou grupos, equipes, funções de trabalho ou empresas cujos usuários você deseja permitir que adicionem esse tipo de registro aos espaços de trabalho que eles gerenciam.

   É possível editar esse campo depois de salvar o tipo de registro.
1. (Opcional) Remova seu nome do campo **Selecione quem pode adicionar este tipo de registro ao espaço de trabalho que eles gerenciam**.

1. Clique em **Salvar**.

   As seguintes situações ocorrem:

   * O tipo de registro e seus campos agora estão disponíveis para serem adicionados a outro espaço de trabalho pelas pessoas designadas.

   >[!NOTE]
   >
   >É possível editar o tipo de registro e seus campos somente no espaço de trabalho original.

   * O cartão de tipo de registro exibe um ícone global ![Ícone de tipo de registro global](assets/global-icon.png) para indicar que o tipo de registro está disponível para ser adicionado a qualquer espaço de trabalho cujo gerente você designou em sua configuração.
   * Um campo **Workspace** gerado pelo sistema é adicionado ao tipo de registro.

     O campo Workspace exibe o espaço de trabalho de onde cada registro foi criado.

     Este campo é somente leitura e não pode ser excluído.

## Configurar a conexão com um tipo de registro de outros espaços de trabalho

É possível configurar um tipo de registro para ser conectado a partir de outros espaços de trabalho ao criar ou editar o tipo de registro.

Para configurar um tipo de registro para conexão a partir de outros espaços de trabalho ao editar o tipo de registro:

{{step1-to-planning}}

1. Clique no espaço de trabalho cujos tipos de registro você deseja editar,

   A página do espaço de trabalho é aberta e os tipos de registro são exibidos.
1. Siga um destes procedimentos:

   * Passe o mouse sobre o cartão de um tipo de registro e clique no menu **Mais** ![Mais menu](assets/more-menu.png) no canto superior direito do cartão de tipo de registro e clique em **Editar**
Ou
   * Clique em um cartão de tipo de registro para abrir a página de tipo de registro, clique no menu **Mais** ![Mais menu](assets/more-menu.png) à direita do nome do tipo de registro e clique em **Editar**.

   ![Mais opções de menu do cartão de tipo de registro](assets/more-menu-options-from-record-type-card.png)

1. Na caixa **Editar tipo de registro**, selecione a guia **Configurações avançadas**.
1. Habilitar a configuração **Permitir conexão com este tipo de registro em outros espaços de trabalho**. <!-- check the setting name, I sent this to Lilit to say FROM instead of IN-->

   ![Editar a guia Configurações avançadas do tipo de registro com conexão de outros espaços de trabalho habilitada](assets/edit-record-type-advanced-settings-connect-from-other-workspaces-enabled.png)

   Quando ativado, o tipo de registro é acessível e pode ser conectado de outros espaços de trabalho.

1. Escolha a partir de quais espaços de trabalho o tipo de registro pode ser acessado. Escolha entre as seguintes opções:

   * **Em todo o sistema**: os usuários podem se conectar a este tipo de registro de todos os espaços de trabalho onde têm permissões de gerenciamento.
   * **Espaços de trabalho específicos**: adicione os nomes dos espaços de trabalho nos quais os gerentes de espaço de trabalho podem se conectar a este tipo de registro.
1. Clique em **Editar**.

   As seguintes situações ocorrem:

   * O tipo de registro e seus campos agora estão disponíveis para conexão a partir dos espaços de trabalho designados.
   * O cartão de tipo de registro exibe um ícone de conexão entre espaços de trabalho ![ícone de conexão entre espaços de trabalho](assets/connect-from-other-workspaces-icon.png) para indicar que o tipo de registro está disponível para ser conectado de qualquer espaço de trabalho designado na sua configuração.

   O tipo de registro fica disponível para conexão a partir dos espaços de trabalho designados.









