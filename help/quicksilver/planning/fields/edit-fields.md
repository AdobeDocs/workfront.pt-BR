---
title: Editar configurações de campo
description: No Adobe Workfront Planning, é possível editar as configurações de campo para campos já criados. Este artigo descreve como é possível editar as configurações para campos do Workfront Planning.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 6c35c313-d6ed-428b-b70d-2ea242da4e8f
source-git-commit: 298c542afea902d9fc14ef6a4470c0bc1d9bd33c
workflow-type: tm+mt
source-wordcount: '663'
ht-degree: 1%

---


# Editar configurações de campo

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

É possível editar as configurações de campos existentes no Adobe Workfront Planning.

Para obter informações sobre como criar campos do Adobe Workfront Planning, consulte [Criar campos](/help/quicksilver/planning/fields/create-fields.md).

Este artigo descreve como é possível editar as configurações para campos do Workfront Planning. Para obter informações sobre a edição de valores de campo para registros, consulte [Editar registros](/help/quicksilver/planning/records/edit-records.md).

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso.

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Produtos</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Planejamento do Adobe Workfront<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>plano do Adobe Workfront*</p></td> 
   <td> 
<p>Qualquer um dos seguintes planos da Workfront:</p> 
<ul><li>Selecionar</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>O Workfront Planning não está disponível para planos herdados do Workfront</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Pacote de planejamento do Adobe Workfront*</p></td> 
   <td> 
<p>Qualquer </p> 
<p>Para obter mais informações sobre o que está incluído em cada plano do Workfront Planning, entre em contato com seu gerente de conta da Workfront. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>plataforma Adobe Workfront</p></td> 
   <td> 
<p>A instância da Workfront de sua organização deve ser integrada à Adobe Unified Experience para acessar o Workfront Planning.</p> 
<p>Para obter mais informações, consulte <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Experiência unificada da Adobe para Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Licença da Adobe Workfront*</p></td> 
   <td><p> Padrão </p>
   <p>O Workfront Planning não está disponível para licenças herdadas do Workfront</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Configuração do nível de acesso</p></td> 
   <td> <p>Não há controles de nível de acesso para o Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Permissões de objeto</p></td> 
   <td>   <p>Gerenciar permissões para um espaço de trabalho e tipo de registro</a> </p>  
   <p>Os administradores do sistema têm permissões para todos os espaços de trabalho, incluindo aqueles que não criaram</p></td> 
  </tr> 
</tbody> 
</table>

*Para obter mais informações sobre requisitos de acesso do Workfront, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


## Considerações sobre a edição de configurações de campo

Você deve considerar o seguinte antes de fazer alterações na configuração de um campo:

* É possível editar configurações de campo somente a partir da tabela de tipo de registro.
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

* Você pode editar campos de pesquisa existentes a partir de registros conectados.

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

1. Atualize as informações sobre o campo e clique em **Salvar**. <!--insert screen shot when finalized-->

   >[!TIP]
   >
   >* Não é possível atualizar o tipo de campo depois que o campo é salvo.
   >
   >* Ao modificar as configurações de campo (opções de campo ou expressões de fórmula), os registros que já contêm informações nos campos modificados atualizarão seus valores em tempo real. Não há aviso e nenhum log de auditoria para as alterações de valor acionadas pelas alterações de configuração do campo. Todos os usuários que visualizam os campos verão imediatamente os novos valores com as modificações.

   As informações do campo são atualizadas para todos com acesso para exibir o espaço de trabalho.

1. (Condicional) Para campos de registro conectados, clique em **Editar campos de pesquisa** e adicione ou remova qualquer um dos campos de pesquisa do tipo de registro conectado.

   Para obter mais informações, consulte [Tipos de registro de conexão](/help/quicksilver/planning/architecture/connect-record-types.md).