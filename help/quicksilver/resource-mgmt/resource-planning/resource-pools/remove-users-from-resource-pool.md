---
product-area: resource-management
navigation-topic: resource-pools
title: Remover usuários do conjunto de recursos
description: Embora não haja limite para o número de usuários que você pode ter em um pool de recursos, a lista de usuários exibe apenas os primeiros 2000 usuários, listados em ordem alfabética.
author: Lisa
feature: Resource Management
exl-id: b888aa95-8d42-4cc3-8a99-6842435c84d2
source-git-commit: 00afc0cbc58fce34059302dfeb8847cfacb9c7e4
workflow-type: tm+mt
source-wordcount: '401'
ht-degree: 1%

---

# Remover usuários do conjunto de recursos

{{highlighted-preview}}

Embora não haja limite para o número de usuários que você pode ter em um pool de recursos, a lista de usuários exibe apenas os primeiros 2000 usuários, listados em ordem alfabética.

Recomendamos que você remova os usuários que foram desativados ou que moveram funções ou departamentos para garantir que sempre tenha uma lista precisa de usuários em todos os pools de recursos.

Para obter mais informações sobre pools de recursos, consulte [Visão geral dos pools de recursos](../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md).

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront*</td> 
   <td> <p>Pro e superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Plano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso ao Gerenciamento de recursos que inclui acesso a Gerenciar conjuntos de recursos</p> <p>Acesso de visualização ou superior aos usuários</p> <p>Observação: se você ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode alterar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Object permissions</td> 
    <td> <p>(NOTE:&nbsp;I don't think this is needed for removing users from the pool)</p> <p>Manage permissions for the projects, templates, and users you associate the Resource Pools with</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
   </tr>
  --> 
 </tbody> 
</table>

&#42;Para saber qual plano, tipo de licença ou acesso você tem, contate o administrador do Workfront.

+++

## Remover usuários de um Conjunto de Recursos

Você pode remover usuários de um Conjunto de recursos quando eles não forem mais necessários nesse conjunto.

Para remover um usuário de um Conjunto de Recursos:

{{step1-to-resourcing}}

1. Clique em **Conjuntos de Recursos** no painel esquerdo.
1. Selecione um Conjunto de Recursos e clique em **Editar**.
Ou\
   Clique no nome de um Conjunto de Recursos.

1. Comece digitando o nome de um usuário que deseja remover no campo **Pesquisar neste Pool de Recursos**.\
   Ou\
   Comece a digitar o nome de uma empresa, função de trabalho, equipe ou grupo se quiser remover todos os usuários associados a essas entidades.

   <span class="preview">Imagem de exemplo no ambiente de Visualização:<span>
   <span class="preview">![Remover usuários do Pool de Recursos](assets/remove-users-from-resource-pool.png)<span>

   Imagem de amostra no ambiente de produção:
   ![Pesquisar no Pool de Recursos](assets/search-inside-new-resource-pool-350x314.png)

1. Clique no ícone &quot;x&quot; no nível do usuário para remover um usuário do Conjunto de recursos. Eles são removidos de todas as listas em que aparecem.\
   Ou\
   Para remover todos os usuários associados a uma função de trabalho, grupo, equipe ou empresa, clique em **Remover** no nível de função de trabalho, grupo, equipe ou empresa. Isso remove todos os usuários associados a essa função de trabalho, grupo, equipe ou empresa do Conjunto de Recursos.

1. Clique em **Salvar**.
