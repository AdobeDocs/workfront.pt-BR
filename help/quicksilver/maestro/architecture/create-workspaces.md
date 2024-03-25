---
title: Criar espaços de trabalho
description: Um espaço de trabalho é uma coleção de tipos de registro usados por uma equipe e representa o ciclo de vida do trabalho da equipe. Você pode personalizar totalmente os espaços de trabalho no Adobe Workfront Planning.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 604b84c1-4ec6-4d4a-b9f4-4223641ff2ea
source-git-commit: 130365bfa220337aa25f27ba03742ea3471972cb
workflow-type: tm+mt
source-wordcount: '698'
ht-degree: 0%

---

<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

# Criar espaços de trabalho

{{maestro-important-intro}}

No planejamento do Adobe Workfront, os espaços de trabalho são locais centralizados para as equipes planejarem o trabalho.

Um espaço de trabalho é uma coleção de tipos de registro usados por uma equipe e representa o ciclo de vida do trabalho da equipe. Você pode personalizar totalmente os espaços de trabalho no Adobe Workfront Planning.

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
<p>Sua organização deve estar inscrita no programa beta fechado de planejamento do Adobe Workfront. Entre em contato com seu representante de conta para obter mais informações sobre esta nova oferta. </p>
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
   Ou
   <p>Atual: Plano</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>Configuração do nível de acesso</p></td>
   <td> <p>Não há controles de nível de acesso para o planejamento do Adobe Workfront</p>
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Permissões</p></td>
   <td> <p>Você recebe permissões para Gerenciar os espaços de trabalho criados. </p>  
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

<!--Maybe enable this at GA - but Planning is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->

<!-- Notes for the table: for the "Workfront access" row: <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p>-->

## Considerações sobre espaços de trabalho

* Você pode criar espaços de trabalho para unidades organizacionais específicas na sua organização, para corresponder à maneira exclusiva como cada unidade funciona.
* Os tipos de registro que um espaço de trabalho contém devem refletir o ciclo de vida de trabalho de uma unidade organizacional.
* Ao criar um espaço de trabalho, somente você tem permissão para acessar e gerenciar seu espaço de trabalho. Você deve compartilhá-lo com outros usuários para que eles colaborem com você no mesmo espaço. Para obter informações, consulte [Compartilhar um espaço de trabalho](/help/quicksilver/maestro/access/share-workspaces.md). Os administradores do sistema podem gerenciar todos os espaços de trabalho, mesmo aqueles que não criaram.
* Você pode ter no máximo 1.000 espaços de trabalho na instância do Workfront da sua organização.
* Os espaços de trabalho contêm tipos de registro exclusivos para cada espaço de trabalho. <!--this might change-->

## Criar um espaço de trabalho

{{step1-to-maestro}}

1. (Condicional) Se você não tiver espaços de trabalho no seu ambiente, clique em **Criar espaço de trabalho**

   Ou, em um espaço de trabalho existente, clique no ponto para baixo à direita do nome do espaço de trabalho e clique em **Criar espaço de trabalho**.

   ![](assets/workspace-drop-down-right-menu.png)

   Isso abre a área Espaços de trabalho do Workfront Planning.
1. (Opcional e condicional) Clique em **Visualizar** em qualquer um dos modelos de espaço de trabalho predefinidos a seguir:

   * Gerenciamento de marketing
   * Gerenciamento de vendas
   * Gerenciamento de produtos

   Há uma indicação de quais tipos de registro operacional, taxonomias e quantos campos estão associados a cada modelo.

   ![](assets/previewing-a-workspace-template.png)

   Para obter informações sobre modelos do Workfront planning workspace, consulte [Lista de modelos do espaço de trabalho](../architecture/workspace-templates.md).

1. Clique em **Usar modelo** para começar a criar o espaço de trabalho a partir do modelo selecionado

   Ou

   Clique em **Criar espaço de trabalho** para criar um espaço de trabalho do zero.

   Um para os seguintes tipos de espaços de trabalho é criado:

   * Um espaço de trabalho vazio em que você pode começar a adicionar tipos de registro manualmente ao criar um espaço de trabalho do zero.
   * Um espaço de trabalho preenchido com tipos de registro de amostra que você pode personalizar ainda mais, ao usar um dos modelos.

1. Clique dentro do nome do espaço de trabalho no cabeçalho do novo espaço de trabalho para renomeá-lo e pressione Enter

   Ou

   Clique em **Mais** menu ![](assets/more-menu.png)à direita do nome do espaço de trabalho no cabeçalho e clique em **Renomear**.

1. (Opcional e condicional) Se o espaço de trabalho já tiver seções, clique em **Adicionar seção** para adicionar uma nova seção a um espaço de trabalho. Uma seção pode conter vários tipos de registro.

1. (Opcional e condicional) Se você criou o espaço de trabalho a partir de um modelo, clique dentro do nome do **Tipos de Registro Operacional** ou **Taxonomias** seções

   Ou

   Passe o mouse sobre o nome de uma seção e clique no **Mais** menu ![](assets/more-menu.png)e, em seguida, clique em **Renomear** para renomear a seção.

   >[!TIP]
   >
   >É possível renomear qualquer seção de qualquer espaço de trabalho, mesmo que a tenha criado.

1. (Opcional) Para alterar o local de uma seção, siga um destes procedimentos:

   * Passe o mouse sobre o nome de uma seção e clique no **agarrar** ícone ![](assets/grab-icon.png), em seguida, arraste e solte-o no ponto correto.
   * Passe o mouse sobre o nome de uma seção e clique no **Mais** menu ![](assets/more-menu.png)e, em seguida, clique em **Mover para cima** ou **Mover para baixo**. A seção se move para cima ou para baixo dentro do espaço de trabalho.

1. (Opcional) Para adicionar uma nova seção, siga um destes procedimentos:

   * Clique em **Adicionar seção** na parte inferior do espaço de trabalho.
   * Passe o mouse sobre o nome de uma seção e clique no **Mais** menu ![](assets/more-menu.png)e, em seguida, clique em **Adicionar seção acima** ou **Adicionar seção abaixo**.

1. (Opcional) Clique em **Adicionar tipo de registro** para adicionar tipos de registro ao espaço de trabalho.

   Para obter informações, consulte [Criar tipos de registro](../architecture/create-record-types.md).


