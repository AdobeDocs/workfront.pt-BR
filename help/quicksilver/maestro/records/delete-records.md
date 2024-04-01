---
title: Excluir registros
description: É possível excluir registros criados por você ou por outro usuário. Não é possível recuperar registros excluídos.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 3f7a3667-8a9f-462a-b706-cf15850a0d1c
source-git-commit: e54142e189cd4f407161401203a7f13c752ad404
workflow-type: tm+mt
source-wordcount: '487'
ht-degree: 2%

---

<!--update the metadata with real information when making this available in TOC and in the left nav-->

# Excluir registros

{{maestro-important-intro}}

Você pode excluir registros que não são mais relevantes no Adobe Workfront Planning.

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
<p>Sua organização deve estar inscrita no programa beta de Planejamento do Adobe Workfront. Entre em contato com seu representante de conta para obter mais informações sobre esta nova oferta. </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>plano do Adobe Workfront</p></td>
   <td>
<p>Qualquer</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Licença do Adobe Workfront</p>
   </td>
   <td>
   <p>Qualquer</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>Configurações de nível de acesso</p></td>
   <td> <p>Não há controles de nível de acesso para o Adobe Workfront Planning </p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Permissões</p></td>
   <td> <p>Contribuir com permissões ou mais altas para um espaço de trabalho</a> </p>  
   <p>Os administradores do sistema têm permissões para todos os espaços de trabalho, incluindo aqueles que não criaram</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Modelo de layout</p></td>
   <td> <p>O administrador do Workfront ou do grupo deve adicionar a área do Planning ao modelo de layout. Para obter informações, consulte <a href="../access/access-overview.md">Visão geral do Access</a>. </p>  
</td>
  </tr>

</tbody>
</table>


<!--Maybe enable this at GA - but Maestro is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

## Considerações sobre a exclusão de registros

* É possível excluir registros criados por você ou por outro usuário.
* Não é possível recuperar registros excluídos. <!--the above statements (and in the metadata description) will change with access levels and recycle bin??-->
* Se os registros excluídos estiverem vinculados a outros registros, os registros vinculados não serão excluídos, mas as informações do registro excluído também serão excluídas.
* Não é possível excluir registros em massa. <!--this will probably change-->
* Não é possível excluir registros da exibição de linha do tempo.

## Excluir registros

É possível excluir um registro das seguintes áreas:

* [Da página do registro](#delete-a-record-from-the-records-page)
* [Na exibição de tabela de um tipo de registro](#delete-a-record-from-the-record-type-table-view)

### Excluir um registro da página do registro

{{step1-to-maestro}}

O espaço de trabalho que você acessa por último é aberto.

1. Clique em um tipo de registro.

   A página de tipo de registro é aberta.
1. Siga um destes procedimentos:

   * Em uma exibição de Tabela, clique no nome de um registro.
   * Na exibição Tabela, passe o mouse sobre o nome de um registro, depois clique no botão **Mais** menu ![](assets/more-menu.png)e, em seguida, clique em **Exibir**

     ![](assets/contextual-menu-for-record-row.png)
   * Em uma exibição de Linha do tempo, clique em uma barra de registro.

   A página de registro é aberta.

1. Clique em **Mais** menu ![](assets/more-menu.png) à direita do nome do registro, clique em **Excluir**, depois **Excluir** novamente para confirmar.

   ![](assets/more-menu-options-from-record-details-page.png) <!--ensure the options have not changed or been renamed-->
O registro é excluído e não pode ser recuperado.

### Excluir um registro da exibição de tabela do tipo de registro

{{step1-to-maestro}}

O espaço de trabalho que você acessou por último é aberto.

1. Clique em um tipo de registro.

   A página de tipo de registro é aberta.
1. (Condicional) No **Exibir** no canto superior esquerdo da tabela, selecione uma visualização Tabela. Essa deve ser a exibição padrão, a menos que você tenha visualizado o tipo de registro na exibição de linha do tempo ao acessá-lo pela última vez.

   Os registros associados ao tipo de registro selecionado são exibidos na exibição de tabela.
1. Siga um destes procedimentos:

   * Clique com o botão direito do mouse em uma linha de registro e clique em **Excluir**.
   * Clique em **Mais** menu ![](assets/more-menu.png) à direita do nome do registro, clique em **Excluir**

     ![](assets/contextual-menu-for-record-row.png)

   * Clique em **Abrir detalhes** ícone ![](assets/open-details-icon-in-table-name-field.png) para abrir a caixa com as informações detalhadas do registro e clique em **Mais** ![](assets/more-menu.png) à direita do nome do registro, então **Excluir**.

   O registro é excluído e não pode ser recuperado.

1. (Opcional) Use os seguintes atalhos de teclado para desfazer ou refazer a exclusão de um registro:

   * CTRL + Z (⌘ + Z para Mac) para desfazer uma alteração
   * CTRL + Shift + Z (⌘ + Shift + Z para Mac) para refazer uma alteração
