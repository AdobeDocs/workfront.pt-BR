---
user-type: administrator
product-area: system-administration;user-management
keywords: gerenciar,subgrupo,editar
navigation-topic: create-and-manage-subgroups
title: Gerenciar um subgrupo
description: Como administrador de grupo de um subgrupo, você pode criar, mover, exibir, editar, copiar, renomear, exportar e excluir o subgrupo. Você também pode tornar um subgrupo um grupo de nível superior removendo-o do grupo pai.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 5186d266-fa9f-445d-9dcc-bc07eb147b60
source-git-commit: a42a167447d2f11b5502e4a0953b5e7eec2e67b1
workflow-type: tm+mt
source-wordcount: '1386'
ht-degree: 0%

---

# Gerenciar um subgrupo

Como administrador de grupo de um subgrupo, você pode criar, mover, exibir, editar, copiar, renomear, exportar e excluir o subgrupo.

Você também pode tornar um subgrupo um grupo de nível superior removendo-o do grupo pai.

Se houver algum grupo acima do seu, os administradores também poderão fazer essas coisas pelo seu grupo. O mesmo se aplica aos administradores do Workfront (para qualquer grupo).

Para obter mais informações sobre subgrupos, consulte [Visão geral dos subgrupos](../../../administration-and-setup/manage-groups/groups-overview/subgroups.md).

>[!TIP]
>
>Ao gerenciar um grupo que contém subgrupos, é útil poder identificar e filtrar dados sobre o grupo inteiro e todos os seus subgrupos. Você pode fazer isso usando o campo ID principal em um relatório ou lista.
>
>Por exemplo, imagine que você gerencia um grande departamento de marketing e deseja uma lista de todos os projetos nos quais todo o departamento está trabalhando.
>
>No Workfront, esse departamento de marketing é representado por um grupo chamado Marketing, com três subgrupos chamados Marketing de campo, Marketing de produto e Marketing digital. Para listar os projetos que pertencem a todo o departamento de marketing (todos os 4 grupos), você pode criar um filtro para a área Projetos com a seguinte regra de filtro:
>
>`Group: Top Parent ID > Equal > Marketing`
>
>Você também pode usar o campo Nome do pai superior para identificar dados associados a um grupo de nível superior, mas somente em exibições, não em filtros ou agrupamentos.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

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
   <td><p>Standard</p>
       <p>Plano</p></td>
  </tr>
  <tr> 
   <td>Configurações de nível de acesso</td> 
   <td>Você deve ser um administrador de grupo do grupo ou um administrador do sistema.</td>
  </tr>
 </tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Criar um subgrupo

{{step-1-to-setup}}

1. No painel esquerdo, clique em **Grupos** ![Grupos](assets/groups-icon.png).

   Na lista exibida, você pode ver os grupos que gerencia, juntamente com quaisquer subgrupos que eles tenham. Os administradores do Adobe Workfront podem visualizar todos os grupos.

1. Clique no nome do grupo ao qual deseja adicionar um subgrupo.
1. No menu esquerdo, clique em **Subgrupos**.
1. Para criar um novo subgrupo um nível abaixo do grupo que você está visualizando, clique em **Adicionar subgrupo**.

   Ou, se quiser criar o novo subgrupo abaixo de outro subgrupo na lista, selecione esse subgrupo e clique em **Adicionar subgrupo**.

   Para obter informações sobre as opções que podem ser usadas para configurar o subgrupo, consulte [Criar um subgrupo](/help/quicksilver/administration-and-setup/manage-groups/create-and-manage-subgroups/create-a-subgroup.md).

   Uma hierarquia de grupo não pode exceder 15 níveis, mas um único nível pode ter um número ilimitado de grupos paralelos.

## Mover um subgrupo

Você pode mover subgrupos existentes para outro grupo que administra.

Uma hierarquia de grupo não pode exceder 15 níveis, mas um único nível pode ter um número ilimitado de grupos paralelos.

{{step-1-to-setup}}

1. No painel esquerdo, clique em **Grupos** ![Grupos](assets/groups-icon.png).

   Na lista exibida, você pode ver os grupos que gerencia, juntamente com quaisquer subgrupos que eles tenham. Os administradores do Adobe Workfront podem visualizar todos os grupos.

1. Clique no nome do grupo de destino (você especificará quais subgrupos deseja mover em uma etapa posterior).
1. No menu esquerdo, clique em **Subgrupos**.
1. (Opcional) Selecione um subgrupo para torná-lo o grupo de destino.

   Se você ignorar esta etapa, o grupo selecionado na etapa 3 será o grupo de destino.

1. Clique em **Adicionar Subgrupo > Grupo Existente**.
1. Na caixa **Grupo Existente** que aparece, comece digitando o nome de um subgrupo que você deseja mover.

   Os resultados exibidos não contêm grupos acima do grupo de destino.

   Você pode verificar se está selecionando o grupo correto passando o cursor do mouse sobre ele e clicando no ícone de informações ![ícone de informações](assets/info-icon.png) que é exibido ao lado dele. Uma dica de ferramenta que lista informações sobre o grupo, como a hierarquia de grupos acima dele e seus administradores.

1. Selecione o nome do subgrupo que deseja mover ao localizá-lo na lista.
1. Repita as etapas 7 a 8 para qualquer outro subgrupo que desejar mover para o grupo de destino.
1. Clique em **Salvar**.

## Editar um subgrupo

{{step-1-to-setup}}

1. No painel esquerdo, clique em **Grupos** ![Grupos](assets/groups-icon.png).

   Na lista exibida, você pode ver os grupos que gerencia, juntamente com quaisquer subgrupos que eles tenham. Os administradores do Adobe Workfront podem visualizar todos os grupos.

1. Clique no nome do grupo que contém o subgrupo que deseja editar.
1. No menu esquerdo, clique em **Subgrupos**.
1. Selecione o subgrupo que você deseja editar e clique no **ícone Editar** ![ícone Editar](assets/edit-icon.png).

   Para obter informações sobre as opções que podem ser usadas para configurar o subgrupo, consulte [Criar um subgrupo](/help/quicksilver/administration-and-setup/manage-groups/create-and-manage-subgroups/create-a-subgroup.md).

## Copiar um subgrupo

>[!NOTE]
>
>Somente um administrador do sistema pode copiar um subgrupo.

Quando você copia um subgrupo, ele se torna um grupo pai. Todos os membros e subgrupos do grupo são copiados com ele. Os membros do grupo mantêm todas as atribuições que tinham no grupo original.

Considere o seguinte ao copiar um subgrupo:

* Se um subgrupo copiado tiver seus próprios subgrupos, eles serão incluídos na cópia e seus nomes serão formatados da seguinte maneira:

  `Original subgroup name (Copy)`

* Qualquer subgrupo que pertença a um grupo público também é público, portanto, qualquer usuário com acesso para editar usuários, dentro ou fora do grupo, pode adicionar usuários ao subgrupo.

Para copiar um subgrupo:

{{step-1-to-setup}}

1. No painel esquerdo, clique em **Grupos** ![Grupos](assets/groups-icon.png).

   Na lista exibida, você pode ver os grupos que gerencia, juntamente com quaisquer subgrupos que eles tenham. Os administradores do Adobe Workfront podem visualizar todos os grupos.

1. Clique no nome do grupo que contém o subgrupo que você deseja copiar.
1. No menu esquerdo, clique em **Subgrupos**.
1. Selecione um subgrupo e clique no ícone **Copiar** ![Copiar ícone](assets/copy-icon.png) para criar um novo grupo de nível superior com base no grupo selecionado.
1. Defina as configurações do novo grupo.

   Para obter ajuda com essas configurações, consulte [Criar um grupo de nível superior copiando um grupo ou subgrupo existente](/help/quicksilver/administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md#create-a-top-level-group-by-copying-an-existing-group-or-subgroup) no artigo [Criar um grupo](/help/quicksilver/administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).

1. Clique em **Criar grupo**.

## Exportar um subgrupo

{{step-1-to-setup}}

1. No painel esquerdo, clique em **Grupos** ![Grupos](assets/groups-icon.png).

   Na lista exibida, você pode ver os grupos que gerencia, juntamente com quaisquer subgrupos que eles tenham. Os administradores do Adobe Workfront podem visualizar todos os grupos.

1. Clique no nome do grupo que contém o subgrupo que você deseja exportar.
1. No menu esquerdo, clique em **Subgrupos**.
1. Selecione o(s) subgrupo(s) que deseja exportar.
1. Clique no ícone **Exportar** ![Ícone Exportar](assets/export.png) e selecione o formato de arquivo desejado.

## Remover um subgrupo do grupo pai e torná-lo um grupo de nível superior

Você pode tornar um subgrupo um grupo de nível superior removendo-o do grupo pai.

>[!TIP]
>
>Quando você desativa um grupo que tem subgrupos abaixo dele, esses subgrupos também se tornam inativos. Se quiser que uma delas esteja ativa, use essas instruções para removê-la do grupo pai e, em seguida, reativá-la.
>>Para obter instruções sobre como desativar e reativar grupos, consulte [Desativar ou reativar um grupo](/help/quicksilver/administration-and-setup/manage-groups/create-and-manage-groups/deactivate-or-reactivate-a-group.md).

{{step-1-to-setup}}

1. No painel esquerdo, clique em **Grupos** ![Grupos](assets/groups-icon.png).
1. Selecione o grupo pai do subgrupo que você deseja tornar um grupo de nível superior e clique no ícone **Editar** ![Ícone Editar](assets/edit-icon.png).
1. Na caixa **Editar grupo** exibida, comece digitando o nome do subgrupo que você deseja tornar um grupo de nível superior no campo **Pesquisa** (em **Membros do grupo e Administradores do grupo**) e, em seguida, clique no X à direita do nome, quando ele aparecer.
1. Clique em **Salvar**.

## Excluir um subgrupo

>[!IMPORTANT]
>
>Ao excluir um grupo ou subgrupo, é necessário preservar os usuários, itens de trabalho e quaisquer subgrupos que estejam atribuídos a ele. Para ajudar você a garantir que eles sejam preservados, um prompt requer que você reatribua os objetos do grupo a um grupo diferente.

{{step-1-to-setup}}

1. No painel esquerdo, clique em **Grupos** ![Grupos](assets/groups-icon.png).

   Na lista exibida, você pode ver os grupos que gerencia, juntamente com quaisquer subgrupos que eles tenham. Os administradores do Adobe Workfront podem visualizar todos os grupos.

1. Clique no nome do grupo que contém o subgrupo que deseja deletar.
1. No menu esquerdo, clique em **Subgrupos**.
1. Selecione o subgrupo e clique no ícone **Excluir** ![Ícone Excluir](assets/delete.png).

   Na caixa **Excluir Grupo** exibida, comece a digitar e selecione o nome do grupo para o qual deseja mover os membros, itens de trabalho e subgrupos do grupo que está sendo excluído.

1. Clique em **Excluir**.

## Exibir e gerenciar os membros de um subgrupo do grupo

Ao visualizar a página principal de um grupo que você administra, é possível visualizar e gerenciar todos os usuários nos subgrupos do grupo. Para obter instruções, consulte [Exibir e gerenciar membros de subgrupo](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/view-and-manage-subgroup-members.md).

