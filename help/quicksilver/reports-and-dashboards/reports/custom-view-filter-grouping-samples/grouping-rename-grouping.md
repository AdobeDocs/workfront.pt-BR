---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: "Agrupamento: editar o nome de exibição em um agrupamento"
description: É possível renomear agrupamentos em listas e relatórios para algo mais familiar aos usuários.
author: Nolan
feature: Reports and Dashboards
exl-id: 072d3c2b-9ede-4bb9-9a27-dc77ceb732c4
source-git-commit: a6874c3a2dfda02b8a25f78056767d8c59c888e9
workflow-type: tm+mt
source-wordcount: '350'
ht-degree: 0%

---

# Agrupamento: editar o nome de exibição em um agrupamento

<!--Audited: 01/2024-->

É possível renomear agrupamentos para algo mais familiar aos usuários.

Por exemplo, ao aplicar o agrupamento padrão de Nome de Portfolio a uma lista de projetos, o nome do agrupamento aparece como *Portfolio: Nome:`<name of portfolio>`*.

![](assets/grouping-unedited-name-350x167.png)

Você pode modificar esse agrupamento usando o modo texto para exibir um nome mais fácil de ler.

![](assets/grouping-edited-name-350x160.png)

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

## Editar o nome de exibição em um agrupamento

Para alterar o nome de exibição em um agrupamento de projeto:

1. Ir para uma lista de projetos.
1. No menu suspenso **Agrupamento**, selecione **Novo agrupamento**.

1. Clique em **Adicionar agrupamento**, comece a digitar &quot;Nome do Portfolio&quot; no campo **Agrupar por:** e selecione-o quando ele for exibido na lista.

1. Clique em **Alternar para Modo de Texto**.
1. Siga um destes procedimentos:

   * Adicione o seguinte código ao texto existente disponível na caixa **Agrupar seu relatório**:


     `group.0.displayname=Your Value`


     Por exemplo, adicione o seguinte código para alterar o nome de exibição para &quot;Portfolio&quot;:

     `group.0.displayname=Portfolio`

   * Remova todas as linhas na interface do modo de texto do agrupamento que tenham a palavra &quot;name&quot; nelas e, em seguida, adicione a linha:

     `group.0.name=Your Value`

     Por exemplo, adicione o seguinte código para alterar o nome de exibição para &quot;Portfolio&quot;:

     `group.0.name=Portfolio`

     >[!TIP]
     >
     >Você também pode deixar as linhas `group.0.name=` e `group.0.displayname=` em branco, nesse caso, o agrupamento mostra o valor pelo qual você está sendo agrupado.


     ![](assets/grouping-edited-name-no-name-350x162.png)

1. Clique em **Concluído** e em **Salvar agrupamento**.
1. (Opcional) Atualize o nome do agrupamento e clique em **Salvar agrupamento**.

   O nome padrão do agrupamento é modificado de acordo com as informações do modo de texto.
