---
content-type: reference
product-area: reporting;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: "Exibir: Porcentagem da Disponibilidade de FTE da Função de Usuário"
description: É possível adicionar uma coluna à exibição de uma lista de usuários para exibir uma lista das Funções de trabalho às quais o usuário está associado, bem como o percentual de disponibilidade de FTE para cada função de trabalho, conforme definido no perfil do usuário.
author: Nolan
feature: Reports and Dashboards
exl-id: d479b0b1-8ad5-47d6-8ef8-80261b46ecea
source-git-commit: 66de6c952272f52876f8e912c96d1526575b6f0b
workflow-type: tm+mt
source-wordcount: '297'
ht-degree: 0%

---

# Exibição: porcentagem da Função de Trabalho do usuário de disponibilidade de FTE

<!--Audited: 11/2024-->

É possível adicionar uma coluna à exibição de uma lista de usuários para exibir uma lista das Funções de trabalho às quais o usuário está associado, bem como o percentual de disponibilidade de FTE para cada função de trabalho, conforme definido no perfil do usuário.

Para obter informações sobre como definir a porcentagem de disponibilidade de FTE para usuários, consulte [Editar perfil de usuário](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

![usuário_com_disponibilidade_percentual_por_função.png](assets/user-with-percent-avialbility-per-role-350x138.png)

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td> <p> Atual: 
   <ul>
   <li>Solicitação para modificar uma exibição</li> 
   <li>Planejar a modificação de um relatório</li>
   </ul>
     </p>
     <p> Novo: 
   <ul>
   <li>Colaborador para modificar uma visualização</li> 
   <li>Padrão para modificar um relatório</li>
   </ul>
     </p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a relatórios, painéis e calendários para modificar um relatório</p> <p>Editar acesso a Filtros, Visualizações, Agrupamentos para modificar uma visualização</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões para um relatório</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Exibir percentual da Função de Trabalho do usuário de disponibilidade de FTE

1. Ir para uma lista de usuários.
1. No menu suspenso **Exibir**, selecione **Nova Exibição**.

1. Na área **Visualização da coluna**, clique em **Adicionar coluna**.

1. Clique no cabeçalho da nova coluna e em **Alternar para Modo de Texto** > **Editar Modo de Texto**.
1. Remova o texto localizado na caixa **Editar Modo de Texto** e substitua-o pelo seguinte código:

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

1. (Opcional) Atualize o nome da exibição e clique em **Salvar exibição**.
