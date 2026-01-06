---
product-area: projects
navigation-topic: update-work-in-a-project
title: Atualizar condição de um projeto
description: A Condição de um projeto é um sinalizador colocado nele para indicar se o trabalho associado a ele está indo bem ou se você encontrou algum obstáculo. Isso é diferente do Status do projeto, que indica se você está trabalhando nele ativamente ou não.
author: Alina
feature: Work Management
exl-id: 1f46386e-e1ae-4845-8cc4-09dd7d39076f
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '526'
ht-degree: 3%

---

# Atualizar condição de um projeto

A Condição de um projeto é um sinalizador colocado nele para indicar se o trabalho associado a ele está indo bem ou se você encontrou algum obstáculo. Isso é diferente do Status do projeto, que indica se você está trabalhando nele ativamente ou não.

Você pode definir a Condição de um projeto automática ou manualmente. Para alterar a Condição de um projeto manualmente, você deve ser o Proprietário do projeto ou ter direitos de Gerenciamento.

O administrador do Adobe Workfront pode criar Condições personalizadas para o seu ambiente, conforme descrito em [Criar ou editar uma condição personalizada](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md).

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacote do Adobe Workfront</td> 
   <td><p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td> 
  <p>Padrão</p>
   <p>Plano</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Exibir ou aumentar o acesso aos projetos</p> <p>Editar acesso a tarefas e problemas </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Exiba permissões ou mais altas em tarefas e problemas para exibir sua Condição</p>
   <p>Gerenciar permissões em tarefas e problemas para atualizar a Condição</p>
     </td> 
  </tr> 
 </tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td><p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> 
   
   For the new licenses:
  <p>Standard</p>
   
   For current licenses:
   <ul><li><p>Plan</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>View or higher access to projects</p> <p>Edit access to tasks and issues </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View or higher permissions on tasks and issues to view their Condition</p>
   <p>Manage permissions on tasks and issues to update the Condition</p>
     </td> 
  </tr> 
 </tbody> 
</table>-->

## Definir automaticamente a Condição

A configuração automática da Condição de um projeto é determinada pelo Tipo de Condição do projeto. O tipo de condição deve ser definido como Status de progresso para que o Workfront defina automaticamente a condição do projeto.

O administrador de Workfront ou de grupo determina o padrão do campo Tipo de condição para novos projetos no sistema ao definir as preferências do projeto na área Configuração. Para obter mais informações, consulte [Configurar preferências de projeto do sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

Ao criar um projeto, a Condição do projeto é automaticamente definida para corresponder ao Status de progresso do projeto nesse momento. O Status de Progresso do projeto é baseado no progresso das tarefas no projeto.

Para obter informações sobre as condições do projeto e como elas são calculadas com base no Status de Progresso, consulte [Visão geral do Status de Progresso do Projeto](../../../manage-work/projects/planning-a-project/project-progress-status.md).

## Atualizar manualmente a Condição de um projeto

Se você definir o Tipo de condição do seu projeto como Manual em vez de Status de progresso, poderá atualizar manualmente a Condição de um projeto.

1. Vá para o projeto para o qual deseja atualizar a Condição.
1. Clique na seção **Detalhes do projeto** no painel esquerdo.

1. Verifique se o campo **Tipo de Condição** está definido como **Manual**.

   ![](assets/project-details-overview-select-condition.png)

1. No campo **Condição**, selecione entre as seguintes opções aquela que corresponde à sua compreensão de se o trabalho associado a ele está indo bem ou se há atrasos:

   * **No Destino**
   * **Em Risco**
   * **Com Problemas**

   Para obter mais informações sobre as condições do projeto, consulte [Visão Geral da Condição do Projeto e do Tipo de Condição](../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md).

   >[!NOTE]
   >
   >As condições podem ser personalizadas para seu ambiente, portanto, você pode encontrar mais de três opções de Condição em seu ambiente. Os nomes das Condições podem ser diferentes dos listados acima. Para obter informações sobre como personalizar Condições no Workfront, consulte [Criar ou editar uma condição personalizada](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md).

1. Clique em **Salvar alterações**.
