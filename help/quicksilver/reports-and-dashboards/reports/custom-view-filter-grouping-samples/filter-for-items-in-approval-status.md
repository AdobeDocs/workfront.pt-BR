---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '"Filtro: exibir somente itens em um status de aprovação'''
description: Você pode exibir somente itens em um determinado status que esteja atualmente em Aprovação pendente. Isso funciona da mesma forma em qualquer outro objeto com status de aprovação.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: c1de5193-d3d5-406c-aa68-e6ba6d6751ae
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '298'
ht-degree: 1%

---

# Filtro: exibir somente itens em um status de aprovação

Você pode exibir somente itens em um determinado status que esteja atualmente em Aprovação pendente. Isso funciona da mesma forma em qualquer outro objeto com status de aprovação.

Você pode colocar os seguintes objetos em um status de aprovação:

* Tarefas
* Problemas
* Projetos

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

## Exibir somente itens no status de aprovação

1. Acesse o filtro que deseja personalizar para obter uma lista de projetos, por exemplo.
1. Clique em **Adicionar uma regra de filtro** para **Status** do objeto da lista.\
   Por exemplo, em um relatório de projeto, adicione **Status Equal Planning**, se desejar exibir apenas projetos que estão em um status de **Planejamento - Aprovação Pendente**.

1. Clique em **Alternar para o modo de texto**.
1. Modifique o

   ```
   status
   ```

   linha adicionando **:A** à chave de 3 letras do status:
   <pre>status=PLN:A<br>status_Mod=in</pre>

1. Clique em **Concluído**, em seguida **Salvar filtro**.

   A lista exibe apenas projetos que estão em um status de Planejamento - Aprovação Pendente.
