---
product-area: projects;user-management
navigation-topic: work-with-custom-forms
title: Gerenciar formulários personalizados anexados a objetos
description: Você pode atualizar a ordem na qual os formulários personalizados anexados a um objeto são exibidos, removê-los ou editar em massa a forma como os formulários personalizados são exibidos em vários objetos.
author: Alina
feature: Get Started with Workfront
exl-id: e5570a09-32cb-43e3-9c1d-4421db42fa24
source-git-commit: eacc6b26bd30ac7da363c6aa1d759a65a20cd9f4
workflow-type: tm+mt
source-wordcount: '1054'
ht-degree: 0%

---

# Gerenciar formulários personalizados anexados a objetos

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available for all customers in the Preview environment and for a select group of customers in the Production environment.</span>-->

Você pode atualizar a ordem na qual os formulários personalizados anexados a um objeto são exibidos, removê-los ou editar em massa a forma como os formulários personalizados são exibidos em vários objetos.

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as ações descritas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront</td> 
   <td> <p>Qualquer </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td> <p>Solicitação ou superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Editar o acesso aos objetos para os quais você gerencia formulários personalizados</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Permissões do Contribute ou superior para os objetos para os quais você gerencia formulários personalizados</p>  </td> 
  </tr> 
 </tbody> 
</table>

*Para obter mais informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Pré-requisitos

* O administrador do Workfront ou um usuário do plano com acesso administrativo a formulários personalizados deve criar formulários personalizados em seu ambiente. Para obter mais informações, consulte [Criar um formulário personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).
* Você deve ter formulários personalizados anexados a um objeto.

  Para obter informações sobre como aplicar formulários personalizados a um objeto, consulte [Adicionar um formulário personalizado a um objeto](../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

## Reordenar vários formulários personalizados anexados a um objeto {#reorder-multiple-custom-forms-attached-to-an-object}

1. Vá para o objeto no qual deseja alterar a ordem dos formulários personalizados adicionados e, em seguida, comece a editar o objeto.

   **Exemplo:** Por exemplo, para gerenciar os formulários personalizados de um projeto, vá para o projeto, clique no menu **&#x200B;**&#x200B;Mais![](assets/more-icon.png) e clique em **Editar**.

1. Na seção **Forms personalizado** para projetos, tarefas e problemas, clique no ícone ![](assets/move-icon---dots.png) ao lado do nome de um formulário personalizado. Para todos os outros objetos, clique em **Gerenciar Forms**. Essa opção é exibida somente se pelo menos um formulário personalizado estiver anexado ao objeto.
1. Arraste um formulário ![](assets/move-icon---dots.png) para um novo local na lista.
1. Para projetos, tarefas e formulários personalizados de problemas, clique em **Salvar**.

   Para todos os outros objetos, clique em **Terminei o gerenciamento** > **Salvar alterações**.

## Remover um formulário personalizado de um objeto {#remove-a-custom-form-from-an-object}

>[!IMPORTANT]
>
>Quando você remove um formulário personalizado de um objeto, todas as informações capturadas nos campos personalizados do formulário são perdidas e não podem ser recuperadas.

1. Vá para o objeto onde deseja remover o formulário personalizado e clique na seção **Detalhes** no painel esquerdo do objeto.

   Por exemplo, vá para um projeto, clique na seção **Detalhes do projeto**.

1. Clique no ícone **Editar** ![Ícone Editar](assets/edit-icon.png) no canto superior direito da página do objeto e clique em **Editar tudo**.
1. Clique no ícone **Excluir** ![](assets/delete-icon.png) à direita de um nome de formulário personalizado e clique em **Excluir** para confirmar e remover o formulário do objeto ou em **Cancelar** para impedir a remoção.
1. Clique em **Salvar alterações**.

## Gerenciar vários formulários personalizados que contêm os mesmos campos personalizados

Você pode fazer com que o mesmo campo apareça em vários formulários personalizados anexados ao mesmo objeto. Nesse caso, considere o seguinte:

* O valor do campo é idêntico em todos os formulários.

  Não é possível ter valores diferentes para os mesmos campos em formulários diferentes anexados ao mesmo objeto.

* Se você tiver os mesmos campos calculados em dois objetos diferentes, seus cálculos deverão ser idênticos para evitar erros. Para obter informações sobre como adicionar campos calculados a formulários personalizados, incluindo vários formulários, consulte [Adicionar campos calculados a um formulário](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md).

## Gerenciar vários formulários personalizados ao editar objetos em massa

<!--
drafted for bulk-editing projects. When it releases to Prod for projects, take "in the preview environment" and the yellow tags out. Add additional objects here in the same way when they become available:-->

>[!NOTE]
>
>O gerenciamento de formulários personalizados para objetos é idêntico para todos os objetos, exceto para projetos.
>
>Para obter informações sobre como adicionar formulários personalizados a projetos em massa, consulte o artigo [Editar projetos](../../manage-work/projects/manage-projects/edit-projects.md).

Ao editar objetos em massa que têm vários formulários personalizados aplicados, você pode editar a forma como os formulários personalizados são exibidos nesses objetos, bem como editar campos comuns entre os formulários personalizados.

Somente os formulários personalizados anexados a todos os objetos selecionados podem ser editados em uma edição em massa.

Para editar vários formulários personalizados ao editar objetos em massa:

1. Em uma lista de objetos, selecione os objetos aos quais os formulários personalizados estão anexados e clique no ícone **Editar** ![](assets/edit-icon.png).
1. Clique em **Forms Personalizado**.

   Você pode editar somente os formulários personalizados anexados a todos os objetos selecionados.

   Formulários personalizados anexados somente a alguns dos objetos não são exibidos.

1. Comece a editar campos nos formulários personalizados.

   Quando os campos são editados, um indicador visual é exibido no campo, mostrando que o campo foi editado.

   Se um campo for incluído em mais de um formulário personalizado, todos os valores desses campos serão atualizados em cada formulário quando você atualizar o campo em um dos formulários.

1. Clique no menu suspenso **Fazer uma seleção** e selecione formulários adicionais para adicionar a todos os objetos selecionados.

   Considere o seguinte ao aplicar formulários adicionais:

   * Os objetos podem ter até 10 formulários personalizados.
   * Você pode aplicar formulários somente quando o formulário ainda não estiver aplicado a nenhum dos objetos que você está editando. Um formulário que já está anexado a um dos objetos não é exibido no menu suspenso.
   * Depois de aplicar um formulário adicional, todos os campos que o formulário tem em comum com outros formulários são exibidos na seção **Campos Comuns** e podem ser editados.

1. (Opcional) Se você tiver adicionado formulários personalizados a todos os objetos, mas ainda não tiver salvado os objetos, será possível alterar a ordem em que os formulários personalizados aparecem nos objetos.

   Para obter mais informações sobre como alterar a ordem dos formulários, consulte [Reordenar vários formulários personalizados anexados a um objeto](#reorder-multiple-custom-forms-attached-to-an-object) neste artigo.

1. Clique em **Remover Formulário** para remover um formulário personalizado dos objetos.

   Para obter mais informações sobre como remover formulários personalizados de objetos, consulte [Remover um formulário personalizado de um objeto](#remove-a-custom-form-from-an-object).

   Considere o seguinte ao remover formulários em massa de vários objetos:

   * Se você tiver feito alterações no formulário, removê-lo resultará na perda das alterações e elas não poderão ser recuperadas.
   * Após remover um formulário, todos os campos desse formulário que estavam na seção **Campos Comuns** serão removidos desta seção e não poderão mais ser editados aqui.

1. Clique em **Restaurar formulário** para restaurar o formulário ao estado em que estava antes de editar os objetos.
1. (Opcional) Clique na seta de recolhimento ao lado do nome do formulário para recolher um formulário de cada vez.

   Ou

   Clique em **Recolher Forms** para recolher todos os formulários ao mesmo tempo.

1. (Opcional) Clique na seta de expansão ao lado do nome do formulário para expandir um formulário de cada vez.

   Ou

   Clique em **Expandir Forms** para expandir todos os formulários ao mesmo tempo. 

1. Clique em **Salvar alterações**.
