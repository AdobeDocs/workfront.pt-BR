---
title: Excluir Tipos de Registro
description: É possível excluir tipos de registro quando eles não forem mais relevantes. A exclusão de tipos de registro também exclui todas as informações associadas aos tipos de registro, como seus registros, campos e exibições.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 70fd3887-3871-45b5-9c21-f57da63662aa
source-git-commit: 476e10f2962f19fd17705cb5f20619d3b636aaa4
workflow-type: tm+mt
source-wordcount: '1062'
ht-degree: 0%

---


<!--keep the global record type reference in yellow till January 2026-->

# Excluir tipos de registro

<span class="preview">As informações destacadas nesta página referem-se a funcionalidades que ainda não estão disponíveis. Ela está disponível somente no ambiente de Pré-visualização para todos os clientes. Depois das versões mensais para produção, os mesmos recursos também ficam disponíveis no ambiente de produção para clientes que ativaram versões rápidas. </span>

<span class="preview">Para obter informações sobre versões rápidas, consulte [Habilitar ou desabilitar versões rápidas para sua organização](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

É possível excluir tipos de registro quando eles não forem mais relevantes.

No entanto, a exclusão de tipos de registro também exclui todas as informações associadas aos tipos de registro. Para obter mais informações, consulte a seção [Considerações ao excluir tipos de registro](#considerations-when-deleting-record-types) neste artigo.

Para obter informações sobre tipos de registros, consulte [Visão geral sobre tipos de registros](/help/quicksilver/planning/architecture/overview-of-record-types.md).

<!-- last sentence might need to be deleted when we can recover or replace deleted record types-->

## Requisitos de acesso

+++ Expanda para exibir os requisitos de acesso para a funcionalidade neste artigo. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
</tr>   
<tr> 
   <td role="rowheader"><p>Pacote do Adobe Workfront</p></td> 
   <td> 
<ul> 
<li><p>Qualquer Workfront e qualquer pacote do Planning</p></li>
Ou
<li><p>Qualquer fluxo de trabalho e qualquer pacote de planejamento</p></li></ul>
<div class="preview">
<p>Para deletar tipos de registro global:</p>
<ul><li><p>Qualquer pacote Workfront e um pacote Planning Plus</p></li>
Ou
<li><p>Qualquer fluxo de trabalho e um pacote do Planning Prime ou Ultimate</p></li></ul>
</div>
<p>Para obter mais informações sobre o que está incluído em cada pacote do Workfront Planning, entre em contato com o representante de conta da Workfront. </p> 
   </td> 
  <tr> 
   <td role="rowheader"><p>Licença do Adobe Workfront</p></td> 
   <td><p>Standard</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Permissões de objeto</p></td> 
   <td>   <p>Gerenciar permissões em um espaço de trabalho</p>  
   <p>Os administradores do sistema têm permissões para todos os espaços de trabalho, incluindo aqueles que não criaram</p>  </td> 
  </tr>  
</tbody> 
</table>

Para obter mais informações sobre requisitos de acesso do Workfront, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++   

<!--Old:
<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Products</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront Planning<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront plan*</p></td> 
   <td> 
<p>Any of the following Workfront plans:</p> 
<ul><li>Select</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning is not available for legacy Workfront plans</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront Planning package*</p></td> 
   <td> 
<p>Any </p> 
<p>For more information about what is included in each Workfront Planning plan, contact your Workfront account manager. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront platform</p></td> 
   <td> 
<p>Your organization's instance of Workfront must be onboarded to the Adobe Unified Experience to be able to access Workfront Planning.</p> 
<p>For more information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront license*</p></td> 
   <td><p> Standard</p>
   <p>Workfront Planning is not available for legacy Workfront licenses</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Access level configuration</p></td> 
   <td> <p>There are no access level controls for Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td>   <p>Manage permissions to a workspace and record type</p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p></td> 
  </tr> 
</tbody> 
</table> 
-->


## Considerações ao excluir tipos de registro

<!--check this and ensure these are still true - some things might change with / after closed beta-->

* Você pode excluir somente tipos de registro de espaços de trabalho para os quais tem permissões de gerenciamento.
* A exclusão de tipos de registro remove as seguintes informações associadas a eles:

   * Todos os registros desse tipo.
   * Todos os campos associados ao tipo de registro.
   * Todas as exibições (incluindo filtros, agrupamentos e critérios de classificação) do tipo de registro.
* O tipo de registro é removido de todos os usuários que acessam o espaço de trabalho.
* Não é possível recuperar tipos de registros excluídos ou suas informações.
* É recomendável recriar os campos e os registros associados ao tipo de registro que você deseja excluir em outro tipo de registro antes de excluí-los.

<div class="preview">

* Não é possível excluir um tipo de registro global que tenha sido adicionado a outros espaços de trabalho.

  Para obter mais informações, consulte a seção [Excluir tipos de registros globais](#delete-global-record-types) neste artigo.

</div>

## Excluir tipos de registro

{{step1-to-planning}}

1. Clique no espaço de trabalho cujos tipos de registro você deseja deletar,

   Ou

   Em um espaço de trabalho, expanda a seta apontando para baixo à direita do nome de um espaço de trabalho existente, procure um espaço de trabalho e selecione-o quando ele for exibido na lista.

   O espaço de trabalho é aberto e os tipos de registro são exibidos.
1. Siga um destes procedimentos:

   * Passe o mouse sobre o cartão de tipo de registro, clique no menu **Mais** e **Excluir**.
   * Clique no cartão do tipo de registro que deseja excluir e, na página de tipo de registro, clique no menu **Mais** ![Mais menu](assets/more-menu.png) à direita do nome do tipo de registro e clique em **Excluir**.

   ![Excluir permanentemente a confirmação do tipo de registro](assets/permanently-delete-record-type-confirmation.png)


1. Digite **excluir** na caixa de confirmação e clique em **Excluir permanentemente**. Isso não diferencia maiúsculas de minúsculas.

   O tipo de registro selecionado, juntamente com seus campos, registros associados e exibições são excluídos e não podem ser recuperados.

<div class="preview">

## Excluir tipos de registro global

Os seguintes cenários existem ao excluir tipos de registros globais:

* Se um tipo de registro configurado como global ainda não tiver sido adicionado a outro espaço de trabalho, você poderá excluí-lo do espaço de trabalho original.

* Se um tipo de registro configurado como um tipo de registro global tiver sido adicionado a pelo menos outro espaço de trabalho, você não poderá excluí-lo do espaço de trabalho original. Primeiro, você deve remover (excluindo) os tipos de registro global dos espaços de trabalho secundários em que foram adicionados e, em seguida, pode excluir permanentemente o tipo de registro global de seu espaço de trabalho original.

### Excluir um tipo de registro global do espaço de trabalho original

Você poderá excluir um tipo de registro de seu espaço de trabalho original se ele não for mais relevante.

1. Vá para o tipo de registro global em seu espaço de trabalho original.

1. (Condicional) Execute um dos seguintes procedimentos, dependendo se o tipo de registro global foi adicionado aos espaços de trabalho secundários:

   * Se o tipo de registro não tiver sido adicionado a um espaço de trabalho secundário, clique no menu **Mais** ![Mais menu](assets/more-menu.png) no cartão do tipo de registro, ou à direita do nome do tipo de registro em sua página, em seguida, clique em **Excluir**.
   * Se o tipo de registro tiver sido adicionado a pelo menos um outro espaço de trabalho secundário, primeiro, vá para o espaço de trabalho secundário e exclua o registro global desse espaço.

     Para obter informações, consulte a seção [Excluir um tipo de registro global de um espaço de trabalho secundário](#delete-a-global-record-type-from-a-secondary-workspace) neste artigo.

1. (Condicional) Continue a excluir o tipo de registro, conforme descrito na seção [Excluir tipos de registro](#delete-record-types-1) deste artigo.

   As seguintes situações ocorrem:

   * O tipo de registro global é removido do espaço de trabalho original e o tipo de registro, seus registros e campos não podem ser recuperados.
   * Todos os tipos de registros globais dos espaços de trabalho secundários e seus registros também são removidos.

### Excluir um tipo de registro global de um espaço de trabalho secundário

É possível excluir um tipo de registro adicionado de outro espaço de trabalho se não for mais necessário.

Considere o seguinte:

* A exclusão de um tipo de registro global de um espaço de trabalho secundário só o removerá do espaço de trabalho secundário. O tipo de registro permanece no espaço de trabalho original.

* Quando você deleta um tipo de registro global de um espaço de trabalho secundário, os itens a seguir também são deletados:

   * Os registros adicionados do espaço de trabalho secundário.

  <!--Coming later: * The fields added from the secondary workspace.-->

* Os tipos de registro global excluídos de seus espaços de trabalho secundários não podem ser recuperados.

* O tipo de registro original permanece em seu espaço de trabalho original, bem como em outros espaços de trabalho aos quais foi adicionado.

Para deletar um tipo de registro global de um espaço de trabalho secundário:

1. Vá para o tipo de registro global no espaço de trabalho secundário.

1. (Opcional) Clique no menu **Mais** ![Mais menu](assets/more-menu.png) no cartão do tipo de registro ou à direita do nome do tipo de registro em sua página e clique em **Excluir**.
1. (Condicional) Digite **delete** no campo fornecido e clique em **Excluir permanentemente**.

   ![Excluir caixa de confirmação do tipo de registro global secundário](assets/delete-secondary-global-record-type.png)

   As seguintes situações ocorrem:

   * O tipo de registro criado a partir de um tipo de registro global é removido do espaço de trabalho selecionado.
   * O tipo de registro original com seus campos permanecem em seu espaço de trabalho original.
   * O tipo de registro permanece em todos os outros espaços de trabalho aos quais foi adicionado.
   * Os registros <!--and fields--> adicionados ao tipo de registro do espaço de trabalho atual são excluídos. Todos os outros registros adicionados de espaços de trabalho adicionais onde o tipo de registro global foi adicionado são preservados em seus respectivos espaços de trabalho e no espaço de trabalho original. &lt;!— Os campos são preservados nos espaços de trabalho onde foram adicionados.

</div>
