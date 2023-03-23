---
product-area: projects;user-management
navigation-topic: work-with-custom-forms
title: Gerenciar formulários personalizados anexados a objetos
description: É possível atualizar a ordem em que os formulários personalizados anexados a um objeto são exibidos, removê-los ou editar em massa a forma como os formulários personalizados são exibidos em vários objetos.
author: Alina
feature: Get Started with Workfront
exl-id: e5570a09-32cb-43e3-9c1d-4421db42fa24
source-git-commit: addcff71ff067be22e9ee80f997af545293fa5db
workflow-type: tm+mt
source-wordcount: '1133'
ht-degree: 0%

---

# Gerenciar formulários personalizados anexados a objetos

<span class="preview">As informações destacadas nesta página se referem à funcionalidade ainda não disponível no geral. Ele está disponível para todos os clientes no ambiente de Visualização e para um grupo selecionado de clientes no ambiente de Produção.</span>

É possível atualizar a ordem em que os formulários personalizados anexados a um objeto são exibidos, removê-los ou editar em massa a forma como os formulários personalizados são exibidos em vários objetos.

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
   <td> <p>Editar acesso aos objetos para os quais você gerencia formulários personalizados</p> <p>Observação: Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Permissões de contribuição ou superior aos objetos para os quais você gerencia formulários personalizados</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

## Pré-requisitos

* O administrador do Workfront ou um usuário do Plan com acesso administrativo a formulários personalizados deve criar formulários personalizados em seu ambiente. Para obter mais informações, consulte [Criar ou editar um formulário personalizado](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).
* É necessário ter formulários personalizados anexados a um objeto.

   Para obter informações sobre como aplicar formulários personalizados a um objeto, consulte [Adicionar um formulário personalizado a um objeto](../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

## Reordenar vários formulários personalizados anexados a um objeto {#reorder-multiple-custom-forms-attached-to-an-object}

1. Vá para o objeto em que deseja alterar a ordem dos formulários personalizados adicionados e comece a editar o objeto.

   **Exemplo:** Por exemplo, para gerenciar os formulários personalizados de um projeto, vá para o projeto, clique no link **Mais** menu ![](assets/more-icon.png), depois clique em **Editar** .

1. No **Forms personalizada** para projetos, tarefas e problemas, clique no botão ![](assets/move-icon---dots.png) ícone ao lado do nome de um formulário personalizado. Para todos os outros objetos, clique em **Gerenciar o Forms**. Essa opção é exibida somente se pelo menos um formulário personalizado estiver anexado ao objeto.
1. Arrastar um formulário ![](assets/move-icon---dots.png) para um novo local na lista.
1. Para projetos, tarefas e problemas de formulários personalizados, clique em **Salvar**.

   Para todos os outros objetos, clique em **Estou farto de gerenciar** > **Salvar alterações**.

## Remover um formulário personalizado de um objeto {#remove-a-custom-form-from-an-object}

>[!IMPORTANT]
>
>Quando um formulário personalizado é removido de um objeto, todas as informações capturadas nos campos personalizados do formulário são perdidas e não podem ser recuperadas.

1. Vá para o objeto onde deseja remover o formulário personalizado e comece a editar o objeto.

   Por exemplo, vá para um projeto, clique no botão **Mais** menu ![](assets/more-icon.png), depois clique em **Editar** .

1. Clique em **Forms personalizada**.
1. Para projetos, tarefas e problemas de formulários personalizados, clique no botão **X** à direita de um formulário para removê-lo do objeto.

   Para todos os outros objetos, clique em **Gerenciar o Forms**, em seguida, clique no botão **X** à direita de um formulário para removê-lo do objeto.

1. Clique em **Salvar** .

## Gerenciar vários formulários personalizados que contêm os mesmos campos personalizados

O mesmo campo pode ser exibido em vários formulários personalizados anexados ao mesmo objeto. Nesse caso, considere o seguinte:

* O valor do campo é idêntico em todos os formulários.

   Não é possível ter valores diferentes para os mesmos campos em formulários diferentes anexados ao mesmo objeto.

* Se você tiver os mesmos campos calculados em dois objetos diferentes, seus cálculos deverão ser idênticos para evitar erros. Para obter informações sobre como adicionar campos calculados a formulários personalizados, incluindo vários formulários, consulte [Adicionar dados calculados a um formulário personalizado](../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md) .

## Gerenciar vários formulários personalizados ao editar objetos em massa

<!--
drafted for bulk-editing projects. When it releases to Prod for projects, take "in the preview environment" and the yellow tags out. Add additional objects here in the same way when they become available:-->

>[!NOTE]
>
><span class="preview">Para obter informações sobre como gerenciar formulários personalizados em projetos em massa no ambiente de Visualização, consulte o artigo [Editar projetos](../../manage-work/projects/manage-projects/edit-projects.md)</span>.

Quando objetos de edição em massa com vários formulários personalizados são aplicados, é possível editar a forma como os formulários personalizados são exibidos nesses objetos, bem como editar campos comuns entre os formulários personalizados.

Somente os formulários personalizados anexados a todos os objetos selecionados podem ser editados em uma edição em massa.

Para editar vários formulários personalizados ao editar objetos em massa:

1. Em uma lista de objetos, selecione os objetos aos quais os formulários personalizados estão anexados e clique no botão **Editar** ícone ![](assets/edit-icon.png).
1. Clique em **Forms personalizada**.

   É possível editar apenas os formulários personalizados anexados a todos os objetos selecionados.

   Os formulários personalizados anexados somente a alguns objetos não são exibidos.

1. Comece a editar campos nos formulários personalizados.

   Quando os campos são editados, um indicador visual é mostrado no campo, mostrando que o campo foi editado.

   Se um campo for incluído em mais de um formulário personalizado, todos os valores desses campos serão atualizados em cada formulário quando você atualizar o campo em um dos formulários.

1. Clique no botão **Fazer uma seleção** e selecione formulários adicionais para adicionar a todos os objetos selecionados.

   Considere o seguinte ao aplicar formulários adicionais:

   * Os objetos podem ter até 10 formulários personalizados.
   * É possível aplicar formulários somente quando o formulário ainda não estiver aplicado a nenhum dos objetos que você está editando. Um formulário que já está anexado a um dos objetos não é exibido no menu suspenso.
   * Depois de aplicar um formulário adicional, todos os campos que o formulário tiver em comum com outros formulários serão exibidos na variável **Campos comuns** e podem ser editados.

1. (Opcional) Se você adicionou formulários personalizados a todos os objetos, mas ainda não salvou os objetos, é possível alterar a ordem em que os formulários personalizados aparecem nos objetos.

   Para obter mais informações sobre como alterar a ordem dos formulários, consulte [Reordenar vários formulários personalizados anexados a um objeto](#reorder-multiple-custom-forms-attached-to-an-object) neste artigo.

1. Clique em **Remover formulário** para remover um formulário personalizado dos objetos.

   Para obter mais informações sobre como remover formulários personalizados de objetos, consulte [Remover um formulário personalizado de um objeto](#remove-a-custom-form-from-an-object).

   Considere o seguinte ao remover formulários em massa de vários objetos:

   * Se você tiver alterado o formulário, removê-lo resultará na perda das alterações e elas não poderão ser recuperadas.
   * Depois de remover um formulário, quaisquer campos desse formulário que estavam no **Campos comuns** são removidas desta seção e não podem mais ser editadas aqui.

1. Clique em **Restaurar formulário** para restaurar o formulário para o estado em que ele estava antes de editar os objetos.
1. (Opcional) Clique na seta para recolher ao lado do nome do formulário para recolher um formulário de cada vez.

   Ou

   Clique em **Recolher Forms** para recolher todos os formulários ao mesmo tempo.

1. (Opcional) Clique na seta de expansão ao lado do nome do formulário para expandir um formulário de cada vez.

   Ou

   Clique em **Expandir Forms** expandir todos os formulários ao mesmo tempo. 

1. Clique em **Salvar alterações**.
