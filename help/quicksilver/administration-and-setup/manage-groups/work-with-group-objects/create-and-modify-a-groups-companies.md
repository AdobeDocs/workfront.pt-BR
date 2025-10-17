---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: work-with-a-groups-objects
title: Criar e Modificar Empresas de um Grupo
description: Ao visualizar um grupo gerenciado na área Grupos, você pode visualizar e trabalhar com empresas associadas ao grupo e a qualquer um de seus subgrupos.
author: Becky
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 407f6631-ecc1-4ed8-bfec-6d726ae87a3d
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '727'
ht-degree: 0%

---

# Criar e modificar as empresas de um grupo

Ao visualizar um grupo gerenciado na área Grupos, você pode visualizar e trabalhar com empresas associadas ao grupo e a qualquer um de seus subgrupos.

Se houver algum grupo acima do seu, os administradores também poderão fazer essas coisas pelo seu grupo. O mesmo se aplica aos administradores do Workfront (para qualquer grupo).

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

## Exiba, trabalhe com e crie empresas para seu grupo na área Grupos

{{step-1-to-setup}}

1. No painel esquerdo, clique em **Grupos** ![Grupos](assets/groups-icon.png).

1. Clique no nome do grupo para o qual deseja criar ou modificar empresas.
1. No painel esquerdo, clique em **Empresas** para listar as empresas associadas ao grupo e seus subgrupos.
1. (Opcional) Para adicionar uma empresa, clique em **Adicionar Empresa** e configure a empresa usando as opções listadas abaixo. Quando terminar, clique em **Criar Empresa**.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Seção Informações básicas</td> 
      <td> 
       <ul> 
        <li> <p><b>Nome da Empresa</b>: digite um nome para a empresa.</p> </li> 
        <li> <p><b>Está ativo</b>: quando esta opção é habilitada, os usuários podem encontrar a empresa e anexá-la aos projetos que eles criam e editam. Uma empresa inativa não pode ser anexada a projetos. Essa opção está ativada por padrão.</p> </li> 
        <li> <p><b>Esta é a Empresa Primária</b>: atribui a empresa como a empresa primária da sua organização. A empresa principal geralmente representa a conta da Workfront na qual a maioria dos usuários trabalha.</p> <p>Ao modificar seus níveis de acesso, você pode restringir os usuários a ver outros usuários:</p> 
         <ul> 
          <li>Somente na empresa primária</li> 
          <li> <p>Na empresa associada e na empresa primária</p> <p>Para obter informações sobre a funcionalidade da empresa primária nos níveis de acesso dos usuários, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">Criar ou modificar níveis de acesso personalizados</a>.</p> <p>Você pode ter somente uma ou nenhuma empresa designada como empresa primária, mas não pode ter várias empresas designadas como empresas primárias. Para obter mais informações, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">Criar ou modificar níveis de acesso personalizados</a>.</p> </li> 
         </ul> </li> 
        <li> <p><b>Grupo</b>: se houver um grupo que faz negócios com a empresa, você pode adicionar o nome do grupo aqui. Isso é útil para administradores de grupos que precisam relatar e gerenciar todas as empresas com as quais seus grupos fazem negócios.</p> <p data-mc-conditions="SnippetConditions-wf-groups.groups">O sistema preenche o campo <strong>Grupo</strong> da nova empresa com o grupo que você está visualizando.</p> <p data-mc-conditions="SnippetConditions-wf-groups.groups">Se você tiver acesso administrativo a empresas no seu nível de acesso, poderá remover o grupo da empresa e atribuir outro, ou deixar a empresa sem um grupo.</p> <p data-mc-conditions="SnippetConditions-wf-groups.groups">Se você não tiver acesso administrativo a empresas, o campo <strong>Grupo</strong> será obrigatório e você poderá selecionar apenas os grupos que gerenciar ou quaisquer subgrupos nesses grupos.</p> <p data-mc-conditions="SnippetConditions-wf-groups.groups">Para obter informações sobre acesso administrativo a empresas, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref" data-mc-variable-override="">Conceder aos usuários acesso administrativo a determinadas áreas</a>.</p> </li> 
        <li> <p><b>Membros da Empresa</b>: adicionar usuários existentes à empresa. Ao fazer isso, você está associando esses usuários a esta empresa.</p> <p>Não há limite para quantos usuários você associa a uma empresa, mas um usuário não pode estar associado a mais de uma empresa.</p> </li> 
       </ul> </td> 
     </tr>
     <tr> 
      <td role="rowheader">Seção Forms personalizada</td> 
      <td> <p>Se houver campos que você deseja adicionar à sua empresa que não estejam disponíveis no Workfront, é possível criar um formulário personalizado e associá-lo à sua empresa. Você pode anexar esse formulário à sua empresa selecionando-o no menu suspenso. Somente as empresas ativas são listadas no menu suspenso. Para obter informações sobre como criar formulários personalizados, consulte <a href="/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md">Criar um formulário personalizado</a>. </p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >Se você tiver acesso administrativo a empresas em seu nível de acesso, também poderá clicar em Adicionar mais empresas na parte inferior da lista. Isso adiciona uma linha onde é possível configurar rapidamente a nova empresa.

1. (Opcional) Para editar ou excluir empresas, selecione pelo menos uma empresa e use os botões da barra de ferramentas para editar o ![ícone Editar](assets/edit-icon.png) ou excluir o ![ícone Excluir](assets/delete.png).

   Para obter informações sobre como editar uma empresa, consulte a seção [Criar ou editar uma empresa no Workfront](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md#adding-a-company-to-workfront) no artigo [Criar e editar empresas](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

1. (Opcional) Para exportar a lista de empresas, clique no ícone Exportar ![ícone Exportar](assets/export.png) e selecione o formato de arquivo desejado para a lista exportada.
