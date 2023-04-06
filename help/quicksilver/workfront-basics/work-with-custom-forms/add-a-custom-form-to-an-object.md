---
product-area: projects;user-management
keywords: anexar,aplicar
navigation-topic: work-with-custom-forms
title: Adicionar um formulário personalizado a um objeto
description: É possível adicionar um formulário personalizado existente a qualquer um dos objetos listados abaixo. Um formulário personalizado contém campos personalizados, onde você pode armazenar informações sobre o objeto.
author: Alina
feature: Get Started with Workfront
exl-id: c06666a7-ab78-4311-8fcb-1d1a68034133
source-git-commit: 78878fa3578e4f3a33baec3806298282d3909d8d
workflow-type: tm+mt
source-wordcount: '850'
ht-degree: 1%

---

# Adicionar um formulário personalizado a um objeto

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available for all customers in the Preview environment and for a select group of customers in the Production environment.</span>-->

É possível adicionar um formulário personalizado existente a qualquer um dos objetos listados abaixo. Um formulário personalizado contém campos personalizados, onde você pode armazenar informações sobre o objeto.

* Projetos (incluindo casos de negócios)
* Tarefas
* Problemas
* Empresas
* Portfólios
* Programas
* Documentos
* Usuários
* Iterações
* Despesas
* Registros de cobrança

É possível adicionar um formulário personalizado somente aos tipos de objetos para os quais o formulário foi criado.

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as ações descritas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plano Adobe Workfront*</td> 
   <td> <p>Qualquer Um </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Solicitação ou superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso aos objetos para os quais você gerencia formulários personalizados</p> <p><b>Nota</b></p>

Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerencie permissões do objeto ao qual deseja anexar um formulário personalizado.</p> <p>Exibir permissões ou permissões superiores ao formulário personalizado, com permissão para <b>Anexar aos dados personalizados</b> objetos (projetos, tarefas e problemas). Para obter mais informações, consulte <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md" class="MCXref xref">Compartilhar um formulário personalizado</a>.</p> <p>Importante: Se você não tiver uma licença do Plano com acesso administrativo ao Forms Personalizado, deverá ter permissões específicas para, pelo menos, visualizar o formulário personalizado, conforme descrito em <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md" class="MCXref xref">Compartilhar um formulário personalizado</a>. Essas permissões devem ser concedidas a você mesmo que o formulário seja visível em todo o sistema. </p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

## Pré-requisito

O administrador do Workfront ou um usuário com uma licença do Plan e acesso administrativo a formulários personalizados deve criar formulários personalizados em seu ambiente antes que você possa adicioná-los a objetos. Para obter mais informações, consulte [Criar ou editar um formulário personalizado](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

## Adicionar um formulário personalizado a um objeto

É possível adicionar um formulário personalizado a um objeto de duas maneiras:

* [Adicionar um formulário personalizado a um objeto editando esse objeto](#add-a-custom-form-to-an-object-by-editing-the-object)
* [Adicionar um formulário personalizado a um objeto a partir da área Detalhes](#add-a-custom-form-to-an-object-from-the-details-area)

### Adicionar um formulário personalizado a um objeto editando esse objeto {#add-a-custom-form-to-an-object-by-editing-the-object}

1. Vá para o objeto ao qual deseja adicionar o formulário personalizado.
1. Clique no botão **Mais** menu ![](assets/more-icon.png), depois clique em **Editar** ![](assets/edit-icon.png).
1. Clique em **Forms personalizada** > **Adicionar Forms**, em seguida, selecione até 10 formulários no menu suspenso.

1. (Opcional) Atualize as informações nos campos editáveis do formulário personalizado.

   Você deve atualizar todos os campos obrigatórios nos formulários adicionados.

1. Clique em **Salvar**.

### Adicionar um formulário personalizado a um objeto a partir da área Detalhes {#add-a-custom-form-to-an-object-from-the-details-area}

1. Vá para o objeto ao qual deseja adicionar o formulário personalizado.
1. Clique no botão **`<Object type>`Detalhes** no painel esquerdo. Por exemplo, clique em **Detalhes do projeto** para adicionar formulários personalizados a um projeto ou **Detalhes do problema** para adicionar formulários personalizados a um problema.
1. Clique no botão **Adicionar formulário personalizado** no canto superior direito, selecione até 10 formulários personalizados na lista exibida.

   Se o formulário contiver qualquer campo obrigatório (marcado com um asterisco vermelho), não será necessário preenchê-los no momento.

   Os formulários selecionados são anexados automaticamente ao objeto.

1. (Opcional) Atualize as informações nos campos personalizados do formulário, em seguida, clique em **Salvar alterações**.

## Vários formulários personalizados em um objeto

É possível adicionar até 10 formulários personalizados em um determinado objeto, permitindo disponibilizar campos para alguns usuários e não para outros, ou permitindo que você atenda melhor aos requisitos de formulário de vários projetos.

**Exemplo:** Se um projeto existente já tiver um formulário personalizado e forem necessários mais campos personalizados que existam em outro formulário personalizado, é possível adicionar um segundo formulário ao projeto com os campos adicionais, em vez de adicionar os campos ao formulário personalizado existente, se esses campos forem necessários apenas para este projeto.

## Adicionar um formulário personalizado a vários objetos em massa

É possível adicionar formulários personalizados a vários objetos selecionando-os em uma lista.

<!--
drafted for bulk-editing projects. When it releases to Prod for projects, take "in the preview environment" and the yellow tags out. Add additional objects here in the same way when they become available:-->

>[!NOTE]
>
>A adição de formulários personalizados a objetos é idêntica para todos os objetos, exceto para projetos.
>
>Para obter informações sobre como adicionar formulários personalizados a projetos em massa, consulte o artigo [Editar projetos](../../manage-work/projects/manage-projects/edit-projects.md).


1. Navegue até uma lista de objetos.
1. Selecione vários objetos na lista.

1. Clique no botão **Mais** menu ![](assets/more-icon.png), em seguida, clique no botão **Editar** ícone  ![](assets/edit-icon.png)ou apenas clique no botão **Editar** ícone ![](assets/edit-icon.png) na parte superior da lista.
1. Clique em **Forms personalizada** no painel esquerdo.
1. Selecione o formulário que deseja associar a todos os objetos selecionados na **Fazer uma seleção** menu suspenso.
   >[!NOTE]
   >
   >Se não for possível localizar o formulário no menu suspenso, significa que pelo menos um dos objetos já possui o formulário associado. Determine qual objeto é e elimine-o de sua seleção antes de adicionar o formulário aos objetos restantes.


1. Clique em **Salvar alterações**.

   Se o formulário contiver qualquer campo obrigatório (marcado com um asterisco vermelho), não será necessário preenchê-los no momento.
