---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: work-with-a-groups-objects
title: Criar e modificar modelos de projeto de um grupo
description: Ao visualizar um grupo que você gerencia na área Grupos , é possível visualizar e trabalhar com modelos de projeto associados ao grupo e a qualquer um de seus subgrupos.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: f97a12eb-9002-4f11-908a-c68c1e6dc9c9
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '1284'
ht-degree: 1%

---

# Criar e modificar modelos de projeto de um grupo

Ao visualizar um grupo que você gerencia na área Grupos , é possível visualizar e trabalhar com modelos de projeto associados ao grupo e a qualquer um de seus subgrupos.

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
   <td> <p>Plano </p> <p>Você deve ser um administrador de grupo do grupo ou um administrador do Workfront. Para obter mais informações, consulte <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Administradores do grupo</a> e <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder ao usuário acesso administrativo total</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Visualize o acesso ou superior nos modelos que deseja visualizar e trabalhar com</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Se precisar descobrir qual plano ou tipo de licença você tem, entre em contato com o administrador da Workfront.

## Exibir, trabalhar e criar modelos para seu grupo na área Grupos

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront, em seguida, clique em **Configuração** ![](assets/gear-icon-settings.png).

1. No painel esquerdo, clique em **Grupos** ![](assets/groups-icon.png).

1. Clique no nome do grupo para o qual deseja criar ou modificar templates.
1. No painel esquerdo, clique em **Modelos** para listar os modelos associados ao grupo e com qualquer subgrupo que ele possa ter.

   Você deve ter acesso de Exibição a um modelo para vê-lo nesta lista. Para obter informações sobre esse acesso, consulte [Conceder acesso aos modelos](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-templates.md).

1. Siga um destes procedimentos:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Adicionar um modelo</td> 
      <td> <p>Clique em <strong>Novo modelo</strong>, configure-a usando as opções disponíveis. Para obter informações sobre essas opções, consulte <a href="../../../manage-work/projects/create-and-manage-templates/create-template.md" class="MCXref xref">Criar um modelo de projeto</a>.</p> <p>O modelo é associado automaticamente ao grupo.</p> <p>Para obter informações sobre como as preferências de grupo se aplicam a novos modelos, consulte <a href="#how-preferences-apply-to-templates-and-template-tasks" class="MCXref xref">Como as preferências se aplicam a modelos e tarefas de modelo</a> neste artigo.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Editar um ou mais modelos</td> 
      <td> <p>Selecione pelo menos um modelo, clique no ícone Editar <img src="assets/edit-icon.png">, em seguida, use qualquer uma das opções disponíveis para configurá-la. Para obter informações sobre essas opções, consulte <a href="../../../manage-work/projects/create-and-manage-templates/edit-templates.md" class="MCXref xref">Editar modelos de projeto</a>.</p> <p>O ícone Editar fica disponível somente se você tiver acesso Editar a todos os modelos selecionados. Para obter informações sobre esse acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-templates.md" class="MCXref xref">Conceder acesso aos modelos</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Excluir um ou mais modelos</td> 
      <td> <p>Selecione pelo menos um modelo e clique no ícone Excluir <img src="assets/delete.png">.</p> <p>Este ícone só estará disponível se você tiver o acesso Editar a todos os modelos selecionados. Para obter informações sobre esse acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-templates.md" class="MCXref xref">Conceder acesso aos modelos</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Compartilhar um ou mais modelos</td> 
      <td> <p>Selecione pelo menos um modelo, clique no ícone Compartilhar <img src="assets/share-icon.png">e, em seguida, clique em uma das seguintes opções no menu suspenso:</p> 
       <ul> 
        <li> <p><strong>Modelo</strong>: No <strong>Acesso ao modelo</strong> , adicione nomes para especificar quem você deseja que tenha acesso ao próprio modelo.</p> <p>Para obter mais informações, consulte a seção <a href="../../../manage-work/projects/create-and-manage-templates/share-project-template.md#share" class="MCXref xref">Compartilhar um modelo</a> no artigo <a href="../../../manage-work/projects/create-and-manage-templates/share-project-template.md" class="MCXref xref">Compartilhar modelos de projeto</a>.</p> </li> 
        <li><strong>Projeto</strong>: No <strong>Acesso ao projeto</strong> caixa exibida, adicione nomes para especificar quem você deseja que tenha acesso aos projetos criados a partir do modelo</li> 
       </ul> <p>O ícone Compartilhar estará disponível somente se você tiver acesso de Compartilhamento a todos os modelos selecionados. Para obter informações sobre esse acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-templates.md" class="MCXref xref">Conceder acesso aos modelos</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Exportar a lista de modelos</td> 
      <td>Clique em <strong>Exportar</strong> <img src="assets/export.png">, em seguida, selecione o formato de arquivo que deseja para a lista exportada.</td> 
     </tr> 
    </tbody> 
   </table>

## Como as preferências se aplicam a modelos e tarefas de modelo {#how-preferences-apply-to-templates-and-template-tasks}

Ao criar um template de projeto, as configurações listadas nas tabelas abaixo são configuradas automaticamente por uma preferência de projeto ou tarefa correlacionada.

>[!NOTE]
>
>Uma preferência de projeto ou tarefa em nível de grupo ou de sistema afeta um modelo de projeto, dependendo de você ter associado o modelo a um grupo ao criá-lo.
>
>Se você associou-o a um grupo, a preferência de nível de grupo entrará em vigor. Isso ocorre nos seguintes cenários:
>
>* Crie o modelo a partir da área Grupos , conforme explicado neste artigo
>* Você especifica um grupo ao criar o modelo usando um arquivo Kickstart
>* Você especifica um grupo ao criar o modelo usando a API
>
>Se você não associou o novo modelo a um grupo, a preferência de nível de sistema entrará em vigor. Isso ocorre nos cenários abaixo. (Se posteriormente você atribuir um grupo à tarefa modelo ou modelo, as preferências do grupo não afetarão.)
>
>* Você cria o modelo a partir da área Modelos
>* Você não especifica um grupo ao criar o modelo usando um arquivo Kickstart
>* Você não especifica um grupo ao criar o modelo usando a API
>


* [Configurações do modelo de projeto definidas pelas preferências do projeto e da tarefa](#project-template-settings-configured-by-project-and-task-preferences)
* [Configurações de tarefa de modelo definidas pelas preferências de tarefa](#template-task-settings-configured-by-task-preferences)

### Configurações do modelo de projeto definidas pelas preferências do projeto e da tarefa {#project-template-settings-configured-by-project-and-task-preferences}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Método Índice de desempenho</p> </td> 
   <td> <p>Configurado pela preferência de projeto em nível de grupo "Método de Índice de Desempenho" se você associar o novo modelo a um grupo ou pela mesma preferência de projeto em nível de sistema, caso não tenha.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Tipo de Condição</p> </td> 
   <td> <p>Configurado pela preferência de projeto em nível de grupo "Definir automaticamente a condição do projeto com base no status de progresso" se você associar o novo modelo a um grupo ou a mesma preferência de projeto em nível de sistema, caso não tenha.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Agendar de</p> </td> 
   <td> <p>Configurado pela preferência de projeto em nível de grupo "Agendar de" se você associar o novo modelo a um grupo ou pela mesma preferência de projeto em nível de sistema, caso não tenha.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Tempo limite do usuário</p> </td> 
   <td> <p>Configurado pela preferência de projeto em nível de grupo "Tempo do usuário desligado" se você associar o novo modelo a um grupo ou pela mesma preferência de projeto em nível de sistema, caso não tenha.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Tipo de atualização</p> </td> 
   <td> <p>Configurado pela preferência de projeto em nível de grupo "As linhas do tempo do projeto serão automaticamente recalculadas" se você associar o novo modelo a um grupo ou a mesma preferência de projeto em nível de sistema, caso não tenha.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Configurações da seção Access</p> </td> 
   <td> <p>Configurado pelas preferências de tarefa em nível de grupo na seção "Acesso" se você associar o novo modelo a um grupo ou a mesma preferência de projeto em nível de sistema, caso não tenha.</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obter informações sobre as preferências do projeto listadas nesta tabela, consulte [Configurar preferências de projeto em todo o sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

Para obter informações sobre a tarefa e a preferência de emissão, consulte [Configurar preferências de emissão e tarefa em todo o sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

>[!NOTE]
>
>* Se você alterar o grupo associado a um modelo de projeto existente, as configurações do modelo permanecerão as mesmas.
>* Se você mover uma tarefa de modelo existente para outro modelo, as seguintes configurações permanecerão inalteradas na tarefa de modelo, independentemente do grupo associado ao novo modelo:>
   >   * Tipo de Duração
   >   * Tipo de Receita
   >   * Tipo de Custo
>
>  No entanto, a tarefa do modelo é afetada pela configuração &quot;Quando alguém é atribuído a uma tarefa&quot; no novo modelo. Para obter mais informações, consulte a seção [Acesso](../../../manage-work/projects/create-and-manage-templates/edit-templates.md#access) no artigo [Editar modelos de projeto](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).
>
>* Quando um administrador salva um projeto como modelo, todas as configurações do modelo são herdadas do projeto, incluindo o grupo .
>
>  Quando um administrador converte uma tarefa ou um problema em um projeto usando um modelo, todas as configurações do modelo são determinadas pelo que já foi salvo no modelo.

### Configurações de tarefa de modelo definidas pelas preferências de tarefa {#template-task-settings-configured-by-task-preferences}

Ao criar uma tarefa de modelo, algumas de suas configurações são configuradas automaticamente por uma preferência de tarefa de correlação. Essas configurações estão listadas na tabela abaixo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Tipo de Duração </p> </td> 
   <td> <p>Configurado pela preferência de tarefa em nível de grupo "Tipo de duração" se você associar o modelo a um grupo ou a mesma tarefa em nível de sistema e emitir preferência se não fizer isso.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Tipo de Receita</p> </td> 
   <td> <p>Configurado pela preferência de tarefa em nível de grupo "Tipo de receita" se você associar o modelo a um grupo ou a mesma tarefa em nível de sistema e emitir preferência caso não esteja.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Tipo de Custo </p> </td> 
   <td> <p> Configurado pela preferência de tarefa em nível de grupo "Tipo de Custo" se você associar o modelo a um grupo ou a mesma tarefa em nível de sistema e emitir preferência caso não esteja.</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obter informações sobre as preferências de tarefa listadas nesta tabela, consulte [Configurar preferências de emissão e tarefa em todo o sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).
