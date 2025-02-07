---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: work-with-a-groups-objects
title: Criar e modificar os modelos de projeto de um grupo
description: Ao visualizar um grupo gerenciado na área Grupos, você pode visualizar e trabalhar com modelos de projeto associados ao grupo e a qualquer um de seus subgrupos.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: f97a12eb-9002-4f11-908a-c68c1e6dc9c9
source-git-commit: 612243e928c6053d9b02715d9fcfef4dae25cb7a
workflow-type: tm+mt
source-wordcount: '1281'
ht-degree: 1%

---

# Criar e modificar os modelos de projeto de um grupo

Ao visualizar um grupo gerenciado na área Grupos, você pode visualizar e trabalhar com modelos de projeto associados ao grupo e a qualquer um de seus subgrupos.

Se houver algum grupo acima do seu, os administradores também poderão fazer essas coisas pelo seu grupo. O mesmo se aplica aos administradores do Workfront (para qualquer grupo).

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Workfront*</td> 
   <td>Qualquer</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Plano </p> <p>Você deve ser um administrador de grupo do grupo ou um administrador do Workfront. Para obter mais informações, consulte <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Administradores de grupo</a> e <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder acesso administrativo total a um usuário</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Exibir acesso ou superior nos modelos que você deseja exibir e trabalhar com</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso aos objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Se precisar descobrir o tipo de plano ou licença, contate o administrador do Workfront.

+++

## Visualize, trabalhe com e crie modelos para seu grupo na área Grupos

{{step-1-to-setup}}

1. No painel esquerdo, clique em **Grupos** ![Grupos](assets/groups-icon.png).

1. Clique no nome do grupo para o qual deseja criar ou modificar modelos.
1. No painel esquerdo, clique em **Modelos** para listar os modelos que estão associados ao grupo e a quaisquer subgrupos que ele possa ter.

   Você deve ter acesso de Visualização a um modelo para vê-lo nesta lista. Para obter informações sobre esse acesso, consulte [Conceder acesso aos modelos](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-templates.md).

1. Siga um destes procedimentos:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Adicionar um modelo</td> 
      <td> <p>Clique em <strong>Novo Modelo</strong> e configure-o usando as opções disponíveis. Para obter informações sobre essas opções, consulte <a href="../../../manage-work/projects/create-and-manage-templates/create-template.md" class="MCXref xref">Criar um modelo de projeto</a>.</p> <p>O template é associado automaticamente ao grupo.</p> <p>Para obter informações sobre como as preferências de grupo se aplicam a novos modelos, consulte <a href="#how-preferences-apply-to-templates-and-template-tasks" class="MCXref xref">Como as preferências se aplicam a modelos e tarefas de modelo</a> neste artigo.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Editar um ou mais modelos</td> 
      <td> <p>Selecione pelo menos um modelo, clique no ícone Editar <img src="assets/edit-icon.png"> e use qualquer uma das opções disponíveis para configurá-lo. Para obter informações sobre essas opções, consulte <a href="../../../manage-work/projects/create-and-manage-templates/edit-templates.md" class="MCXref xref">Editar modelos de projeto</a>.</p> <p>O ícone Editar só estará disponível se você tiver acesso para Editar a todos os modelos selecionados. Para obter informações sobre esse acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-templates.md" class="MCXref xref">Conceder acesso aos modelos</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Excluir um ou mais modelos</td> 
      <td> <p>Selecione pelo menos um modelo e clique no ícone Excluir <img src="assets/delete.png">.</p> <p>Esse ícone só estará disponível se você tiver acesso para Editar a todos os modelos selecionados. Para obter informações sobre esse acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-templates.md" class="MCXref xref">Conceder acesso aos modelos</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Compartilhar um ou mais modelos</td> 
      <td> <p>Selecione pelo menos um modelo, clique no ícone Compartilhar <img src="assets/share-icon.png"> e, em seguida, clique em uma das seguintes opções no menu suspenso:</p> 
       <ul> 
        <li> <p><strong>Modelo</strong>: na caixa <strong>Acesso ao Modelo</strong> que é exibida, adicione nomes para especificar quem você deseja que tenha acesso ao próprio modelo.</p> <p>Para obter mais informações, consulte a seção <a href="../../../manage-work/projects/create-and-manage-templates/share-project-template.md#share" class="MCXref xref">Compartilhar um modelo</a> no artigo <a href="../../../manage-work/projects/create-and-manage-templates/share-project-template.md" class="MCXref xref">Compartilhar modelos de projeto</a>.</p> </li> 
        <li><strong>Projeto</strong>: na caixa <strong>Acesso ao Projeto</strong> que é exibida, adicione nomes para especificar quem você deseja que tenha acesso aos projetos criados a partir do modelo</li> 
       </ul> <p>O ícone Compartilhar só estará disponível se você tiver acesso para Compartilhar a todos os modelos selecionados. Para obter informações sobre esse acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-templates.md" class="MCXref xref">Conceder acesso aos modelos</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Exportar a lista de modelos</td> 
      <td>Clique em <strong>Exportar</strong> <img src="assets/export.png"> e selecione o formato de arquivo desejado para a lista exportada.</td> 
     </tr> 
    </tbody> 
   </table>

## Como as preferências se aplicam a modelos e tarefas de modelo {#how-preferences-apply-to-templates-and-template-tasks}

Ao criar um modelo de projeto, as configurações listadas nas tabelas abaixo são definidas automaticamente por uma preferência de projeto ou tarefa correlacionada.

>[!NOTE]
>
>Uma preferência de projeto ou de tarefa no nível do grupo ou do sistema afeta um modelo de projeto, dependendo se você o associou a um grupo quando o criou.
>
>Se você o associou a um grupo, a preferência de nível de grupo é aplicada. Isso ocorre nos seguintes cenários:
>
>* Crie o template a partir da área Grupos, conforme explicado neste artigo
>* Você especifica um grupo ao criar o modelo usando um arquivo Kickstart
>* Você especifica um grupo ao criar o modelo usando a API
>
>Se você não associou o novo modelo a um grupo, a preferência de nível de sistema entrará em vigor. Isso ocorre quando nos cenários abaixo. (Se, posteriormente, você atribuir um grupo ao modelo ou à tarefa de modelo, as preferências do grupo não o afetarão.)
>
>* Crie o modelo na área Modelos
>* Você não especifica um grupo ao criar o modelo usando um arquivo Kickstart
>* Você não especifica um grupo ao criar o modelo usando a API
>

* [Configurações do modelo de projeto definidas pelas preferências do projeto e da tarefa](#project-template-settings-configured-by-project-and-task-preferences)
* [Configurações do modelo de tarefa definidas pelas preferências da tarefa](#template-task-settings-configured-by-task-preferences)

### Configurações do modelo de projeto definidas pelas preferências do projeto e da tarefa {#project-template-settings-configured-by-project-and-task-preferences}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Método Índice de desempenho</p> </td> 
   <td> <p>Configurado pela preferência de projeto em nível de grupo "Método Índice de desempenho" se você associar o novo modelo a um grupo, ou a mesma preferência de projeto em nível de sistema se você não associar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Tipo de condição</p> </td> 
   <td> <p>Configurado pela preferência de projeto no nível do grupo "Definir automaticamente a condição do projeto com base no status do progresso" se você associar o novo modelo a um grupo, ou a mesma preferência de projeto no nível do sistema se você não associar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Agendar de</p> </td> 
   <td> <p>Configurado pela preferência de projeto em nível de grupo "Agendar de" se você associar o novo modelo a um grupo, ou a mesma preferência de projeto em nível de sistema se você não associar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Tempo de folga do usuário</p> </td> 
   <td> <p>Configurado pela preferência de projeto em nível de grupo "Folga do usuário" se você associar o novo modelo a um grupo, ou pela mesma preferência de projeto em nível de sistema se não associar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Tipo de atualização</p> </td> 
   <td> <p>Configurado pela preferência de projeto no nível do grupo "As linhas do tempo do projeto serão recalculadas automaticamente" se você associar o novo modelo a um grupo, ou a mesma preferência de projeto no nível do sistema se você não associar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Configurações da seção de acesso</p> </td> 
   <td> <p>Configurado pelas preferências da tarefa no nível do grupo na seção "Acesso" se você associar o novo modelo a um grupo, ou a mesma preferência do projeto no nível do sistema se você não associar.</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obter informações sobre as preferências de projeto listadas nesta tabela, consulte [Configurar preferências de projeto do sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

Para obter informações sobre a preferência de tarefas e problemas, consulte [Configurar preferências de tarefas e problemas em todo o sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

>[!NOTE]
>
>* Se você alterar o grupo associado a um modelo de projeto existente, as configurações do modelo permanecerão as mesmas.
>* Se você mover uma tarefa de modelo existente para outro modelo, as seguintes configurações permanecerão inalteradas na tarefa de modelo, independentemente do grupo associado ao novo modelo:>
>   * Tipo de Duração
>   * Tipo de Receita
>   * Tipo de Custo
>
>  No entanto, a tarefa de modelo é afetada pela configuração &quot;Quando alguém é atribuído a uma tarefa&quot; no novo modelo. Para obter mais informações, consulte a seção [Acesso](../../../manage-work/projects/create-and-manage-templates/edit-templates.md#access) no artigo [Editar modelos de projeto](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).
>
>* Quando um administrador salva um projeto como modelo, todas as configurações do modelo são herdadas do projeto, incluindo o grupo.
>
>  Quando um administrador converte uma tarefa ou problema em um projeto usando um modelo, todas as configurações do modelo são determinadas pelo que já está salvo no modelo.
>

### Configurações do modelo de tarefa definidas pelas preferências da tarefa {#template-task-settings-configured-by-task-preferences}

Quando você cria uma tarefa de modelo, algumas de suas configurações são definidas automaticamente por uma preferência de tarefa correlacionada. Essas configurações estão listadas na tabela abaixo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Tipo de Duração </p> </td> 
   <td> <p>Configurado pela preferência de tarefa em nível de grupo "Tipo de duração" se você associar o modelo a um grupo, ou pela mesma preferência de tarefa em nível de sistema e de problema se você não associar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Tipo de Receita</p> </td> 
   <td> <p>Configurado pela preferência de tarefa em nível de grupo "Tipo de Receita" se você associar o modelo a um grupo, ou pela mesma preferência de tarefa em nível de sistema e de ocorrência se você não associar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Tipo de Custo </p> </td> 
   <td> <p> Configurado pela preferência de tarefa em nível de grupo "Tipo de Custo" se você associar o modelo a um grupo, ou pela mesma preferência de tarefa e ocorrência em nível de sistema se você não associar.</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obter informações sobre as preferências de tarefa listadas nesta tabela, consulte [Configurar preferências de tarefas e problemas em todo o sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).
