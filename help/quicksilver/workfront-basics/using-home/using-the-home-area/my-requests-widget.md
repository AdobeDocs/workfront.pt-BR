---
product-area: projects
navigation-topic: use-the-home-area
title: Use o widget Minhas solicitações
description: Você pode enviar solicitações no widget Minhas solicitações. Você também pode personalizar o widget com filtros e colunas.
author: Alina, Courtney
feature: Get Started with Workfront
exl-id: 2b994f44-2404-4aa3-8c38-0686a0c287b7
last-update: 2026-04-01T18:23:03Z
git-commit-file: c04fc32836179ccbd80a7de3978493caf8ba8670
source-git-commit: f4d7484145226eb85bc547e582438e5202dec023
workflow-type: tm+mt
source-wordcount: '777'
ht-degree: 6%

---

# Use o widget Minhas solicitações

<!--remove Preview and Production references at Production release April 15, 2026-->

<span class="preview">As informações destacadas nesta página referem-se a funcionalidades que ainda não estão disponíveis. Ela está disponível somente no ambiente de Pré-visualização para todos os clientes. Depois das versões mensais para produção, os mesmos recursos também ficam disponíveis no ambiente de produção para clientes que ativaram versões rápidas. </span>

<span class="preview">Para obter informações sobre versões rápidas, consulte [Habilitar ou desabilitar versões rápidas para sua organização](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

>[!IMPORTANT]
>
>Este artigo descreve o novo widget Minhas solicitações. Você deve ter a nova experiência de solicitação habilitada para ver o novo widget.
>Você pode ativar a nova experiência de solicitação na área Solicitações.

O widget Minhas solicitações exibe as solicitações que você enviou. Você pode filtrar as solicitações, pesquisar solicitações específicas ou ajustar a ordem e a visibilidade da coluna. Você também pode criar uma nova solicitação no widget Minhas solicitações.

>[!NOTE]
>
>* Quando o widget Minhas solicitações é carregado, ele exibe até 50 solicitações. Para exibir mais solicitações, role para baixo na lista.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront package]</strong></td> 
   <td> <p>Qualquer pacote do Workfront ou Workflow</p>
   <p>Qualquer pacote do Workfront Planning para acessar solicitações do Workfront Planning e seus objetos criados</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licença</strong></td> 
   <td> <p>Colaborador ou posterior</p>
   <p>Solicitação ou posterior</p> </td> 
  </tr> 
  <tr> 
   <!--
   <tr> 
   <td role="rowheader"><strong>Additional products</strong></td> 
   <td> You must have Adobe Workfront Planning to view Planning requests or request forms</td> 
   </tr> 
   -->
   <td role="rowheader"><strong>Configuração do nível de acesso</strong></td> 
   <td> <p>Acesso maior ou igual a quaisquer objetos para os quais você esteja marcado em uma conversa ou precise resolver uma aprovação (Projetos, Tarefas, Problemas, Documentos)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Permissões de objeto</strong></td> 
   <td> <p>Permissões [!UICONTROL View] ou superior para projetos, tarefas, problemas, documentos nos quais você está marcado em uma conversa ou precisa resolver uma aprovação</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Criar uma solicitação

Você pode criar uma solicitação diretamente do widget Minhas solicitações.

Para obter instruções, consulte a seção [Criar uma solicitação](/help/quicksilver/workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md#create-a-request) no artigo [Criar itens de trabalho e projetos da Área inicial](/help/quicksilver/workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md).

## Copiar uma solicitação

Você pode copiar uma solicitação no widget Minhas solicitações, editá-la e enviá-la como uma nova solicitação.

Para obter instruções, consulte [Copiar e enviar solicitações](/help/quicksilver/manage-work/requests/create-requests/copy-and-submit-requests.md).

## Gerenciar informações na lista de solicitações no widget Minhas solicitações

<!--
This is similar to what we document in Enhanced lists, so we will link to that to avoid documentation duplication:
The My Requests widget features a customizable filter that allows you to control which requests appear in the widget. You can configure this filter for different fields and values, and can stack conditions using AND and OR operators.

To configure the filter in the My Requests widget:
-->

1. Clique no **[!UICONTROL Menu principal]** ![Ícone do Menu principal](assets/lines-main-menu.png), no canto superior esquerdo, e clique em **[!UICONTROL Página inicial]**.
1. (Condicional) Para adicionar o widget **Minhas solicitações** à sua tela inicial. Clique em **Personalizar**, localize **Minhas Solicitações** e clique nele para adicioná-lo à **Página Inicial**.
1. (Opcional) Para gerenciar a forma como as informações são exibidas na lista de solicitações, crie ou atualize os seguintes elementos de exibição para a lista:

   * Visualizar
   * Filtro
   * Colunas

   <div class="preview">

   * Grupo
   * Formatar células
   * Altura da linha

   </div>

   Para obter mais informações sobre como atualizar elementos de exibição na lista de solicitações, consulte [Usar listas aprimoradas](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md).


<!--
 Removed all these sections because this is common to ALL the Glists/ enhanced lists. So, we will update that article with all the specific steps: 
1. Select the field that you want to filter by. Available options are:

   * Workspace
   * Object type
   * Entry date
   * Request form
   * Status
   * Entered by
   * Custom fields from the request or from the created object   

1. In the next field, select the operator that you want to use for this filter condition. Available operators depend on the chosen field.
1. (Conditional) If a field appears to the right of the operator, select the value that you want to filter by.
1. (Optional) To add another filter condition, click **Add condition** and repeat steps 4-6.
1. (Optional and conditional) If you have multiple conditions, switch the And or Or value by clicking **And** or **Or** to the left of the condition.
The filter is saved automatically.
-->

>[!TIP]
>
>Se sua organização adquiriu o Workfront Planning além do Adobe Workfront, o widget Minhas solicitações incluirá as solicitações do Workfront e do Workfront Planning.
> 
>* Para filtrar apenas por solicitações Workfront, defina o filtro como **Tipo de objeto** > **Tem qualquer um dos** > **Problemas**.
>* Para filtrar apenas por solicitações do Workfront Planning, defina o filtro como **Tipo de objeto** > **Não tem nenhum de** > **Problemas**.

<!--

Use enhanced lists and other requests articles describe all of these:

## Adjust or add columns

You can choose which of the available columns appear on the My Requests widget, and set their order.

Available columns include:

* Subject
* Created object
* Object type
* Status
* Request form
* Entry date
* Entered by

To adjust the columns on the My Requests widget:

1. Click the **[!UICONTROL Main Menu]** ![Main Menu icon](assets/main-menu-icon.png) in the upper-right corner, then click **[!UICONTROL Home]**.
1. (Conditional) To add the **My Requests** widget to your home screen. Click **Customize**, and find **My Requests**, then click it to add it to **Home**. 
1. In the **My Requests** widget, click **Columns**.
1. (Optional) To reorder columns, click the drag handle ![drag handle](assets/drag-handle.png) of the column you want to move and drag it to the desired locations. The column at the top of the list appears in the My Requests widget as the first column.
1. (Optional) Use the toggle to hide or show the column in the requests list.
1. To add a custom field as a column, click the **Add column** icon ![Add column](assets/add-column.png) in the upper-right corner of the list, and click the plus icon next to the custom field that you want to add as a column to the widget.

   Custom fields on forms attached to the object in the list are available to add as columns.

Column preferences are saved automatically.

-->

<!--

## Create a view

You can create views in the My Requests widget to change the way the information displays in the request list. 

Consider the following when working with views in the My Requests widget:

* A view in the My Requests widget contains the columns and filters applied to the view.
* You can create views and share them with others. The filters and columns you select for the view before you share it are included in the views you share. 
* The following is a system view which you cannot edit, share, or delete: 

   * Widget Unified Requests Default View
* Creating and editing a view in the My Requests widget is similar to enhanced lists. For information, see [Use enhanced lists](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md). 

-->

## Pesquisar solicitações

Para pesquisar solicitações específicas no widget Minhas solicitações:

1. Clique no **[!UICONTROL Menu principal]** ![Ícone do Menu principal](assets/lines-main-menu.png), no canto superior esquerdo, e clique em **[!UICONTROL Página inicial]**.
1. (Condicional) Para adicionar o widget **Minhas solicitações** à sua tela inicial. Clique em **Personalizar**, localize **Minhas Solicitações** e clique nele para adicioná-lo à **Página Inicial**.
1. Na barra de pesquisa próxima ao canto superior direito do widget Minhas solicitações, digite o termo que você deseja pesquisar.

   As solicitações que contêm o termo são realçadas em laranja.

1. (Opcional) Para ir para as solicitações destacadas, clique nas setas para cima ou para baixo na barra de pesquisa.

## Ir para um objeto criado por uma solicitação

Você pode encontrar objetos criados por uma solicitação no widget Minhas solicitações.

>[!NOTE]
>
>Os seguintes objetos têm links da lista de solicitações no widget Minhas solicitações, quando você ativa a nova experiência de solicitações na área Solicitações:
>
>* Solicitações de Planning e Workfront no campo Assunto.
>* Registros de planejamento criados a partir de solicitações do Planning no campo Objeto criado.
>* <span class="preview">Tarefas e problemas do Workfront convertidos a partir de solicitações do Workfront no campo Objeto criado, no ambiente de Visualização.</span>

1. Clique no **[!UICONTROL Menu principal]** ![Ícone do Menu principal](assets/lines-main-menu.png), no canto superior esquerdo, e clique em **[!UICONTROL Página inicial]**.
1. (Condicional) Para adicionar o widget **Minhas solicitações** à sua tela inicial. Clique em **Personalizar**, localize **Minhas Solicitações** e clique nele para adicioná-lo à **Página Inicial**.
1. Localize a solicitação que criou o objeto.
1. Clique no nome do objeto na coluna **Objeto criado** para essa solicitação.

   A página do objeto é aberta.

   >[!TIP]
   >
   >No ambiente de Produção, somente os registros do Planning têm um link no campo **Objeto criado**.
   >   
   ><span class="preview">No ambiente de Visualização, tarefas e projetos do Workfront convertidos de problemas, bem como registros do Planning criados a partir de solicitações do Planning têm um link no campo **Objeto criado**.</span>
   >



