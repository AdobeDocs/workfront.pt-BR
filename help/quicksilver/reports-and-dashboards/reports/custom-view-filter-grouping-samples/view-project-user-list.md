---
content-type: reference
product-area: reporting;projects;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Exibir: Lista de Usuários do Projeto com Funções de Job'
description: Você pode aplicar essa exibição em uma lista de projetos ou relatório para exibir uma lista de usuários associados ao projeto, bem como uma lista das funções de job que estão executando no projeto.
author: Courtney
feature: Reports and Dashboards
exl-id: a3f59f69-7f39-4814-bd2f-7734d620081e
source-git-commit: 6a6d3d47ed5741e3202c44b7240a2e67b687ea95
workflow-type: tm+mt
source-wordcount: '335'
ht-degree: 14%

---

# Exibição: lista de usuários do projeto com funções de trabalho

<!--Audited: 11/2024-->

Você pode aplicar essa exibição em uma lista de projetos ou relatório para exibir uma lista de usuários associados ao projeto, bem como uma lista das funções de job que estão executando no projeto.

As informações deste relatório também podem ser encontradas na área Pessoas do projeto.

>[!TIP]
>
>Se nenhuma função de job estiver listada para os usuários, mas você souber que eles estão associados a funções de job em seus perfis de usuário, isso pode significar que eles estão atribuídos a tarefas e ocorrências, mas eles podem não estar associados a uma função de job na tarefa ou ocorrência, ou os usuários listados no relatório não são os designados em tarefas e ocorrências, mas cumprem outras funções no projeto (por exemplo, Proprietário ou Patrocinador).

![project_with_user_and_role_information_report.png](assets/project-with-user-and-role-information-report-350x100.png)

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo.

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
   <p>Colaborador ou Solicitação de modificação de uma exibição </p>
   <p>Padrão ou Plano para modificar um relatório</p>
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Acesso de edição a relatórios, painéis e calendários para modificar um relatório</p> <p>Acesso de edição a filtros, visualizações, agrupamentos para modificar uma visualização</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões para um relatório</p>  </td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações contidas nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).


+++


## Exibir uma lista de usuários do projeto com funções de job

1. Ir para uma lista de projetos.
1. No menu suspenso **Exibição**, selecione **Nova Exibição**.
1. Na área **Visualização de coluna**, elimine todas as colunas, exceto uma.
1. Clique no cabeçalho da coluna restante e clique em **Alternar para o Modo de Texto** > **Editar Modo de Texto**.
1. Remova o texto encontrado na caixa **Editar Modo de Texto** e substitua-o pelo seguinte código:

   ```
   column.0.link.valueformat=val
   column.0.linkedname=direct
   column.0.listsort=string(name)
   column.0.namekey=name.abbr
   column.0.querysort=name
   column.0.section=0
   column.0.shortview=false
   column.0.stretch=100
   column.0.valuefield=name
   column.0.valueformat=HTML
   column.0.width=200
   column.1.displayname=Project Users
   column.1.listdelimiter=<br>
   column.1.listmethod=nested(projectUsers).lists
   column.1.textmode=true
   column.1.type=iterate
   column.1.valueexpression={user}.{name}
   column.1.valueformat=HTML
   column.2.displayname=Project Roles
   column.2.listdelimiter=<br>
   column.2.listmethod=nested(projectUserRoles).lists
   column.2.textmode=true
   column.2.type=iterate
   column.2.valueexpression={role}.{name}
   column.2.valueformat=HTML
   ```

1. Clique em **Concluído** > **Salvar Exibição**.
