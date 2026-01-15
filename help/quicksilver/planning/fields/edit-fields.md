---
title: Editar configurações de campo
description: No Adobe Workfront Planning, é possível editar as configurações de campo para campos já criados. Este artigo descreve como é possível editar as configurações para campos do Workfront Planning.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 6c35c313-d6ed-428b-b70d-2ea242da4e8f
source-git-commit: 5d326776b9c5b4d9d24e802375df4630508c8bd0
workflow-type: tm+mt
source-wordcount: '919'
ht-degree: 0%

---


# Editar configurações de campo

<!--leave the choice value information in yellow till January 2026-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

É possível editar as configurações de campos existentes no Adobe Workfront Planning.

Para obter informações sobre como criar campos do Adobe Workfront Planning, consulte [Criar campos](/help/quicksilver/planning/fields/create-fields.md).

Este artigo descreve como é possível editar as configurações para campos do Workfront Planning. Para obter informações sobre a edição de valores de campo para registros, consulte [Editar registros](/help/quicksilver/planning/records/edit-records.md).

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
<p>Qualquer Workfront e qualquer pacote do Planning</p> <p>Qualquer fluxo de trabalho e qualquer pacote de planejamento</p>
<p>Para obter mais informações sobre o que está incluído em cada pacote do Workfront Planning, entre em contato com o representante de conta da Workfront. </p> 
   </td> 
  <tr> 
   <td role="rowheader"><p>Licença do Adobe Workfront</p></td> 
   <td><p>Padrão</p>
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
   <td><p> Standard </p>
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
   <td>   <p>Manage permissions to a workspace and record type</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p></td> 
  </tr> 
</tbody> 
</table> -->

## Considerações sobre a edição de configurações de campo

Você deve considerar o seguinte antes de fazer alterações na configuração de um campo:

* É possível editar configurações de campo somente a partir da tabela de tipo de registro.
* Não é possível editar as configurações de um campo na página de registro ou em qualquer outra exibição fora da exibição de tabela.
* Não é possível editar o tipo de campo depois que o campo é salvo.
* Não é possível desmarcar a configuração Permitir números negativos que foi selecionada anteriormente para um campo Número, Porcentagem ou Moeda se já houver valores negativos armazenados nos registros aos quais está anexado.
* Você pode editar a configuração dos seguintes elementos de campo, depois de salvar o campo:

   * O Nome ou a Descrição de qualquer campo
   * As Opções de um campo de seleção única ou de seleção múltipla.
   * A expressão de um campo Formula.

  >[!WARNING]
  >
  >Quando as expressões de fórmula forem alteradas ou as opções forem adicionadas ou removidas de um campo do tipo select, haverá perda de dados para os registros que já têm informações armazenadas nos campos cuja configuração é modificada.
  >
  >Não há aviso ou indicação de que essa perda de dados possa ocorrer ao alterar a configuração dos campos.
  >
  >Não há notificação para outros usuários informando que a configuração do campo foi alterada.

* Você pode editar campos de pesquisa existentes a partir de registros conectados.
* Além de editar o campo conforme descrito na seção [Editar configurações de campo](#edit-field-settings-1) deste artigo, você pode editar as opções de um campo de seleção única ou múltipla ao editar um registro na exibição de tabela, à medida que atualiza os valores do campo. Para obter informações, consulte a seção [Adicionar novas opções a um campo de seleção existente ao editar registros na exibição de tabela](#add-new-choices-to-an-existing-select-field-when-editing-records-in-the-table-view) deste artigo.

<!--at production - April 10, 2025 - remove the last bullet altogether-->

<!--this is not yet true, but it might come later:
* You can deselect Allow negative numbers option from a Number, Percentage, or Currency field after you save the field. 
-->

## Editar configurações de campo

{{step1-to-planning}}

1. Clique no espaço de trabalho cujos campos de registro você deseja editar.

   O espaço de trabalho é aberto e todos os tipos de registro no espaço de trabalho são exibidos em cartões.

1. Clique no cartão de um tipo de registro.

   Essa ação abre a página do tipo de registro.

1. (Condicional) Clique na guia de uma **exibição de Tabela**.

   Todos os registros existentes associados ao tipo de registro são exibidos nas linhas da exibição de tabela.
1. Passe o mouse sobre o cabeçalho da coluna de um campo que você deseja editar, clique na seta para baixo após o nome do campo e clique em **Editar campo**

   Ou

   Clique duas vezes no cabeçalho da coluna do campo.

   ![Menu de seta após o nome do campo no cabeçalho da tabela realçado](assets/arrow-menu-after-name-of-field-in-table-header-highlighted.png)

1. Atualize as informações sobre o campo e clique em **Salvar**.

   Para obter informações, consulte [Criar campos](/help/quicksilver/planning/fields/create-fields.md).

   <!--insert screen shot when finalized-->

   >[!TIP]
   >
   >* Não é possível atualizar o tipo de campo depois que o campo é salvo.
   >
   >* Ao modificar as configurações de campo (opções de campo ou expressões de fórmula), os registros que já contêm informações nos campos modificados atualizarão seus valores em tempo real. Não há aviso e nenhum log de auditoria para as alterações de valor acionadas pelas alterações de configuração do campo. Todos os usuários que visualizam os campos verão imediatamente os novos valores com as modificações.

   As informações do campo são atualizadas para todos com acesso para exibir o espaço de trabalho.

1. (Condicional) Para campos de registro conectados, clique em **Editar campos de pesquisa** e adicione ou remova qualquer um dos campos de pesquisa do tipo de registro conectado.

   Para obter mais informações, consulte [Tipos de registro de conexão](/help/quicksilver/planning/architecture/connect-record-types.md).


## Adicionar novas opções a um campo de seleção existente ao editar registros na exibição de tabela

<!--some of this information is also available in Edit records article - update both when necessary-->

Você pode adicionar novas opções a um campo de seleção única ou múltipla existente ao editar registros na exibição de tabela.

>[!IMPORTANT]
>
>A funcionalidade descrita nesta seção está disponível somente na exibição de tabela. Não está disponível em nenhuma outra área em que campos de seleção única ou múltipla são exibidos.

**EXEMPLO**

Você pode ter um campo de seleção única chamado Status que tem as opções Novo e Fechado e deseja adicionar uma opção para um status Em andamento. Você pode adicionar a escolha executando um dos procedimentos a seguir:

* Edição do campo. Para obter informações, consulte a seção [Editar configurações de campo](#edit-field-settings-1) neste artigo.
* Adicionar uma nova opção ao editar o registro na exibição de tabela, conforme descrito abaixo.

Para adicionar uma nova opção a um campo de seleção existente ao editar um registro:

1. Ir para uma página do tipo registro e abrir a exibição de tabela.
1. Adicione o campo de seleção única ou múltipla ao qual você deseja adicionar uma opção na exibição de tabela como uma nova coluna. Para obter informações, consulte [Criar campos](/help/quicksilver/planning/fields/create-fields.md).
1. Comece a editar o campo em linha clicando duas vezes na célula do campo.
1. Digite o nome da opção que deseja adicionar e clique em **Adicionar opção**.

   ![Adicionar opção em campo de seleção única na exibição de tabela](assets/add-choice-in-table-view-for-single-select-field.png)

   A nova opção é adicionada imediatamente ao campo de seleção única.

   Um novo valor também é adicionado a cada escolha. Você pode usar os valores de opção em chamadas de API ou outras integrações. Para obter informações, consulte [Criar campos](/help/quicksilver/planning/fields/create-fields.md).

