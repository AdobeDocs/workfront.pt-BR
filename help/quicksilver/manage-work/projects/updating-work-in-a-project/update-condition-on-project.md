---
product-area: projects
navigation-topic: update-work-in-a-project
title: Atualizar condição de um projeto
description: A Condição de um projeto é um sinalizador colocado nele para indicar se o trabalho associado a ele está indo bem ou se você encontrou algum bloqueio de estradas. Isso é diferente do Status do projeto, que indica se você está trabalhando ativamente nele ou não.
author: Alina
feature: Work Management
exl-id: 1f46386e-e1ae-4845-8cc4-09dd7d39076f
source-git-commit: dc3461803e23f61877c31efa2c52fffdc7bd79bf
workflow-type: tm+mt
source-wordcount: '557'
ht-degree: 1%

---

# Atualizar condição de um projeto

A Condição de um projeto é um sinalizador colocado nele para indicar se o trabalho associado a ele está indo bem ou se você encontrou algum bloqueio de estradas. Isso é diferente do Status do projeto, que indica se você está trabalhando ativamente nele ou não.

Você pode definir a Condição de um projeto automática ou manualmente. Para alterar a Condição de um projeto manualmente, você deve ser o Proprietário do projeto ou ter direitos de Gerenciar para ele.

O administrador do Adobe Workfront pode criar Condições personalizadas para o seu ambiente, conforme descrito em [Criar ou editar uma condição personalizada](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md).

## Requisitos de acesso

<!--drafted for P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td><p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> 
   
   For the current licenses:
  <p>Standard</p>
   
   For legacy licenses:
   <ul><li><p>Plan</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>View or higher access to projects</p> <p>Edit access to tasks and issues </p> <p><b>NOTE</b> 
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View or higher permissions on tasks and issues to view their Condition</p>
   <p>Manage permissions on tasks and issues to update the Condition</p>
    <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plano Adobe Workfront*</td> 
   <td> <p>Qualquer Um</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Plano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a Projetos</p> <p><b>Nota</b>

Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões do projeto</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

## Definir automaticamente a condição

A configuração automática da Condição de um projeto é determinada pelo Tipo de condição do projeto. O Tipo de condição deve ser definido como Status de progresso para Workfront para definir automaticamente a Condição do projeto.

O administrador do Workfront ou do Grupo determina o padrão do campo Tipo de Condição para novos projetos no sistema ao definir as preferências do projeto na área Configuração. Para obter mais informações, consulte [Configurar preferências de projeto em todo o sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

Ao criar um projeto, a Condição do projeto é automaticamente definida para corresponder ao Status de Andamento do projeto no momento. O Status de Progresso do projeto baseia-se no progresso das tarefas no projeto.

Para obter informações sobre as condições do projeto e como elas são calculadas com base no Status de Andamento, consulte [Visão geral do status de progresso do projeto](../../../manage-work/projects/planning-a-project/project-progress-status.md).

## Atualizar manualmente a condição de um projeto

Se você definir o Tipo de condição do projeto como Manual em vez de Status de progresso, poderá atualizar manualmente a Condição de um projeto.

1. Vá para o projeto para o qual deseja atualizar a Condição.
1. Clique no botão **Detalhes do projeto** seção.

   ![](assets/project-details-overview-edit-enabled-with-condition-shot-nwe-350x251.png)

1. Certifique-se de que **Tipo de condição** estiver definido como **Manual**.

1. No **Condição** , selecione entre as seguintes opções a opção que corresponda à sua compreensão de que o trabalho associado está funcionando sem problemas ou se há atrasos:

   * **No Prazo**
   * **Em Risco**
   * **Com problemas**

   Para obter mais informações sobre as condições do projeto, consulte [Visão geral da condição do projeto e do tipo de condição](../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md).

   >[!NOTE]
   >
   >As condições podem ser personalizadas para o seu ambiente, portanto, você pode encontrar mais de três opções para Condição no seu ambiente. Os nomes das Condições podem ser diferentes dos acima enumerados. Para obter informações sobre como personalizar Condições no Workfront, consulte [Criar ou editar uma condição personalizada](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md).

1. Clique em **Salvar**.Click **Salvar alterações**.
