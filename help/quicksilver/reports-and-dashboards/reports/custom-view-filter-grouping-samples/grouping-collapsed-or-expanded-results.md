---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '"Agrupamento: indica se os resultados de um agrupamento devem ser recolhidos ou expandidos usando o modo de texto'''
description: '"Agrupamento: indica se os resultados de um agrupamento devem ser recolhidos ou expandidos usando o modo de texto'''
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 2880e06f-34f3-47b1-9462-5a15a20d6fee
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '349'
ht-degree: 0%

---

# Agrupamento: indica se os resultados de um agrupamento devem ser recolhidos ou expandidos usando o modo de texto

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this article: NWE only; not possible in classic) </p>
-->

Você pode indicar se os resultados em um agrupamento devem exibir recolhidos ou expandidos em uma lista ou relatório usando o Construtor de relatórios padrão. Os resultados em um agrupamento são expandidos, por padrão. Para obter informações sobre como criar um agrupamento, consulte [Criar agrupamentos no Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/create-groupings.md).

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: the tips repeat in the Create groupings to organize results article, Understanding text mode, Edit groupings to organize reports, Create a Custom Report; create a snippet when convenient)</p>
-->

>[!TIP]
>
>* Ao ajustar manualmente os agrupamentos ao visualizar uma lista, o Adobe Workfront lembra de sua preferência manual até que você saia. Quando você faz logon novamente, a lista é exibida de acordo com essa configuração.
>* Os resultados de um agrupamento sempre são exibidos expandidos depois de acessá-los a partir de um elemento de gráfico.
>


Você também pode indicar se um agrupamento deve exibir expandido ou recolhido usando o modo de texto.

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plano Adobe Workfront*</td> 
   <td> <p>Qualquer Um</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Plano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a Relatórios, Painéis, Calendários</p> <p>Editar acesso a filtros, visualizações, agrupamentos</p> <p>Observação: Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões de um relatório</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

## Indique se os resultados de um agrupamento devem ser recolhidos ou expandidos usando o modo de texto

1. Vá para uma lista de objetos.
1. No **Agrupamento**, selecione **Novo agrupamento**.

1. Adicione um agrupamento e clique em **Alternar para o modo de texto**.

   Ou

   Se o agrupamento já estiver no modo de texto, adicione o seguinte código ao nível de agrupamento que você deseja exibir recolhido:

   ```
   group.0.iscollapsed=true
   ```

1. (Opcional) Se desejar que o agrupamento seja exibido expandido, adicione o seguinte código ao nível de agrupamento apropriado:

   ```
   group.0.iscollapsed=false
   ```

1. Clique em **Concluído**, em seguida **Salvar Agrupamento**.
