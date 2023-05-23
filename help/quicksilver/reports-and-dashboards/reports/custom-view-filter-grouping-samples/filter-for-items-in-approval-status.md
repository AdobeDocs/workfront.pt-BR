---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: "Filtro: exibir somente itens em um status de aprovação"
description: Você pode exibir somente itens em um determinado status que está atualmente em Aprovação pendente. Isso funciona da mesma forma para qualquer outro objeto com status de aprovação.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: c1de5193-d3d5-406c-aa68-e6ba6d6751ae
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '315'
ht-degree: 1%

---

# Filtro: exibir somente itens em um status de aprovação

Você pode exibir somente itens em um determinado status que está atualmente em Aprovação pendente. Isso funciona da mesma forma para qualquer outro objeto com status de aprovação.

Você pode colocar os seguintes objetos em um status de aprovação:

* Tarefas
* Problemas
* Projetos

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
   <td> <p>Solicitação para modificar um filtro </p>
   <p>Planejar a modificação de um relatório</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a relatórios, painéis e calendários para modificar um relatório</p> <p>Editar acesso a Filtros, Visualizações, Agrupamentos para modificar um filtro</p> <p><b>Nota</b>

Se você ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td>
</tr>
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões para um relatório</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir seu plano, tipo de licença ou acesso, entre em contato com o administrador do Workfront.

## Exibir somente itens no status de aprovação

1. Acesse o filtro que deseja personalizar para obter uma lista de projetos, por exemplo.
1. Clique em **Adicionar uma regra de filtro** para o **Status** do objeto da lista.\
   Por exemplo, em um relatório de projeto, adicione **Planejamento de Status Igual**, se quiser exibir somente projetos com status de **Planejamento - Pendente de Aprovação**.

1. Clique em **Alternar para modo de texto**.
1. Modifique o

   ```
   status
   ```

   linha adicionando **:A** à chave de 3 letras do status:
   <pre>status=PLN:A<br>status_Mod=in</pre>

1. Clique em **Concluído**, depois **Salvar Filtro**.

   A lista exibe somente projetos com status Planejamento - Aprovação Pendente.
