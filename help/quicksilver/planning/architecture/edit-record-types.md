---
title: Editar Tipos de Registro
description: Você poderá editar os tipos de registro depois que eles forem salvos. Os tipos de registro são os tipos de objeto do Adobe Workfront Planning.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 7d6de742-9657-4286-968c-1fc78ebbb94e
source-git-commit: 939f3d9a4fac609c014acfc3be3d1485f469e947
workflow-type: tm+mt
source-wordcount: '753'
ht-degree: 2%

---


# Editar tipos de registro

<span class="preview">As informações nesta página se referem a funcionalidades que ainda não estão disponíveis. Ela está disponível somente no ambiente de Pré-visualização para todos os clientes. Depois das versões mensais para produção, os mesmos recursos também ficam disponíveis no ambiente de produção para clientes que ativaram versões rápidas. </span>

<span class="preview">Para obter informações sobre versões rápidas, consulte [Habilitar ou desabilitar versões rápidas para sua organização](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

Os tipos de registro são os tipos de objeto do Adobe Workfront Planning. É possível editar a aparência dos tipos de registros criados por você ou por qualquer outra pessoa. Para obter informações sobre como criar tipos de registro do Workfront Planning, consulte [Criar tipos de registro](/help/quicksilver/planning/architecture/create-record-types.md).

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso.

Você deve ter o seguinte acesso para executar as etapas deste artigo:

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
   <td>   <p>Gerenciar permissões para um espaço de trabalho <span class="preview">e tipo de registro</span> </p>  
   <p>Os administradores do sistema têm permissões para todos os espaços de trabalho, incluindo aqueles que não criaram</p>
   <p>Somente administradores do sistema podem habilitar tipos de registro para se conectar de outros espaços de trabalho</p> </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Modelo de layout</p></td> 
   <td> <p>No ambiente de Produção, todos os usuários, inclusive os Administradores do Sistema, devem ser atribuídos a um modelo de layout que inclua o Planning.</p>
<p><span class="preview">No ambiente de Pré-visualização, os usuários do Standard e os administradores do sistema têm o Planning habilitado por padrão.</span></p> </td> 
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

1. (Condicional) Se você for um administrador do sistema, clique na guia **Configurações avançadas** na caixa **Editar tipo de registro**. <!--the info here is duplicated in the Create record types article-->

   ![Guia de configurações avançadas da caixa Editar tipo de registro](assets/edit-record-type-box-advanced-settings-tab.png)

1. (Condicional) Atualize as seguintes informações na guia **Configurações avançadas**:

   * Habilitar a configuração **Conectar de outro espaço de trabalho**. Quando ativado, o tipo de registro é acessível e pode ser conectado de outros espaços de trabalho.
   * Escolha a partir de quais espaços de trabalho o tipo de registro pode ser acessado. Escolha entre as seguintes opções:

      * **Em todo o sistema**: os usuários podem se conectar a este tipo de registro de todos os espaços de trabalho onde têm permissões de gerenciamento.
      * **Espaços de trabalho específicos**: adicione os nomes dos espaços de trabalho nos quais os gerentes de espaço de trabalho podem se conectar a este tipo de registro.

1. Clique em **Salvar**.

   O cartão de tipo de registro no espaço de trabalho exibe um ícone de conectividade ![Conectar-se de outros espaços de trabalho](assets/connect-from-other-workspaces-icon.png) no canto superior direito para indicar que o registro agora pode ser acessado de outros espaços de trabalho.

1. (Opcional) Clique no cartão de tipo de registro na área do espaço de trabalho para abrir a página do tipo de registro e, em seguida, renomeie o tipo de registro no cabeçalho.

1. (Opcional) Para editar outro tipo de registro, na página Tipo de registro, expanda a seta apontando para baixo à direita do nome de um tipo de registro, procure um tipo de registro e selecione-o quando ele for exibido na lista.

   ![Menu suspenso de tipo de registro na página de tipo de registro com caixa de pesquisa](assets/record-type-drop-down-on-record-type-page-with-search-box.png)
