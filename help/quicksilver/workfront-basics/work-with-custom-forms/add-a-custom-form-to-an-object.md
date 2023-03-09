---
product-area: projects;user-management
keywords: anexar,aplicar
navigation-topic: work-with-custom-forms
title: Adicionar um formulário personalizado a um objeto
description: Você pode adicionar um formulário personalizado existente a qualquer um dos objetos listados abaixo. Um formulário personalizado contém campos personalizados onde você pode armazenar informações sobre o objeto.
author: Alina
feature: Get Started with Workfront
exl-id: c06666a7-ab78-4311-8fcb-1d1a68034133
source-git-commit: 23257f11b0795aa1f1e422923f6d596017c58126
workflow-type: tm+mt
source-wordcount: '856'
ht-degree: 1%

---

# Adicionar um formulário personalizado a um objeto

<span class="preview">As informações destacadas nesta página se referem a funcionalidades ainda não disponíveis no geral. Ela está disponível somente no ambiente de Pré-visualização.</span>

Você pode adicionar um formulário personalizado existente a qualquer um dos objetos listados abaixo. Um formulário personalizado contém campos personalizados onde você pode armazenar informações sobre o objeto.

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

Você pode adicionar um formulário personalizado somente aos tipos de objetos para os quais o formulário foi criado.

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as ações descritas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront*</td> 
   <td> <p>Qualquer Um </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Solicitação ou superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar o acesso aos objetos para os quais você gerencia formulários personalizados</p> <p><b>Nota</b></p>

Se você ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerencie permissões para o objeto ao qual você deseja anexar um formulário personalizado.</p> <p>Exibir permissões ou mais altas para o formulário personalizado, com permissão para <b>Anexar aos dados personalizados</b> objetos (projetos, tarefas e problemas). Para obter mais informações, consulte <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md" class="MCXref xref">Compartilhar um formulário personalizado</a>.</p> <p>Importante: se você não tiver uma licença de Plano com acesso administrativo ao Forms Personalizado, deverá ter permissões específicas para pelo menos exibir o formulário personalizado, conforme descrito em <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md" class="MCXref xref">Compartilhar um formulário personalizado</a>. Essas permissões devem ser concedidas a você mesmo se o formulário estiver visível em todo o sistema. </p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir seu plano, tipo de licença ou acesso, entre em contato com o administrador do Workfront.

## Pré-requisito

O administrador do Workfront ou um usuário com uma licença de Plano e acesso administrativo a formulários personalizados deve criar formulários personalizados em seu ambiente antes que você possa adicioná-los aos objetos. Para obter mais informações, consulte [Criar ou editar um formulário personalizado](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

## Adicionar um formulário personalizado a um objeto

Você pode adicionar um formulário personalizado a um objeto de duas maneiras:

* [Adicionar um formulário personalizado a um objeto ao editar o objeto](#add-a-custom-form-to-an-object-by-editing-the-object)
* [Adicionar um formulário personalizado a um objeto da área Detalhes](#add-a-custom-form-to-an-object-from-the-details-area)

### Adicionar um formulário personalizado a um objeto ao editar o objeto {#add-a-custom-form-to-an-object-by-editing-the-object}

1. Vá para o objeto ao qual deseja adicionar o formulário personalizado.
1. Clique em **Mais** menu ![](assets/more-icon.png)e, em seguida, clique em **Editar** ![](assets/edit-icon.png).
1. Clique em **Forms personalizado** > **Adicionar o Forms**, selecione até 10 formulários no menu suspenso.

1. (Opcional) Atualize as informações nos campos editáveis no formulário personalizado.

   É necessário atualizar todos os campos obrigatórios nos formulários adicionados.

1. Clique em **Salvar**.

### Adicionar um formulário personalizado a um objeto da área Detalhes {#add-a-custom-form-to-an-object-from-the-details-area}

1. Vá para o objeto ao qual deseja adicionar o formulário personalizado.
1. Clique em **`<Object type>`Detalhes** no painel esquerdo. Por exemplo, clique **Detalhes do projeto** para adicionar formulários personalizados a um projeto ou **Detalhes do problema** para adicionar formulários personalizados a um problema.
1. Clique em **Adicionar formulário personalizado** no canto superior direito e selecione até 10 formulários personalizados na lista exibida.

   Se o formulário contiver campos obrigatórios (marcados com um asterisco vermelho), não é necessário preenchê-los neste momento.

   Os formulários selecionados são anexados automaticamente ao objeto.

1. (Opcional) Atualize as informações nos campos personalizados do formulário e clique em **Salvar alterações**.

## Vários formulários personalizados em um objeto

Você pode adicionar até 10 formulários personalizados em um determinado objeto, o que permite disponibilizar campos para alguns usuários e não para outros, ou permitir que você atenda melhor aos requisitos de formulário de vários projetos.

**Exemplo:** Se um projeto existente já tiver um formulário personalizado e mais campos personalizados forem necessários que existam em outro formulário personalizado, você poderá adicionar um segundo formulário ao projeto com os campos adicionais, em vez de adicionar os campos ao formulário personalizado existente, se esses campos forem necessários apenas para este projeto.

## Adicionar um formulário personalizado a vários objetos em massa

Você pode adicionar formulários personalizados a vários objetos selecionando-os em uma lista.

<!--
drafted for bulk-editing projects. When it releases to Prod for projects, take "in the preview environment" and the yellow tags out. Add additional objects here in the same way when they become available:-->

>[!NOTE]
>
><span class="preview">Para obter informações sobre como adicionar formulários personalizados a projetos em massa no ambiente de Pré-visualização, consulte o artigo [Editar projetos](../../manage-work/projects/manage-projects/edit-projects.md)</span>.

—>

1. Navegue até uma lista de objetos.
1. Selecione vários objetos na lista.

1. Clique em **Mais** menu ![](assets/more-icon.png)e, em seguida, clique na guia **Editar** ícone  ![](assets/edit-icon.png)ou apenas clique no link **Editar** ícone ![](assets/edit-icon.png).
1. Clique em **Forms personalizado** no painel esquerdo.
1. Selecione o formulário que deseja associar a todos os objetos selecionados na **Faça uma seleção** menu suspenso.
   >[!NOTE]
   >
   >Se não for possível encontrar o formulário no menu suspenso, significa que pelo menos um dos objetos já tem o formulário associado a ele. Determine qual objeto é e elimine-o da seleção antes de adicionar o formulário aos objetos restantes.

1. Clique em **Salvar alterações**.

   Se o formulário contiver campos obrigatórios (marcados com um asterisco vermelho), não é necessário preenchê-los neste momento.
