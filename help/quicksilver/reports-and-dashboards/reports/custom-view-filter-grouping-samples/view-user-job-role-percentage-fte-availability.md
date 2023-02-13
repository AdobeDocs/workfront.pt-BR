---
content-type: reference
product-area: reporting;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: '"Exibir: Percentual da Função de Trabalho do Usuário da disponibilidade de FTE'''
description: É possível adicionar uma coluna à visualização de uma lista de usuários para exibir uma lista das Funções de Trabalho às quais o usuário está associado, bem como a porcentagem da disponibilidade do FTE para cada função de cargo, conforme definido no perfil do usuário.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: d479b0b1-8ad5-47d6-8ef8-80261b46ecea
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '341'
ht-degree: 0%

---

# Exibir: Percentual da Função de Trabalho do Usuário da disponibilidade de FTE

É possível adicionar uma coluna à visualização de uma lista de usuários para exibir uma lista das Funções de Trabalho às quais o usuário está associado, bem como a porcentagem da disponibilidade do FTE para cada função de cargo, conforme definido no perfil do usuário.

Para obter informações sobre como definir a porcentagem de disponibilidade de FTE para usuários, consulte [Editar o perfil de um usuário](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

![user_with_percent_avialbility_per_role.png](assets/user-with-percent-avialbility-per-role-350x138.png)

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

## Exibir porcentagem da Função de Trabalho do usuário da disponibilidade de FTE

1. Vá para uma lista de usuários.
1. No **Exibir** , selecione **Nova exibição**.

1. No **Visualização de coluna** , clique em **Adicionar coluna**.

1. Clique no cabeçalho da nova coluna e, em seguida, clique em **Alternar para o modo de texto**.
1. Passe o mouse sobre a área do modo de texto e clique em **Clique para editar texto**.
1. Remova o texto que você encontrar no **Modo de texto** e substitua-a pelo seguinte código:

   <pre>exibir nome=Percentual de Tempo das Funções<br>listdelimiter=<p><br>listmethod=nested(userRoles).lists<br>textmode=true<br>type=iterate<br>valueexpression=CONCAT({role},'-',{timePercentage},'%')<br>valueformat=HTML</pre>

1. Clique em **Salvar**, em seguida **Salvar exibição**.

1. (Opcional) Especifique um nome para sua exibição e clique em **Salvar exibição**.
