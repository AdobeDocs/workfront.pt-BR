---
product-area: requests
navigation-topic: create-requests
title: Criar e gerenciar exibições na área Solicitações
description: Se estiver usando a nova experiência de solicitação, é possível criar e salvar exibições para a área Solicitações.
author: Alina
feature: Work Management
exl-id: ed066075-6411-4350-8b39-f21dc4fa96c9
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: ff87e425389f30dfaa1a178ea2b548d1c41179bb
workflow-type: tm+mt
source-wordcount: '725'
ht-degree: 9%

---


# Criar e gerenciar exibições na área Solicitações

<span class="preview">As informações nesta página se referem a funcionalidades que ainda não estão disponíveis. Ela está disponível somente no ambiente de Pré-visualização para todos os clientes. Depois das versões mensais para produção, os mesmos recursos também ficam disponíveis no ambiente de produção para clientes que ativaram versões rápidas. </span>

<span class="preview">Para obter informações sobre versões rápidas, consulte [Habilitar ou desabilitar versões rápidas para sua organização](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>


Se estiver usando a nova experiência de solicitação no Adobe Workfront, você pode criar e salvar exibições para a área Solicitações. Esses modos de exibição incluem filtros, arranjos de colunas <span class="preview"> e agrupamentos.</span>


>[!IMPORTANT]
>
>* Essa funcionalidade está disponível somente na nova experiência de solicitação na área Solicitações.
>* As configurações de exibição também estão disponíveis no widget Minhas solicitações na Página inicial. No entanto, as exibições da área Solicitações são separadas das do widget Minhas solicitações.
>* A lista de solicitações na área Solicitações e no widget Meu trabalho usam a lista aprimorada no Workfront. Para obter mais informações, consulte [Usar listas aprimoradas](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md).

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

<div class="preview">

## Visualizações do sistema para solicitações

Além das exibições que você pode criar por conta própria, o Workfront oferece as seguintes exibições do sistema para a área Solicitações e o widget Minhas solicitações na Página inicial:

* **Todas as Solicitações**: todas as solicitações que você ou qualquer outra pessoa enviou em filas ou espaços de trabalho que você tem permissões para exibir. Isso não está disponível para o widget Minhas solicitações.
* **Minhas Solicitações**: Solicitações que você enviou, independentemente do status.
* **Minhas solicitações abertas**: as solicitações que você enviou e ainda estão abertas.
* **Meus rascunhos**: rascunhos de suas consultas que ainda não foram enviados.
* **Solicitações Abertas**: Solicitações que você ou qualquer outra pessoa enviou em filas ou para espaços de trabalho que você tem permissões para exibir e que ainda estão abertos. Isso não está disponível para o widget Minhas solicitações.

Não é possível editar visualizações do sistema. Você pode modificar os elementos, copiar a exibição e editar ou compartilhar a cópia.

</div>

## Criar uma visualização para solicitações

Você pode criar uma visualização na área Solicitações do Workfront ao usar a nova experiência de solicitações. Depois de ativar e criar uma nova experiência de solicitações, você também pode criar exibições para o widget Minhas solicitações na Página inicial.

1. Para acessar a lista **Solicitações**:

   {{step1-to-requests}}

   1. Verifique se a configuração **Usar nova experiência** está ativada.

1. Para acessar o widget **Minhas solicitações** na página inicial:

   {{step1-to-home}}

   1. Adicionar ou ir para o widget **Minhas solicitações**.

1. Na lista de solicitações, clique no menu suspenso **Exibições** ![Exibições](assets/view-icon-requests.png) e clique em **Nova exibição**.

   ![Nova exibição](assets/create-new-view.png)

1. Insira um nome para o novo modo de exibição e clique em **Criar**.
1. Continue em [Editar um modo de exibição para solicitações](#edit-a-view-for-requests).

## Editar uma visualização de solicitações

Você pode editar as exibições existentes, incluindo as que acabou de criar na área Solicitações ou no widget Minhas solicitações na Página inicial.

Ao editar uma visualização, você pode alterar os seguintes elementos da visualização:

* Nome
* Filtros
* Colunas

<div class="preview">

* Agrupamento
* Formatar células
* Altura da linha

</div>

Para obter mais informações, consulte [Usar listas aprimoradas](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md).

<!-- 
hide these details - all the information is in "Use enhanced lists" - we need one point of messaging for this feature: 

1. To access a list of requests in the Requests are: 
   
   {{step1-to-requests}}

1. Ensure the **Use new experience** setting is turned on.
1. In the **Requests** list, locate the view that you want to edit from the **Views** dropdown menu ![Views dropdown](assets/view-icon-requests.png).

1. Click the **Views** dropdown ![Views dropdown](assets/view-icon-requests.png) and click the three-dot menu next to the view, select **Rename**, then type in the new name for the view.
1. Press Enter to save the new name. 
1. Click the **Views** dropdown ![Views dropdown](assets/view-icon-requests.png) and select the view you want to edit.
1. To add a field as a column, click the **Add column** icon ![Add column](assets/add-column.png) in the upper-right corner of the list. 

   The **Column manager** opens.
1. Click the plus icon next to the field that you want to add as a column to the view, then click **Save**.

   Fields associated with the objects in the list are available to add as columns. <!-keeping this general, and not referring to custom fields because there are some native fields that are supported and there will be more in the future->

   >[!TIP]
   >
   >Fields you add to the columns must exist before they are available in the **Column manager**.

1. (Optional) Click **Columns** to open the **Fields visibility and order** box. 
1. Turn on the setting for each field  you want to show in the list, turn it off to hide it, or drag and drop the fields in a different order.

1. (Optional) Click **Filters** and start adding conditions for what requests you want to view. 

    You can filter by the following request fields:  

    * **Workspace**: The workspace the request form is associated with.
    * **Object type**: The record type the request form is associated with.
    * **Entry date**: The date when the request was submitted.
    * **Request form**: The name of the request form used to submit the request.
    * **Status**: The status of the request.
    * **Entered by**: The name of the user who added the request. If the request was added by someone outside of Workfront, the **Entered by** field shows `N/A`.

    You can also filter by any fields that have been added to the view for any object visible in the view.

    You can have multiple filters joined by either **And** or **Or**.
    The request list is filtered automatically, as you add the filter conditions. 
-->

<!--
1. <Span class="preview">(Optional) Click **Group** and select the column that you want to group by.</span>

-->

>[!IMPORTANT]
>
> * As alterações nas exibições são salvas automaticamente.
> * As alterações nos modos de exibição só estarão visíveis para qualquer pessoa que use o modo de exibição <span class="preview"> quando você compartilhar uma nova cópia do modo de exibição depois de ter feito alterações nele.</span>
> * Use o curinga de filtro **Me (usuário conectado)** em qualquer campo que tenha usuários como o valor.

## Adicionar a exibição de solicitações a um modelo de layout

Um administrador do Workfront pode adicionar uma nova exibição aos modelos de layout da área Solicitações.

Para obter instruções, consulte [Personalizar filtros, exibições e agrupamentos usando um modelo de layout](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md).

## Compartilhar uma exibição

Você pode compartilhar visualizações criadas com outros usuários, equipes, grupos ou empresas.

Depois de compartilhar uma visualização, outros usuários podem visualizá-la antes de compartilhá-la, os elementos de visualização atualizados que você editou.

<span class="preview">Se eles atualizarem o modo de exibição, suas alterações não ficarão visíveis para outras pessoas, a menos que façam uma cópia do mesmo modo de exibição e preservem suas alterações antes de compartilharem a cópia.

Para obter mais informações, consulte [Usar listas aprimoradas](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md). </span>

<!--
Let's just redirect to Use enhanced lists so we avoid duplicating information. 

1. To access a list of requests in the Requests are: 
   
   {{step1-to-requests}}

1. Ensure the **Use new experience** setting is turned on.
1. In the **Requests** list, locate the view that you want to share.
1. Hover over the view that you want to share, then click on the three-dot menu to the right of the view name, then click  **Share**.
1. In the **Share** box, enter the people, teams, roles, groups, or companies that you want to share the view with, then select them from the list when they appear.
1. Click **Save**.

   The view is shared with the entities you indicate. 
-->