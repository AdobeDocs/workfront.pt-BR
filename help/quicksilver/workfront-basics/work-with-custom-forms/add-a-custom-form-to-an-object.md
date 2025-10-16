---
product-area: projects;user-management
keywords: anexar,aplicar
navigation-topic: work-with-custom-forms
title: Adicionar um formulário personalizado a um objeto
description: Você pode adicionar um formulário personalizado existente a qualquer um dos objetos listados abaixo. Um formulário personalizado contém campos personalizados onde você pode armazenar informações sobre o objeto.
author: Alina
feature: Get Started with Workfront
exl-id: c06666a7-ab78-4311-8fcb-1d1a68034133
source-git-commit: 4ef71db5d93e314b746e8acdbf90fd041c6e71ae
workflow-type: tm+mt
source-wordcount: '730'
ht-degree: 2%

---

# Adicionar um formulário personalizado a um objeto

<!--Audited: 12/2023-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available for all customers in the Preview environment and for a select group of customers in the Production environment.</span>-->

Você pode adicionar um formulário personalizado existente a qualquer um dos objetos listados abaixo. Um formulário personalizado contém campos personalizados onde você pode armazenar informações sobre o objeto.

* Projetos (incluindo casos de negócios)
* Tarefas
* Problemas
* Empresas
* Portfólios
* Programas
* Documentos
* Usuários
* Grupos
* Iterações
* Despesas
* Registros de cobrança

Você pode adicionar um formulário personalizado somente aos tipos de objetos para os quais o formulário foi criado.

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
  <td> <p>Colaborador ou superior</p>
 <p>Solicitação ou superior</p> 
</td> 
 </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Editar o acesso aos objetos para os quais você gerencia formulários personalizados</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerencie permissões para o objeto ao qual você deseja anexar um formulário personalizado.</p> <p>Exiba ou aumente as permissões do formulário personalizado, com permissão para <b>Anexar a objetos de Dados Personalizados</b> (projetos, tarefas e problemas).</td> 
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
   <td> <p>Any </p> </td> 
  </tr> 
<tr> 
  <td role="rowheader">Adobe Workfront license</td> 
  <td> <p>New: Contributor or higher </p>
 <p>or</p> 
<p>Current: Request or higher </p> 
</td> 
 </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to the objects for which you manage custom forms</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the object for which you want to attach a custom form.</p> <p>View or higher permissions to the custom form, with permission to <b>Attach to Custom Data</b> objects (projects, tasks, and issues). For more information, see <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md" class="MCXref xref">Share a custom form</a>.</p> <p>Important: If you do not have a Plan license with administrative access to&nbsp;Custom&nbsp;Forms, you must have specific permissions to at least view the custom form, as described in <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md" class="MCXref xref">Share a custom form</a>. These permissions must be granted to you even if the form is visible system-wide. </p> <p>For information on requesting additional access, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Pré-requisitos

O administrador do Workfront ou um usuário com uma licença de Plano e acesso administrativo a formulários personalizados deve criar formulários personalizados em seu ambiente antes que você possa adicioná-los aos objetos. Para obter mais informações, consulte [Criar um formulário personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

## Adicionar um formulário personalizado a um objeto

Você pode adicionar um formulário personalizado a um objeto de duas maneiras:

* [Adicione um formulário personalizado a um objeto editando o objeto](#add-a-custom-form-to-an-object-by-editing-the-object)
* [Adicionar um formulário personalizado a um objeto da área Detalhes](#add-a-custom-form-to-an-object-from-the-details-area)

### Adicionar um formulário personalizado a um objeto ao editar o objeto {#add-a-custom-form-to-an-object-by-editing-the-object}

1. Vá para o objeto ao qual deseja adicionar o formulário personalizado.
1. Clique no menu **Mais** ![](assets/more-icon.png) e em **Editar** ![](assets/edit-icon.png).
1. Clique em **Forms Personalizado** > **Adicionar Forms** e selecione até 10 formulários no menu suspenso.

1. (Opcional) Atualize as informações nos campos editáveis no formulário personalizado.

   É necessário atualizar todos os campos obrigatórios nos formulários adicionados.

1. Clique em **Salvar**.

### Adicionar um formulário personalizado a um objeto da área Detalhes {#add-a-custom-form-to-an-object-from-the-details-area}

1. Vá para o objeto ao qual deseja adicionar o formulário personalizado.
1. Clique na seção **`<Object type>`Detalhes** no painel esquerdo. Por exemplo, clique em **Detalhes do Projeto** para adicionar formulários personalizados a um projeto ou em **Detalhes do Problema** para adicionar formulários personalizados a um problema.
1. Clique no campo **Adicionar formulário personalizado** no canto superior direito e selecione até 10 formulários personalizados na lista a ser exibida.

   Se o formulário contiver campos obrigatórios (marcados com um asterisco vermelho), não é necessário preenchê-los neste momento.

   Os formulários selecionados são anexados automaticamente ao objeto.

1. (Opcional) Atualize as informações nos campos personalizados do formulário e clique em **Salvar alterações**.

## Vários formulários personalizados em um objeto

Você pode adicionar até 10 formulários personalizados em um determinado objeto, o que permite disponibilizar campos para alguns usuários e não para outros, ou permitir que você atenda melhor aos requisitos de formulário de vários projetos.

**Exemplo:** Se um projeto existente já tiver um formulário personalizado, e mais campos personalizados forem necessários para esse projeto, que existe em outro formulário personalizado, você poderá adicionar um segundo formulário ao projeto com os campos adicionais, em vez de adicionar os campos ao formulário personalizado existente.

## Adicionar um formulário personalizado a vários objetos em massa

Você pode adicionar formulários personalizados a vários objetos selecionando-os em uma lista.

<!--
drafted for bulk-editing projects. When it releases to Prod for projects, take "in the preview environment" and the yellow tags out. Add additional objects here in the same way when they become available:-->

>[!NOTE]
>
>A adição de formulários personalizados a objetos é idêntica para todos os objetos, exceto para projetos.
>
>Para obter informações sobre como adicionar formulários personalizados a projetos em massa, consulte o artigo [Editar projetos](../../manage-work/projects/manage-projects/edit-projects.md).


1. Navegue até uma lista de objetos.
1. Selecione vários objetos na lista.

1. Clique no menu **&#x200B;**&#x200B;Mais![](assets/more-icon.png) e no ícone **&#x200B;**&#x200B;Editar![](assets/edit-icon.png).

   Ou

   Clique no ícone **de** Editar![](assets/edit-icon.png) na parte superior da lista.
1. Clique em **Forms Personalizado** no painel esquerdo.
1. no menu suspenso **Fazer uma seleção**, selecione o formulário que deseja associar a todos os objetos selecionados.

   >[!NOTE]
   >
   >Se não for possível encontrar o formulário no menu suspenso, significa que pelo menos um dos objetos já tem o formulário associado a ele. Determine qual objeto é e elimine-o da seleção antes de adicionar o formulário aos objetos restantes.


1. Clique em **Salvar alterações**.

   Se o formulário contiver campos obrigatórios (marcados com um asterisco vermelho), não é necessário preenchê-los neste momento.
