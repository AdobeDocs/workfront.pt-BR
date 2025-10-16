---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Agrupamento: editar o nome de exibição em um agrupamento'
description: É possível renomear agrupamentos em listas e relatórios para algo mais familiar aos usuários.
author: Nolan
feature: Reports and Dashboards
exl-id: 072d3c2b-9ede-4bb9-9a27-dc77ceb732c4
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '351'
ht-degree: 0%

---

# Agrupamento: editar o nome de exibição em um agrupamento

<!--Audited: 01/2024-->

É possível renomear agrupamentos para algo mais familiar aos usuários.

Por exemplo, ao aplicar o agrupamento padrão do Portfolio Name a uma lista de projetos, o nome do agrupamento aparece como *Portfolio: Name:`<name of portfolio>`*.

![Agrupamento por nome não editado](assets/grouping-unedited-name-350x167.png)

Você pode modificar esse agrupamento usando o modo texto para exibir um nome mais fácil de ler.

![Agrupamento por nome editado](assets/grouping-edited-name-350x160.png)

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo. 

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
   <p>Colaborador ou Solicitação para modificar um filtro </p>
   <p>Padrão ou Plano para modificar um relatório</p>
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

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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


     ![Agrupamento por nome editado sem nome](assets/grouping-edited-name-no-name-350x162.png)

1. Clique em **Concluído** e em **Salvar agrupamento**.
1. (Opcional) Atualize o nome do agrupamento e clique em **Salvar agrupamento**.

   O nome padrão do agrupamento é modificado de acordo com as informações do modo de texto.
