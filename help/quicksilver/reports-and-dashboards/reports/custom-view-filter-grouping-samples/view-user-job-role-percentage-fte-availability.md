---
content-type: reference
product-area: reporting;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: "Exibir: porcentagem da função de trabalho do usuário da disponibilidade do FTE"
description: Você pode adicionar uma coluna à exibição de uma lista de usuários para exibir uma lista das funções de tarefa às quais o usuário está associado, bem como a porcentagem de disponibilidade do FTE para cada função, conforme definido no perfil do usuário.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: d479b0b1-8ad5-47d6-8ef8-80261b46ecea
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '353'
ht-degree: 0%

---

# Exibição: porcentagem da Função de Trabalho do usuário de disponibilidade de FTE

É possível adicionar uma coluna à exibição de uma lista de usuários para exibir uma lista das Funções de trabalho às quais o usuário está associado, bem como o percentual de disponibilidade de FTE para cada função de trabalho, conforme definido no perfil do usuário.

Para obter informações sobre como definir a porcentagem de disponibilidade de FTE para usuários, consulte [Editar perfil de usuário](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

![user_with_percent_avialbility_per_role.png](assets/user-with-percent-avialbility-per-role-350x138.png)

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plano da Adobe Workfront*</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Solicitar para modificar uma exibição </p>
   <p>Planejar modificar um relatório</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a relatórios, painéis e calendários para modificar um relatório</p> <p>Editar acesso a Filtros, Visualizações, Agrupamentos para modificar uma visualização</p> <p><b>Nota</b>

Se você ainda não tem acesso, pergunte ao administrador da Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador da área de trabalho pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis</a> de acesso personalizados.</p> </td>
</tr>   
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões para um relatório</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso aos objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qual plano, tipo de licença ou acesso, entre em contato com o administrador da área de trabalho.

## Visualizar a porcentagem de função de trabalho do usuário da disponibilidade do FTE

1. Vá para uma lista de usuários.
1. No menu suspenso **Exibir**, selecione **Nova Exibição**.

1. Na área **Visualização da coluna**, clique em **Adicionar coluna**.

1. Clique no cabeçalho da nova coluna e, em seguida, clique **em Alternar para modo** de texto.
1. Passe o mouse sobre a área do modo de texto e clique **em Clicar para editar o texto**.
1. Remova o texto encontrado na **caixa Modo** de texto e substitua-o pelo seguinte código:
   <pre>displayname=Roles Time Percentagem<br>listdelimiter=<p><br>listmethod=aninhado (userRoles).lists<br>textmode=true<br>type=iterate<br>valueexpression=CONCAT({role},'-',{timePercentage}'%')<br>valueformat=HTML</pre>

1. Clique **em Salvar** e, em seguida **, em Salvar exibição**.

1. (Opcional) Especifique um nome para sua exibição e clique **em Salvar visualização**.
