---
title: Criar espaços de trabalho
description: Um espaço de trabalho é uma coleção de tipos de registros operacionais e taxonomias usadas por uma equipe e representa o ciclo de vida do trabalho da equipe. Você pode personalizar totalmente os espaços de trabalho no Maestro.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 604b84c1-4ec6-4d4a-b9f4-4223641ff2ea
source-git-commit: 811eb1453c140808b0d6c5d9a3b4a0729cb16b2d
workflow-type: tm+mt
source-wordcount: '559'
ht-degree: 0%

---

<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

# Criar espaços de trabalho

>[!IMPORTANT]
>
>As informações neste artigo referem-se ao Adobe Maestro, que é uma nova oferta da Adobe Workfront.
>
>Atualmente, o Adobe Maestro faz parte de um programa beta aberto a um número limitado de clientes. Você deve ser um cliente do Workfront para usar os recursos do Maestro.
>
>Entre em contato com seu representante de conta para obter mais informações sobre como participar do programa beta para o Maestro.
>
>Para obter informações, consulte [Visão geral do Adobe Maestri](../maestro-overview.md).

No Adobe Maestri, os espaços de trabalho são locais centralizados para as equipes planejarem o trabalho.

Um espaço de trabalho é uma coleção de tipos de registros operacionais e taxonomias usadas por uma equipe e representa o ciclo de vida do trabalho da equipe. Você pode personalizar totalmente os espaços de trabalho no Maestro.

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
<p>Sua organização deve estar inscrita no programa beta fechado do Adobe Maestro. Entre em contato com seu representante de conta para obter mais informações sobre esta nova oferta. </p>
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
   <td> <p>Não há controles de nível de acesso para o Maestro</p>
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Permissões</p></td>
   <td> <p>Você recebe permissões para Gerenciar os espaços de trabalho criados. </p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Modelo de layout</p></td>
   <td> <p>Você deve adicionar a área Maestro ao modelo de layout. Para obter informações, consulte <a href="../access/access-overview.md">Visão geral do Access</a>. </p>  
</td>
  </tr>

</tbody>
</table>

Para obter mais informações sobre requisitos de acesso, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

<!--Maybe enable this at GA - but Maestro is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->

<!-- Notes for the table: for the "Workfront access" row: <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p>-->

## Considerações sobre espaços de trabalho

* Você pode criar espaços de trabalho para unidades organizacionais específicas na sua organização, para corresponder à maneira exclusiva como cada unidade funciona.
* Os tipos de registro e taxonomias contidos em um espaço de trabalho devem refletir o ciclo de vida do trabalho de uma unidade organizacional.
* Ao criar um espaço de trabalho, somente você tem permissão para acessar e gerenciar seu espaço de trabalho. Você deve compartilhá-lo com outros usuários para que eles colaborem com você no mesmo espaço. Para obter informações, consulte [Compartilhar um espaço de trabalho](/help/quicksilver/maestro/access/share-workspaces.md).
* Você pode ter no máximo 1.000 espaços de trabalho em sua organização.
* Os espaços de trabalho contêm tipos de registro exclusivos para cada espaço de trabalho. <!--this might change-->

## Criar um espaço de trabalho

{{step1-to-maestro}}

1. (Condicional) Se você não tiver espaços de trabalho no seu ambiente, clique em **Criar espaço de trabalho**

   Ou, em um espaço de trabalho existente, clique no ponto para baixo à direita do nome do espaço de trabalho e clique em **Criar espaço de trabalho**.

   ![](assets/workspace-drop-down-right-menu.png)

   Isso abre a área Espaços de trabalho do Maestro.
1. (Opcional e condicional) Clique em **Visualizar** em qualquer um dos modelos de espaço de trabalho predefinidos a seguir:

   * Gerenciamento de marketing
   * Gerenciamento de vendas
   * Gerenciamento de produtos

   Há uma indicação de quais tipos de registro operacional, taxonomias e quantos campos estão associados a cada modelo.

   ![](assets/previewing-a-workspace-template.png)

   Para obter informações sobre modelos do espaço de trabalho Maestro, consulte [Lista de modelos do espaço de trabalho](../architecture/workspace-templates.md).

1. Clique em **Usar modelo** para começar a criar o espaço de trabalho a partir do modelo selecionado

   Ou

   Clique em **Criar espaço de trabalho** para criar um espaço de trabalho do zero.

   Um para os seguintes tipos de espaços de trabalho é criado:

   * Um espaço de trabalho vazio em que você pode começar a adicionar tipos de registro manualmente.
   * Um espaço de trabalho preenchido com exemplos de tipos de registro que podem ser personalizados.

1. Clique dentro do nome do espaço de trabalho no cabeçalho do novo espaço de trabalho para renomeá-lo e pressione Enter

   Ou

   Clique em **Mais** menu ![](assets/more-menu.png)à direita do nome do espaço de trabalho no cabeçalho e clique em **Renomear**.

1. (Opcional) Clique em **Adicionar tipo de registro** para adicionar tipos de registro ao espaço de trabalho.

   Para obter informações, consulte [Criar tipos de registro](../architecture/create-record-types.md).

1. (Opcional) Clique em **Adicionar taxonomia** para adicionar taxonomias ao espaço de trabalho.

   Para obter informações, consulte [Criar taxonomias](../architecture/create-a-taxonomy.md).
