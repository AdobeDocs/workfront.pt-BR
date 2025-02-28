---
product-area: projects;templates
navigation-topic: manage-projects
title: Salvar um projeto como modelo
description: Salve um projeto como um modeloSalve como modelo" no nível do projeto, para que os usuários vejam isso na interface do usuário do; há outro artigo que esse link aborda com mais detalhes (passo a passo). Essa funcionalidade precisa ficar nas áreas de projetos E modelos.)"
author: Alina
feature: Work Management
exl-id: 4b5dfe12-f984-47c6-8e19-78b549f19159
source-git-commit: f21fd0761d942916039f6364e62f489a07217bfe
workflow-type: tm+mt
source-wordcount: '452'
ht-degree: 1%

---

# Salvar um projeto como modelo

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Keep this the way it is in the Managing Projects area because the functionality in the UI is "Save as template" at the project level, so users see that in the UI; there is another article that this links to which is more in depth (step-by-step). This functionality needs to stay in both projects AND templates areas.)</p>
-->

Se você decidir que um projeto ocorrerá novamente em algum momento no futuro, poderá criar um modelo a partir desse projeto existente. Em seguida, é possível usar o modelo novamente para criar projetos futuros que podem conter informações semelhantes ou compartilhar a mesma linha do tempo ou atribuições com o projeto existente.

## Requisitos de acesso

<!--drafted for P&P:
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
   <td> <p>Current license: Standard </p>
   Or 
   <p>Legacy license: Plan </p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Templates</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View or higher permissions to a project </p> <p>You obtain Manage permissions to the template after you save the project as a template</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront*</td> 
   <td> <p>Qualquer </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Plano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a modelos</p> <p><b>Nota</b>

Se você ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Visualizar ou aumentar as permissões de um projeto </p> <p>Você obtém permissões de Gerenciamento para o modelo depois de salvar o projeto como um modelo</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso aos objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qual plano, tipo de licença ou acesso você tem, contate o administrador do Workfront.

## Salvar um projeto como modelo

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

   ![](assets/save-as-template-first-step-350x159.png)

1. Clique em **Próxima etapa.**
1. Na seção **Opções**, marque a caixa de seleção ao lado de qualquer informação que você deseja apagar do modelo.

   ![](assets/save-as-template-options-step-350x109.png)

1. Clique em **Próxima etapa.**
1. Na seção **Excluir**, selecione as tarefas que deseja excluir do projeto.

   ![](assets/save-as-template-exclude-350x205.png)

1. Clique em **Concluir e Salvar Modelo.**

   Seu modelo agora aparece na lista de modelos disponíveis e pode ser anexado a um projeto existente ou usado para criar um novo.
