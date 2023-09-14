---
title: Gerenciar exibições de registro
description: Você pode exibir registros em uma tabela ou exibição de linha do tempo ao usar o Adobe Maestro.
hidefromtoc: true
hide: true
source-git-commit: f058c369bdb3b991910d3a820895de73ea4709f0
workflow-type: tm+mt
source-wordcount: '731'
ht-degree: 1%

---


# Gerenciar exibições de registro

<!--update the metadata with real information when making this available in TOC and in the left nav-->

>[!IMPORTANT]
>
>Atualmente, o Adobe Maestro faz parte de um programa beta aberto a um número limitado de clientes.
>
>Entre em contato com seu representante de conta para obter mais informações sobre como participar do programa beta para o Maestro.
>
>Para obter informações, consulte [Visão geral do Adobe Maestri](../maestro-overview.md).

Depois de selecionar um tipo de registro no Adobe Maestro, você pode exibir todos os registros desse tipo nas seguintes exibições:

* Tabela

  Para obter mais informações, consulte [Gerenciar a exibição de tabela](../views/manage-the-table-view.md).
* Linha do tempo

  Para obter mais informações, consulte [Gerenciar a exibição de linha do tempo](../views/manage-the-timeline-view.md).

## Requisitos de acesso

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
   <p> produto Adobe</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>contrato do Adobe Workfront</p></td>
   <td>
<p>Sua organização deve estar inscrita no programa beta fechado do Adobe Maestro. Entre em contato com seu representante de conta para obter mais informações sobre esta nova oferta. </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>plano do Adobe Workfront</p></td>
   <td>
<p>Qualquer Um</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Licença do Adobe Workfront</p></td>
   <td>
   <p>Qualquer Um</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader">Nível de acesso</td>
   <td> <p>Qualquer Um</p>  
</td>
  </tr>

<tr>
   <td role="rowheader">Modelo de layout</td>
   <td> <p>O administrador do sistema deve adicionar a área Maestro no modelo de layout. Para obter informações, consulte <a href="../access/grant-access.md">Conceder acesso ao Adobe Maestro</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

<!--Maybe enable this at GA - but Maestro is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->

<!-- Notes for the table: for the "Workfront access" row: <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p>-->

## Considerações ao trabalhar com as visualizações do Maestro

* As opiniões no Maestro são específicas do tipo de registro. Não é possível aplicar a mesma exibição a dois tipos de registro diferentes.
* As vistas que você cria são visíveis para todos que acessam a área do Maestro. <!-- edit this when we have permissions and the views will be shared only to be visible by others-->
  <!-- this is not yet possible: * You can share views with others if you want them to also apply them to the same record types.-->
* A criação de exibições para tipos de registro operacional é idêntica à criação de exibições para tipos de registro de taxonomia.
* Quando você modifica ou exclui uma visualização, ela é modificada e excluída para todos os usuários que podem acessar a área Maestro.
* Os seguintes elementos são exclusivos para cada visualização no Maestro:

   * Filtro
   * Agrupamento
   * Ordenar

  <!-- some of these are not available in all of the views - edit above-->

  Por exemplo, ao criar um filtro em uma exibição de tabela, os resultados do filtro ficam visíveis somente na exibição selecionada e não em todas as exibições listadas no menu suspenso Exibir.

  >[!NOTE]
  >
  > Como o Maestri está atualmente em um estado beta, alguns elementos de visualização podem não estar disponíveis para ambas as visualizações.


Este artigo descreve as seguintes informações sobre as visualizações Maestri:

* [Criar e editar uma visualização](#create-or-edit-record-views)
* [Excluir um modo de exibição](#delete-views)
  <!--* [Duplicate a view](#duplicate-views)-->
  <!--* [Add a view as a favorite](#add-a-view-as-a-favorite) - not possible yet-->
  <!--* [Share a view](#share-views) - not possible yet-->

## Semelhanças e diferenças entre as visualizações de tabela e linha do tempo

A tabela a seguir mostra as semelhanças e diferenças entre as visualizações de tabela e linha do tempo no Maestro:

<!--some of these are NOT available right now; if you make this public, comment out the ones not there-->

| Recurso | Visualização em tabela | Exibição da linha do tempo |
|-----------------------------------------------------------------------|------------|---------------|
| Exibir registros em uma lista ou tabela | ✓ µ |              |
| Exibir todos os campos como colunas na tabela, por padrão | ✓ |              |
| Ocultar ou mostrar campos (ou colunas) | ✓ |               |
| Editar valores de campo para cada registro | ✓ |               |
| Adicionar registros como novas linhas na exibição | ✓ |               |
| Adicionar campos como novas colunas na exibição | ✓ |               |
| Copiar linhas de uma lista externa e colá-las em uma tabela | ✓ |               |
| Exibir registros em uma linha do tempo |            | ✓ |
| Filtrar registros | ✓ | ✓ |
| Registros de grupo |           | ✓ |
| Classificar registros | ✓ |              |

<!--| Sort groupings                                                        | ✓          | ✓             |-->

<!--| Display a limited number of fields as columns, by default                      | ✓          |               |-->

<!--| Color-code records                     |           | ✓              |-->
<!--| Color-code groupings                     |           | ✓              |-->

## Criar ou editar exibições {#create-or-edit-views}

1. Clique em **Menu principal** ícone ![](assets/main-menu-workfront.png) no canto superior direito <!--or the **Main Menu** icon ![](assets/main-menu-shell.png) in the upper-left corner, if available-->e, em seguida, clique em **Maestro** ![](assets/maestro-icon.png).
O espaço de trabalho acessado pela última vez é aberto por padrão. Para obter informações sobre como criar espaços de trabalho, consulte [Criar espaços de trabalho](../architecture-and-fields/create-workspaces.md).
1. Clique em um cartão de tipo de registro. Para obter informações sobre como criar um tipo de registro, consulte [Criar tipos de registro](../architecture-and-fields/create-record-types.md).

   Por padrão, todos os registros do tipo selecionado são exibidos na exibição de tabela.

1. Clique em **Exibir** e selecione um existente **Visualização em tabela** ![](assets/table-view-icon.png) ou clique em **Criar visualização > Tabela** para criar uma exibição de tabela

   Ou

   Selecionar um existente **Exibição da linha do tempo** ![](assets/timeline-view-icon.png) exibir ou clicar **Criar exibição > Linha do tempo** para criar uma visualização de linha do tempo.

   ![](assets/view-types-drop-down-from-record-type-list.png)

   >[!NOTE]
   >
   >    Para criar uma exibição de linha do tempo, o tipo de registro para o qual você cria a exibição deve ter pelo menos dois campos de data. Caso contrário, a opção Linha do tempo ficará esmaecida.

1. (Opcional) Atualize o nome da exibição e clique em **Criar** para salvá-lo.

   Por padrão, o Maestri nomeia a exibição como &quot;Tabela &lt; número >&quot; ou &quot;Linha do tempo &lt; número >&quot;. O número é um incremento gerado automaticamente.

1. (Opcional) Para renomear uma view após sua criação, clique no menu suspenso exibir e, em seguida, clique na **Mais** menu ![](assets/more-menu.png) > **Renomear** para atualizar o nome da exibição. <!--ensure there is not another saving step here?!-->
1. (Opcional) Para gerenciar uma exibição, consulte os seguintes artigos para obter mais informações:

   * [Gerenciar a exibição de tabela](../views/manage-the-table-view.md)
   * [Gerenciar a exibição de linha do tempo](../views/manage-the-timeline-view.md)


<!--# Add a view as a favorite - this is not possible yet-->

<!-- ## Share views - not possible yet-->

## Excluir visualizações

1. No **Menu principal** ![](assets/main-menu-workfront.png) no canto superior direito da tela, <!--or the **Main Menu** ![](assets/main-menu-shell.png) in the upper-left corner of the screen, if available,--> click **Maestro** ![](assets/maestro-icon.png).

   O espaço de trabalho acessado pela última vez é aberto por padrão. Para obter informações sobre como criar espaços de trabalho, consulte [Criar espaços de trabalho](../architecture-and-fields/create-workspaces.md).
1. Clique em um cartão de tipo de registro.

   Para obter informações sobre como criar um tipo de registro, consulte [Criar tipos de registro](../architecture-and-fields/create-record-types.md).

   Por padrão, todos os registros do tipo selecionado são exibidos na exibição de tabela.

1. Clique no menu suspenso Exibir, passe o mouse sobre uma das exibições na lista e clique no botão **Mais** menu ![](assets/more-menu.png) > **Excluir**.
1. Clique em **Excluir** para confirmar. <!--ensure there is not another saving step here?!-->

   A visualização é excluída para todos os usuários que podem acessar a área Maestro e não pode ser recuperada.

<!--not possible yet - August 30, 2023: 

## Duplicate views

If you want to keep multiple versions of a view and make slight changes between the version, you can duplicate a view. Duplicating a view creates identical copies of an existing view. 

1. From the **Main Menu**, click **Maestro**. 
    The workspace you last accessed opens by default. For information about creating workspaces, see [Create workspaces](../architecture-and-fields/create-workspaces.md).
1. Click a record type. For information about creating a record type, see [Create record types](../architecture-and-fields/create-record-types.md). 

    By default, all the records of the type selected display in the table view. 

1. Click the view drop-down menu, then click the **More** menu ![](assets/more-menu.png) to the right of the view name > **Duplicate**. (**********ensure there is not another saving step here?! also, add how this view is named; the button to duplicate was there but not the functionality yet************)
    
    The view is duplicated and visible to all users who can access the Maestro area. 

-->