---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: "Agrupamento: indique se os resultados de um agrupamento devem ser recolhidos ou expandidos usando o modo de texto"
description: "Agrupamento: indica se os resultados de um agrupamento devem ser recolhidos ou expandidos usando o modo de texto"
author: Nolan
feature: Reports and Dashboards
exl-id: 2880e06f-34f3-47b1-9462-5a15a20d6fee
source-git-commit: 7b25d3b5fe69f610e245db5ada116ea967f22c7b
workflow-type: tm+mt
source-wordcount: '343'
ht-degree: 0%

---

# Agrupamento: indica se os resultados de um agrupamento devem ser recolhidos ou expandidos usando o modo de texto

<!--Audited: 10/2024-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this article: NWE only; not possible in classic) </p>
-->

Você pode indicar se os resultados em um agrupamento devem ser exibidos recolhidos ou expandidos em uma lista ou relatório usando o Report Builder padrão. Os resultados em um agrupamento são expandidos por padrão. Para obter informações sobre como criar um agrupamento, consulte [Criar agrupamentos no Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/create-groupings.md).

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: the tips repeat in the Create groupings to organize results article, Understanding text mode, Edit groupings to organize reports, Create a Custom Report; create a snippet when convenient)</p>
-->

>[!TIP]
>
>* Quando você ajusta agrupamentos manualmente ao visualizar uma lista, o Adobe Workfront lembra de sua preferência manual até que você faça logout. Ao fazer logon novamente, a lista é exibida de acordo com essa configuração.
>* Os resultados de um agrupamento sempre são exibidos expandidos depois de acessados de um elemento do gráfico.
>

Você também pode indicar se um agrupamento deve ser exibido expandido ou recolhido usando o modo de texto.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> 
    <p>Novo:</p>
   <ul><li><p>Colaborador para modificar um filtro </p></li>
   <li><p>Padrão para modificar um relatório</p></li> </ul>

<p>Atual:</p>
   <ul><li><p>Solicitação para modificar um filtro </p></li>
   <li><p>Planejar a modificação de um relatório</p></li> </ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Editar acesso a relatórios, painéis e calendários para modificar um relatório</p> <p>Editar acesso a Filtros, Visualizações, Agrupamentos para modificar um filtro</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões para um relatório</p>  </td> 
  </tr> 
 </tbody> 
</table>

*Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Indica se os resultados de um agrupamento devem ser recolhidos ou expandidos usando o modo de texto

1. Ir para uma lista de objetos.
1. No menu suspenso **Agrupamento** selecione **Novo Agrupamento**.

1. Adicione um agrupamento e clique em **Alternar para Modo de Texto**.

   Ou

   Se o agrupamento já estiver no modo de texto, adicione o seguinte código ao nível de agrupamento que deseja exibir recolhido:

   `group.0.iscollapsed=true`

1. (Opcional) Se desejar que o agrupamento seja exibido expandido, adicione o seguinte código ao nível de agrupamento apropriado:

   `group.0.iscollapsed=false`

1. Clique em **Concluído** e em **Salvar agrupamento**.
1. (opcional) Atualize o nome do agrupamento e clique em **Salvar agrupamento**.
