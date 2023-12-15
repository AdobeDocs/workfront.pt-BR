---
title: Editar registros
description: Você pode editar informações de registro no Adobe Maestro. Você deve criar tipos de registro antes de começar a criar e editar registros.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 981b8e44-b548-4f94-bf89-5f5dec3a6166
source-git-commit: 6f026590f0030b564f0d110afead9ade1acd7896
workflow-type: tm+mt
source-wordcount: '845'
ht-degree: 1%

---

<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

# Editar registros

>[!IMPORTANT]
>
>As informações neste artigo referem-se ao Adobe Maestro, que é uma nova oferta da Adobe Workfront.
>
>Atualmente, o Adobe Maestro faz parte de um programa beta aberto a um número limitado de clientes. Você deve ser um cliente do Workfront para usar os recursos do Maestro.
>
>Entre em contato com seu representante de conta para obter mais informações sobre como participar do programa beta para o Maestro.
>
>Para obter informações, consulte [Visão geral do Adobe Maestri](../maestro-overview.md).

Você pode editar informações de registro no Adobe Maestro. Você deve criar tipos de registro antes de começar a criar e editar registros.
Para obter informações, consulte [Criar tipos de registro](../architecture/create-record-types.md).

&lt;!— mencione aqui que os campos na exibição Detalhes são os mesmos da exibição de tabela — este artigo é vinculado da opção Gerenciar exibições de registro para fazer referência a essas informações—>

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
   <td role="rowheader">Nível de acesso</td>
   <td> <p>Qualquer</p>  
</td>
  </tr>
<tr>
   <td role="rowheader">Modelo de layout</td>
   <td> <p>O administrador do sistema deve adicionar a área Maestro no modelo de layout. Para obter informações, consulte <a href="../access/grant-access.md">Conceder acesso ao Adobe Maestro</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

<!--
After permssions - replace the table with: 

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Adobe product</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront agreement</p></td>
   <td>
<p>Your organization must be enrolled in the Adobe Maestro closed beta program. Contact your account representative to inquire about this new offering. </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront plan</p></td>
   <td>
<p>Any</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront license</p></td>
   <td>
   <p>Any</p> 
  </td>
  </tr>
  
  <tr>
   <td role="rowheader"><p>Access level</p></td>
   <td> <p>Any</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>Your Workfront or group administrator must add the Maestro area in your layout template. For information, see <a href="../access/grant-access.md">Grant access to Adobe Maestro</a>. </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>Contribute or higher permissions to a workspace</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>
</td>
  </tr>
 </tbody>
</table>

-->


<!--Maybe enable this at GA - but Maestro is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->

<!-- Notes for the table: for the "Workfront access" row: <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p>-->

## Considerações sobre a edição de registros

* É possível editar registros criados por você ou por outro usuário. <!--will change with access levels-->
* Não é possível editar campos vinculados a partir de outros registros ou campos que contêm cálculos.
* Se os registros exibidos estiverem vinculados a outros registros, as novas informações dos registros que você está editando serão refletidas nos registros vinculados.
* Não é possível editar registros em massa. <!--this will probably change-->
* Os URLs são reconhecidos como links em tipos de campo de texto de linha única somente quando começam com o seguinte: http://, https://, ftp:// ou www. .
* Você pode usar as seguintes opções de formatação de Rich Text ao editar um campo do tipo Parágrafo:

   * Negrito
   * Itálico
   * Sublinhar
   * Adicionar um link
   * Adicionar uma lista com marcadores
   * Adicionar uma lista numerada

## Editar registros

É possível editar um registro das seguintes áreas:

* [Na página Detalhes de um registro](#edit-a-record-from-the-records-details-page)
* [Na exibição de tabela de um tipo de registro](#edit-a-record-from-the-record-type-table-view)

### Editar um registro na página Detalhes do registro

{{step1-to-maestro}}

O espaço de trabalho que você acessa por último é aberto.

1. (Opcional) Clique na seta para baixo à direita do nome do espaço de trabalho para selecionar o espaço de trabalho cujos registros você deseja atualizar.
1. Siga um destes procedimentos:

   * Em uma exibição de Tabela, clique no nome de um registro.
   * Na exibição Tabela, passe o mouse sobre o nome de um registro, depois clique no botão **Mais** menu ![](assets/more-menu.png)e, em seguida, clique em **Exibir**

     ![](assets/contextual-menu-for-record-row.png)
   * Em uma exibição de Linha do tempo, clique em uma barra de registro.

   O registro **Detalhes** é aberta.

1. Clique em **Mais** menu ![](assets/more-menu.png) à direita do nome do registro, clique em **Editar**

   Ou

   Clique dentro de qualquer campo editável na página Detalhes para editar as informações.

   ![](assets/more-menu-options-from-record-details-page.png) <!--ensure the options have not changed or been renamed-->

1. Clique em **Salvar alterações**. <!--logged a bug for this - this needs to be "Save"-->

### Editar um registro da exibição de tabela de um tipo de registro

1. Clique em **Menu principal** ![](assets/main-menu-workfront.png) no canto superior direito, ou na guia **Menu principal** ![](assets/main-menu-shell.png) no canto superior esquerdo, se estiver disponível, clique em **Maestro** ![](assets/maestro-icon.png).

   O espaço de trabalho que você acessou por último é aberto.

1. (Opcional) Clique na seta para baixo à direita do nome do espaço de trabalho para selecionar o espaço de trabalho cujos registros você deseja atualizar.
1. Clique em um cartão de tipo de registro.

   A página de tipo de registro é aberta.
1. (Condicional) No **Exibir** no canto superior direito da tabela, selecione uma **Tabela** exibição. Essa deve ser a exibição padrão, a menos que você tenha visualizado o tipo de registro na exibição de linha do tempo ao acessá-lo pela última vez.

   Os registros associados ao tipo de registro selecionado são exibidos na exibição de tabela.
1. Clique dentro da linha de um registro para começar a editar informações sobre o registro em linha.

   ![](assets/edit-record-paragraph-field-with-formatting-table-view.png)
1. Pressione **Enter** no teclado ou clique fora de uma linha para salvar as alterações. As alterações são salvas automaticamente. Um indicador Salvo é exibido brevemente no canto superior direito da exibição de tabela para mostrar que as alterações foram salvas.

   >[!NOTE]
   >
   >  Não é possível editar as informações dos seguintes campos, pois eles são somente leitura e o Workfront os atualiza automaticamente:
   >  
   >  * Campos vinculados criados pela conexão de tipos de registro. Para obter mais informações, consulte [Conectar tipos de registro](../architecture/connect-record-types.md).
   >  * Campos dos seguintes tipos: Criado por, Data de criação, Última modificação por, Data da última modificação


1. (Opcional) Copie um ou vários valores existentes de um campo, cole-os em um campo do mesmo tipo em outro registro e clique em **Enter** no teclado para salvar as alterações.

   >[!NOTE]
   >
   >Considere o seguinte:
   >
   >* Você não pode copiar informações de outra fonte, que não seja um campo Maestro do mesmo tipo do campo no qual você cola as informações.
   >
   >* Não é possível copiar e colar valores de campo na área Detalhes de um registro. Essa funcionalidade é compatível somente na exibição de tabela de um tipo de registro.
   >* Não é possível copiar e colar valores de campo para os seguintes tipos de campo:
   >
   >
   >    * Campos vinculados criados pela conexão de tipos de registro. Você pode copiar e colar campos de registro vinculados. Para obter mais informações, consulte [Conectar tipos de registro](../architecture/connect-record-types.md).
   >    * Campos dos seguintes tipos: Criado por, Data de criação, Última modificação por, Data da última modificação


   <!--take People out of the list above when they release this - this might be coming later-->
