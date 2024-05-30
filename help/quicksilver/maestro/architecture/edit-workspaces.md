---
title: Editar espaços de trabalho
description: É possível editar as informações de um espaço de trabalho existente, como renomeá-lo.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 374b6d9c-69a9-4a73-8708-51c14a78c7c9
source-git-commit: 49335ec86057e4985477034558a271bf4efcab5e
workflow-type: tm+mt
source-wordcount: '561'
ht-degree: 0%

---

<!--update the metadata with real information when making this available in TOC and in the left nav-->

# Editar espaços de trabalho

{{planning-important-intro}}

No Adobe Workfront Planning, os espaços de trabalho são locais centralizados para as equipes planejarem o trabalho.

Um espaço de trabalho é uma coleção de tipos de registro usados por uma equipe e representa o ciclo de vida do trabalho da equipe. Você pode personalizar totalmente os espaços de trabalho no Adobe Workfront Planning.

Para obter informações sobre como criar espaços de trabalho, consulte [Criar espaços de trabalho](/help/quicksilver/maestro/architecture/create-workspaces.md).

Todas as alterações feitas em um espaço de trabalho ficam visíveis para todos aqueles que têm pelo menos permissões de Exibição para o espaço de trabalho.

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
   <td role="rowheader"><p>Licença da Adobe Workfront*</p></td>
   <td>
   <p>Novo: Padrão</p>
   <p>Atual: Plano</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>Configuração do nível de acesso</p></td>
   <td> <p>Não há controles de nível de acesso para o Workfront Planning</p>
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Permissões</p></td>
   <td> <p>Gerenciar permissões no espaço de trabalho </p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Modelo de layout</p></td>
   <td> <p>Você deve adicionar a área do Planning ao seu modelo de layout. Para obter informações, consulte <a href="../access/access-overview.md">Visão geral do Access</a>. </p>  
</td>
  </tr>

</tbody>
</table>

Para obter mais informações sobre requisitos de acesso, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).


## Editar um espaço de trabalho

{{step1-to-maestro}}

Isso abre a área Espaços de trabalho do Workfront Planning.

1. Clique dentro do nome do espaço de trabalho no cabeçalho do novo espaço de trabalho para renomeá-lo e pressione **Enter**.
1. Clique em **Mais** menu ![](assets/more-menu.png)à direita do nome do espaço de trabalho no cabeçalho e clique em **Editar**.

   ![](assets/edit-workspace-box.png)

   Atualize as seguintes informações no **Editar espaço de trabalho** caixa:

   * Adicione um nome ao espaço de trabalho. <!--did they add a label for this field?-->
   * **Descrição**: adicione informações sobre o espaço de trabalho.
   * Selecione um ícone para associar ao espaço de trabalho.

1. Clique em **Salvar** para fechar a caixa Editar espaço de trabalho e aplicar as alterações.

1. (Opcional) Para adicionar uma nova seção do espaço de trabalho, siga um destes procedimentos:

   * Clique em **Adicionar seção** na parte inferior do espaço de trabalho.
   * Passe o mouse sobre o nome de uma seção e clique no **Mais** menu ![](assets/more-menu.png)e, em seguida, clique em **Adicionar seção acima** ou **Adicionar seção abaixo**.

1. (Opcional) Para alterar o local de uma seção, siga um destes procedimentos:

   * Passe o mouse sobre o nome de uma seção e clique no **agarrar** ícone ![](assets/grab-icon.png), em seguida, arraste e solte-o no ponto correto.
   * Passe o mouse sobre o nome de uma seção e clique no **Mais** menu ![](assets/more-menu.png)e, em seguida, clique em **Mover para cima** ou **Mover para baixo**. A seção se move para cima ou para baixo dentro do espaço de trabalho.

1. (Opcional) Para excluir uma seção do espaço de trabalho, faça o seguinte:

   1. Passe o mouse sobre o nome de uma seção, em seguida, clique no **Mais** menu ![](assets/more-menu.png)e, em seguida, clique em **Excluir**. <!--add screen shot when UI is final?-->
   1. Selecione uma nova seção para mover todos os tipos de registro para ela e clique em **Excluir**. <!--check the button name; logged a bug to change it to "Delete" from "Delete section".-->

      Todos os tipos de registro são movidos para a seção de seleção, e a seção é excluída.

1. (Opcional) Clique em **Adicionar tipo de registro** para adicionar tipos de registro ao espaço de trabalho.

   Para obter informações, consulte [Criar tipos de registro](../architecture/create-record-types.md).

1. (Opcional) Passe o mouse sobre um cartão de tipo de registro, clique no **Mais** menu ![](assets/more-menu.png) no canto superior direito e clique em **Editar** para modificar a aparência de um tipo de registro.

   Para obter informações, consulte [Editar tipos de registro](/help/quicksilver/maestro/architecture/edit-record-types.md).

1. (Opcional) Passe o mouse sobre um cartão de tipo de registro, clique no **Mais** menu ![](assets/more-menu.png) no canto superior direito e clique em **Excluir** para excluir um tipo de registro.

   Para obter informações, consulte [Excluir tipos de registro](/help/quicksilver/maestro/architecture/delete-record-types.md).

1. (Opcional) Pressione e clique em um cartão de tipo de registro para arrastá-lo e soltá-lo em um novo ponto. Você pode arrastar e soltar tipos de registro de uma seção do espaço de trabalho para outra.

   ![](assets/drag-and-drop-record-types-in-a-workspace.png)

1. (Opcional) Clique em **Compartilhar** no canto superior direito do espaço de trabalho para compartilhá-lo com outras pessoas.

   Para obter informações, consulte [Compartilhar espaços de trabalho](/help/quicksilver/maestro/access/share-workspaces.md).
