---
user-type: administrator
product-area: system-administration
navigation-topic: organization-setup
title: Criar e editar empresas
description: Você pode adicionar empresas a [!DNL Adobe Workfront] e usá-las para fins de planejamento financeiro, relatórios, para definir permissões sobre objetos e para manter a confidencialidade das informações.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: bb597032-3395-4c9a-b622-5c920ba55131
source-git-commit: 5e81e18ef667af3e4d08f4fc8987f7a3b6617971
workflow-type: tm+mt
source-wordcount: '1440'
ht-degree: 0%

---

# Criar e editar empresas

<!--Audited: 01/2024-->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

<span class="preview">As informações destacadas nesta página referem-se a funcionalidades que ainda não estão disponíveis. Ele está disponível somente no ambiente de Pré-visualização da Sandbox e está sendo lançado em uma implantação em fases para Produção.</span>

Uma empresa é uma unidade organizacional no [!DNL Adobe Workfront] que pode representar sua organização, um departamento dentro da organização ou um cliente com o qual você trabalha. Você pode adicionar empresas a [!DNL Workfront] e usá-las para fins de planejamento financeiro, relatórios, para definir permissões sobre objetos e para manter as informações confidenciais.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Workfront] pacote</p> </td> 
   <td><p>Qualquer</p></td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] licença</p> </td> 
   <td><p>[!UICONTROL Plano]</p>
   <p>[!UICONTROL Padrão]</p>
   </td> 
  </tr> 
  <tr> 
   <td>Configuração do nível de acesso</td> 
   <td> <p>Você deve ter um dos seguintes:</p> 
    <ul> 
     <li> <p>O nível de acesso do [!UICONTROL System Administrator], que permite editar qualquer empresa no sistema.</p> </li> 
     <li> <p>Acesso administrativo para gerenciar empresas, que permite editar qualquer empresa no sistema.</p> </li> 
    </ul> <p><b>NOTA</b>:  
     <ul> 
      <li> <p>Você também pode gerenciar empresas associadas a qualquer grupo ao qual esteja atribuído como administrador de grupo.</p> </li> 
      <li> <p>Para adicionar e remover usuários do sistema [!DNL Workfront], você deve ter um dos seguintes:</p> 
       <ul> 
        <li> <p>O nível de acesso do [!UICONTROL System Administrator]. </p> </li> 
        <li> <p>Configuração de <b>[!UICONTROL Usuários]</b> em seu nível de acesso configurada para <b>[!UICONTROL Editar]</b> acesso, com <b>[!UICONTROL Criar]</b> e pelo menos uma das duas opções <b>[!UICONTROL Administrador de Usuários]</b> habilitadas em <b>[!UICONTROL Ajustar suas configurações]</b> <img src="assets/gear-icon-in-access-levels.png">. </p> <p> <img src="assets/access-req-users.png"> </p> <p>Dessas duas opções, se <b>[!UICONTROL Usuário Admin (Usuários de Grupo)]</b> estiver habilitado, você deverá ser um administrador de grupo de um grupo do qual o usuário seja membro.</p> </li> 
       </ul>
       </li> 
     </ul> </p> </td> 
  </tr> 
 </tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Benefícios de adicionar usuários a uma empresa {#benefits-of-adding-users-to-a-company}

* Você pode criar o organograma de uma empresa associando usuários a subordinados diretos. Somente usuários da mesma empresa podem ser adicionados como subordinados diretos de outro usuário dessa empresa.
* Como gerente de projeto, você pode identificar os recursos disponíveis na mesma empresa.
* É possível manter as informações privadas entre empresas ao escolher uma ou todas as seguintes configurações:

   * Usuários da mesma empresa podem ver as solicitações um do outro.

     Para obter mais informações sobre como um administrador do [!DNL Workfront] pode conceder acesso semelhante a solicitações com base na empresa dos usuários, consulte a seção [Configurar preferências de tarefas e problemas para todos em [!DNL Workfront]](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md#changing-task-and-issue-preferences) no artigo [Configurar preferências de tarefas e problemas em todo o sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

     Para obter mais informações sobre como um administrador de grupo pode conceder acesso semelhante a solicitações com base na empresa dos usuários, consulte [Configurar preferências de tarefas e problemas para um grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

   * Os usuários podem visualizar somente as filas de solicitações associadas a suas empresas. Para obter mais informações sobre como restringir a visibilidade de uma fila de solicitações, consulte [Fornecer acesso às filas de solicitações](../../../manage-work/requests/create-and-manage-request-queues/provide-access-to-request-queues.md).
   * É possível restringir os usuários para que vejam apenas os usuários em sua empresa ou na empresa e na empresa primária. Para obter informações sobre a funcionalidade principal da empresa em relação à privacidade do usuário, consulte [Criar ou modificar níveis de acesso personalizados](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
   * Os usuários podem restringir as atualizações feitas nos itens para que fiquem visíveis somente pelos usuários da empresa. Para obter mais informações sobre como tornar uma atualização privada para uma empresa, consulte [Trabalho de atualização](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

## Criar ou editar uma empresa em [!DNL Workfront] {#create-or-edit-a-company-in-workfront}

Não há limite para o número de empresas que podem ser adicionadas. No entanto, recomendamos que você limite o número de empresas usadas devido a problemas que podem ocorrer com permissões de objeto; uma fragmentação excessiva pode interferir na visibilidade dos usuários para itens de trabalho.

Por padrão, a empresa associada à sua instância do [!DNL Workfront] já está criada no sistema [!DNL Workfront] e é a Empresa primária da sua organização. Ele tem o mesmo nome do seu cliente. Para obter mais informações sobre o cliente no [!DNL Workfront], consulte [Configurar informações básicas do sistema](../../../administration-and-setup/get-started-wf-administration/configure-basic-info.md).

Para adicionar ou editar uma empresa:

{{step-1-to-setup}}

1. Clique em **[!UICONTROL Empresas]**.

   Uma lista de empresas é exibida.

1. Se você estiver adicionando uma empresa, clique em **[!UICONTROL Nova Empresa]**.

   Ou

   Se você estiver editando uma empresa existente, selecione a empresa e clique no **[!UICONTROL ícone Editar]** ![ícone Editar](assets/edit-icon.png) na parte superior da lista de empresas.

1. Atualize as seguintes informações na seção **Informações Básicas**:

   * **Nome da Empresa** <span class="preview"> ou **Nome**</span>: digite um nome para a empresa.
   * **Está ativo**: quando esta opção é habilitada, os usuários podem encontrar a empresa e anexá-la aos projetos que eles criam e editam. Uma empresa inativa não pode ser anexada a projetos. Essa opção está ativada por padrão.
   * **Esta é a Empresa Primária** <span class="preview">ou **É Primária**</span>: atribui a empresa como a empresa primária da sua organização. A empresa principal geralmente representa a conta da Workfront na qual a maioria dos usuários trabalha.

     Você pode ter uma empresa ou nenhuma empresa designada como empresa primária, mas não pode ter várias empresas designadas como empresas primárias. Para obter mais informações, consulte [Criar e modificar níveis de acesso personalizados](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

     >[!NOTE]
     >
     >Ao modificar seus níveis de acesso, você pode restringir os usuários a ver outros usuários: somente na empresa principal ou na empresa associada e na empresa principal. Para obter informações sobre como a empresa primária funciona com os níveis de acesso dos usuários, consulte [Criar e modificar níveis de acesso personalizados](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

   * **Grupo**: se houver um grupo que faz negócios com a empresa, você pode adicionar o nome do grupo aqui. Isso é útil para administradores de grupos que precisam relatar e gerenciar todas as empresas com as quais seus grupos fazem negócios.

     Se você não associar o grupo que trabalhará com esta empresa, os administradores do grupo não poderão acessar a empresa a menos que tenham acesso administrativo a empresas em seus níveis de acesso. Para obter informações sobre como esse acesso é concedido, consulte [Conceder aos usuários acesso administrativo a determinadas áreas](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

     Comece a digitar o nome do grupo e selecione-o quando ele for exibido.

     Quando você atribui um grupo a uma empresa, os administradores do grupo obtêm acesso de gerenciamento à empresa. Para obter mais informações, consulte [Administradores de grupo e empresas](#group-administrators-and-companies) neste artigo.

   * **Membros da Empresa**: adicionar usuários existentes à empresa. Ao fazer isso, você está associando esses usuários a esta empresa.

     Comece digitando o nome de um usuário e, em seguida, selecione-o quando ele for exibido.

     Não há limite para quantos usuários você associa a uma empresa, mas um usuário não pode estar associado a mais de uma empresa.

1. Adicionar ou atualizar formulários personalizados na seção **Forms Personalizado**.

   Se houver campos que você deseja adicionar à sua empresa que não estejam disponíveis no Workfront, é possível criar um formulário personalizado e associá-lo à sua empresa.

   Você pode anexar esse formulário à sua empresa selecionando-o no menu suspenso. Somente formulários personalizados ativos são listados no menu.

   >[!NOTE]
   >
   >Recursos avançados de formulário personalizado, como campos de pesquisa externos e campos nativos do Workfront, só estão disponíveis quando você abre o registro da empresa na página de detalhes, não na caixa de diálogo Editar empresa. (Na lista de empresas, clique no nome da empresa para abrir os detalhes.)

   Para obter informações sobre como criar formulários personalizados, consulte [Criar um formulário personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

1. (Condicional) Se você estiver criando uma empresa, clique em **[!UICONTROL Criar Empresa]**<span class="preview">ou** Salvar **.</span>

   Ou

   Se você estiver editando uma empresa existente, clique em **[!UICONTROL Salvar alterações]**<span class="preview">ou** Salvar **.</span>

## Gerenciar associações de empresa

Para obter informações sobre como gerenciar associações de uma empresa existente, consulte [Gerenciar associações de empresa](../../../administration-and-setup/set-up-workfront/organizational-setup/manage-company-memberships.md).

## Gerenciar taxas de cobrança

Para obter informações sobre como substituir taxas de cobrança no nível da empresa, consulte [Substituir taxas de cobrança de função de trabalho no nível da empresa](/help/quicksilver/administration-and-setup/set-up-workfront/organizational-setup/override-job-role-billing-rates-company-level.md).

## Visão geral do compartilhamento de objetos com empresas

Determinadas permissões estão disponíveis para usuários associados a uma empresa, conforme explicado na seção [Vantagens de adicionar usuários a uma empresa](#benefits-of-adding-users-to-a-company). Além dessas permissões, você pode permitir que os usuários tenham permissões para exibir, contribuir ou editar objetos no [!DNL Workfront], compartilhando o objeto com a empresa deles.

Em vez de compartilhar um objeto com um usuário individual por vez, você pode compartilhá-lo com toda a empresa. Cada usuário na empresa tem as mesmas permissões nesse objeto.

Para obter mais informações sobre objetos de compartilhamento, consulte [Visão geral das permissões de compartilhamento em objetos](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

## Administradores de grupo e empresas {#group-administrators-and-companies}

Quando um administrador do [!DNL Workfront] atribui um grupo a uma empresa, os administradores do grupo obtêm acesso de [!UICONTROL Gerenciar] à empresa em [!UICONTROL Configuração]. Isso inclui o acesso à página [!UICONTROL Empresas] em [!UICONTROL Configuração], onde é possível ver e gerenciar a empresa associada ao grupo.

Com esse acesso à página [!UICONTROL Empresas], um administrador de grupo pode atribuir um grupo a uma empresa, mas ela deve ser uma empresa criada pelo administrador do grupo. Se o nível de acesso do administrador de grupo não estiver configurado com acesso administrativo a empresas, o campo [!UICONTROL Grupo] será necessário quando o administrador de grupo criar a empresa. Seu título em negrito indica que:

![Editar empresa](assets/group-admin-add-company.png)

Para obter informações sobre como os usuários obtêm acesso administrativo a empresas em seu nível de acesso, consulte [Conceder aos usuários acesso administrativo a determinadas áreas](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

Para obter informações sobre como gerenciar uma empresa na área [!UICONTROL Configuração], consulte [Criar ou editar uma empresa [!DNL Workfront]](#create-or-edit-a-company-in-workfront) neste artigo.

<!-- OLD HTML TABLE
<table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Basic Info] section</td> 
      <td> 
       <ul> 
        <li> <p><b>[!UICONTROL Company Name]</b>: Type a name for the company.</p> </li> 
        <li> <p><b>[!UICONTROL Is Active]</b>: When this option is enabled, users can find the company and attach it to projects that they create and edit. An inactive company cannot be attached to projects. This option is enabled by default.</p> </li> 
        <li> <p><b>[!UICONTROL This is the Primary Company]</b>: Assigns the company as your organization's primary company. The primary company typically represents your [!DNL Workfront] account where most of your users work.</p> <p>You can have one company or no company designated as a primary company, but you cannot have multiple companies designated as primary companies. For more information, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> <p><b>NOTE</b>: By modifying their access levels, you can restrict users to see other users: only in their primary company, or in their associated company and the primary company. For information about how the primary company works with users' access levels, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </li> 
        <li> <p><b>[!UICONTROL Group]</b>: If there is a group that conducts business with the company, you can add the name of the group here. This is useful for group administrators who need to report on and manage all the companies that their groups do business with.</p> <p><b>IMPORTANT</b>: If you don't associate the group that will be working with this company, administrators for the group can't access the company unless they have administrative access to companies in their access level. For information about how this access is granted, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Grant users administrative access to certain areas</a>.</p> <p data-mc-conditions="SnippetConditions-wf-groups.system-level">Start typing the name of the group, then press <strong>[!UICONTROL Enter]</strong> when it appears.</p> <p data-mc-conditions="SnippetConditions-wf-groups.system-level">When you assign a group to a company, the group administrators for the group gain [!UICONTROL Manage] access to the company. For more information, see <a href="#group-administrators-and-companies" class="MCXref xref">Group administrators and companies</a> in this article.</p> </li> 
        <li> <p><b>[!UICONTROL Company Members]</b>: Add existing users to the company. By doing this, you are associating these users with this company.</p> <p>There is no limit to how many users you associate with one company, but a user cannot be associated with more than one company.</p> </li> 
       </ul> </td> 
     </tr>
     <tr> 
      <td role="rowheader">[!UICONTROL Custom Forms] section</td> 
      <td> <p>If there are fields that you want to add to your company that are not available in [!DNL Workfront], you can build a custom form and associate it with your company. </p> <p>You can attach this form to your company by selecting it from the drop-down menu. Only active custom forms are listed in the menu.</p> <p><strong>Note:</strong> Advanced custom form features such as External lookup fields and Workfront native fields are only available when you open the company record on the details page, not on the Edit Company dialog. (From the list of companies, click the company name to open the details.)</p> <p> For information about creating custom forms, see <a href="/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md">Create a custom form</a>. </p> </td>
     </tr> 
    </tbody> 
   </table>
   -->
