---
user-type: administrator
product-area: system-administration;user-management
keywords: gerenciar,subgrupo,editar
navigation-topic: create-and-manage-subgroups
title: Gerenciar um subgrupo
description: Como administrador de grupo de um subgrupo, você pode criar, mover, exibir, editar, copiar, renomear, exportar e excluir o subgrupo. Também é possível fazer de um subgrupo um grupo de nível superior, removendo-o do grupo pai.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 5186d266-fa9f-445d-9dcc-bc07eb147b60
source-git-commit: 02191d80ea58f80de2e7be2ff55f43663e415e31
workflow-type: tm+mt
source-wordcount: '1269'
ht-degree: 1%

---

# Gerenciar um subgrupo

Como administrador de grupo de um subgrupo, você pode criar, mover, exibir, editar, copiar, renomear, exportar e excluir o subgrupo.

Também é possível fazer de um subgrupo um grupo de nível superior, removendo-o do grupo pai.

Se houver algum grupo acima do seu grupo, os administradores também poderão fazer essas tarefas para o seu grupo. O mesmo se aplica aos administradores do Workfront (para qualquer grupo).

Para obter mais informações sobre subgrupos, consulte [Visão geral de subgrupos](../../../administration-and-setup/manage-groups/groups-overview/subgroups.md).

## Requisitos de acesso

Você deve ter o seguinte para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plano Workfront*</td> 
   <td>Qualquer Um</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Plano </p> <p>Você deve ser um administrador de grupo do grupo ou um administrador do Workfront. Para obter mais informações, consulte <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Administradores do grupo</a> e <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder ao usuário acesso administrativo total</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Se precisar descobrir qual plano ou tipo de licença você tem, entre em contato com o administrador da Workfront.

## Criar, mover, exibir, editar, copiar, renomear, exportar ou excluir um subgrupo

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront, em seguida, clique em **Configuração** ![](assets/gear-icon-settings.png).

1. No painel esquerdo, clique em **Grupos** ![](assets/groups-icon.png).

   Na lista que é exibida, é possível ver os grupos gerenciados, juntamente com os subgrupos que eles possuem. Os administradores do Adobe Workfront podem visualizar todos os grupos.

1. Clique no nome do grupo que contém o subgrupo em que deseja trabalhar.

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
      <td> <p>É possível mover subgrupos existentes em outro grupo que você administra.</p> <p>Uma hierarquia de grupo não pode exceder 15 níveis, mas um único nível pode ter um número ilimitado de grupos paralelos.</p> 
       <ol> 
        <li value="1"> <p>(Opcional) Selecione um subgrupo para torná-lo o grupo de destino.</p> <p>Se você ignorar esta etapa, o grupo selecionado na etapa 3 será o grupo de destino.</p> </li> 
        <li value="2">Clique em <strong>Adicionar subgrupo</strong> &gt; <strong>Grupo existente</strong>.</li> 
        <li value="3"> <p>No <strong>Grupo existente</strong> for exibida, comece a digitar o nome de um subgrupo que deseja mover.</p> <p>Os resultados exibidos não contêm grupos acima do grupo de destino.</p> <p>Você pode selecionar o grupo certo ao passar o mouse sobre ele e clicar no ícone de informações <img src="assets/info-icon.png"> que é exibido ao lado dele. Isso exibe uma dica de ferramenta listando informações sobre o grupo, como a hierarquia de grupos acima dele e seus administradores.</p> </li> 
        <li value="4"> <p>Clique no nome do subgrupo que deseja mover quando for exibido na lista.</p> </li> 
        <li value="5"> <p>Repita as Etapas c-d para qualquer outro subgrupo que desejar mover para o grupo de destino</p> </li> 
        <li value="6">Clique em <strong>Salvar</strong>.</li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Editar um subgrupo</td> 
      <td> <p>Selecione o subgrupo que deseja editar e clique no ícone Editar <img src="assets/edit-icon.png">.</p> <p>Para obter informações sobre as opções que podem ser usadas para configurar o subgrupo, consulte a tabela em <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md" class="MCXref xref">Criar um grupo</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Exportar um ou mais subgrupos</td> 
      <td> 
       <ol> 
        <li value="1">Selecione o subgrupo ou subgrupos que deseja exportar.</li> 
        <li value="2">Clique no ícone Exportar <img src="assets/export.png">e selecione o formato de arquivo desejado.</li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Copiar um subgrupo para criar um novo grupo de nível superior</td> 
      <td> <p>(Disponível somente para administradores do Workfront.) Ao copiar um subgrupo, ele se torna um grupo pai. Todos os membros do grupo e subgrupos são copiados com ele. Os membros dos grupos mantêm quaisquer atribuições que tinham no grupo original.</p> <p>Para obter mais informações sobre cópia de um subgrupo, consulte <a href="#about-copying-a-subgroup" class="MCXref xref">Sobre cópia de um subgrupo</a> neste artigo.</p> 
       <ol> 
        <li value="1">Selecione um subgrupo e clique no ícone Copiar <img src="assets/copy-icon.png"> para criar um novo grupo de nível superior com base no grupo selecionado.</li> 
        <li value="2"> <p>Defina as configurações do novo grupo.</p> <p>Para obter ajuda com essas configurações, consulte a tabela na seção . <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md#copying-an-existing-group-and-sub-group" class="MCXref xref">Criar um grupo de nível superior copiando um grupo ou subgrupo existente</a> no artigo <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md#copying-an-existing-group-and-sub-group" class="MCXref xref">Criar um grupo de nível superior copiando um grupo ou subgrupo existente</a>.</p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Excluir um subgrupo</td> 
      <td> <p><b>IMPORTANTE</b>: Ao excluir um grupo ou subgrupo, é necessário preservar os usuários, itens de trabalho e quaisquer subgrupos atribuídos a ele no momento. Para ajudar você a garantir que sejam preservados, um prompt exige que você reatribua os objetos do grupo a um grupo diferente na etapa abaixo.</p> 
       <ol> 
        <li value="1">Selecione o subgrupo e clique no ícone Excluir <img src="assets/delete.png">.</li> 
        <li value="2">No <strong>Excluir grupo</strong> será exibida, começando a digitar e depois selecione o nome do grupo no qual deseja mover os membros, itens de trabalho e subgrupos do grupo que você está excluindo.</li> 
        <li value="3">Clique em <strong>Excluí-los</strong>.</li> 
       </ol> </td> 
     </tr> 
    </tbody> 
   </table>

>[!TIP]
>
>Ao gerenciar um grupo que contém subgrupos, é útil identificar e filtrar dados sobre todo o grupo e todos os seus subgrupos. Você pode fazer isso usando o campo ID principal superior em um relatório ou lista.
>
>Por exemplo, imagine que você gerencia um departamento de Marketing grande e deseja uma lista de todos os projetos em que o departamento inteiro está trabalhando.
>
>No Workfront, esse departamento de marketing é representado por um grupo chamado Marketing, com 3 subgrupos chamados Marketing de campo, Marketing de produto e Marketing digital. Para listar os projetos que pertencem a todo o departamento de Marketing (todos os 4 grupos), você pode criar um Filtro para a área Projetos com a seguinte Regra de filtro:
>
>
```
>Group: Top Parent ID > Equal > Marketing
>```
>
>Você também pode usar o campo Nome principal principal superior para identificar os dados associados a um grupo de nível superior, mas somente em Exibições, não em Filtros ou Agrupamentos.

## Remova um subgrupo de seu grupo pai e torne-o um grupo de nível superior

Você pode transformar um subgrupo em um grupo de nível superior, removendo-o de seu grupo pai.

>[!TIP]
>
>Quando você desativa um grupo que tem subgrupos abaixo dele, esses subgrupos também ficam inativos. Se quiser que uma delas esteja ativa, você pode usar essas instruções para removê-la de seu grupo pai e reativá-la.
>
>Para obter instruções sobre como desativar e reativar grupos, consulte as seções [Exibir e gerenciar os detalhes de um grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-manage-a-groups-details.md#view) e [Exibir e gerenciar os detalhes de um grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-manage-a-groups-details.md#inactive) no artigo [Exibir e gerenciar os detalhes de um grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-manage-a-groups-details.md).

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront, em seguida, clique em **Configuração** ![](assets/gear-icon-settings.png).

1. No painel esquerdo, clique em **Grupos** ![](assets/groups-icon.png).

1. Selecione o grupo pai do grupo que deseja criar um grupo de nível superior e clique no ícone Editar ![](assets/edit-icon.png).
1. No **Editar grupo** que aparece, em **Membros do grupo e administradores de grupo**, comece digitando o nome do subgrupo que deseja criar um grupo de nível superior e clique no X à direita do nome quando aparecer.
1. Clique em **Salvar**.

## Exibir e gerenciar membros de subgrupo de um grupo

Ao visualizar a página principal de um grupo administrado, é possível visualizar e gerenciar todos os usuários dos subgrupos do grupo. Para obter instruções, consulte [Exibir e gerenciar membros do subgrupo](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/view-and-manage-subgroup-members.md).

## Sobre cópia de um subgrupo {#about-copying-a-subgroup}

Considere o seguinte ao copiar um subgrupo.

* Se um subgrupo copiado tiver seus próprios subgrupos, eles serão incluídos na cópia e seus nomes serão formatados da seguinte maneira:

   ```
   Original subgroup name (Copy)
   ```

* Qualquer subgrupo que pertença a um grupo público também é público, portanto, qualquer usuário com acesso de usuário de edição, dentro ou fora do grupo, pode adicionar usuários ao subgrupo.
