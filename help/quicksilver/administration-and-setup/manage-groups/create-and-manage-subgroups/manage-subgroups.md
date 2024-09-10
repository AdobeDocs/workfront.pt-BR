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
source-git-commit: dc64fef83c2b1e9f8bf9438017155bd47b83ab23
workflow-type: tm+mt
source-wordcount: '1247'
ht-degree: 1%

---

# Gerenciar um subgrupo

Como administrador de grupo de um subgrupo, você pode criar, mover, exibir, editar, copiar, renomear, exportar e excluir o subgrupo.

Você também pode tornar um subgrupo um grupo de nível superior removendo-o do grupo pai.

Se houver algum grupo acima do seu, os administradores também poderão fazer essas coisas pelo seu grupo. O mesmo se aplica aos administradores do Workfront (para qualquer grupo).

Para obter mais informações sobre subgrupos, consulte [Visão geral dos subgrupos](../../../administration-and-setup/manage-groups/groups-overview/subgroups.md).

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront</td> 
   <td>Qualquer</td> 
  </tr> 
  <tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td><p>Novo: Padrão</p>
       <p>Ou</p>
       <p>Atual: Plano</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td>Você deve ser um administrador de grupo do grupo ou um administrador do sistema.</td>
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Criar, mover, exibir, editar, copiar, renomear, exportar ou excluir um subgrupo

{{step-1-to-setup}}

1. No painel esquerdo, clique em **Grupos** ![](assets/groups-icon.png).

   Na lista exibida, você pode ver os grupos que gerencia, juntamente com quaisquer subgrupos que eles tenham. Os administradores do Adobe Workfront podem visualizar todos os grupos.

1. Clique no nome do grupo que contém o subgrupo no qual você deseja trabalhar.

   Ou

   Se estiver movendo um ou mais subgrupos, clique no nome do grupo de destino (você especificará quais subgrupos deseja mover em uma etapa posterior).

1. No menu esquerdo, clique em **Subgrupos**.

1. Siga um destes procedimentos:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Criar um novo subgrupo</td> 
      <td> <p>Para criar o novo subgrupo um nível abaixo do grupo que você está visualizando, clique em <strong>Adicionar subgrupo</strong>.</p> <p>Ou, se quiser criar o novo subgrupo abaixo de outro subgrupo na lista, selecione esse subgrupo e clique em <strong>Adicionar s</strong><strong>subgrupo</strong>.</p> <p>Para obter informações sobre as opções que podem ser usadas para configurar o subgrupo, consulte a tabela em <a href="../../../administration-and-setup/manage-groups/create-and-manage-subgroups/create-a-subgroup.md" class="MCXref xref">Criar um subgrupo</a>.</p> <p>Uma hierarquia de grupo não pode exceder 15 níveis, mas um único nível pode ter um número ilimitado de grupos paralelos.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Mover um subgrupo </td> 
      <td> <p>Você pode mover subgrupos existentes para outro grupo que administra.</p> <p>Uma hierarquia de grupo não pode exceder 15 níveis, mas um único nível pode ter um número ilimitado de grupos paralelos.</p> 
       <ol> 
        <li value="1"> <p>(Opcional) Selecione um subgrupo para torná-lo o grupo de destino.</p> <p>Se você ignorar esta etapa, o grupo selecionado na etapa 3 será o grupo de destino.</p> </li> 
        <li value="2">Clique em <strong>Adicionar Subgrupo</strong> &gt; <strong>Grupo Existente</strong>.</li> 
        <li value="3"> <p>Na caixa <strong>Grupo Existente</strong> que aparece, comece digitando o nome de um subgrupo que você deseja mover.</p> <p>Os resultados exibidos não contêm grupos acima do grupo de destino.</p> <p>Você pode verificar se está selecionando o grupo correto passando o cursor do mouse sobre ele e clicando no ícone de informações <img src="assets/info-icon.png"> que é exibido ao lado dele. Uma dica de ferramenta que lista informações sobre o grupo, como a hierarquia de grupos acima dele e seus administradores.</p> </li> 
        <li value="4"> <p>Clique no nome do subgrupo que deseja mover ao vê-lo exibido na lista.</p> </li> 
        <li value="5"> <p>Repita as etapas c-d para quaisquer outros subgrupos que você deseja mover para o grupo de destino</p> </li> 
        <li value="6">Clique em <strong>Salvar</strong>.</li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Editar um subgrupo</td> 
      <td> <p>Selecione o subgrupo que você deseja editar e clique no ícone Editar <img src="assets/edit-icon.png">.</p> <p>Para obter informações sobre as opções que podem ser usadas para configurar o subgrupo, consulte a tabela em <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md" class="MCXref xref">Criar um grupo</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Exportar um ou mais subgrupos</td> 
      <td> 
       <ol> 
        <li value="1">Selecione o(s) subgrupo(s) que deseja exportar.</li> 
        <li value="2">Clique no ícone Exportar <img src="assets/export.png"> e selecione o formato de arquivo desejado.</li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Copiar um subgrupo para criar um novo grupo de nível superior</td> 
      <td> <p>(Disponível somente para administradores do Workfront.) Quando você copia um subgrupo, ele se torna um grupo pai. Todos os membros e subgrupos do grupo são copiados com ele. Os membros dos grupos mantêm todas as atribuições que tinham no grupo original.</p> <p>Para obter mais informações sobre copiar um subgrupo, consulte <a href="#about-copying-a-subgroup" class="MCXref xref">Sobre copiar um subgrupo</a> neste artigo.</p> 
       <ol> 
        <li value="1">Selecione um subgrupo e clique no ícone Copiar <img src="assets/copy-icon.png"> para criar um novo grupo de nível superior com base no grupo selecionado.</li> 
        <li value="2"> <p>Defina as configurações do novo grupo.</p> <p>Para obter ajuda com essas configurações, consulte a tabela na seção <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md#copying-an-existing-group-and-sub-group" class="MCXref xref">Criar um grupo de nível superior copiando um grupo ou subgrupo existente</a> no artigo <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md#copying-an-existing-group-and-sub-group" class="MCXref xref">Criar um grupo de nível superior copiando um grupo ou subgrupo existente</a>.</p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Excluir um subgrupo</td> 
      <td> <p><b>IMPORTANTE</b>: ao excluir um grupo ou subgrupo, é necessário preservar os usuários, itens de trabalho e quaisquer subgrupos que estejam atribuídos a ele no momento. Para ajudá-lo a garantir que eles sejam preservados, um prompt requer que você reatribua os objetos do grupo a um grupo diferente na etapa abaixo.</p> 
       <ol> 
        <li value="1">Selecione o subgrupo e clique no ícone Excluir <img src="assets/delete.png">.</li> 
        <li value="2">Na caixa <strong>Excluir Grupo</strong> exibida, comece a digitar e selecione o nome do grupo para o qual deseja mover os membros, itens de trabalho e subgrupos do grupo que está sendo excluído.</li> 
        <li value="3">Clique em <strong>Excluí-los</strong>.</li> 
       </ol> </td> 
     </tr> 
    </tbody> 
   </table>

>[!TIP]
>
>Ao gerenciar um grupo que contém subgrupos, é útil poder identificar e filtrar dados sobre o grupo inteiro e todos os seus subgrupos. Você pode fazer isso usando o campo ID principal em um relatório ou lista.
>
>Por exemplo, imagine que você gerencia um grande departamento de marketing e deseja uma lista de todos os projetos nos quais todo o departamento está trabalhando.
>
>No Workfront, esse departamento de marketing é representado por um grupo chamado Marketing, com três subgrupos chamados Marketing de campo, Marketing de produto e Marketing digital. Para listar os projetos que pertencem a todo o departamento de marketing (todos os 4 grupos), você pode criar um Filtro para a área Projetos com a seguinte Regra de filtro:
>
>`Group: Top Parent ID > Equal > Marketing`
>
>Você também pode usar o campo Nome do pai superior para identificar dados associados a um grupo de nível superior, mas somente em Exibições, não em Filtros ou Agrupamentos.

## Remover um subgrupo do grupo pai e torná-lo um grupo de nível superior

Você pode tornar um subgrupo um grupo de nível superior removendo-o do grupo pai.

>[!TIP]
>
>Quando você desativa um grupo que tem subgrupos abaixo dele, esses subgrupos também se tornam inativos. Se quiser que uma delas esteja ativa, use essas instruções para removê-la do grupo pai e, em seguida, reativá-la.
>
>Para obter instruções sobre como desativar e reativar grupos, consulte as seções [Exibir e gerenciar os detalhes de um grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-manage-a-groups-details.md#view) e [Exibir e gerenciar os detalhes de um grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-manage-a-groups-details.md#inactive) no artigo [Exibir e gerenciar os detalhes de um grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-manage-a-groups-details.md).

{{step-1-to-setup}}

1. No painel esquerdo, clique em **Grupos** ![](assets/groups-icon.png).

1. Selecione o grupo pai do grupo que você deseja tornar um grupo de nível superior e clique no ícone Editar ![](assets/edit-icon.png).
1. Na caixa **Editar Grupo** que aparece, em **Membros do Grupo e Administradores do Grupo**, comece digitando o nome do subgrupo que você deseja tornar um grupo de nível superior e, em seguida, clique no X à direita do seu nome quando ele aparecer.
1. Clique em **Salvar**.

## Exibir e gerenciar os membros de um subgrupo do grupo

Ao visualizar a página principal de um grupo que você administra, é possível visualizar e gerenciar todos os usuários nos subgrupos do grupo. Para obter instruções, consulte [Exibir e gerenciar membros de subgrupo](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/view-and-manage-subgroup-members.md).

## Sobre copiar um subgrupo {#about-copying-a-subgroup}

Considere o seguinte ao copiar um subgrupo.

* Se um subgrupo copiado tiver seus próprios subgrupos, eles serão incluídos na cópia e seus nomes serão formatados da seguinte maneira:

  `Original subgroup name (Copy)`

* Qualquer subgrupo que pertença a um grupo público também é público, portanto, qualquer usuário com acesso de edição de usuário, dentro ou fora do grupo, pode adicionar usuários ao subgrupo.
