---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Agrupamento: Indica se os resultados de um Agrupamento devem ser recolhidos ou expandidos usando o Modo de Texto'
description: 'Agrupamento: indicar se os resultados de um agrupamento devem ser recolhidos ou expandidos usando o modo de texto'
author: Courtney
feature: Reports and Dashboards
exl-id: 2880e06f-34f3-47b1-9462-5a15a20d6fee
source-git-commit: 6a6d3d47ed5741e3202c44b7240a2e67b687ea95
workflow-type: tm+mt
source-wordcount: '329'
ht-degree: 22%

---

# Agrupamento: indicar se os resultados de um agrupamento devem ser recolhidos ou expandidos usando o modo de texto

<!--Audited: 10/2024-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this article: NWE only; not possible in classic) </p>
-->

Você pode indicar se os resultados em um agrupamento devem ser exibidos recolhidos ou expandidos em uma lista ou relatório usando o construtor de relatórios padrão. Os resultados em uma exibição de agrupamento são expandidos, por padrão. Para obter informações sobre como criar um agrupamento, consulte [Criar agrupamentos no Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/create-groupings.md).

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: the tips repeat in the Create groupings to organize results article, Understanding text mode, Edit groupings to organize reports, Create a Custom Report; create a snippet when convenient)</p>
-->

>[!TIP]
>
>* Quando você ajusta os agrupamentos manualmente ao exibir uma lista, o Adobe Workfront se lembra de sua preferência manual até que você faça logoff. Ao efetuar logon novamente, a lista é exibida de acordo com essa configuração.
>* Os resultados de um agrupamento sempre são exibidos expandidos após acessá-los a partir de um elemento de gráfico.
>

Você também pode indicar se um agrupamento deve ser exibido expandido ou recolhido usando o modo de texto.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacote do Adobe Workfront</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td> 
   <p>Colaborador ou solicitação para modificar um filtro </p>
   <p>Padrão ou Plano para modificar um relatório</p>
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Acesso de edição a relatórios, painéis e calendários para modificar um relatório</p> <p>Editar acesso a filtros, exibições e agrupamentos para modificar um filtro</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões para um relatório</p>  </td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações contidas nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Indica se os resultados de um agrupamento devem ser recolhidos ou expandidos usando o modo de texto

1. Ir para uma lista de objetos.
1. No menu suspenso **Agrupamento** selecione **Novo Agrupamento**.

1. Adicione um agrupamento e clique em **Alternar para o Modo de Texto**.

   Ou

   Se o agrupamento já estiver no modo de texto, adicione o seguinte código ao nível de agrupamento que você deseja exibir recolhido:

   `group.0.iscollapsed=true`

1. (Opcional) Para que o agrupamento seja exibido expandido, adicione o seguinte código ao nível de agrupamento apropriado:

   `group.0.iscollapsed=false`

1. Clique em **Concluído** e depois em **Salvar Agrupamento**.
1. (opcional) Atualize o nome do agrupamento e clique em **Salvar agrupamento**.
