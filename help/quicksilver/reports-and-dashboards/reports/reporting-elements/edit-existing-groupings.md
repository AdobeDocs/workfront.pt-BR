---
title: Editar agrupamentos existentes
description: Editar agrupamentos existentes
author: Nolan
feature: Reports and Dashboards
exl-id: bd9e6794-3196-4a73-a86a-9ba6048e613b
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '485'
ht-degree: 0%

---

# Editar agrupamentos existentes

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: This is the third part of a former artcle split in 3: two how-tos and one refernece article about creating and customizing groupings)</p>
-->

Você pode personalizar um agrupamento existente criado originalmente ou que foi compartilhado com você. Em seguida, é possível salvá-lo como um novo agrupamento.

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>plano do Adobe Workfront*</strong></td> 
   <td> <p>Qualquer Um</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Licença da Adobe Workfront*</strong></td> 
   <td> <p>Solicitação ou superior </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurações de nível de acesso*</strong></td> 
   <td> <p>Editar acesso a Filtros, Visualizações, Agrupamentos</p> <p>Editar acesso a Relatórios, Painéis, Calendários para editar um agrupamento em um relatório</p> <p>Observação: se você ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Permissões de objeto</strong></td> 
   <td> <p>Gerenciar permissões de um relatório para editar um agrupamento em um relatório</p> <p>Gerenciar permissões para um agrupamento </p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir seu plano, tipo de licença ou acesso, entre em contato com o administrador do Workfront.

## Pré-requisitos

Você deve criar um agrupamento antes de editá-lo.

Para obter informações sobre como criar um agrupamento, consulte [Criar agrupamentos no Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/create-groupings.md).

## Etapas passo a passo

1. Vá para uma lista de objetos que contém o agrupamento que você deseja personalizar.
1. Clique em **Agrupamento** ícone.
1. Selecione o agrupamento que deseja personalizar e clique no botão **Editar** ícone.

   ![Selecione o ícone de edição.](assets/customizegrouping-nwe-standard-350x291.png)

   O construtor de interface para personalizar o agrupamento é aberto.

1. No **Visualização do agrupamento** clique em **Adicionar Agrupamento** para definir como você deseja que as informações no relatório sejam organizadas. Uma visualização da aparência do agrupamento no relatório é mostrada abaixo.

1. Comece digitando o nome do campo que representa a maneira como deseja organizar as informações no relatório e, em seguida, clique nele quando ele aparecer na lista suspensa.
1. (Opcional e condicional) Ao visualizar uma lista atualizada, selecione **Recolher este agrupamento por padrão** se desejar que os resultados no agrupamento sejam exibidos recolhidos, em vez de expandidos. Essa configuração é desabilitada por padrão e os resultados do agrupamento sempre são exibidos na lista expandida.

   Para obter informações sobre listas atualizadas e herdadas, consulte a seção &quot;A diferença entre listas atualizadas e herdadas&quot; no artigo [Introdução a listas no Adobe Workfront](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Quicksilver,QuicksilverOrClassic.Draft mode">(NOTE: the tips repeat in the Create grouping article and Common uses of text mode)</p>
   -->

   >[!TIP]
   >
   >* Quando você ajusta agrupamentos manualmente ao visualizar uma lista, o Workfront lembra de sua preferência manual até que você faça logout. Ao fazer logon novamente, a lista é exibida de acordo com essa configuração.
   >* Os resultados de um agrupamento sempre são exibidos expandidos depois de acessá-los a partir de um elemento do gráfico ou em uma lista herdada. Nesses casos, essa configuração é ignorada.


1. Repita as etapas 4, 5 e 6 para definir agrupamentos adicionais.\
   É possível definir até três agrupamentos para organizar as informações. Você pode organizar ainda mais suas informações com até quatro agrupamentos criando um relatório de matriz. Para obter mais informações sobre relatórios de matriz, consulte [Criar um relatório de matriz](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-matrix-report.md).

1. Clique em **Salvar como novo agrupamento** para substituir o agrupamento atual pelas alterações.
