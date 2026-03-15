---
content-type: reference
product-area: reporting;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Exibir: Percentual de Disponibilidade FTE da Função de Job do Usuário'
description: Você pode adicionar uma coluna à exibição de uma lista de usuários para exibir uma lista das Funções de Job às quais o usuário está associado, bem como o percentual de disponibilidade de FTE para cada função de job, conforme definido no perfil do usuário.
author: Courtney
feature: Reports and Dashboards
exl-id: d479b0b1-8ad5-47d6-8ef8-80261b46ecea
source-git-commit: 6a6d3d47ed5741e3202c44b7240a2e67b687ea95
workflow-type: tm+mt
source-wordcount: '276'
ht-degree: 17%

---

# Exibição: porcentagem da função no trabalho do usuário em relação à disponibilidade de FTE

<!--Audited: 11/2024-->

Você pode adicionar uma coluna à exibição de uma lista de usuários para exibir uma lista das Funções de Job às quais o usuário está associado, bem como o percentual de disponibilidade de FTE para cada função de job, conforme definido no perfil do usuário.

Para obter informações sobre como definir a porcentagem de disponibilidade de FTE para usuários, consulte [Editar o perfil de um usuário](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

![user_with_percent_availability_per_role.png](assets/user-with-percent-avialbility-per-role-350x138.png)

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

## Exibir porcentagem da Função de Trabalho do usuário da disponibilidade de FTE

1. Vá para uma lista de usuários.
1. No menu suspenso **Exibição**, selecione **Nova Exibição**.

1. Na área **Visualização da Coluna**, clique em **Adicionar Coluna**.

1. Clique no cabeçalho da nova coluna e clique em **Alternar para o Modo de Texto** > **Editar Modo de Texto**.
1. Remova o texto encontrado na caixa **Editar Modo de Texto** e substitua-o pelo seguinte código:

   ```
   displayname=Roles Time Percentage
   listdelimiter=
   listmethod=nested(userRoles).lists
   textmode=true
   type=iterate
   valueexpression=CONCAT({role},'-',{timePercentage},'%')
   valueformat=HTML
   ```

1. Clique em **Concluído** e depois em **Salvar exibição**.

1. (Opcional) Atualize o nome da exibição e clique em **Salvar Exibição**.
