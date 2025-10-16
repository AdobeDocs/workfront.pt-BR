---
product-area: reporting
navigation-topic: reporting-elements
title: Remover filtros, visualizações e agrupamentos
description: É possível remover um filtro, uma exibição ou um agrupamento de listas e relatórios se você os criou ou se eles foram compartilhados com você. Não é possível remover filtros, visualizações ou agrupamentos padrão.
author: Nolan
feature: Reports and Dashboards
exl-id: 422d262e-e19d-4070-85f1-77ecb7430342
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '801'
ht-degree: 1%

---

# Remover filtros, visualizações e agrupamentos

<!-- Audited: 11/2024 -->

É possível remover um filtro, uma exibição ou um agrupamento de listas e relatórios se você os criou ou se eles foram compartilhados com você. Não é possível remover filtros, visualizações ou agrupamentos padrão.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacote do Adobe Workfront</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</strong></td> 
   <td> 
    <p>Colaborador ou superior</p>
    <p>Solicitação ou superior</p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Editar acesso a Filtros, Visualizações, Agrupamentos</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
    <td> <p>Exibir permissões com acesso para compartilhar com o filtro, exibição ou agrupamento que você deseja remover</p></td> 
   </td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Remover ou excluir um filtro usando o construtor padrão

Você pode remover um filtro que foi compartilhado com você em listas de projetos, tarefas ou problemas usando a interface do construtor padrão. A interface padrão do construtor não está disponível para outros objetos, exibições ou agrupamentos.

Também é possível excluir filtros de sua propriedade de listas de projetos, tarefas ou problemas usando a interface do construtor padrão.

Os filtros padrão do sistema não podem ser removidos ou excluídos.

### Considerações sobre a remoção ou exclusão de filtros usando o construtor padrão

Os cenários a seguir existem ao remover ou excluir um filtro usando o construtor padrão:

* Se o filtro foi compartilhado com você e você o remove, o filtro é removido somente para você. O usuário que o criou originalmente e todos os outros usuários com os quais ele foi compartilhado ainda têm acesso ao filtro.
* Se você for o proprietário do filtro e excluí-lo, ele será removido do sistema do Workfront. O filtro não está mais disponível para os usuários com quem você o compartilhou anteriormente.
* Se você for um administrador do Workfront, é possível excluir o filtro, que é excluído permanentemente para todos os usuários, incluindo o proprietário.

### Remover um filtro usando o construtor padrão

1. Vá para uma lista de projetos, tarefas, problemas, portfólios, programas, usuários, modelos ou grupos.
1. Clique no ícone **Filtro** ![Ícone Filtro](assets/filter-nwepng.png).
1. Passe o mouse sobre um filtro em **Compartilhado comigo**, clique no menu **Mais** ![Ícone Mais](assets/more-icon-spectrum.png) e clique em **Remover**.
1. Selecione **Remover** na mensagem de confirmação para remover permanentemente o filtro.

### Excluir um filtro usando o construtor padrão

1. Vá para uma lista de projetos, tarefas, problemas, portfólios, programas, usuários, modelos ou grupos.
1. Clique no ícone **Filtro** ![Ícone Filtro](assets/filter-nwepng.png).
1. Passe o mouse sobre um filtro que você tem permissão para excluir, clique no menu **Mais** ![ícone Mais](assets/more-icon-spectrum.png) e clique em **Excluir**.

   ![Excluir filtro](assets/new-filters-more-menu-options-with-delete.png)

1. (Opcional) Clique em **Cancelar** na mensagem de confirmação para evitar a exclusão e retornar à lista de filtros.
1. Clique em **Excluir** na mensagem de confirmação para confirmar a exclusão.

   O filtro é excluído para você e todos os usuários que têm permissões para ele.

## Remover um filtro, uma visualização ou um agrupamento usando o construtor herdado

Você pode remover um filtro, uma visualização ou um agrupamento de todas as listas de objetos usando a interface do construtor herdada.

### Considerações sobre a remoção de filtros, visualizações e agrupamentos usando o construtor herdado

A maneira como você remove um elemento de relatório depende se você o criou inicialmente ou se ele foi compartilhado com você.

Os cenários a seguir existem ao remover um filtro, uma exibição ou um agrupamento:

* **Se você criou o elemento e o removeu**, ele será removido do sistema Workfront. Ele não está mais disponível para os usuários com os quais você o compartilhou anteriormente.
* **Se o elemento foi compartilhado com você e você o remove**, ele será removido somente para você. O usuário que o criou originalmente e todos os outros usuários com os quais ele foi compartilhado ainda têm acesso a ele.

### Remover um filtro, uma visualização ou um agrupamento usando o construtor herdado

1. Ir para uma lista de objetos ou um relatório.
1. (Condicional) Em uma lista, clique no ícone **Filtro**, **Exibição** ou **Agrupamento** e passe o mouse sobre o filtro, a exibição ou o agrupamento que deseja remover, clique no ícone **Mais** ![Mais ícone](assets/more-icon.png) e **Remover**. O filtro, a visualização ou o agrupamento é removido.
1. (Condicional) Em um relatório, clique no menu suspenso **Agrupamento**, **Filtro** ou **Exibir** e selecione **Remover Agrupamento**, **Remover Filtro** ou **Remover Exibição**.

   A caixa de diálogo **Meus Agrupamentos**, **Meus Filtros** ou **Minhas Exibições** é exibida.

   Todos os elementos de relatórios que você tem direitos para remover estão disponíveis para remoção. Outros elementos de relatórios são exibidos como esmaecidos.

1. Clique no ícone **x** ao lado de qualquer elemento de relatório que você deseja remover.
1. (Condicional) Clique em **Sim, exclua-o** se você selecionou excluir um filtro, exibição ou agrupamento que você criou e depois compartilhou com outras pessoas. Isso exclui o filtro, a exibição ou o agrupamento do sistema do Workfront.

   >[!TIP]
   >
   >Remover um filtro, uma visualização ou um agrupamento que você criou sem compartilhá-lo com outras pessoas remove-o do sistema sem solicitar uma confirmação.

1. Clique em **Concluído**.

