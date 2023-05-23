---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: "Agrupamento: indica se os resultados de um agrupamento devem ser recolhidos ou expandidos usando o modo de texto"
description: "Agrupamento: indica se os resultados de um agrupamento devem ser recolhidos ou expandidos usando o modo de texto"
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 2880e06f-34f3-47b1-9462-5a15a20d6fee
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '366'
ht-degree: 0%

---

# Agrupamento: indica se os resultados de um agrupamento devem ser recolhidos ou expandidos usando o modo de texto

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

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront*</td> 
   <td> <p>Qualquer Um</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Solicitação para modificar um agrupamento </p>
   <p>Planejar a modificação de um relatório</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a relatórios, painéis e calendários para modificar um relatório</p> <p>Editar acesso a Filtros, Visualizações, Agrupamentos para modificar um agrupamento</p> <p><b>Nota</b>

Se você ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td>
</tr>  
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões para um relatório</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir seu plano, tipo de licença ou acesso, entre em contato com o administrador do Workfront.

## Indica se os resultados de um agrupamento devem ser recolhidos ou expandidos usando o modo de texto

1. Ir para uma lista de objetos.
1. No **Agrupamento** selecione **Novo Agrupamento**.

1. Adicione um agrupamento e clique em **Alternar para modo de texto**.

   Ou

   Se o agrupamento já estiver no modo de texto, adicione o seguinte código ao nível de agrupamento que deseja exibir recolhido:

   ```
   group.0.iscollapsed=true
   ```

1. (Opcional) Se desejar que o agrupamento seja exibido expandido, adicione o seguinte código ao nível de agrupamento apropriado:

   ```
   group.0.iscollapsed=false
   ```

1. Clique em **Concluído**, depois **Salvar Agrupamento**.
