---
product-area: reporting
navigation-topic: reporting-elements
title: Remover filtros, visualizações e agrupamentos
description: É possível remover um filtro, uma exibição ou um agrupamento de listas e relatórios se você os criou ou se eles foram compartilhados com você. Não é possível remover filtros, visualizações ou agrupamentos padrão.
author: Lisa
feature: Reports and Dashboards
exl-id: 422d262e-e19d-4070-85f1-77ecb7430342
source-git-commit: b56e6591c7da166bd1548420b562b838cc7fe0f2
workflow-type: tm+mt
source-wordcount: '869'
ht-degree: 0%

---

# Remover filtros, visualizações e agrupamentos

<span class="preview">Observe que, no ambiente de Pré-visualização, a experiência de filtro aprimorada (anteriormente chamada de &quot;beta&quot;) agora é o padrão. Esses filtros aprimorados agora são &quot;padrão&quot; e a experiência de filtro mais antiga é &quot;herdada&quot;.</span>

É possível remover um filtro, uma exibição ou um agrupamento de listas e relatórios se você os criou ou se eles foram compartilhados com você. Não é possível remover filtros, visualizações ou agrupamentos padrão.

## Requisitos de acesso

Você deve ter o seguinte:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>plano do Adobe Workfront*</strong></td> 
   <td> <p>Qualquer Um </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Licença da Adobe Workfront*</strong></td> 
   <td> <p>Solicitação ou superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurações de nível de acesso*</strong></td> 
   <td> <p>Acesso de visualização ou superior a filtros, visualizações, agrupamentos</p> <p>Observação: se você ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Permissões de objeto</strong></td> 
   <td> <p>Exibir permissões com acesso para compartilhar com o filtro, exibição ou agrupamento que você deseja remover</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir seu plano, tipo de licença ou acesso, entre em contato com o administrador do Workfront.

## Remover um filtro, uma visualização ou um agrupamento usando o construtor padrão

Você pode remover um filtro, uma visualização ou um agrupamento de todas as listas de objetos usando a interface do construtor padrão.

### Considerações sobre a remoção de filtros, visualizações e agrupamentos

A maneira como você remove um elemento de relatório depende se você o criou inicialmente ou se ele foi compartilhado com você.

Os cenários a seguir existem ao remover um agrupamento:

* **Se você criou o agrupamento e o removeu**, o agrupamento é removido do sistema Workfront. O agrupamento não está mais disponível para os usuários com quem você o compartilhou anteriormente.
* **Se o agrupamento foi compartilhado com você e você o removeu**, o agrupamento será removido somente para você. O usuário que o criou originalmente e todos os outros usuários com os quais ele foi compartilhado ainda têm acesso ao agrupamento.

### Remover um filtro, uma visualização ou um agrupamento usando o construtor padrão

1. Ir para uma lista de objetos ou um relatório.
1. (Condicional) Em uma lista, clique no link **Filtro**, **Exibir** ou **Agrupamento** e passe o mouse sobre o filtro, a exibição ou o agrupamento que deseja remover, clique no ícone **Mais** ícone ![](assets/more-icon.png), depois **Remover**. O filtro, a visualização ou o agrupamento é removido.
1. (Condicional) Em um relatório, clique no link **Agrupamento**, **Filtro** ou **Exibir** e selecione **Remover agrupamento**, **Remover filtro** ou **Remover Visão**.

   A variável **Meus Agrupamentos**, **Meus filtros,** ou **Minhas Visualizações** é exibida.

   Todos os elementos de relatórios que você tem direitos para remover estão disponíveis para remoção. Outros elementos de relatórios são exibidos como esmaecidos.

1. Clique em **x** ícone ao lado de qualquer elemento de relatório que você deseja remover.
1. (Condicional) Clique em **Sim, exclua** se você optou por excluir um filtro, uma exibição ou um agrupamento criado e compartilhado posteriormente com outras pessoas. Isso exclui o filtro, a exibição ou o agrupamento do sistema do Workfront.

   >[!TIP]
   >
   >Remover um filtro, uma visualização ou um agrupamento que você criou sem compartilhá-lo com outras pessoas remove-o do sistema sem solicitar uma confirmação.

1. Clique em **Concluído**.

## Remover ou excluir um filtro usando o construtor beta

Você pode remover um filtro que foi compartilhado com você em listas de projetos, tarefas ou problemas usando a interface do construtor beta. A interface do construtor beta não está disponível para outros objetos, exibições ou agrupamentos.

Também é possível excluir filtros de sua propriedade de listas de projetos, tarefas ou problemas usando a interface do construtor beta.

Os filtros padrão do sistema não podem ser removidos ou excluídos.

### Considerações sobre a remoção ou exclusão de filtros usando o construtor beta

Os cenários a seguir existem ao remover ou excluir um filtro:

* Se o filtro foi compartilhado com você e você o remove, o filtro é removido somente para você. O usuário que o criou originalmente e todos os outros usuários com os quais ele foi compartilhado ainda têm acesso ao filtro.
* Se você for o proprietário do filtro e excluí-lo, ele será removido do sistema do Workfront. O filtro não está mais disponível para os usuários com quem você o compartilhou anteriormente.
* Se você for um administrador do Workfront, é possível excluir o filtro, que é excluído permanentemente para todos os usuários, incluindo o proprietário.

### Remover um filtro usando o construtor beta

1. Ir para uma lista de projetos, tarefas ou problemas.
1. Clique em **Filtro** ícone ![Ícone Filtrar](assets/filter-nwepng.png) e ative o construtor beta, se necessário.
1. Passe o mouse sobre um filtro em **Compartilhado comigo**, clique no link **Mais** menu ![Ícone Mais](assets/more-icon-spectrum.png)e, em seguida, clique em **Remover**.

   ![Remover filtro](assets/new-filters-more-menu-remove-filter.png)

1. Selecionar **Remover** na mensagem de confirmação para remover permanentemente o filtro.

### Excluir um filtro usando o construtor beta

1. Ir para uma lista de projetos, tarefas ou problemas.
1. Clique em **Filtro** ícone ![Ícone Filtrar](assets/filter-nwepng.png) e ative o construtor beta, se necessário.
1. Passe o mouse sobre um filtro que você tem permissão para excluir, clique no **Mais** menu ![Ícone Mais](assets/more-icon-spectrum.png)e, em seguida, clique em **Excluir**.

   ![Excluir Filtro](assets/new-filters-more-menu-options-with-delete.png)

1. (Opcional) Clique em **Cancelar** na mensagem de confirmação para evitar a exclusão e retornar à lista de filtros.
1. Clique em **Excluir** na mensagem de confirmação para confirmar a exclusão.

   O filtro é excluído para você e todos os usuários que têm permissões para ele.

