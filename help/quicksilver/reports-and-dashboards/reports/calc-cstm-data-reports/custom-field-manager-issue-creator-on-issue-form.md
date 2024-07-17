---
content-type: reference
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: "Exemplo de campo personalizado calculado: exibir o gerente do criador de um problema no formulário personalizado de problema"
description: Usando um campo personalizado calculado, você pode exibir o nome do gerente do criador de um problema em um formulário personalizado anexado ao problema. Usando a mesma instrução, é possível construir campos calculados semelhantes para projetos, problemas e outros objetos.
author: Nolan
feature: Reports and Dashboards
exl-id: f501ce1a-7a80-458b-9b30-2292426c9262
source-git-commit: 888c938e5d649557df69374a55d4e4ecc2da6f55
workflow-type: tm+mt
source-wordcount: '413'
ht-degree: 0%

---

# Exemplo de campo personalizado calculado: exibir o gerente do criador de um problema no formulário personalizado de problema

Usando um campo personalizado calculado, você pode exibir o nome do gerente do criador de um problema em um formulário personalizado anexado ao problema. Usando a mesma instrução, é possível construir campos calculados semelhantes para projetos, problemas e outros objetos.

<!--outdated link: 
>[!TIP]
>
>For information about additional custom text mode examples from other customers, follow the [Text Mode Reporting](https://one.workfront.com/s/topic/0TO0z000000cdHmGAI/text-mode-reporting?tabset-21363=3) topic on our Community site.
-->

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>plano do Adobe Workfront*</p> </td> 
   <td>Qualquer</td> 
  </tr> 
  <tr> 
   <td> <p>Licença da Adobe Workfront*</p> </td> 
   <td> <p>Plano </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Configurações de nível de acesso*</td> 
   <td> <p>Acesso administrativo a formulários personalizados<br>Para obter informações sobre como conceder acesso administrativo a partir do nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Conceder aos usuários acesso administrativo a determinadas áreas</a>.</p> <p>Observação: se você ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode alterar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>Permissões de objeto</p> </td> 
   <td> <p>Acesso do Contribute ao objeto ao qual o formulário está anexado com acesso a Editar o formulário personalizado</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso aos objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qual plano, tipo de licença ou acesso você tem, contate o administrador do Workfront.

## Exibir o gerente do criador de um problema no formulário personalizado de problema

As etapas a seguir mostram como criar um campo calculado para um formulário personalizado de ocorrência em que é possível capturar o nome do gerente do usuário que criou a ocorrência. O processo é idêntico quando você deseja capturar o nome do gerente de um usuário que criou uma tarefa, um projeto, um portfólio, por exemplo.

1. Crie um formulário personalizado de problema e adicione um campo calculado a ele.

   Para obter informações sobre como criar um formulário personalizado e adicionar campos calculados a ele, consulte os seguintes artigos:

   * [Criar ou editar um formulário personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md)
   * [Adicionar dados calculados a um formulário personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md)

1. Copie e cole o seguinte código do modo de texto no campo **Cálculo** do formulário personalizado:

   ```
   {owner}.{manager}.{name}
   ```

   >[!TIP]
   >
   >Os cálculos de campo personalizado diferenciam maiúsculas de minúsculas.

1. Clique em **Concluído** e depois em **Salvar + Fechar**.

   O gerente do usuário que criou o problema é exibido no campo calculado quando o formulário que contém o campo é anexado a um problema.
