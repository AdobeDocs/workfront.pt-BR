---
title: Excluir registros
description: É possível excluir registros criados por você ou por outro usuário. Não é possível recuperar registros excluídos.
hidefromtoc: true
hide: true
source-git-commit: 14b456f32dd2c8735e0a5252387f25305efc7610
workflow-type: tm+mt
source-wordcount: '466'
ht-degree: 2%

---


<!--udpate the metadata with real information when making this available in TOC and in the left nav-->

# Excluir registros

>[!IMPORTANT]
>
>Atualmente, o Adobe Maestro faz parte de um programa beta fechado que está aberto a um número limitado de clientes.
>
>Entre em contato com seu representante de conta para obter mais informações sobre como participar do programa beta para o Maestro.
>
>Para obter informações, consulte [Visão geral do Adobe Maestri](../maestro-overview.md).

Você pode excluir registros que não são mais relevantes no Adobe Maestro.

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

## Considerações sobre a exclusão de registros

* É possível excluir registros criados por você ou por outro usuário.
* Não é possível recuperar registros excluídos. <!--the above statements (and in the metadata description) will change with access levels and recycle bin??-->
* Se os registros excluídos estiverem vinculados a outros registros, os registros vinculados não serão excluídos, mas as informações do registro excluído também serão excluídas.
* Não é possível excluir registros em massa. <!--this will probably change-->
* Não é possível excluir registros da exibição de linha do tempo.

## Excluir registros

É possível excluir um registro das seguintes áreas:

* [Na página Detalhes de um registro](#delete-a-record-from-the-records-details-page)
* [Na exibição de tabela de um tipo de registro](#delete-a-record-from-the-record-type-table-view)

### Excluir um registro da página Detalhes do registro

1. Clique em **Menu principal** ![](assets/main-menu-workfront.png) no canto superior direito, ou na guia **Menu principal** ![](assets/main-menu-shell.png) no canto superior esquerdo, se estiver disponível, clique em Maestro.

   O espaço de trabalho que você acessa por último é aberto.
1. Clique em um tipo de registro.

   A página de tipo de registro é aberta.
1. Siga um destes procedimentos:

   * Em uma exibição de Tabela, clique no nome de um registro.
   * Na exibição Tabela, passe o mouse sobre o nome de um registro, depois clique no botão **Mais** menu ![](assets/more-menu.png)e, em seguida, clique em **Exibir**

     ![](assets/contextual-menu-for-record-row.png)
   * Em uma exibição de Linha do tempo, clique em uma barra de registro.

   O registro **Detalhes** é aberta.

1. Clique em **Mais** menu ![](assets/more-menu.png) à direita do nome do registro, clique em **Excluir**, depois **Excluir** novamente para confirmar.

   ![](assets/more-menu-options-from-record-details-page.png) <!--ensure the options have not changed or been renamed-->
O registro é excluído e não pode ser recuperado.

### Excluir um registro da exibição de tabela do tipo de registro

1. Clique em **Menu principal** ![](assets/main-menu-workfront.png) no canto superior direito, ou na guia **Menu principal** ![](assets/main-menu-shell.png) no canto superior esquerdo, se estiver disponível, clique em **Maestro**.

   O espaço de trabalho que você acessou por último é aberto.
1. Clique em um tipo de registro.

   A página de tipo de registro é aberta.
1. (Condicional) No **Exibir** no canto superior direito da tabela, selecione uma visualização Tabela. Essa deve ser a exibição padrão, a menos que você tenha visualizado o tipo de registro na exibição de linha do tempo ao acessá-lo pela última vez.

   Os registros associados ao tipo de registro selecionado são exibidos na exibição de tabela.
1. Clique com o botão direito do mouse em uma linha de registro e clique em **Excluir**.

   ![](assets/contextual-menu-for-record-row.png)

   O registro é excluído e não pode ser recuperado.