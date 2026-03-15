---
content-type: reference
product-area: reporting;projects;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Exibir: Projeto com Todos os Usuários e Funções da Equipe do Projeto'
description: Este modo de exibição de projeto mostra uma lista de usuários e funções de trabalho atribuídas à equipe do projeto.
author: Courtney
feature: Reports and Dashboards
exl-id: 84a1e065-992e-4aa5-81ba-e699ac704837
source-git-commit: 6a6d3d47ed5741e3202c44b7240a2e67b687ea95
workflow-type: tm+mt
source-wordcount: '330'
ht-degree: 14%

---

# Exibição: projeto com todos os usuários e funções da equipe do projeto

<!--Audited: 11/2024-->

Este modo de exibição de projeto mostra uma lista de usuários e funções de trabalho atribuídas à equipe do projeto.

>[!NOTE]
>
>Se a função de trabalho estiver listada na mesma linha que um usuário, isso não significa que o usuário está preenchendo essa função no projeto nem que o usuário recebe essa função em seu perfil.

![project_custom_view_with_all_users_and_roles_on_the_project_.png](assets/project-custom-view-350x52.png)

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

## Exibir um projeto com todos os usuários e funções da equipe do projeto

1. Ir para uma lista de projetos.
1. No menu suspenso **Exibição**, selecione **Nova Exibição**.

1. Na área **Visualização de coluna**, elimine todas as colunas, exceto uma.
1. Clique no cabeçalho da coluna restante e clique em **Alternar para o Modo de Texto** > **Editar Modo de Texto**.
1. Remova o texto encontrado na caixa **Editar Modo de Texto** e substitua-o pelo seguinte código:




   <pre>column.0.link.linkproperty.0.name=ID<br>column.0.link.linkproperty.0.valuefield=ID<br>column.0.link.linkproperty.0.valueformat=int<br>column.0.link.lookup=link.view<br>column.0.link.valuefield=objCode<br>column.0.link.valueformat=val<br>column.0.linkedname=direct<br>column.0.listsort=string(name)<br>column.0.namekey name.abbr<br>column.0.querysort=name<br>column.0.shortview=false<br>column.0.stretch=60<br>column.0.valuefield=name<br>column.0.valueformat=HTML<br>column.0.width=150<br>column.1.description=Equipe Usuários<br>column.1.link.linkproperty.0.name=ID<br>column.1.link.linkproperty.0.valuefield=userID<br>column.1.link.linkproperty.0.valueformat=int<br>column.1.link.page=/userView.cmd<br>column.1.listdelimiter=<br>column.1.listmethod=nested(projectUsers).lists<br>column.1.namekey=user.column<br>column.column.2 1.valueformat=HTML HTML<br>column.1.width=150<br>column.2.description=Equipe Roles<br>column.2.link.linkproperty.0.name=ID<br>column.2.link.linkproperty.0.valuefield=ID<br>column.2.link.linkproperty.0.valueformat=int<br>column.2.link.page=/roleView.cmd<br>column.2.listdelimiter=<br>column.2.listmethod=nested(roles).lists<br>column.2.namekey=jobrole.plural<br>column.itercolumn.2<br><br><br><br><br><br><br></pre>

1. Clique em **Concluído** > **Salvar Exibição**.
