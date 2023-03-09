---
product-area: projects;user-management
navigation-topic: work-with-custom-forms
title: Gerenciar formulários personalizados anexados a objetos
description: Você pode atualizar a ordem na qual os formulários personalizados anexados a um objeto são exibidos, removê-los ou editar em massa a forma como os formulários personalizados são exibidos em vários objetos.
author: Alina
feature: Get Started with Workfront
exl-id: e5570a09-32cb-43e3-9c1d-4421db42fa24
source-git-commit: 23257f11b0795aa1f1e422923f6d596017c58126
workflow-type: tm+mt
source-wordcount: '1120'
ht-degree: 0%

---

# Gerenciar formulários personalizados anexados a objetos

<span class="preview">As informações destacadas nesta página se referem a funcionalidades ainda não disponíveis no geral. Ela está disponível somente no ambiente de Pré-visualização.</span>

Você pode atualizar a ordem na qual os formulários personalizados anexados a um objeto são exibidos, removê-los ou editar em massa a forma como os formulários personalizados são exibidos em vários objetos.

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
   <td> <p>Editar o acesso aos objetos para os quais você gerencia formulários personalizados</p> <p>Observação: se você ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Permissões do Contribute ou superior para os objetos para os quais você gerencia formulários personalizados</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir seu plano, tipo de licença ou acesso, entre em contato com o administrador do Workfront.

## Pré-requisitos

* O administrador do Workfront ou um usuário do plano com acesso administrativo a formulários personalizados deve criar formulários personalizados em seu ambiente. Para obter mais informações, consulte [Criar ou editar um formulário personalizado](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).
* Você deve ter formulários personalizados anexados a um objeto.

   Para obter informações sobre como aplicar formulários personalizados a um objeto, consulte [Adicionar um formulário personalizado a um objeto](../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

## Reordenar vários formulários personalizados anexados a um objeto {#reorder-multiple-custom-forms-attached-to-an-object}

1. Vá para o objeto no qual deseja alterar a ordem dos formulários personalizados adicionados e, em seguida, comece a editar o objeto.

   **Exemplo:** Por exemplo, para gerenciar os formulários personalizados de um projeto, vá para o projeto, clique no link **Mais** menu ![](assets/more-icon.png)e, em seguida, clique em **Editar** .

1. No **Forms personalizado** para projetos, tarefas e problemas, clique no link ![](assets/move-icon---dots.png) ícone ao lado do nome de um formulário personalizado. Para todos os outros objetos, clique em **Gerenciar o Forms**. Essa opção é exibida somente se pelo menos um formulário personalizado estiver anexado ao objeto.
1. Arrastar um formulário ![](assets/move-icon---dots.png) para um novo local na lista.
1. Para projetos, tarefas e problemas, clique em **Salvar**.

   Para todos os outros objetos, clique em **Terminei o gerenciamento** > **Salvar alterações**.

## Remover um formulário personalizado de um objeto {#remove-a-custom-form-from-an-object}

>[!IMPORTANT]
>
>Quando você remove um formulário personalizado de um objeto, todas as informações capturadas nos campos personalizados do formulário são perdidas e não podem ser recuperadas.

1. Vá para o objeto onde deseja remover o formulário personalizado e comece a editar o objeto.

   Por exemplo, vá para um projeto, clique no botão **Mais** menu ![](assets/more-icon.png)e, em seguida, clique em **Editar** .

1. Clique em **Forms personalizado**.
1. Para projetos, tarefas e problemas de formulários personalizados, clique no **X** ícone à direita de um formulário para removê-lo do objeto.

   Para todos os outros objetos, clique em **Gerenciar o Forms** e, em seguida, clique na guia **X** ícone à direita de um formulário para removê-lo do objeto.

1. Clique em **Salvar** .

## Gerenciar vários formulários personalizados que contêm os mesmos campos personalizados

Você pode fazer com que o mesmo campo apareça em vários formulários personalizados anexados ao mesmo objeto. Nesse caso, considere o seguinte:

* O valor do campo é idêntico em todos os formulários.

   Não é possível ter valores diferentes para os mesmos campos em formulários diferentes anexados ao mesmo objeto.

* Se você tiver os mesmos campos calculados em dois objetos diferentes, seus cálculos deverão ser idênticos para evitar erros. Para obter informações sobre como adicionar campos calculados a formulários personalizados, incluindo vários formulários, consulte [Adicionar dados calculados a um formulário personalizado](../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md) .

## Gerenciar vários formulários personalizados ao editar objetos em massa

<!--
drafted for bulk-editing projects. When it releases to Prod for projects, take "in the preview environment" and the yellow tags out. Add additional objects here in the same way when they become available:-->

>[!NOTE]
>
><span class="preview">Para obter informações sobre como gerenciar formulários personalizados em projetos em massa no ambiente de Pré-visualização, consulte o artigo [Editar projetos](../../manage-work/projects/manage-projects/edit-projects.md)</span>.

Ao editar objetos em massa que têm vários formulários personalizados aplicados, você pode editar a forma como os formulários personalizados são exibidos nesses objetos, bem como editar campos comuns entre os formulários personalizados.

Somente os formulários personalizados anexados a todos os objetos selecionados podem ser editados em uma edição em massa.

Para editar vários formulários personalizados ao editar objetos em massa:

1. Em uma lista de objetos, selecione os objetos aos quais os formulários personalizados estão anexados e clique no **Editar** ícone ![](assets/edit-icon.png).
1. Clique em **Forms personalizado**.

   Você pode editar somente os formulários personalizados anexados a todos os objetos selecionados.

   Formulários personalizados anexados somente a alguns dos objetos não são exibidos.

1. Comece a editar campos nos formulários personalizados.

   Quando os campos são editados, um indicador visual é exibido no campo, mostrando que o campo foi editado.

   Se um campo for incluído em mais de um formulário personalizado, todos os valores desses campos serão atualizados em cada formulário quando você atualizar o campo em um dos formulários.

1. Clique em **Faça uma seleção** e selecione formulários adicionais para adicionar a todos os objetos selecionados.

   Considere o seguinte ao aplicar formulários adicionais:

   * Os objetos podem ter até 10 formulários personalizados.
   * Você pode aplicar formulários somente quando o formulário ainda não estiver aplicado a nenhum dos objetos que você está editando. Um formulário que já está anexado a um dos objetos não é exibido no menu suspenso.
   * Depois de aplicar um formulário adicional, todos os campos que o formulário tem em comum com outros formulários são exibidos no **Campos comuns** e eles poderão ser editados.

1. (Opcional) Se você tiver adicionado formulários personalizados a todos os objetos, mas ainda não tiver salvado os objetos, será possível alterar a ordem em que os formulários personalizados aparecem nos objetos.

   Para obter mais informações sobre como alterar a ordem dos formulários, consulte [Reordenar vários formulários personalizados anexados a um objeto](#reorder-multiple-custom-forms-attached-to-an-object) neste artigo.

1. Clique em **Remover Formulário** para remover um formulário personalizado dos objetos.

   Para obter mais informações sobre como remover formulários personalizados de objetos, consulte [Remover um formulário personalizado de um objeto](#remove-a-custom-form-from-an-object).

   Considere o seguinte ao remover formulários em massa de vários objetos:

   * Se você tiver feito alterações no formulário, removê-lo resultará na perda das alterações e elas não poderão ser recuperadas.
   * Após remover um formulário, todos os campos desse formulário que estavam na **Campos comuns** são removidas desta seção e não podem mais ser editadas aqui.

1. Clique em **Restaurar Formulário** para restaurar o formulário ao estado em que estava antes de você editar os objetos.
1. (Opcional) Clique na seta de recolhimento ao lado do nome do formulário para recolher um formulário de cada vez.

   Ou

   Clique em **Recolher o Forms** para recolher todos os formulários ao mesmo tempo.

1. (Opcional) Clique na seta de expansão ao lado do nome do formulário para expandir um formulário de cada vez.

   Ou

   Clique em **Expandir Forms** para expandir todos os formulários ao mesmo tempo. 

1. Clique em **Salvar alterações**.
