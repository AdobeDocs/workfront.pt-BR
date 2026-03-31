---
product-area: requests
navigation-topic: create-requests
title: Criar e gerenciar exibições na área Solicitações
description: Se estiver usando a nova experiência de solicitação, é possível criar e salvar exibições para a área Solicitações.
author: Alina
feature: Work Management
exl-id: ed066075-6411-4350-8b39-f21dc4fa96c9
source-git-commit: a9cc76139c0f542e4b27e8e3591a40bf626342f4
workflow-type: tm+mt
source-wordcount: '962'
ht-degree: 6%

---


# Criar e gerenciar exibições na área Solicitações

<span class="preview">As informações nesta página se referem a funcionalidades que ainda não estão disponíveis. Ela está disponível somente no ambiente de Pré-visualização para todos os clientes. Depois das versões mensais para produção, os mesmos recursos também ficam disponíveis no ambiente de produção para clientes que ativaram versões rápidas. </span>

<span class="preview">Para obter informações sobre versões rápidas, consulte [Habilitar ou desabilitar versões rápidas para sua organização](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>


Se estiver usando a nova experiência de solicitação no Adobe Workfront, você pode criar e salvar exibições para a área Solicitações. Essas exibições incluem filtros e organização de colunas.

<!--<span class="preview"> and groupings.</span>-->


>[!IMPORTANT]
>
>* Essa funcionalidade está disponível somente na nova experiência de solicitação na área Solicitações.
>* As configurações de exibição também estão disponíveis no widget Minhas solicitações na Página inicial. No entanto, as exibições da área Solicitações são separadas das do widget Minhas solicitações.
>* A lista de solicitações na área Solicitações usa a lista aprimorada no Workfront. Para obter mais informações, consulte [Usar listas aprimoradas](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md).

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo.


<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacote do Adobe Workfront</td> 
   <td> <p>Qualquer pacote do Workfront ou Workflow</p>

<p>Qualquer licença do Workfront Planning, para exibir solicitações do Workfront Planning em listas de solicitações</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td> <p>Colaborador ou posterior</p>
   <p>Solicitação ou posterior</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Editar acesso a ocorrências</p>  <p>Você deve ser um administrador do Workfront para adicionar exibições a modelos de layout</td> 
  </tr> 
  <!--
  <tr> 
   <td role="rowheader"> Product</td> 
   <td> <ul><li>Adobe Workfront</li><li>You must have Adobe Workfront Planning to view Planning requests or request forms</td> 
   </tr> 
   -->
 </tbody> 
</table>

Para obter mais detalhes sobre as informações contidas nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Criar uma visualização para solicitações

Você pode criar uma visualização na área Solicitações do Workfront ao usar a nova experiência de solicitações.

1. Para acessar a lista Solicitações:

   {{step1-to-requests}}

1. Verifique se a configuração **Usar nova experiência** está ativada.

1. Na lista **Solicitações**, clique no menu suspenso **Exibições** ![Exibições](assets/view-icon-requests.png) e clique em **Nova exibição**.

   ![Nova exibição](assets/create-new-view.png)

1. Insira um nome para o novo modo de exibição e clique em **Criar**.
1. Continue em [Editar um modo de exibição na área Solicitações](#edit-a-view-in-the-requests-area).

## Editar uma visualização de solicitações

É possível editar exibições existentes, incluindo as que você acabou de criar na área Solicitações do Workfront.

Ao editar uma exibição na área Solicitações, é possível alterar os seguintes elementos da exibição:

* Nome
* Filtros
* Colunas

As alterações feitas em uma exibição ficam visíveis para todos com quem você compartilha a exibição.

1. Para acessar uma lista de solicitações na seção Solicitações:

   {{step1-to-requests}}

1. Verifique se a configuração **Usar nova experiência** está ativada.
1. Na lista **Solicitações**, localize a exibição que você deseja editar no menu suspenso **Exibições** ![Exibições](assets/view-icon-requests.png).

1. Clique na lista suspensa **Exibições** ![Exibições](assets/view-icon-requests.png) e clique no menu de três pontos ao lado da exibição, selecione **Renomear** e digite o novo nome da exibição.
1. Pressione Enter para salvar o novo nome.
1. Clique na lista suspensa **Exibições** ![Exibições](assets/view-icon-requests.png) e selecione o modo de exibição que deseja editar.
1. Para adicionar um campo como coluna, clique no ícone **Adicionar coluna** ![Adicionar coluna](assets/add-column.png) no canto superior direito da lista.

   O **Gerenciador de colunas** se abre.
1. Clique no ícone de adição ao lado do campo que você deseja adicionar como coluna ao modo de exibição e clique em **Salvar**.

   Campos associados aos objetos na lista estão disponíveis para serem adicionados como colunas. <!--keeping this general, and not referring to custom fields because there are some native fields that are supported and there will be more in the future-->

   >[!TIP]
   >
   >Os campos adicionados às colunas devem existir antes de serem disponibilizados no **Gerenciador de colunas**.

1. (Opcional) Clique em **Colunas** para abrir a caixa **Visibilidade e ordem dos campos**.
1. Ative a configuração para cada campo que deseja mostrar na lista, desative-o para ocultá-lo ou arraste e solte os campos em uma ordem diferente.

1. (Opcional) Clique em **Filtros** e comece a adicionar condições para quais solicitações você deseja exibir.

   Você pode filtrar pelos seguintes campos de solicitação:

   * **Workspace**: o espaço de trabalho ao qual o formulário de solicitação está associado.
   * **Tipo de objeto**: o tipo de registro ao qual o formulário de solicitação está associado.
   * **Data de entrada**: a data em que a solicitação foi enviada.
   * **Formulário de solicitação**: o nome do formulário de solicitação usado para enviar a solicitação.
   * **Status**: o status da solicitação.
   * **Inserido por**: o nome do usuário que adicionou a solicitação. Se a solicitação foi adicionada por alguém fora do Workfront, o campo **Informado por** mostrará `N/A`.

   Também é possível filtrar por qualquer campo que tenha sido adicionado à exibição para qualquer objeto visível na exibição.

   Você pode ter vários filtros unidos por **And** ou **Or**.
A lista de solicitações é filtrada automaticamente ao adicionar as condições de filtro.


<!--
1. <Span class="preview">(Optional) Click **Group** and select the column that you want to group by.</span>

-->

>[!IMPORTANT]
>
> * As alterações nas exibições são salvas automaticamente.
> * As alterações nas exibições ficam visíveis para qualquer pessoa que a use.
> * Use o curinga de filtro **Me (usuário conectado)** em qualquer campo que tenha usuários como o valor.

## Adicione a visualização de solicitações a um modelo de layout.

Um administrador do Workfront pode adicionar a nova visualização aos modelos de layout.

Para obter instruções, consulte [Personalizar filtros, exibições e agrupamentos usando um modelo de layout](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md).

## Compartilhar uma exibição

Você pode compartilhar visualizações criadas com outros usuários, equipes ou grupos.

1. Para acessar uma lista de solicitações na seção Solicitações:

   {{step1-to-requests}}

1. Verifique se a configuração **Usar nova experiência** está ativada.
1. Na lista **Solicitações**, localize o modo de exibição que você deseja compartilhar.
1. Passe o mouse sobre a exibição que você deseja compartilhar, clique no menu de três pontos à direita do nome da exibição e clique em **Compartilhar**.
1. Na caixa **Compartilhar**, insira as pessoas, equipes, funções, grupos ou empresas com as quais deseja compartilhar a exibição e selecione-as na lista quando forem exibidas.
1. Clique em **Salvar**.

   A exibição é compartilhada com as entidades indicadas. Eles podem exibir os elementos de visualização atualizados que você editou para a visualização antes de compartilhá-la. <span class="preview">Se eles atualizarem o modo de exibição, suas alterações não ficarão visíveis para outras pessoas, a menos que façam uma cópia do mesmo modo de exibição e preservem suas alterações antes de compartilharem a cópia. Para obter mais informações, consulte [Usar listas aprimoradas](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md). </span>
