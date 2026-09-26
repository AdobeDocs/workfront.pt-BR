---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: Excluir perfis de folha de horas
description: Você pode excluir um perfil de planilha de horas que pode não ser mais relevante.
author: Lisa
feature: Timesheets
exl-id: 1fb39f74-205b-485e-9e8b-a2ab3f9f1ac4
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
subfeature_v2:
  - id: ce22a157-dd2c-405f-b740-c2f204bb4c1a
    internal-label: Timesheets
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
source-git-commit: 4c642a8ef31f3b9a03288f2d74e704be6ee86c55
workflow-type: tm+mt
source-wordcount: '259'
ht-degree: 18%
---
# Excluir perfis de folha de horas

<!--Audited:6/2025-->

A criação e atribuição de perfis de folha de horas a usuários garante a consistência na maneira como o Adobe Workfront cria suas folhas de horas.

Você pode excluir um perfil de planilha de horas que pode não ser mais relevante.

Para obter informações sobre perfis de folha de horas, consulte [Criar, editar e atribuir perfis de folha de horas](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo.

<table style="table-layout:auto">
 <col> 
 <col>
 <tbody> 
  <tr> 
   <td>Pacote do Adobe Workfront</td> 
   <td><p>Qualquer</p></td> 
  </tr> 
  <tr> 
   <td>Licença do Adobe Workfront</td> 
   <td>
   <p>Padrão</p>
   <p>Plano</p></td>
  </tr> 
  <tr> 
   <td>Configurações de nível de acesso</td> 
   <td><p>Acesso administrativo a planilhas de horas</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Excluir perfis de folha de horas

{{step-1-to-setup}}

1. Se você estiver excluindo um perfil de planilha de horas no nível do sistema, clique em **Folhas de horas e Horas > Perfis de Planilha de Horas**.

   Ou

   Se você estiver excluindo um perfil de planilha de horas de um grupo, clique em **Grupos** > clique no nome do grupo e, em seguida, clique em **Perfis de Planilha de Horas**.

1. Para o nível do sistema, selecione pelo menos um perfil de planilha de horas que você deseja excluir e clique no ícone **Mais** ![Mais ícone](assets/more-icon.png) > **Excluir**.

   Ou

   Clique em **Mais** > **Excluir** para o perfil da folha de horas de nível de grupo.

1. (Condicional) Se o perfil da folha de horas já estiver atribuído aos usuários, a caixa **Perfil de Folha de Horas de Substituição** será exibida. Faça o seguinte:
   1. Selecione outro perfil de planilha de horas na lista suspensa. O perfil de planilha de horas que você está excluindo será substituído pelo perfil de planilha de horas com o qual você o substitui para todos os usuários atribuídos. As folhas de horas serão geradas de acordo com o perfil atribuído recentemente no ciclo de geração de folha de horas a seguir.
   1. Clique em **Excluir** para confirmar a exclusão.

1. (Condicional) Se o perfil de folha de horas não for atribuído a usuários, a caixa **Excluir folha de horas** será exibida.

   Clique em **Excluir** para confirmar a exclusão.
