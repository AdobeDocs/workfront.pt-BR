---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: work-with-a-groups-objects
title: Criar e modificar empresas de um grupo
description: Ao visualizar um grupo que você gerencia na área Grupos , é possível visualizar e trabalhar com empresas associadas ao grupo e a qualquer um de seus subgrupos.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 407f6631-ecc1-4ed8-bfec-6d726ae87a3d
source-git-commit: e20934501c2117455ca7950834d868f78576dee7
workflow-type: tm+mt
source-wordcount: '811'
ht-degree: 0%

---

# Criar e modificar empresas de um grupo

Ao visualizar um grupo que você gerencia na área Grupos , é possível visualizar e trabalhar com empresas associadas ao grupo e a qualquer um de seus subgrupos.

Se houver algum grupo acima do seu grupo, os administradores também poderão fazer essas tarefas para o seu grupo. O mesmo se aplica aos administradores do Workfront (para qualquer grupo).

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
   <td> <p>Plano </p> <p>Você deve ser um administrador de grupo do grupo ou um administrador do Workfront. Para obter mais informações, consulte <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref" data-mc-variable-override="">Administradores do grupo</a> e <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref" data-mc-variable-override="">Conceder ao usuário acesso administrativo total</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Se precisar descobrir qual plano ou tipo de licença você tem, entre em contato com o administrador da Workfront.

## Exibir, trabalhar e criar empresas para seu grupo na área Grupos

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront, em seguida, clique em **Configuração** ![](assets/gear-icon-settings.png).

1. No painel esquerdo, clique em **Grupos** ![](assets/groups-icon.png).

1. Clique no nome do grupo para o qual você deseja criar ou modificar empresas.
1. No painel esquerdo, clique em **Empresas** para listar as empresas associadas ao grupo e quaisquer subgrupos que ele possa ter.
1. (Opcional) Para adicionar uma empresa, clique em **Adicionar empresa**, configure a empresa usando as opções listadas abaixo. Quando terminar, clique em **Criar empresa**.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Seção Informações básicas</td> 
      <td> 
       <ul> 
        <li> <p><b>Nome da empresa</b>: Digite um nome para a empresa.</p> </li> 
        <li> <p><b>Está ativo</b>: Quando essa opção está ativada, os usuários podem encontrar a empresa e anexá-la a projetos que eles criam e editam. Uma empresa inativa não pode ser anexada a projetos. Essa opção é ativada por padrão.</p> </li> 
        <li> <p><b>Esta é a principal empresa</b>: Atribui a empresa como a empresa principal de sua organização. A empresa principal geralmente representa sua conta do Workfront onde a maioria dos usuários trabalha.</p> <p>Ao modificar os níveis de acesso, é possível restringir os usuários a ver outros usuários:</p> 
         <ul> 
          <li>Apenas na empresa principal</li> 
          <li> <p>Na empresa associada e na empresa primária</p> <p>Para obter informações sobre a funcionalidade principal da empresa nos níveis de acesso dos usuários, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">Criar ou modificar níveis de acesso personalizados</a>.</p> <p>Você pode ter apenas uma ou nenhuma empresa designada como empresa primária, mas não pode ter várias empresas designadas como empresas primárias. Para obter mais informações, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">Criar ou modificar níveis de acesso personalizados</a>.</p> </li> 
         </ul> </li> 
        <li> <p><b>Grupo</b>: Se houver um grupo que faça negócios com a empresa, você poderá adicionar o nome do grupo aqui. Isso é útil para administradores de grupo que precisam criar relatórios e gerenciar todas as empresas com as quais seus grupos fazem negócios.</p> <p data-mc-conditions="SnippetConditions-wf-groups.groups">O sistema preenche a <strong>Grupo</strong> para a nova empresa com o grupo que você está visualizando.</p> <p data-mc-conditions="SnippetConditions-wf-groups.groups">Se você tiver acesso administrativo a empresas em seu nível de acesso, poderá remover o grupo da empresa e atribuir um outro grupo, ou deixar a empresa sem um grupo.</p> <p data-mc-conditions="SnippetConditions-wf-groups.groups">Se você não tiver acesso administrativo às empresas, a variável <strong>Grupo</strong> é obrigatório e é possível selecionar apenas os grupos gerenciados ou qualquer subgrupo nesses grupos.</p> <p data-mc-conditions="SnippetConditions-wf-groups.groups">Para obter informações sobre o acesso administrativo às empresas, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref" data-mc-variable-override="">Conceder aos usuários acesso administrativo a determinadas áreas</a>.</p> </li> 
        <li> <p><b>Membros da Empresa</b>: Adicionar usuários existentes à empresa. Ao fazer isso, você está associando esses usuários a essa empresa.</p> <p>Não há limite para quantos usuários você associa a uma empresa, mas um usuário não pode ser associado a mais de uma empresa.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Seção Taxas de Faturamento</td> 
      <td> <p>Você pode sobrepor as taxas de faturamento associadas às suas funções de cargo no nível da empresa. Para obter informações sobre como criar funções de cargo e associá-las a taxas de faturamento, consulte <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref" data-mc-variable-override="">Criar e gerenciar funções de trabalho</a>.</p> <p>Para obter mais informações sobre a sobreposição de taxas de faturamento no nível da empresa, consulte <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/override-job-role-billing-rates-company-level.md" class="MCXref xref" data-mc-variable-override="">Substituir as taxas de faturamento da função de trabalho no nível da empresa</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Seção Forms personalizada</td> 
      <td> <p>Se houver campos que você deseja adicionar à sua empresa que não estão disponíveis no Workfront, crie um Formulário personalizado e associe-o à sua empresa. Você pode anexar esse formulário à sua empresa selecionando-o no menu suspenso. Somente empresas ativas são listadas no menu suspenso. Para obter informações sobre como criar o Forms personalizado, consulte <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref" data-mc-variable-override="">Criar ou editar um formulário personalizado</a>. </p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >Se você tiver acesso administrativo a empresas em seu nível de acesso, também poderá clicar em Adicionar mais empresas na parte inferior da lista. Isso adiciona uma linha onde você pode configurar rapidamente a nova empresa.

1. (Opcional) Para editar ou excluir empresas, selecione pelo menos uma empresa e use os botões da barra de ferramentas para editar ![](assets/edit-icon.png) ou excluir ![](assets/delete.png) sim.

   Para obter informações sobre como editar uma empresa, consulte a seção [Criar ou editar uma empresa no Workfront](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md#adding-a-company-to-workfront) no artigo [Criar e editar empresas](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

1. (Opcional) Para exportar a lista de empresas, clique no ícone Exportar ![](assets/export.png), em seguida, selecione o formato de arquivo que deseja para a lista exportada.
