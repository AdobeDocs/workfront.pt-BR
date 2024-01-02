---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: "Agrupamento: editar o nome de exibição em um agrupamento"
description: É possível renomear agrupamentos em listas e relatórios para algo mais familiar aos usuários.
author: Nolan
feature: Reports and Dashboards
exl-id: 072d3c2b-9ede-4bb9-9a27-dc77ceb732c4
source-git-commit: 138181de2ad8257785773a5296bc5bcfc144a801
workflow-type: tm+mt
source-wordcount: '369'
ht-degree: 0%

---

# Agrupamento: editar o nome de exibição em um agrupamento

<!--Audited: 01/2024-->

É possível renomear agrupamentos para algo mais familiar aos usuários.

Por exemplo, quando você aplica o agrupamento de Nome de Portfolio padrão a uma lista de projetos, o nome do agrupamento aparece como *Portfolio: Nome:`<name of portfolio>`*.

![](assets/grouping-unedited-name-350x167.png)

Você pode modificar esse agrupamento usando o modo texto para exibir um nome mais fácil de ler.

![](assets/grouping-edited-name-350x160.png)

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront*</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td>

<p>Novo: </p>
   <ul>
   <li> <p>Colaborador para modificar um agrupamento </p></li>
   <li><p>Padrão para modificar um relatório</p></li></ul>

<p> Atual:</p>
   <ul>  
   <li><p>Solicitação para modificar um agrupamento </p></li>
   <li><p>Planejar a modificação de um relatório</p></li> </td> 
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

## Editar o nome de exibição em um agrupamento

Para alterar o nome de exibição em um agrupamento de projeto:

1. Ir para uma lista de projetos.
1. No **Agrupamento** selecione **Novo Agrupamento**.

1. Clique em **Adicionar Agrupamento** e comece digitando &quot;Portfolio Name&quot; no campo **Primeiro por:** e selecione-o quando ele for exibido na lista.

1. Clique em **Alternar para modo de texto**.
1. Siga um destes procedimentos:

   * Adicione o seguinte código ao texto existente disponível na **Agrupar seu relatório** caixa:


     `group.0.displayname=Your Value`


     Ou, neste caso:

     `group.0.displayname=Portfolio`

   * Remova todas as linhas na interface do modo de texto do agrupamento que tenham a palavra &quot;name&quot; nelas e, em seguida, adicione a linha:

     `group.0.name=Your Value`

     Ou, neste caso:

     `group.0.name=Portfolio`

     >[!TIP]
     >
     >Você também pode deixar a variável `group.0.name=` e a variável `group.0.displayname=` linhas em branco, nesse caso, o agrupamento mostra o valor pelo qual você está agrupando.


     ![](assets/grouping-edited-name-no-name-350x162.png)

1. Clique em **Concluído**, depois **Salvar Agrupamento**.

   O nome padrão do agrupamento é modificado de acordo com as informações do modo de texto.
