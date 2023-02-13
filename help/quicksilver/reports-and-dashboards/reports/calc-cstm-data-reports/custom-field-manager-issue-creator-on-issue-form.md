---
content-type: reference
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: "Exemplo de campo personalizado calculado: exibir o gerente do criador de um problema no formulário personalizado do problema"
description: Usando um campo personalizado calculado, você pode exibir o nome do gerente do criador de uma ocorrência em um formulário personalizado anexado à ocorrência. Usando a mesma instrução, é possível criar campos calculados semelhantes para projetos, problemas e outros objetos.
author: Nolan
feature: Reports and Dashboards
exl-id: f501ce1a-7a80-458b-9b30-2292426c9262
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '443'
ht-degree: 0%

---

# Exemplo de campo personalizado calculado: exibir o gerente do criador de um problema no formulário personalizado do problema

Usando um campo personalizado calculado, você pode exibir o nome do gerente do criador de uma ocorrência em um formulário personalizado anexado à ocorrência. Usando a mesma instrução, é possível criar campos calculados semelhantes para projetos, problemas e outros objetos.

>[!TIP]
>
>Para obter informações sobre exemplos adicionais de modo de texto personalizado de outros clientes, siga o [Relatório do modo de texto](https://one.workfront.com/s/topic/0TO0z000000cdHmGAI/text-mode-reporting?tabset-21363=3) tópico em nosso site da Comunidade.

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>Plano Adobe Workfront*</p> </td> 
   <td>Qualquer Um</td> 
  </tr> 
  <tr> 
   <td> <p>Licença da Adobe Workfront*</p> </td> 
   <td> <p>Plano </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Configurações de nível de acesso*</td> 
   <td> <p>Acesso administrativo aos formulários personalizados<br>Para obter informações sobre a concessão de acesso administrativo a partir do nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Conceder aos usuários acesso administrativo a determinadas áreas</a>.</p> <p>Observação: Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode alterar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>Permissões de objeto</p> </td> 
   <td> <p>Contribua para o acesso ao objeto ao qual o formulário está anexado com acesso para Editar o formulário personalizado</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

## Exibir o gerente do criador de um problema no formulário personalizado do problema

As etapas a seguir mostram como criar um campo calculado para um formulário personalizado de ocorrência, onde é possível capturar o nome do gerente do usuário que criou o problema. O processo é idêntico quando você deseja capturar o nome do gerente de um usuário que criou uma tarefa, um projeto, um portfólio, por exemplo.

1. Crie um formulário personalizado de ocorrência e adicione um campo calculado a ele.

   Para obter informações sobre como criar um formulário personalizado e adicionar campos calculados a ele, consulte os seguintes artigos:

   * [Criar ou editar um formulário personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md)
   * [Adicionar dados calculados a um formulário personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md)

1. Copie e cole o seguinte código do modo de texto no **Cálculo** campo do formulário personalizado:

   ```
   {owner}.{manager}.{name}
   ```

   >[!TIP]
   >
   >Os cálculos de campo personalizado fazem distinção entre maiúsculas e minúsculas.

1. Clique em **Concluído**, em seguida **Salvar + Fechar**.

   O gerente do usuário que criou o problema é exibido no campo calculado quando o formulário que contém o campo é anexado a um problema.
