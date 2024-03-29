---
title: Editar tipos de registro
description: Você poderá editar os tipos de registro depois que eles forem salvos. Os tipos de registro são os tipos de objeto do Adobe Workfront Planning.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 7d6de742-9657-4286-968c-1fc78ebbb94e
source-git-commit: a0f12a016ae8ac73136f05bf3255f9882e2ce6d4
workflow-type: tm+mt
source-wordcount: '455'
ht-degree: 0%

---

<!--update the metadata with real information when making this available in TOC and in the left nav
---
title: Edit record types
description: You can edit record types after they have been saved. Record types are the object types of Adobe Workfront planning.
author: Alina
role: User
feature: Work Management 
topic: Architecture
hidefromtoc: yes
hide: yes
---

-->

# Editar tipos de registro

{{maestro-important-intro}}

Os tipos de registro são os tipos de objeto do Adobe Workfront Planning. É possível editar a aparência dos tipos de registros criados por você ou por qualquer outra pessoa. Para obter informações sobre a criação de tipos de registro do Workfront Planning, consulte [Criar tipos de registro](../architecture/create-record-types.md).

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
   <p> Adobe Workfront</p> <p>Para conectar os tipos de registro de planejamento do Adobe Workfront com o Experience Manager Assets, você deve ter uma licença do Adobe Experience Manager Assets e a instância da Workfront de sua organização deve ser integrada à Adobe Business Platform ou à Adobe Admin Console.</p> </td>
  </tr>  
 <td role="rowheader"><p>contrato do Adobe Workfront</p></td>
   <td>
<p>Sua organização deve estar inscrita no programa beta fechado de planejamento da Adobe Workfront. Entre em contato com seu representante de conta para obter mais informações sobre esta nova oferta. </p>
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
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>Configurações de nível de acesso</p></td>
   <td> <p>Não há controles de nível de acesso para o planejamento do Workfront</p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Permissões</p></td>
   <td> <p>Gerenciar permissões em um espaço de trabalho</a> </p>  
   <p>Os administradores do sistema têm permissões para todos os espaços de trabalho, incluindo aqueles que não criaram
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Modelo de layout</p></td>
   <td> <p>O administrador do Workfront ou do grupo deve adicionar a área do Planning ao modelo de layout. Para obter informações, consulte <a href="../access/access-overview.md">Visão geral do Access</a>. </p>  
</td>
  </tr>

</tbody>
</table>

<!--Maybe enable this at GA - but Planning is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

## Editar tipos de registro

{{step1-to-maestro}}

O espaço de trabalho acessado por último deve ser aberto por padrão.

1. (Opcional) Expanda a seta apontando para baixo à direita de um nome de espaço de trabalho existente e selecione o espaço de trabalho para o qual deseja editar tipos de registro.
1. Passe o mouse sobre o cartão de um tipo de registro e clique no **Mais** menu ![](assets/more-menu.png) no canto superior direito do cartão de tipo de registro e clique em **Atualizar aparência**.

   ![](assets/update-appearance-link-from-more-menu-on-record-type-card.png)

1. No **Atualizar tipo de registro** , atualize as seguintes informações:

   * **Nome do registro**: edite o nome do tipo de registro, se necessário. <!--correct this - I asked Garik to change this field to "Record type name"-->
   * **Aparência**: Edite a cor e a forma do ícone associado ao tipo de registro. Faça o seguinte:
      * Selecione uma cor para identificar o tipo de registro. Esta é a cor do ícone do tipo de registro. O cinza é selecionado por padrão.
      * Selecione um ícone na lista ou comece a digitar o nome de um ícone para descrever o que ele representa e, em seguida, selecione-o quando ele for exibido. Este é o ícone do tipo de registro. Um ícone de arquivo é selecionado por padrão.

     ![](assets/update-record-type-box.png)

1. Clique fora da **Atualizar tipo de registro** para salvar as alterações.
1. (Opcional) Clique no cartão de tipo de registro na área do espaço de trabalho para abrir a página do tipo de registro.
1. Clique em **Mais** à direita do nome do tipo de registro e clique em **Renomear** para renomear o tipo de registro

   Ou

   Renomeie o tipo de registro no cabeçalho.  <!--check to see if they renamed this to "Rename" - it kept going back and forth between Rename and Edit-->

   ![](assets/more-menu-options-from-record-details-page.png) <!--check this screen shot - not sure this is valid ???-->

   Você também pode renomear um tipo de registro no cabeçalho da página do tipo de registro.
1. (Opcional) Expanda a seta apontando para baixo à direita de um nome de tipo de registro e selecione outro tipo de registro para editar.
