---
title: Editar agrupamentos existentes
description: Editar agrupamentos existentes
author: Nolan
feature: Reports and Dashboards
exl-id: bd9e6794-3196-4a73-a86a-9ba6048e613b
source-git-commit: 302771f4d64b386149623f87a3436d0c40f421d5
workflow-type: tm+mt
source-wordcount: '483'
ht-degree: 0%

---

# Editar agrupamentos existentes

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: This is the third part of a former artcle split in 3: two how-tos and one refernece article about creating and customizing groupings)</p>
-->

Você pode personalizar um agrupamento existente criado originalmente ou que foi compartilhado com você. Em seguida, você pode salvá-lo como um novo agrupamento.

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Plano Adobe Workfront*</strong></td> 
   <td> <p>Qualquer Um</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Licença da Adobe Workfront*</strong></td> 
   <td> <p>Plano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurações de nível de acesso*</strong></td> 
   <td> <p>Editar acesso a filtros, visualizações, agrupamentos</p> <p>Editar o acesso a Relatórios, Painéis, Calendários para editar um agrupamento em um relatório</p> <p>Observação: Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Permissões de objeto</strong></td> 
   <td> <p>Gerenciar permissões de um relatório para editar um agrupamento em um relatório</p> <p>Gerenciar permissões em um agrupamento </p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

## Pré-requisitos

É necessário criar um agrupamento antes de editá-lo.

Para obter informações sobre como criar um agrupamento, consulte [Criar agrupamentos no Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/create-groupings.md).

## Etapas de instruções

1. Vá para uma lista de objetos que contém o agrupamento que deseja personalizar.
1. Clique no botão **Agrupamento** ícone .
1. Selecione o agrupamento que deseja personalizar e clique no botão **Editar** ícone .

   ![Selecione o ícone de edição.](assets/customizegrouping-nwe-standard-350x291.png)

   O construtor de interface para personalizar o agrupamento é aberto.

1. No **Visualização de agrupamento** seção , clique em **Adicionar agrupamento** para definir como deseja que as informações no relatório sejam organizadas. Uma visualização da aparência do agrupamento no relatório é mostrada abaixo.

1. Comece digitando o nome do campo que representa a maneira como você deseja organizar as informações no relatório e clique nele quando ele for exibido na lista suspensa.
1. (Opcional e condicional) Ao exibir uma lista atualizada, selecione **Recolher este agrupamento por predefinição** se desejar que os resultados no agrupamento exibam os resultados recolhidos em vez de expandidos. Essa configuração é desativada por padrão e os resultados do agrupamento sempre são exibidos na lista expandida.

   Para obter informações sobre listas atualizadas e herdadas, consulte a seção &quot;A diferença entre listas atualizadas e herdadas&quot; no artigo [Introdução a listas no Adobe Workfront](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Quicksilver,QuicksilverOrClassic.Draft mode">(NOTE: the tips repeat in the Create grouping article and Common uses of text mode)</p>
   -->

   >[!TIP]
   >
   >* Ao ajustar manualmente os agrupamentos ao visualizar uma lista, o Workfront lembra de sua preferência manual até que você saia. Quando você faz logon novamente, a lista é exibida de acordo com essa configuração.
   >* Os resultados de um agrupamento sempre são expandidos depois de acessá-los a partir de um elemento de gráfico ou em uma lista herdada. Nesses casos, essa configuração é ignorada.


1. Repita as Etapas 4, 5 e 6 para definir agrupamentos adicionais.\
   É possível definir até três agrupamentos para organizar informações. Você pode ainda organizar suas informações com até quatro agrupamentos, criando um relatório de matriz. Para obter mais informações sobre relatórios de matriz, consulte [Criar um relatório de matriz](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-matrix-report.md).

1. Clique em **Salvar como novo agrupamento** para substituir o agrupamento atual por suas alterações.
