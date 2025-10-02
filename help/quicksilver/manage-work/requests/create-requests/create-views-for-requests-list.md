---
product-area: requests
navigation-topic: create-requests
title: Criar exibições na área Solicitações
description: Se estiver usando a nova experiência de solicitação, é possível criar e salvar exibições para a área Solicitações.
author: Becky
feature: Work Management
source-git-commit: 1c7e2fb7de500083f0f7e42f1016323305054d88
workflow-type: tm+mt
source-wordcount: '608'
ht-degree: 0%

---

# Criar ou editar exibições na área Solicitações

<span class="preview">As informações nesta página se referem a funcionalidades que ainda não estão disponíveis. Ele está disponível somente no ambiente de Pré-visualização da Sandbox.</span>

Se estiver usando a nova experiência de solicitação, é possível criar e salvar exibições para a área Solicitações. Essas exibições incluem filtros e organização de colunas.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.


<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacote do Adobe Workfront</td> 
   <td> <p>Qualquer </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td> <p>Colaborador ou superior</p>
   <p>Solicitação ou superior</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Editar acesso a ocorrências</p>  <p>Você deve ser um administrador do Workfront para adicionar exibições a modelos de layout</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> Produto</td> 
   <td> <ul><li>Adobe Workfront</li><li>Você precisa ter o Adobe Workfront Planning para exibir solicitações ou formulários de solicitação do Planning</td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Criar uma visualização na área Solicitações

{{step1-to-requests}}

1. (Opcional e condicional) Selecione a configuração **Alternar para nova experiência** no canto superior direito da tela se os seguintes itens se aplicarem à sua organização e instância do Workfront:

   * Sua organização adquiriu um pacote do Workfront
   * Sua organização foi integrada à Adobe Unified Experience.
   * Seu administrador concedeu acesso ao Workfront Planning
   * Você tem pelo menos permissões de exibição para um espaço de trabalho do Workfront Planning

   Para obter mais informações, consulte [Enviar solicitações do Adobe Workfront Planning para criar registros](/help/quicksilver/planning/requests/submit-requests.md)

1. Clique na lista suspensa **Exibições** ![Exibições](assets/view-icon-requests.png) e selecione **Nova exibição**.

   ![Nova exibição](assets/create-new-view.png)

1. Insira um nome para o novo modo de exibição e clique em **Criar**.
1. Continue em [Editar um modo de exibição na área Solicitações](#edit-a-view-in-the-requests-area).

## Editar uma exibição na área Solicitações

É possível editar visualizações existentes, incluindo aquelas que você acabou de criar.

{{step1-to-requests}}

1. (Opcional e condicional) Selecione a configuração **Alternar para nova experiência** no canto superior direito da tela se os seguintes itens se aplicarem à sua organização e instância do Workfront:

   * Sua organização adquiriu um pacote do Workfront
   * Sua organização foi integrada à Adobe Unified Experience.
   * Seu administrador concedeu acesso ao Workfront Planning
   * Você tem pelo menos permissões de exibição para um espaço de trabalho do Workfront Planning

   Para obter mais informações, consulte [Enviar solicitações do Adobe Workfront Planning para criar registros](/help/quicksilver/planning/requests/submit-requests.md)1.

1. (Opcional) Para renomear uma exibição, clique na lista suspensa **Exibições** ![Exibições](assets/view-icon-requests.png) e clique no menu de três pontos ao lado da exibição, selecione **Renomear** e digite o novo nome da exibição.
1. Clique na lista suspensa **Exibições** ![Exibições](assets/view-icon-requests.png) e selecione o modo de exibição que deseja editar.
1. (Opcional) Clique em **Filtros** e comece a adicionar condições para quais solicitações você deseja exibir na guia Planning.

   ![Editar filtros na guia de solicitações do Planning](assets/filters-editing-box-in-requests-planning-tab.png)

   Você pode filtrar pelos seguintes campos:

   * **Workspace**: o espaço de trabalho ao qual o formulário de solicitação está associado.
   * **Tipo de registro**: o tipo de registro ao qual o formulário de solicitação está associado.
   * **Data de entrada**: a data em que a solicitação foi enviada.
   * **Formulário de solicitação**: o nome do formulário de solicitação usado para enviar a solicitação.
   * **Status**: o status da solicitação.
   * **Inserido por**: o nome do usuário que adicionou a solicitação. Se a solicitação foi adicionada por alguém fora do Workfront, o campo **Informado por** mostrará `N/A`.

   Você pode ter vários filtros unidos por **And** ou **Or**.
A lista de solicitações é filtrada automaticamente ao adicionar as condições de filtro.

1. (Opcional) Clique em **Colunas** e oculte, exiba ou reorganize as colunas da lista de solicitações.

   ![Caixa Colunas](assets/columns-editing-box-in-requests-planning-tab.png)

   >[!TIP]
   >
   >Não é possível adicionar mais colunas.

>[!IMPORTANT]
>
> * As alterações nas exibições são salvas automaticamente.
> * As alterações nas exibições ficam visíveis para qualquer pessoa que a use.

## Adicione a exibição a um modelo de layout.

Um administrador do Workfront pode adicionar a nova visualização aos modelos de layout.

Para obter instruções, consulte [Personalizar filtros, exibições e agrupamentos usando um modelo de layout](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md).
