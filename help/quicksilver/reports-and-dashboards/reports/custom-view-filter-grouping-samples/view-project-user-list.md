---
content-type: reference
product-area: reporting;projects;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: "Exibição: lista de usuários do projeto com funções de trabalho"
description: Você pode aplicar essa visualização em uma lista de projeto ou relatório para exibir uma lista de usuários associados ao projeto, bem como uma lista das funções de trabalho que eles estão executando no projeto.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: a3f59f69-7f39-4814-bd2f-7734d620081e
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '449'
ht-degree: 0%

---

# Exibição: lista de usuários do projeto com funções de trabalho

Você pode aplicar essa visualização em uma lista de projeto ou relatório para exibir uma lista de usuários associados ao projeto, bem como uma lista das funções de trabalho que eles estão executando no projeto.

As informações neste relatório também podem ser encontradas na área Pessoas do projeto.

>[!TIP]
>
>Se nenhuma função de trabalho for listada para os usuários, mas você souber que eles estão associados a funções de trabalho em seus perfis de usuário, isso pode significar que eles estão atribuídos a tarefas e problemas, mas podem não estar associados a uma função de trabalho na tarefa ou problema, ou os usuários listados no relatório não são os atribuídos em tarefas e problemas, mas cumprem outras funções no projeto (por exemplo, Proprietário ou Patrocinador).

![projeto_com_usuário_e_função_informações_relatório.png](assets/project-with-user-and-role-information-report-350x100.png)

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
   <td> <p>Solicitação para modificar uma exibição </p>
   <p>Planejar a modificação de um relatório</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a relatórios, painéis e calendários para modificar um relatório</p> <p>Editar acesso a Filtros, Visualizações, Agrupamentos para modificar uma visualização</p> <p><b>Nota</b>

Se você ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td>
</tr>  
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões para um relatório</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso aos objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qual plano, tipo de licença ou acesso você tem, contate o administrador do Workfront.

## Exibir uma lista de usuários do projeto com funções de trabalho

1. Ir para uma lista de projetos.
1. No menu suspenso **Exibir**, selecione **Nova Exibição**.

1. Na área **Visualização da coluna**, elimine todas as colunas, exceto uma.
1. Clique no cabeçalho da coluna restante e em **Alternar para Modo de Texto**.
1. Passe o mouse sobre a área de modo de texto e clique em **Clicar para editar o texto**.
1. Remova o texto localizado na caixa **Modo de Texto** e substitua-o pelo seguinte código:
   <pre>column.0.link.valueformat=val<br>column.0.linkedname=direct<br>column.0.listsort=string(name)<br>column.0.namekey=name.abbr<br>column.0.querysort=name<br>column.0.section=0<br>column.0.shortview=false<br>column.0.stretch=100<br>column.0.valuefield=name<br>column.0.valueformat=HTML<br>column.0.width=200 10}coluna.1.displayname=Usuários do Projeto<br>coluna.1.listdelimititer=&lt;br&gt;<br>coluna.1.listmethod=nested(projectUsers).lists<br>coluna.1.textmode=true<br>coluna.1.type=iterate<br>coluna.1.valueexpression={user}.<br>{name}<br>coluna.1.valueformat=HTML<br>coluna.2.displayname=Funções de Projeto<br>coluna.2.listdelimititer=&lt;br&gt;<br>coluna.2.listmethod=nested(projectUserRoles).lists<br>coluna.2.textmode=true<br>coluna.2.type=iterate<br>coluna.2.valueexpression={role}.{name}<br>column.2.valueformat=HTML</pre>

1. Clique em **Salvar visualização**.
