---
title: Editar configurações de campo
description: No Adobe Workfront Planning, é possível editar as configurações de campo para campos já criados. Este artigo descreve como é possível editar as configurações para campos do Workfront Planning.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 6c35c313-d6ed-428b-b70d-2ea242da4e8f
source-git-commit: 5c7b60ac5b78bd065ffc270588ec72ab3eb2f41d
workflow-type: tm+mt
source-wordcount: '622'
ht-degree: 0%

---

<!--update the metadata with real information when making this available in TOC and in the left nav-->

<!---
title: Edit fields
description: In Adobe Workfront Planning, you can edit the field settings for fields that are already created.
hidefromtoc: yes
hide: yes
author: Alina
feature: (*******************WE NEED A NEW ONE*******************)
role: User, Administrator (************is this right???************)
recommendations: noDisplay, noCatalog
--->

# Editar configurações de campo

{{planning-important-intro}}

É possível editar as configurações de campo para campos já criados no Adobe Workfront Planning.

Para obter informações sobre como criar campos do Adobe Workfront Planning, consulte [Criar campos](/help/quicksilver/planning/fields/create-fields.md).

Este artigo descreve como é possível editar as configurações para campos do Workfront Planning. Para obter informações sobre a edição de valores de campo para registros, consulte [Editar registros](/help/quicksilver/planning/records/edit-records.md).

## Requisitos de acesso

+++ Expanda para exibir os requisitos de acesso do Workfront Planning.

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
   <p>Atual: Plano</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>Configuração do nível de acesso</p></td>
   <td> <p>Não há controles de acesso para o Workfront Planning</p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Permissões</p></td>
   <td> <p>Gerenciar permissões para um espaço de trabalho</a> </p>  
   <p>Os administradores do sistema têm permissões para todos os espaços de trabalho, incluindo aqueles que não criaram</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Modelo de layout</p></td>
   <td> <p>O administrador do Workfront ou do grupo deve adicionar a área do Planning ao modelo de layout. Para obter informações, consulte <a href="/help/quicksilver/planning/access/access-overview.md">Visão geral sobre acesso</a>. </p>  
</td>
  </tr>

</tbody>
</table>

*Para obter mais informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Maybe enable this at GA - but Planning is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

## Considerações sobre a edição de configurações de campo

Você deve considerar o seguinte antes de fazer alterações na configuração de um campo:

* É possível editar campos criados ou campos criados por outros usuários, se você tiver permissões de gerenciamento para o espaço de trabalho ao qual os campos pertencem.
* É possível editar um campo na tabela de tipo de registro.
* Não é possível editar um campo na página de registro ou em qualquer outra exibição fora da exibição de tabela.
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

   ![](assets/arrow-menu-after-name-of-field-in-table-header-highlighted.png)

1. Atualize as informações sobre o campo e clique em **Salvar**. <!--insert screen shot when finalized-->

   >[!TIP]
   >
   >* Não é possível atualizar o tipo de campo depois que o campo é salvo.
   >
   >* Ao modificar as configurações de campo (opções de campo ou expressões de fórmula), os registros que já contêm informações nos campos modificados atualizarão seus valores em tempo real. Não há aviso e nenhum log de auditoria para as alterações de valor acionadas pelas alterações de configuração do campo. Todos os usuários que visualizam os campos verão imediatamente os novos valores com as modificações.

   As informações do campo são atualizadas para todos com acesso para exibir o espaço de trabalho.

1. (Condicional) Para campos de registro vinculados, clique em **Editar campos de pesquisa** e adicione ou remova qualquer um dos campos do tipo de registro vinculado.

   Para obter mais informações, consulte [Tipos de registro de conexão](/help/quicksilver/planning/architecture/connect-record-types.md).

