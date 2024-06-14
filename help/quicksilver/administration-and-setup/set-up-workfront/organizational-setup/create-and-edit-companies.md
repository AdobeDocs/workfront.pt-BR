---
user-type: administrator
product-area: system-administration
navigation-topic: organization-setup
title: Criar e editar empresas
description: É possível adicionar empresas a [!DNL Adobe Workfront] e usá-los para fins de planejamento financeiro, relatórios, para definir permissões sobre objetos e para manter as informações confidenciais.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: bb597032-3395-4c9a-b622-5c920ba55131
source-git-commit: 84c5772d130be78d9f9b9aef342c57183d5ec985
workflow-type: tm+mt
source-wordcount: '1472'
ht-degree: 0%

---

# Criar e editar empresas

<!--Audited: 01/2024-->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

Uma empresa é uma unidade organizacional no [!DNL Adobe Workfront] que podem representar sua organização, um departamento dentro da organização ou um cliente com o qual você trabalha. É possível adicionar empresas a [!DNL Workfront] e usá-los para fins de planejamento financeiro, relatórios, para definir permissões sobre objetos e para manter as informações confidenciais.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte para gerenciar empresas no [!DNL Workfront]:

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Workfront] plano</p> </td> 
   <td>Qualquer</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Adobe Workfront] licença*</p> </td> 
   <td><p>Atual: [!UICONTROL Plano]</p>
   Ou
   <p>Novo: [!UICONTROL Padrão]</p>
   </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configuração do nível de acesso</td> 
   <td> <p>Uma das seguintes opções:</p> 
    <ul> 
     <li> <p>O nível de acesso do [!UICONTROL System Administrator], que permite editar qualquer empresa no sistema. Para obter mais informações, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md">Conceder acesso administrativo total a um usuário</a>. </p> </li> 
     <li> <p>Acesso administrativo para gerenciar empresas, que permite editar qualquer empresa no sistema. Para obter mais informações, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md">Conceder aos usuários acesso administrativo a determinadas áreas</a>.</p> </li> 
    </ul> <p><b>NOTA</b>:  
     <ul> 
      <li> <p>Você também pode gerenciar empresas associadas a qualquer grupo ao qual esteja atribuído como administrador de grupo.</p> </li> 
      <li> <p>Para adicionar e remover usuários do [!DNL Workfront] sistema, você deve ter um dos seguintes:</p> 
       <ul> 
        <li> <p>O nível de acesso do [!UICONTROL System Administrator]. Para obter mais informações, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder acesso administrativo total a um usuário</a>. </p> </li> 
        <li> <p>Em seu nível de acesso, [!UICONTROL Editar] deve ser selecionado para a configuração [!UICONTROL Usuários]. Além disso, para a configuração [!UICONTROL Usuários], em [!UICONTROL Ajuste as configurações] <img src="assets/gear-icon-in-access-levels.png">, a opção [!UICONTROL Criar] e pelo menos uma das duas opções [!UICONTROL Administrador de Usuário] devem ser habilitadas. </p> <p> <img src="assets/access-req-users.png"> </p> <p>Se você estiver usando a opção [!UICONTROL Administrador de Usuários (Usuários de Grupo)], deverá ser um administrador de grupo de um grupo do qual o usuário seja membro.</p> </li> 
       </ul> <p>Para obter informações sobre a configuração Usuários em um nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Conceder acesso aos usuários</a>.</p> </li> 
     </ul> </p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir que plano, tipo de licença ou configurações de nível de acesso você tem, entre em contato com o [!DNL Workfront] administrador. Para obter mais informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Benefícios de adicionar usuários a uma empresa {#benefits-of-adding-users-to-a-company}

* Você pode criar o organograma de uma empresa associando usuários a subordinados diretos. Somente usuários da mesma empresa podem ser adicionados como subordinados diretos de outro usuário dessa empresa.
* Como gerente de projeto, você pode identificar os recursos disponíveis na mesma empresa.
* É possível manter as informações privadas entre empresas ao escolher uma ou todas as seguintes configurações:

   * Usuários da mesma empresa podem ver as solicitações um do outro.

     Para obter mais informações sobre como [!DNL Workfront] administrador pode conceder acesso semelhante a solicitações com base na empresa dos usuários, consulte a seção [Configurar preferências de tarefas e problemas para todos em [!DNL Workfront]](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md#changing-task-and-issue-preferences) no artigo [Configurar preferências de tarefas e problemas em todo o sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

     Para obter mais informações sobre como um administrador de grupo pode conceder acesso semelhante a solicitações com base na empresa dos usuários, consulte [Configurar preferências de tarefas e problemas para um grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

   * Os usuários podem visualizar somente as filas de solicitações associadas a suas empresas. Para obter mais informações sobre como restringir a visibilidade de uma fila de solicitações, consulte [Fornecer acesso a filas de solicitações](../../../manage-work/requests/create-and-manage-request-queues/provide-access-to-request-queues.md).
   * É possível restringir os usuários para que vejam apenas os usuários em sua empresa ou na empresa e na empresa primária. Para obter informações sobre a funcionalidade principal da empresa em relação à privacidade do usuário, consulte [Criar ou modificar níveis de acesso personalizados](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
   * Os usuários podem restringir as atualizações feitas nos itens para que fiquem visíveis somente pelos usuários da empresa. Para obter mais informações sobre como tornar uma atualização privada para uma empresa, consulte [Atualizar trabalho](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

## Criar ou editar uma empresa no [!DNL Workfront] {#create-or-edit-a-company-in-workfront}

Não há limite para o número de empresas que podem ser adicionadas. No entanto, recomendamos que você limite o número de empresas usadas devido a problemas que podem ocorrer com permissões de objeto; uma fragmentação excessiva pode interferir na visibilidade dos usuários para itens de trabalho.

Por padrão, a empresa associada à sua instância de [!DNL Workfront] já foi criado em seu [!DNL Workfront] e é a Empresa primária da sua organização. Ele tem o mesmo nome do seu cliente. Para obter mais informações sobre o cliente, consulte [!DNL Workfront], consulte [Configurar informações básicas do seu sistema](../../../administration-and-setup/get-started-wf-administration/configure-basic-info.md).

Para adicionar ou editar uma empresa:

{#step-1-to-setup}

1. Clique em **[!UICONTROL Empresas]**.

   Uma lista de empresas é exibida.
1. Se estiver adicionando uma empresa, clique em **[!UICONTROL Nova Empresa]**.

   Ou

   Se você estiver editando uma empresa existente, selecione-a e clique em **[!UICONTROL Editar]** no topo da lista de empresas.

1. Atualize as seguintes informações:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Seção [!UICONTROL Informações Básicas]</td> 
      <td> 
       <ul> 
        <li> <p><b>[!UICONTROL Nome da Empresa]</b>: digite um nome para a empresa.</p> </li> 
        <li> <p><b>[!UICONTROL Está Ativo]</b>: quando essa opção é ativada, os usuários podem encontrar a empresa e anexá-la aos projetos que criam e editam. Uma empresa inativa não pode ser anexada a projetos. Essa opção está ativada por padrão.</p> </li> 
        <li> <p><b>[!UICONTROL Esta é a Empresa Primária]</b>: atribui a empresa como a empresa principal da organização. A empresa primária geralmente representa seu [!DNL Workfront] conta na qual a maioria dos usuários trabalha.</p> <p>Você pode ter uma empresa ou nenhuma empresa designada como empresa primária, mas não pode ter várias empresas designadas como empresas primárias. Para obter mais informações, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> <p><b>NOTA</b>: ao modificar seus níveis de acesso, você pode restringir os usuários a ver outros usuários: somente na empresa principal ou na empresa associada e na empresa principal. Para obter informações sobre como a empresa primária funciona com os níveis de acesso dos usuários, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </li> 
        <li> <p><b>[!UICONTROL Grupo]</b>: se houver um grupo que faz negócios com a empresa, você pode adicionar o nome do grupo aqui. Isso é útil para administradores de grupos que precisam relatar e gerenciar todas as empresas com as quais seus grupos fazem negócios.</p> <p><b>IMPORTANTE</b>: se você não associar o grupo que trabalhará com essa empresa, os administradores do grupo não poderão acessar a empresa, a menos que tenham acesso administrativo a empresas em seu nível de acesso. Para obter informações sobre como esse acesso é concedido, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Conceder aos usuários acesso administrativo a determinadas áreas</a>.</p> <p data-mc-conditions="SnippetConditions-wf-groups.system-level">Comece a digitar o nome do grupo e pressione <strong>[!UICONTROL Enter]</strong> quando ele aparecer.</p> <p data-mc-conditions="SnippetConditions-wf-groups.system-level">Quando você atribui um grupo a uma empresa, os administradores do grupo obtêm acesso à empresa para o [!UICONTROL Manager]. Para obter mais informações, consulte <a href="#group-administrators-and-companies" class="MCXref xref">Administradores de grupo e empresas</a> neste artigo.</p> </li> 
        <li> <p><b>[!UICONTROL Membros da Empresa]</b>: adicione usuários existentes à empresa. Ao fazer isso, você está associando esses usuários a esta empresa.</p> <p>Não há limite para quantos usuários você associa a uma empresa, mas um usuário não pode estar associado a mais de uma empresa.</p> </li> 
       </ul> </td> 
     </tr>
     <tr> 
      <td role="rowheader">Seção [!UICONTROL Custom Forms]</td> 
      <td> <p>Se houver campos que você deseja adicionar à sua empresa que não estejam disponíveis no [!DNL Workfront], você pode criar um formulário personalizado e associá-lo à sua empresa. </p> <p>Você pode anexar esse formulário à sua empresa selecionando-o no menu suspenso. Somente formulários personalizados ativos são listados no menu.</p> <p><strong>Nota:</strong> Recursos avançados de formulário personalizado, como campos de Pesquisa externa e campos nativos do Workfront, só estarão disponíveis quando você abrir o registro da empresa na página de detalhes, não na caixa de diálogo Editar empresa. (Na lista de empresas, clique no nome da empresa para abrir os detalhes.)</p> <p> Para obter informações sobre como criar formulários personalizados, consulte <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">Criar ou editar um formulário personalizado</a>. </p> </td>
     </tr> 
    </tbody> 
   </table>

1. (Condicional) Se você estiver criando uma empresa, clique em **[!UICONTROL Criar empresa]**.

   Ou

   Se você estiver editando uma empresa existente, clique em **[!UICONTROL Salvar alterações]**.

## Gerenciar associações de empresa

Para obter informações sobre como gerenciar associações de uma empresa existente, consulte [Gerenciar associações de empresa](../../../administration-and-setup/set-up-workfront/organizational-setup/manage-company-memberships.md).

## Gerenciar taxas de cobrança

Para obter informações sobre substituição de taxas de faturamento no nível da empresa, consulte [Substituir taxas de cobrança de função de trabalho no nível da empresa](/help/quicksilver/administration-and-setup/set-up-workfront/organizational-setup/override-job-role-billing-rates-company-level.md).

## Visão geral do compartilhamento de objetos com empresas

Determinadas permissões estão disponíveis para usuários associados a uma empresa, conforme explicado na seção [Benefícios de adicionar usuários a uma empresa](#benefits-of-adding-users-to-a-company). Além dessas permissões, você pode permitir que os usuários tenham permissões para exibir, contribuir ou editar objetos no [!DNL Workfront] compartilhando o objeto com sua empresa.

Em vez de compartilhar um objeto com um usuário individual por vez, você pode compartilhá-lo com toda a empresa. Cada usuário na empresa tem as mesmas permissões nesse objeto.

Para obter mais informações sobre objetos de compartilhamento, consulte [Visão geral das permissões de compartilhamento em objetos](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

## Administradores de grupo e empresas {#group-administrators-and-companies}

Quando um [!DNL Workfront] administrador atribui um grupo a uma empresa, os administradores do grupo novamente [!UICONTROL Gerenciar] acesso à empresa em [!UICONTROL Configuração]. Isso inclui o acesso à [!UICONTROL Empresas] página em [!UICONTROL Configuração], onde podem ver e gerenciar a empresa associada ao grupo.

Com esse acesso à [!UICONTROL Empresas] página, um administrador de grupo pode atribuir um grupo a uma empresa, mas ela deve ser uma empresa criada pelo administrador do grupo. Se o nível de acesso do administrador de grupo não estiver configurado com acesso administrativo a empresas, a variável [!UICONTROL Grupo] o campo é obrigatório quando o administrador de grupo cria a empresa — seu título em negrito indica isso:

![Editar empresa](assets/group-admin-add-company.png)

Para obter informações sobre como os usuários obtêm acesso administrativo a empresas em seus níveis de acesso, consulte [Conceder aos usuários acesso administrativo a determinadas áreas](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

Para obter informações sobre o gerenciamento de uma empresa na [!UICONTROL Configuração] , consulte [Criar ou editar uma empresa no [!DNL Workfront]](#create-or-edit-a-company-in-workfront) neste artigo.
