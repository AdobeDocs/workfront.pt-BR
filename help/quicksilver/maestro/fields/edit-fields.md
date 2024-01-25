---
title: Editar campos
description: No Adobe Maestri, você pode editar as configurações de campo para campos já criados.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 6c35c313-d6ed-428b-b70d-2ea242da4e8f
source-git-commit: c264c0c96b818934a7c25ed54c7666d2d6c95e54
workflow-type: tm+mt
source-wordcount: '528'
ht-degree: 0%

---

<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

<!---
title: Edit foelds
description: In Adobe Maestro, you can edit the field settings for fields that are already created.
hidefromtoc: yes
hide: yes
author: Alina
feature: (*******************WE NEED A NEW ONE*******************)
role: User, Administrator (************is this right???************)
recommendations: noDisplay, noCatalog
--->


# Editar campos

>[!IMPORTANT]
>
>As informações neste artigo referem-se ao Adobe Maestro, que é uma nova oferta da Adobe Workfront.
>
>Atualmente, o Adobe Maestro faz parte de um programa beta aberto a um número limitado de clientes. Você deve ser um cliente do Workfront para usar os recursos do Maestro.
>
>Entre em contato com seu representante de conta para obter mais informações sobre como participar do programa beta para o Maestro.
>
>Para obter informações, consulte [Visão geral do Adobe Maestri](../maestro-overview.md).

É possível editar as configurações de campo para campos já criados.

Para obter informações sobre como criar campos do Adobe Maestri, consulte [Criar campos](../fields/create-fields.md).

Este artigo descreve como você pode editar as configurações para campos Maestro. Para obter informações sobre a edição de valores de campo para registros Maestro, consulte [Editar registros](/help/quicksilver/maestro/records/edit-records.md).

## Considerações sobre a edição de informações de campo

* É possível editar campos criados ou campos criados por outros usuários, se você tiver permissões de gerenciamento para o espaço de trabalho ao qual os campos pertencem.
* É possível editar um campo na tabela de tipo de registro.
* Não é possível editar um campo na página Detalhes de um registro ou na exibição de linha do tempo.
* Não é possível editar o tipo de campo depois que o campo é salvo.
* Não é possível desmarcar a configuração Permitir números negativos que foi selecionada anteriormente para um campo Número, Porcentagem ou Moeda se já houver valores negativos armazenados nos registros aos quais está anexado.
<!--this is not true yet; one piece of it is true and I added it as the bullet above: 
* You cannot edit the options, or the special format of the following fields, after they are saved:

    * Allow negative numbers option from a Number, Percentage, or Currency field. 
    * The Options of a Single-select or a Multi-select field.
-->

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
   <td role="rowheader"><p>Licença do Adobe Workfront</p></td>
   <td>
   <p>Qualquer</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>Configuração do nível de acesso</p></td>
   <td> <p>Não há controles de acesso para o Maestro</p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Permissões</p></td>
   <td> <p>Gerenciar permissões em um espaço de trabalho</a> </p>  
   <p>Os administradores do sistema têm permissões para todos os espaços de trabalho, incluindo aqueles que não criaram</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Modelo de layout</p></td>
   <td> <p>O administrador do Workfront ou do grupo deve adicionar a área Maestri no modelo de layout. Para obter informações, consulte <a href="../access/access-overview.md">Visão geral do Access</a>. </p>  
</td>
  </tr>

</tbody>
</table>

<!--Maybe enable this at GA - but Maestro is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

## Editar campos

1. Clique em **Menu principal** ícone ![](assets/main-menu-workfront.png) no canto superior direito do Workfront ou na guia **Menu principal** ícone ![](assets/main-menu-shell.png)  no canto superior esquerdo, se disponível, clique em **Maestro** ![](assets/maestro-icon.png).

   O espaço de trabalho acessado por último deve ser aberto por padrão.

1. (Opcional) Expanda a seta apontando para baixo à direita de um nome de espaço de trabalho existente e selecione o espaço de trabalho para o qual deseja excluir tipos de registro.

   O espaço de trabalho é aberto e os tipos de registro e taxonomias associadas a ele são exibidos.
1. Clique no cartão do tipo de registro ou na taxonomia cujos campos você deseja editar.

   Essa ação abre a página do tipo de registro.
1. (Condicional) Selecione um **Visualização em tabela** do **Exibir** no canto superior direito da página tipo de registro.
1. Passe o mouse sobre o cabeçalho da coluna de um campo que deseja editar, clique na seta para baixo após o nome do campo e clique em **Editar campo**

   Ou

   Clique duas vezes no cabeçalho da coluna do campo.

   ![](assets/arrow-menu-after-name-of-field-in-table-header-highlighted.png)

1. Atualize as informações sobre o campo e clique em **Salvar**.

   <!--insert screen shot when finalized-->

   >[!TIP]
   >
   >Não é possível atualizar o tipo de campo depois que o campo é salvo.


1. (Condicional) Para campos de registro vinculados, clique em **Editar campos de pesquisa** e adicionar ou remover qualquer um dos campos do tipo de registro vinculado.

   Para obter mais informações, consulte [Conectar tipos de registro](../architecture/connect-record-types.md).
