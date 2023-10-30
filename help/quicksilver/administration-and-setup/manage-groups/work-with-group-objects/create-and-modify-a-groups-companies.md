---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: work-with-a-groups-objects
title: Criar e modificar as empresas de um grupo
description: Ao visualizar um grupo gerenciado na área Grupos, você pode visualizar e trabalhar com empresas associadas ao grupo e a qualquer um de seus subgrupos.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 407f6631-ecc1-4ed8-bfec-6d726ae87a3d
source-git-commit: ab7877c048ea87180dd518c978b258d266e0f95c
workflow-type: tm+mt
source-wordcount: '755'
ht-degree: 0%

---

# Criar e modificar as empresas de um grupo

Ao visualizar um grupo gerenciado na área Grupos, você pode visualizar e trabalhar com empresas associadas ao grupo e a qualquer um de seus subgrupos.

Se houver algum grupo acima do seu, os administradores também poderão fazer essas coisas pelo seu grupo. O mesmo se aplica aos administradores do Workfront (para qualquer grupo).

## Requisitos de acesso

Você deve ter o seguinte para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Workfront*</td> 
   <td>Qualquer Um</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Plano </p> <p>Você deve ser um administrador de grupo do grupo ou um administrador do Workfront. Para obter mais informações, consulte <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref" data-mc-variable-override="">Administradores de grupo</a> e <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref" data-mc-variable-override="">Conceder acesso administrativo total a um usuário</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Se precisar descobrir o tipo de plano ou licença que possui, entre em contato com o administrador do Workfront.

## Exiba, trabalhe com e crie empresas para seu grupo na área Grupos

1. Clique em **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront e clique em **Configuração** ![](assets/gear-icon-settings.png).

1. No painel esquerdo, clique em **Grupos** ![](assets/groups-icon.png).

1. Clique no nome do grupo para o qual deseja criar ou modificar empresas.
1. No painel esquerdo, clique em **Empresas** para listar as empresas associadas ao grupo e quaisquer subgrupos que ele possa ter.
1. (Opcional) Para adicionar uma empresa, clique em **Adicionar Empresa**, em seguida, configure a empresa usando as opções listadas abaixo. Quando terminar, clique em **Criar empresa**.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Seção Informações básicas</td> 
      <td> 
       <ul> 
        <li> <p><b>Nome da empresa</b>: digite um nome para a empresa.</p> </li> 
        <li> <p><b>Está ativo</b>: quando essa opção é ativada, os usuários podem encontrar a empresa e anexá-la aos projetos que criam e editam. Uma empresa inativa não pode ser anexada a projetos. Essa opção está ativada por padrão.</p> </li> 
        <li> <p><b>Esta é a Empresa Primária</b>: atribui a empresa como a empresa principal da organização. A empresa principal geralmente representa a conta da Workfront na qual a maioria dos usuários trabalha.</p> <p>Ao modificar seus níveis de acesso, você pode restringir os usuários a ver outros usuários:</p> 
         <ul> 
          <li>Somente na empresa primária</li> 
          <li> <p>Na empresa associada e na empresa primária</p> <p>Para obter informações sobre a funcionalidade principal da empresa nos níveis de acesso dos usuários, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">Criar ou modificar níveis de acesso personalizados</a>.</p> <p>Você pode ter somente uma ou nenhuma empresa designada como empresa primária, mas não pode ter várias empresas designadas como empresas primárias. Para obter mais informações, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">Criar ou modificar níveis de acesso personalizados</a>.</p> </li> 
         </ul> </li> 
        <li> <p><b>Grupo</b>: se houver um grupo que faz negócios com a empresa, você pode adicionar o nome do grupo aqui. Isso é útil para administradores de grupos que precisam relatar e gerenciar todas as empresas com as quais seus grupos fazem negócios.</p> <p data-mc-conditions="SnippetConditions-wf-groups.groups">O sistema preenche o <strong>Grupo</strong> para a nova empresa com o grupo que você está visualizando.</p> <p data-mc-conditions="SnippetConditions-wf-groups.groups">Se você tiver acesso administrativo a empresas no seu nível de acesso, poderá remover o grupo da empresa e atribuir outro, ou deixar a empresa sem um grupo.</p> <p data-mc-conditions="SnippetConditions-wf-groups.groups">Se você não tiver acesso administrativo a empresas, a variável <strong>Grupo</strong> é obrigatório e você pode selecionar apenas os grupos que gerencia ou quaisquer subgrupos sob esses grupos.</p> <p data-mc-conditions="SnippetConditions-wf-groups.groups">Para obter informações sobre acesso administrativo a empresas, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref" data-mc-variable-override="">Conceder aos usuários acesso administrativo a determinadas áreas</a>.</p> </li> 
        <li> <p><b>Membros da empresa</b>: adicione usuários existentes à empresa. Ao fazer isso, você está associando esses usuários a esta empresa.</p> <p>Não há limite para quantos usuários você associa a uma empresa, mas um usuário não pode estar associado a mais de uma empresa.</p> </li> 
       </ul> </td> 
     </tr>
     <tr> 
      <td role="rowheader">Seção Forms personalizada</td> 
      <td> <p>Se houver campos que você deseja adicionar à sua empresa que não estejam disponíveis no Workfront, é possível criar um Formulário personalizado e associá-lo à sua empresa. Você pode anexar esse formulário à sua empresa selecionando-o no menu suspenso. Somente as empresas ativas são listadas no menu suspenso. Para obter informações sobre como criar um Forms personalizado, consulte <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref" data-mc-variable-override="">Criar ou editar um formulário personalizado</a>. </p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >Se você tiver acesso administrativo a empresas em seu nível de acesso, também poderá clicar em Adicionar mais empresas na parte inferior da lista. Isso adiciona uma linha onde é possível configurar rapidamente a nova empresa.

1. (Opcional) Para editar ou excluir empresas, selecione pelo menos uma empresa e use os botões da barra de ferramentas para editar ![](assets/edit-icon.png) ou excluir ![](assets/delete.png) o mesmo.

   Para obter informações sobre como editar uma empresa, consulte a seção [Criar ou editar uma empresa no Workfront](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md#adding-a-company-to-workfront) no artigo [Criar e editar empresas](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

1. (Opcional) Para exportar a lista de empresas, clique no ícone Exportar ![](assets/export.png), em seguida, selecione o formato de arquivo desejado para a lista exportada.
