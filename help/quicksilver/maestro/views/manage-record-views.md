---
title: Gerenciar exibições de registro
description: É possível exibir registros em uma exibição de tabela, linha do tempo ou calendário ao usar o Adobe Workfront Planning.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 77342724-0182-4134-903b-4428d54cdceb
source-git-commit: b11ab1dd0fdcc22cf2a99751d0aa4979556ec3fc
workflow-type: tm+mt
source-wordcount: '1085'
ht-degree: 1%

---

# Gerenciar exibições de registro

<!--update the metadata with real information when making this available in TOC and in the left nav-->

{{maestro-important-intro}}

Depois de selecionar um tipo de registro na área Adobe Workfront Planning, você pode exibir todos os registros desse tipo nas seguintes exibições:

* Tabela

  Para obter mais informações, consulte [Gerenciar a exibição de tabela](../views/manage-the-table-view.md).

* Linha do tempo

  Para obter mais informações, consulte [Gerenciar a exibição de linha do tempo](../views/manage-the-timeline-view.md).

* Calendário

  Para obter mais informações, consulte [Gerenciar a exibição de calendário](/help/quicksilver/maestro/views/manage-the-calendar-view.md).

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
   <p> Produto</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>contrato do Adobe Workfront</p></td>
   <td>
<p>Sua organização deve estar inscrita no programa beta fechado do Adobe Workfront Planning. Entre em contato com seu representante de conta para obter mais informações sobre esta nova oferta. </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>plano do Adobe Workfront</p></td>
   <td>
<p>Qualquer</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Licença do Adobe Workfront</p></td>
   <td>
   <p>Qualquer</p> 
   <p>Os administradores do sistema têm acesso somente às exibições criadas ou compartilhadas com eles. </p>
  </td>
  </tr>

<tr>
   <td role="rowheader">Configuração do nível de acesso</td>
   <td> <p>Não há controles de nível de acesso para o Workfront Planning</p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Permissões</p></td>
   <td> <p>Gerenciar permissões para a exibição</p>  
</td>
  </tr>

<tr>
   <td role="rowheader">Modelo de layout</td>
   <td> <p>O administrador do sistema deve adicionar a área Planejamento ao modelo de layout. Para obter informações, consulte <a href="../access/access-overview.md">Visão geral do Access</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

## Considerações ao trabalhar com visualizações de registro

* As exibições no Workfront Planning são específicas do tipo de registro. Não é possível aplicar a mesma exibição a dois tipos de registro diferentes.
* As exibições criadas estão visíveis somente para você e os usuários com os quais você compartilha as exibições.
* Quando você modifica ou exclui uma exibição, ela é modificada e excluída para todos os usuários que têm permissões para a exibição.
<!--* Each user can create a maximum of 100 views. -->
* Os seguintes elementos são exclusivos para cada exibição de registro:

   * Filtro
   * Agrupamento
   * Ordenar

  <!-- some of these are not available in all of the views - edit above-->

  Por exemplo, ao criar um filtro em uma exibição de tabela, os resultados do filtro ficam visíveis somente na exibição selecionada e não em todas as exibições associadas ao tipo de registro.

  >[!NOTE]
  >
  > Como o Adobe Workfront Planning atualmente está em um estado beta, alguns elementos de exibição podem não estar disponíveis para todas as exibições.

Este artigo descreve as seguintes informações sobre visualizações de registro:

* [Criar e editar uma visualização](#create-or-edit-record-views)
* [Excluir um modo de exibição](#delete-views)
* [Duplicar uma visualização](#duplicate-views)
* [Compartilhar uma exibição](#share-a-view)
  <!--* [Add a view as a favorite](#add-a-view-as-a-favorite) - not possible yet-->

## Semelhanças e diferenças entre visualizações de registro

A tabela a seguir mostra as semelhanças e diferenças entre as exibições de tabela, linha do tempo e calendário:

<!--some of these are NOT available right now; if you make this public, comment out the ones not there-->

| Recurso | Visualização em tabela | Exibição da linha do tempo | Exibição de calendário |
|-----------------------------------------------------------------------|------------|---------------|--------------|
| Exibir registros em uma lista ou tabela | ✓ µ |              | |
| Exibir todos os campos como colunas na tabela, por padrão | ✓ µ |              |    |
| Ocultar ou mostrar campos (ou colunas) | ✓ µ |               |    |
| Editar valores de campo para cada registro | ✓ µ |               |             |
| Adicionar registros como novas linhas na exibição | ✓ µ |               |        |
| Adicionar campos como novas colunas na exibição | ✓ µ |               |         |
| Copiar linhas de uma lista externa e colá-las em uma tabela | ✓ µ |               |          |
| Exibir registros em uma linha do tempo |            | ✓ µ |             |
| Filtrar registros | ✓ µ | ✓ µ | ✓ µ |
| Exibir registros em um calendário |           |              | ✓ µ |
| Registros de grupo | ✓ µ | ✓ µ |
| Classificar registros | ✓ µ |              |
| Registros de código de cores |           | ✓ µ | ✓ µ |
| Agrupamentos de código de cores |           | ✓ µ |
| Pesquisar registros específicos | ✓ µ | ✓ µ |
| Compartilhar visualização | ✓ µ | ✓ µ | ✓ µ |
| Abrir a página do registro na exibição | ✓ µ | ✓ µ |    |


## Criar ou editar exibições {#create-or-edit-views}

{{step1-to-maestro}}


O espaço de trabalho acessado pela última vez é aberto por padrão. Para obter informações sobre como criar espaços de trabalho, consulte [Criar espaços de trabalho](../architecture/create-workspaces.md).

1. Clique em um cartão de tipo de registro. Para obter informações sobre como criar um tipo de registro, consulte [Criar tipos de registro](../architecture/create-record-types.md).

   Por padrão, todos os registros do tipo selecionado são exibidos na exibição de tabela.

1. Clique em **+ Exibir** para adicionar uma nova visualização.
1. Selecione entre os seguintes tipos de exibições:

   * Tabela
   * Linha do tempo
   * Calendário

   Uma nova guia é criada com a exibição selecionada.

   Dependendo da largura da tela, podem ser exibidas visualizações adicionais no **Mais** menu ![](assets/more-menu.png).


>[!TIP]
>
>Quando você cria um tipo de registro, a exibição de tabela também é criada por padrão.
>
>Para criar uma exibição de linha do tempo ou calendário, o tipo de registro para o qual você cria a exibição deve ter pelo menos dois campos de data. Caso contrário, as opções Linha do tempo e Calendário estarão esmaecidas.
>

![](assets/view-types-drop-down-from-record-type-list.png)

>[!NOTE]
>
>    Para criar uma exibição de linha do tempo ou calendário, o tipo de registro para o qual você cria a exibição deve ter pelo menos dois campos de data. Caso contrário, as opções Linha do tempo ou Calendário estarão esmaecidas.

1. (Condicional) Clique em **Próxima**, ao criar uma exibição de linha do tempo ou calendário.

   Por padrão, o Workfront atribui à exibição um dos seguintes nomes:

   * `Table < number >`
   * `Timeline < number >`
   * `Calendar < number >`

   O número é um incremento gerado automaticamente.

1. (Condicional) Selecione a variável **Início** e **Datas finais** para os registros que serão exibidos na exibição de linha do tempo ou calendário.
1. Clique em **Criar**.

   A visualização é exibida como uma nova guia. As exibições são exibidas na ordem cronológica de quando foram criadas ou compartilhadas com você.
1. (Opcional) Clique no link **Mais** menu ![](assets/more-caret-down-icon-views.png) ao lado da última exibição para exibir todas as exibições do tipo de registro selecionado.

   Exibições adicionais são exibidas sob o **Mais** após a última guia view. O número ao lado do **Mais** mostra o número de visualizações adicionais.
1. (Opcional) Para renomear uma view após sua criação, clique no menu suspenso exibir e, em seguida, clique na **Mais** menu ![](assets/more-menu.png) > **Renomear** para atualizar o nome da exibição

   Ou

   Clique duas vezes no nome da exibição e comece a digitar o novo nome.  <!--ensure there is not another saving step here?!-->

1. (Opcional) Para gerenciar um tipo específico de visualização, consulte os seguintes artigos:

   * [Gerenciar a exibição de tabela](../views/manage-the-table-view.md)
   * [Gerenciar a exibição de linha do tempo](../views/manage-the-timeline-view.md)
   * [Gerenciar a exibição de calendário](/help/quicksilver/maestro/views/manage-the-calendar-view.md)


## Excluir visualizações

{{step1-to-maestro}}

O espaço de trabalho acessado pela última vez é aberto por padrão. Para obter informações sobre como criar espaços de trabalho, consulte [Criar espaços de trabalho](../architecture/create-workspaces.md).

1. Clique em um cartão de tipo de registro.

   Para obter informações sobre como criar um tipo de registro, consulte [Criar tipos de registro](../architecture/create-record-types.md).

   Por padrão, todos os registros do tipo selecionado são exibidos na exibição de tabela.

1. Passe o mouse sobre um dos nomes da exibição na guia Exibir e clique em **Mais** ![](assets/more-menu.png) à esquerda do nome da exibição, clique em **Excluir**.
Primeiro, talvez seja necessário clicar em **Mais** à esquerda da última guia para localizar a exibição que deseja excluir.

1. Clique em **Excluir** para confirmar. <!--ensure there is not another saving step here?!-->

   A exibição é excluída para todos os usuários que podem acessar a área de registros e não pode ser recuperada.

## Compartilhar uma exibição

Para obter informações sobre o compartilhamento de exibições, consulte [Compartilhar exibições](/help/quicksilver/maestro/access/share-views.md).

<!--## Add a view as a favorite - this is not possible yet-->

<!--not possible yet - August 30, 2023: -->

## Duplicar uma visualização

Se quiser manter várias versões de uma exibição e fazer pequenas alterações entre as versões, você poderá duplicar uma exibição.

A duplicação de uma exibição cria cópias idênticas de uma exibição existente.

As permissões de compartilhamento da exibição original não são transferidas para a exibição duplicada.

{{step1-to-maestro}}

O espaço de trabalho acessado pela última vez é aberto por padrão.

Para obter informações sobre como criar espaços de trabalho, consulte [Criar espaços de trabalho](../architecture/create-workspaces.md).

1. Clique em um cartão de tipo de registro. Para obter informações sobre como criar um tipo de registro, consulte [Criar tipos de registro](../architecture/create-record-types.md).

   Por padrão, todos os registros do tipo selecionado são exibidos na exibição de tabela.

1. Passe o mouse sobre a guia da exibição que deseja duplicar e clique no ícone **Mais** menu ![](assets/more-menu.png) à direita do nome da exibição, clique em **Duplicar**.

   ![](assets/view-more-menu-with-duplicate-option.png)


   A visualização é duplicada e o nome da nova visualização segue o seguinte padrão: `Original view's name (Copy)`. A nova guia de exibição é exibida no final de todas as guias de exibição.

