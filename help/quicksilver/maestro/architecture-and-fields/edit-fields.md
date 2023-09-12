---
title: Editar campos
description: No Adobe Maestri, você pode editar as configurações de campo para campos já criados.
hidefromtoc: true
hide: true
source-git-commit: 6e219089f68db651f5eb8369e3c6df83b6cd823b
workflow-type: tm+mt
source-wordcount: '428'
ht-degree: 1%

---


<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

# Editar campos

>[!IMPORTANT]
>
>Atualmente, o Adobe Maestro faz parte de um programa beta fechado que está aberto a um número limitado de clientes.
>
>Entre em contato com seu representante de conta para obter mais informações sobre como participar do programa beta para o Maestro.
>
>Para obter informações, consulte [Visão geral do Adobe Maestri](../maestro-overview.md).

É possível editar as configurações de campo para campos já criados.

Para obter informações sobre como criar campos do Adobe Maestri, consulte [Criar campos](../architecture-and-fields/create-fields.md).

Este artigo descreve como você pode editar as configurações para campos Maestro. Para obter informações sobre a edição de valores de campo para registros Maestro, consulte [Editar registros](../records/edit-records.md).

## Considerações sobre a edição de informações de campo

* É possível editar campos criados ou campos criados por outros usuários. <!--this will change with access levels/ permissions-->
* É possível editar um campo na tabela de tipo de registro.
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
 <tbody>
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

## Editar campos

1. Clique em **Menu principal** ícone ![](assets/main-menu-workfront.png) no canto superior direito do Workfront, <!---or the **Main menu** icon ![](assets/main-menu-shell.png)  in the upper-left corner, if available--> e clique em **Maestro** ![](assets/maestro-icon.png).

   O espaço de trabalho acessado por último deve ser aberto por padrão.

1. (Opcional) Expanda a seta apontando para baixo à direita de um nome de espaço de trabalho existente e selecione o espaço de trabalho para o qual deseja excluir tipos de registro.

   O espaço de trabalho é aberto e os tipos de registro e taxonomias associadas a ele são exibidos.
1. Clique no cartão do tipo de registro ou na taxonomia cujos campos você deseja editar.

   Essa ação abre a página do tipo de registro.
1. (Condicional) Selecione um **Visualização em tabela** do **Exibir** no canto superior direito da página tipo de registro.
1. Passe o mouse sobre o cabeçalho da coluna de um campo que você deseja editar, em seguida, clique na seta para baixo após o nome do campo.
1. Clique em **Editar campo**, atualize as informações sobre o campo e clique em **Salvar**.

   <!--insert screen shot when finalized-->

   >[!TIP]
   >
   >Não é possível atualizar o tipo de campo depois que o campo é salvo.


1. (Condicional) Para campos de registro vinculados, clique em **Editar campos de pesquisa** e adicionar ou remover qualquer um dos campos do tipo de registro vinculado.

   Para obter mais informações, consulte [Conectar tipos de registro](../architecture-and-fields/connect-record-types.md).
