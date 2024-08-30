---
product-area: resource-management
navigation-topic: resource-pools
title: Remover usuários do conjunto de recursos
description: Embora não haja limite para o número de usuários que você pode ter em um pool de recursos, a lista de usuários exibe apenas os primeiros 2000 usuários, listados em ordem alfabética.
author: Lisa
feature: Resource Management
exl-id: b888aa95-8d42-4cc3-8a99-6842435c84d2
source-git-commit: a9d507bfcc0a602e71bcdd3142d63cc40175ebf4
workflow-type: tm+mt
source-wordcount: '378'
ht-degree: 1%

---

# Remover usuários do conjunto de recursos

{{preview-and-fast-release-Q424}}

Embora não haja limite para o número de usuários que você pode ter em um pool de recursos, a lista de usuários exibe apenas os primeiros 2000 usuários, listados em ordem alfabética.

Recomendamos que você remova os usuários que foram desativados ou que moveram funções ou departamentos para garantir que sempre tenha uma lista precisa de usuários em todos os pools de recursos.

Para obter mais informações sobre pools de recursos, consulte [Visão geral dos pools de recursos](../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md).

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront</td> 
   <td><p>Novo: Qualquer um</p>
       <p>ou</p>
       <p>Atual: Pro e superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td><p>Novo: Padrão</p>
       <p>ou</p>
       <p>Atual: Plano</p></td>
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Editar acesso ao Gerenciamento de recursos que inclui acesso a Gerenciar conjuntos de recursos</p> <p>Acesso de visualização ou superior aos usuários</p></td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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

   ![Remover usuários do Pool de Recursos](assets/remove-users-from-resource-pool.png)

   Imagem de amostra no ambiente de produção:
   ![Pesquisar no Pool de Recursos](assets/search-inside-new-resource-pool-350x314.png)

1. Clique no ícone &quot;x&quot; no nível do usuário para remover um usuário do Conjunto de recursos. Eles são removidos de todas as listas em que aparecem.\
   Ou\
   Para remover todos os usuários associados a uma função de trabalho, grupo, equipe ou empresa, clique em **Remover** no nível de função de trabalho, grupo, equipe ou empresa. Isso remove todos os usuários associados a essa função de trabalho, grupo, equipe ou empresa do Conjunto de Recursos.

1. Clique em **Salvar**.
