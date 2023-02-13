---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '"Agrupamento: editar o nome de exibição em um agrupamento'''
description: É possível renomear agrupamentos para algo mais familiar aos usuários.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 072d3c2b-9ede-4bb9-9a27-dc77ceb732c4
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '323'
ht-degree: 0%

---

# Agrupamento: editar o nome de exibição em um agrupamento

É possível renomear agrupamentos para algo mais familiar aos usuários.

Por exemplo, ao aplicar o agrupamento Portfolio Name padrão a uma lista de projetos, o nome do agrupamento aparece como *Portfolio: Nome:`<name of portfolio>`*.

![](assets/grouping-unedited-name-350x167.png)

Você pode modificar esse agrupamento usando o modo de texto para exibir um nome mais fácil de ler.

![](assets/grouping-edited-name-350x160.png)

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

## Editar o nome de exibição em um agrupamento

Para alterar o nome de exibição em um agrupamento de projeto:

1. Acesse uma lista de projetos.
1. No **Agrupamento**, selecione **Novo agrupamento**.

1. Clique em **Adicionar agrupamento** e comece a digitar &quot;Nome do Portfolio&quot; no **Primeiro por:** e, em seguida, selecione-o quando for exibido na lista.

1. Clique em **Alternar para o modo de texto**.
1. Feito um dos seguintes procedimentos:

   * Adicione o seguinte código ao texto existente disponível na **Agrupar seu relatório** Caixa:

      ```
      group.0.displayname=Your
      ```

      ```
      Value
      ```

      Ou, neste caso:

      ```
      group.0.displayname=Portfolio
      ```

   * Remova todas as linhas na interface do modo de texto do agrupamento que têm a palavra &quot;name&quot; nelas e adicione a linha:

      ```
      group.0.name=Your Value
      ```

      Ou, neste caso:

      ```
      group.0.name=Portfolio
      ```

      Você também pode deixar a variável

      ```
      group.0.name
      ```

      em branco, nesse caso, o agrupamento mostra o nome do valor que você está agrupando por.

      ![](assets/grouping-edited-name-no-name-350x162.png)

1. Clique em **Concluído**, em seguida **Salvar Agrupamento**.
