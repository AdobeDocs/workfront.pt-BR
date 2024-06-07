---
title: Criar espaços de trabalho
description: Um espaço de trabalho é uma coleção de tipos de registro usados por uma equipe e representa o ciclo de vida do trabalho da equipe. Você pode personalizar totalmente os espaços de trabalho no Adobe Workfront Planning. Os tipos de registro são organizados por seções em um espaço de trabalho.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 604b84c1-4ec6-4d4a-b9f4-4223641ff2ea
source-git-commit: c593eab154a0942995b1f913e7189450913faac0
workflow-type: tm+mt
source-wordcount: '635'
ht-degree: 1%

---

<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

# Criar espaços de trabalho

{{planning-important-intro}}

No Adobe Workfront Planning, os espaços de trabalho são locais centralizados para as equipes planejarem o trabalho.

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
<p>Sua organização deve estar inscrita no estágio de acesso antecipado do Workfront Planning </p>
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
   <td> <p>Não há controles de nível de acesso para o Adobe Workfront Planning</p>
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Permissões</p></td>
   <td> <p>Você recebe permissões para Gerenciar os espaços de trabalho criados. </p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Modelo de layout</p></td>
   <td> <p>Você deve adicionar a área do Planning ao seu modelo de layout. Para obter informações, consulte <a href="/help/quicksilver/planning/access/access-overview.md">Visão geral do Access</a>. </p>  
</td>
  </tr>

</tbody>
</table>

Para obter mais informações sobre requisitos de acesso, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

<!--Maybe enable this at GA - but Planning is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](/help/quicksilver/administration-and-setup/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->

<!-- Notes for the table: for the "Workfront access" row: <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p>-->

## Considerações sobre espaços de trabalho

* Você pode criar espaços de trabalho para unidades organizacionais específicas na sua organização, para corresponder à maneira exclusiva como cada unidade funciona.
* Os tipos de registro que um espaço de trabalho contém devem refletir o ciclo de vida de trabalho de uma unidade organizacional.
* Ao criar um espaço de trabalho, somente você tem permissão para acessar e gerenciar seu espaço de trabalho. Você deve compartilhá-lo com outros usuários para que eles colaborem com você no mesmo espaço. Para obter informações, consulte [Compartilhar um espaço de trabalho](/help/quicksilver/planning/access/share-workspaces.md). Os administradores do sistema podem gerenciar todos os espaços de trabalho, mesmo aqueles que não criaram.
* Você pode ter o seguinte:

   * Até 50 seções em um espaço de trabalho.
   * Até um total de 1.000 tipos de registro de todas as seções em um espaço de trabalho. Todos os tipos de registro são exclusivos para cada espaço de trabalho. <!--this might change-->
   * Até 1.000 espaços de trabalho na instância do Workfront da sua organização.


## Criar um espaço de trabalho

Você pode criar um espaço de trabalho e adicionar tipos de registro a ele para organizar seus objetos no Workfront Planning. Para obter mais informações sobre a edição de um espaço de trabalho, consulte [Editar espaços de trabalho](/help/quicksilver/planning/architecture/edit-workspaces.md).

{{step1-to-planning}}

1. Clique em **Criar espaço de trabalho**

   A caixa Criar espaço de trabalho é exibida. Você pode criar um espaço de trabalho do zero ou criá-lo usando um dos modelos disponíveis.

1. (Opcional e condicional) Clique em **Visualizar** em qualquer um dos modelos de espaço de trabalho predefinidos a seguir:

   * Gerenciamento de marketing
   * Gerenciamento de vendas
   * Gerenciamento de produtos

   A caixa de pré-visualização do modelo é aberta.

   Há uma indicação de quais tipos de registro operacional, taxonomias e quantos campos estão associados a cada modelo.

   ![](assets/previewing-a-workspace-template.png)

   Para obter informações sobre modelos do Workfront Planning Workspace, consulte [Lista de modelos do espaço de trabalho](/help/quicksilver/planning/architecture/workspace-templates.md).

1. Na caixa de visualização do modelo, clique em **Usar modelo** para começar a criar o espaço de trabalho a partir do modelo selecionado

   Ou

   Clique em **Voltar** e, em seguida, clique em **Criar espaço de trabalho** para criar um espaço de trabalho do zero.

   Um para os seguintes tipos de espaços de trabalho é criado:

   * Um espaço de trabalho vazio chamado **Espaço de trabalho sem título** onde você pode começar a adicionar tipos de registro manualmente ao criar um espaço de trabalho do zero.
   * Um espaço de trabalho nomeado com base no modelo selecionado que é preenchido com tipos de registro de amostra. É possível personalizar ainda mais os tipos de registro e o espaço de trabalho.

1. Clique dentro do nome do espaço de trabalho no cabeçalho do novo espaço de trabalho para renomeá-lo e pressione Enter.

1. (Opcional e condicional) Se você criou o espaço de trabalho a partir de um modelo, clique dentro do nome do **Tipos de Registro Operacional** ou **Taxonomias** seções

   Ou

   Passe o mouse sobre o nome de uma seção e clique no **Mais** menu ![](assets/more-menu.png)e, em seguida, clique em **Renomear** para renomear a seção.

   >[!TIP]
   >
   >É possível renomear qualquer seção de qualquer espaço de trabalho, mesmo que você não tenha criado a seção.

   Para obter mais informações sobre a edição de espaços de trabalho, incluindo a edição de seções do espaço de trabalho, consulte [Editar espaços de trabalho](/help/quicksilver/planning/architecture/edit-workspaces.md).

1. (Opcional) Clique em **Adicionar tipo de registro** para adicionar tipos de registro ao espaço de trabalho em qualquer seção.

   Para obter informações, consulte [Criar tipos de registro](/help/quicksilver/planning/architecture/create-record-types.md).

   Para obter mais informações sobre edição e exclusão de tipos de registro em um espaço de trabalho, consulte [Editar espaços de trabalho](/help/quicksilver/planning/architecture/edit-workspaces.md).


