---
product-area: templates
navigation-topic: templates-navigation-topic
title: Criar modelo a partir do projeto
description: É possível criar modelos ao salvar um projeto existente como um modelo.
author: Alina
feature: Work Management, Projects
role: User
exl-id: 923deab4-205b-4312-9ec4-4471fd6cea26
source-git-commit: d7600a55b3dffb242957234de9d85a0deb1ad2e3
workflow-type: tm+mt
source-wordcount: '442'
ht-degree: 1%

---

# Criar modelo a partir do projeto

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(Note: Keep this article in the Creating and Managing Templates area with the detailed information that this contains. Since this is an article about creating TEMPLATES, this needs to be detailed under Templates; there is a similar article with almost the same title in Managing projects that points to this one - since this functionality is in the UI under Projects, this article must have a presence in that areas as well. Keep both, but make this one the only editable one (iterative))</p>
-->

É possível criar modelos ao salvar um projeto existente como um modelo.

Depois de salvar um projeto existente como modelo, você pode usar o novo modelo para criar novos projetos. Isso simplifica e agiliza o processo de criação de projetos.

>[!NOTE]
>
>Ao salvar um projeto como modelo, as datas reais das tarefas e do projeto não são salvas para o modelo.
>
>Um modelo e suas tarefas não têm datas reais, mas uma indicação de qual dia (de quando o projeto futuro pode começar) uma tarefa pode começar e em qual dia a tarefa pode precisar ser concluída. Ao usar modelos para criar os projetos futuros, os projetos receberão datas reais. Para obter informações, consulte [Criar um projeto](../create-projects/create-project.md).

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacote do Adobe Workfront</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td><p>Standard</p> 
   <p>Plano</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Editar acesso a modelos</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Visualizar ou aumentar as permissões de um projeto </p> <p>Você obtém permissões de gerenciamento para o modelo após criá-lo</p></td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:
<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Templates</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View or higher permissions to a project </p> <p>You obtain Manage permissions to the template after you create it</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Criar modelo a partir do projeto

1. Vá para o projeto que deseja salvar como modelo.
1. Clique no menu **Mais** ![Ícone Mais](assets/qs-more-icon-on-an-object.png) e **Salvar como Modelo**.
1. Especifique as seguintes informações para o modelo:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Nome</td> 
      <td>Especifique um nome para o modelo.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Descrição</td> 
      <td>Forneça uma descrição para o modelo.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Está ativo</td> 
      <td> <p>Selecione entre as seguintes opções:</p> 
       <ul> 
        <li> <p><strong>Sim</strong>: outros usuários podem encontrar o modelo e anexá-lo aos projetos.</p> </li> 
        <li><strong>Não</strong>: outros usuários não podem encontrar o modelo e não podem anexá-lo a projetos.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Formulários personalizados</td> 
      <td>Use a lista suspensa para selecionar qualquer formulário personalizado para anexar ao modelo. Se algum formulário personalizado já tiver sido associado ao projeto, todos os campos de dados desses formulários personalizados serão exibidos.<br>Você pode incluir até 10 formulários personalizados em um único modelo.</td> 
     </tr> 
    </tbody> 
   </table>

1. Clique em **Gerenciar Forms** para remover ou reordenar os formulários. Para obter informações sobre como remover e reordenar formulários personalizados no modelo, consulte [Formulários personalizados](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-and-manage-custom-forms.md).

   ![Primeira etapa do modelo Salvar como](assets/save-as-template-first-step-350x159.png)

1. Clique em **Próxima etapa.**
1. Na seção **Opções**, marque a caixa de seleção ao lado de qualquer informação que você deseja apagar do modelo.

   ![Salvar como opções de modelo](assets/save-as-template-options-step-350x109.png)

1. Clique em **Próxima etapa.**
1. Na seção **Excluir**, selecione as tarefas que deseja excluir do projeto.

   ![Salvar como exclusão de modelo](assets/save-as-template-exclude-350x205.png)

1. Clique em **Concluir e Salvar Modelo.**

   Seu modelo agora aparece na lista de modelos disponíveis e pode ser anexado a um projeto existente ou usado para criar um novo.

 
