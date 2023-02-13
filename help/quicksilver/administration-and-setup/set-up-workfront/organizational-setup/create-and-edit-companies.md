---
user-type: administrator
product-area: system-administration
navigation-topic: organization-setup
title: Criar e editar empresas
description: Você pode adicionar empresas ao [!DNL Workfront] e usá-las para planejamento financeiro, fins de relatório, para definir permissões em torno de objetos e manter as informações confidenciais.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: bb597032-3395-4c9a-b622-5c920ba55131
source-git-commit: b6f6964bb80f172849434c669df2b0ecd735a590
workflow-type: tm+mt
source-wordcount: '1440'
ht-degree: 0%

---

# Criar e editar empresas

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

Uma empresa é uma unidade organizacional em [!DNL Adobe Workfront] que pode representar sua organização, um departamento dentro da organização ou um cliente com o qual você trabalha. Você pode adicionar empresas ao [!DNL Workfront] e usá-las para planejamento financeiro, fins de relatório, para definir permissões em torno de objetos e manter as informações confidenciais.

## Requisitos de acesso

Você deve ter o seguinte para gerenciar empresas no [!DNL Workfront]:

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Workfront] plano*</p> </td> 
   <td>[!UICONTROL Team] ou superior</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Adobe Workfront] licença*</p> </td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Um dos seguintes:</p> 
    <ul> 
     <li> <p>O nível de acesso do [!UICONTROL System Administrator], que permite a edição de qualquer empresa no sistema. Para obter mais informações, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder ao usuário acesso administrativo total</a>. </p> </li> 
     <li> <p>Acesso administrativo para gerenciar empresas, o que permite editar qualquer empresa no sistema. Para obter mais informações, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Conceder aos usuários acesso administrativo a determinadas áreas</a>.</p> </li> 
    </ul> <p><b>Nota</b>:  
     <ul> 
      <li> <p>Também é possível gerenciar empresas associadas a qualquer grupo, onde você está atribuído como administrador de grupo.</p> </li> 
      <li> <p>Para adicionar e remover usuários do [!DNL Workfront] , você deve ter um dos seguintes itens:</p> 
       <ul> 
        <li> <p>O nível de acesso do [!UICONTROL System Administrator]. Para obter mais informações, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder ao usuário acesso administrativo total</a>. </p> </li> 
        <li> <p>No nível de acesso, [!UICONTROL Editar] deve ser selecionado para a configuração [!UICONTROL Usuários]. Além disso, para a configuração [!UICONTROL Usuários], em [!UICONTROL Otimizar suas configurações] <img src="assets/gear-icon-in-access-levels.png"> , a opção [!UICONTROL Criar] e pelo menos uma das duas opções do [!UICONTROL User Admin] devem estar habilitadas. </p> <p> <img src="assets/access-req-users.png"> </p> <p>Se estiver usando a opção [!UICONTROL Administrador de usuário (Usuários de grupo)], você deve ser um administrador de grupo de um grupo no qual o usuário é membro.</p> </li> 
       </ul> <p>Para obter informações sobre a configuração Usuários em um nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Conceder acesso aos usuários</a>.</p> </li> 
     </ul> </p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir que plano, tipo de licença ou configurações de nível de acesso você possui, entre em contato com seu [!DNL Workfront] administrador.

## Benefícios da adição de usuários a uma empresa {#benefits-of-adding-users-to-a-company}

* Você pode criar o gráfico de organização de uma empresa ao associar usuários a relatórios diretos. Somente usuários da mesma empresa podem ser adicionados como relatórios diretos de outro usuário dessa empresa.
* Como gerente de projeto, você pode identificar os recursos disponíveis na mesma empresa.
* Você pode manter as informações privadas entre empresas escolhendo uma ou todas as seguintes configurações:

   * Os usuários da mesma empresa podem ver as solicitações uns dos outros.

      Para obter mais informações sobre como uma [!DNL Workfront] o administrador pode conceder acesso semelhante a solicitações com base na empresa dos usuários; consulte a seção [Configurar preferências de tarefa e problemas para todos em [!DNL Workfront]](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md#changing-task-and-issue-preferences) no artigo [Configurar preferências de emissão e tarefa em todo o sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

      Para obter mais informações sobre como um administrador de grupo pode conceder acesso semelhante a solicitações com base na empresa dos usuários, consulte [Configurar preferências de tarefa e emissão para um grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

   * Os usuários podem ver somente as filas de solicitação que estão associadas às empresas. Para obter mais informações sobre como restringir a visibilidade de uma fila de solicitações, consulte [Fornecer acesso às filas de solicitação](../../../manage-work/requests/create-and-manage-request-queues/provide-access-to-request-queues.md).
   * Você pode restringir usuários a ver somente usuários em sua empresa ou na empresa e na empresa principal. Para obter informações sobre a funcionalidade principal da empresa em relação à privacidade do usuário, consulte [Criar ou modificar níveis de acesso personalizados](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
   * Os usuários podem restringir as atualizações que fazem nos itens para que sejam visíveis apenas pelos usuários da empresa. Para obter mais informações sobre como tornar uma atualização privada para uma empresa, consulte [Atualizar trabalho](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

## Crie ou edite uma empresa em [!DNL Workfront] {#create-or-edit-a-company-in-workfront}

Não há limite para o número de empresas que você pode adicionar. No entanto, recomendamos limitar o número de empresas que você usa devido a problemas que podem ocorrer com permissões de objeto. Grande fragmentação pode interferir na visibilidade dos usuários em itens de trabalho.

Por padrão, a empresa associada à sua instância de [!DNL Workfront] já foi criada no [!DNL Workfront] e é a principal empresa da sua organização. Ele tem o mesmo nome do seu cliente. Para obter mais informações sobre seus clientes em [!DNL Workfront], consulte [Configurar informações básicas para seu sistema](../../../administration-and-setup/get-started-wf-administration/configure-basic-info.md).

Para adicionar ou editar uma empresa:

1. Clique no botão **[!UICONTROL Menu principal]** ícone ![](assets/main-menu-icon.png) no canto superior direito de [!DNL Adobe Workfront], depois clique em **[!UICONTROL Configuração]** ![](assets/gear-icon-settings.png).

1. Clique em **[!UICONTROL Empresas]**.
1. Se você estiver adicionando uma empresa, clique em **[!UICONTROL Nova empresa]**.

   Ou

   Se você estiver editando uma empresa existente, selecione a empresa e clique em **[!UICONTROL Editar]**.

1. Use as opções exibidas para configurar as seguintes informações:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Seção [!UICONTROL Informações básicas]</td> 
      <td> 
       <ul> 
        <li> <p><b>[!UICONTROL Nome da empresa]</b>: Digite um nome para a empresa.</p> </li> 
        <li> <p><b>[!UICONTROL Está Ativo]</b>: Quando essa opção está ativada, os usuários podem encontrar a empresa e anexá-la a projetos que eles criam e editam. Uma empresa inativa não pode ser anexada a projetos. Essa opção é ativada por padrão.</p> </li> 
        <li> <p><b>[!UICONTROL Esta é a empresa principal]</b>: Atribui a empresa como a empresa principal de sua organização. A principal empresa geralmente representa o seu [!DNL Workfront] onde a maioria dos usuários trabalha.</p> <p>É possível ter uma empresa ou nenhuma empresa designada como empresa primária, mas não é possível ter várias empresas designadas como empresas primárias. Para obter mais informações, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> <p><b>OBSERVAÇÃO</b>: Ao modificar os níveis de acesso, é possível restringir os usuários a ver outros usuários: apenas na sua empresa principal ou na empresa associada e na empresa principal. Para obter informações sobre como a empresa principal funciona com os níveis de acesso dos usuários, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </li> 
        <li> <p><b>[!UICONTROL Grupo]</b>: Se houver um grupo que faça negócios com a empresa, você poderá adicionar o nome do grupo aqui. Isso é útil para administradores de grupo que precisam criar relatórios e gerenciar todas as empresas com as quais seus grupos fazem negócios.</p> <p><b>IMPORTANTE</b>: Se você não associar o grupo que trabalhará com essa empresa, os administradores do grupo não poderão acessar a menos que tenham acesso administrativo a empresas em seu nível de acesso. Para obter informações sobre como esse acesso é concedido, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Conceder aos usuários acesso administrativo a determinadas áreas</a>.</p> <p data-mc-conditions="SnippetConditions-wf-groups.system-level">Comece a digitar o nome do grupo e pressione <strong>[!UICONTROL Enter]</strong> quando for exibido.</p> <p data-mc-conditions="SnippetConditions-wf-groups.system-level">Ao atribuir um grupo a uma empresa, os administradores de grupo do grupo obtêm acesso à empresa no [!UICONTROL Gerenciar]. Para obter mais informações, consulte <a href="#group-administrators-and-companies" class="MCXref xref">Administradores de grupos e empresas</a> neste artigo.</p> </li> 
        <li> <p><b>[!UICONTROL Membros da empresa]</b>: Adicionar usuários existentes à empresa. Ao fazer isso, você está associando esses usuários a essa empresa.</p> <p>Não há limite para quantos usuários você associa a uma empresa, mas um usuário não pode ser associado a mais de uma empresa.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Seção [!UICONTROL Taxas de Faturamento]</td> 
      <td> <p>Você pode sobrepor as taxas de faturamento associadas às suas funções de cargo no nível da empresa. Para obter informações sobre como criar funções de cargo e associá-las a taxas de faturamento, consulte <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Criar e gerenciar funções de trabalho</a>.</p> <p>Para obter mais informações sobre a sobreposição de taxas de faturamento no nível da empresa, consulte <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/override-job-role-billing-rates-company-level.md" class="MCXref xref">Substituir as taxas de faturamento da função de trabalho no nível da empresa</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Seção [!UICONTROL Forms personalizado]</td> 
      <td> <p>Se houver campos que você deseja adicionar à sua empresa que não estão disponíveis em [!DNL Workfront], crie um Formulário personalizado e associe-o à sua empresa. Você pode anexar esse formulário à sua empresa selecionando-o no menu suspenso. Somente empresas ativas são listadas no menu suspenso. Para obter informações sobre como criar o Forms personalizado, consulte <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">Criar ou editar um formulário personalizado</a>. </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Se você estiver criando uma nova empresa, clique em **[!UICONTROL Criar empresa]**.

   Ou

   Se você estiver editando uma empresa existente, clique em **[!UICONTROL Salvar alterações]**.

## Gerenciar associações de empresas

Para obter informações sobre o gerenciamento de associações para uma empresa existente, consulte [Gerenciar associações de empresas](../../../administration-and-setup/set-up-workfront/organizational-setup/manage-company-memberships.md).

## Sobre o compartilhamento de objetos com empresas

Certas permissões estão disponíveis para usuários associados a uma empresa, conforme explicado na seção [Benefícios da adição de usuários a uma empresa](#benefits-of-adding-users-to-a-company). Além dessas permissões, você pode permitir que os usuários tenham permissões para visualizar, contribuir ou editar objetos no [!DNL Workfront] compartilhando o objeto com a empresa.

Em vez de compartilhar um objeto com um usuário individual por vez, você pode compartilhá-lo com toda a empresa. Cada usuário na empresa tem as mesmas permissões nesse objeto.

Para obter mais informações sobre o compartilhamento de objetos, consulte [Visão geral do compartilhamento de permissões em objetos](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

## Administradores de grupos e empresas {#group-administrators-and-companies}

Quando uma [!DNL Workfront] administrador atribui um grupo a uma empresa, os administradores do grupo ganham [!UICONTROL Gerenciar] acesso à empresa em [!UICONTROL Configuração]. Isso inclui o acesso à [!UICONTROL Empresas] em [!UICONTROL Configuração], onde podem ver e gerenciar a empresa associada ao seu grupo.

Com esse acesso à [!UICONTROL Empresas] , um administrador de grupo pode atribuir um grupo a uma empresa, mas deve ser uma empresa criada pelo administrador do grupo. Se o nível de acesso do administrador de grupo não estiver configurado com acesso administrativo às empresas, a variável [!UICONTROL Grupo] é necessário quando o administrador do grupo cria a empresa. O título em negrito indica o seguinte:

![](assets/manage-company-group-field-req.jpg)

Para obter informações sobre como os usuários obtêm acesso administrativo às empresas em seu nível de acesso, consulte [Conceder aos usuários acesso administrativo a determinadas áreas](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

Para obter informações sobre como gerenciar uma empresa no [!UICONTROL Configuração] área, consulte [Crie ou edite uma empresa em [!DNL Workfront]](#create-or-edit-a-company-in-workfront) neste artigo.
