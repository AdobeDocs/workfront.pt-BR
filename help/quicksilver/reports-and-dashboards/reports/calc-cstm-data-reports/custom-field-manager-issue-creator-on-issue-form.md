---
content-type: reference
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: 'Exemplo de campo personalizado calculado: exibir o gerente do criador de um problema no formulário personalizado de problema'
description: Usando um campo personalizado calculado, você pode exibir o nome do gerente do criador de um problema em um formulário personalizado anexado ao problema. Usando a mesma instrução, é possível construir campos calculados semelhantes para projetos, problemas e outros objetos.
author: Jenny
feature: Reports and Dashboards
exl-id: f501ce1a-7a80-458b-9b30-2292426c9262
source-git-commit: a1ead6d0c1c85bfbe6d7302506743db8d8b3e205
workflow-type: tm+mt
source-wordcount: '334'
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

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>Pacote do Adobe Workfront</p> </td> 
   <td><p>Qualquer</p></td> 
  </tr> 
  <tr> 
   <td> <p>Licença do Adobe Workfront</p> </td> 
   <td>
      <p>Standard</p>
      <p>Plano</p></td>
  </tr> 
  <tr> 
   <td><p>Configurações de nível de acesso</p></td> 
   <td> <p>Acesso administrativo a formulários personalizados</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Permissões de objeto</p> </td> 
   <td> <p>Contribuir com acesso ao objeto ao qual o formulário está anexado com acesso a Editar o formulário personalizado</p></td> 
  </tr> 
 </tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Exibir o gerente do criador de um problema no formulário personalizado de problema

As etapas a seguir mostram como criar um campo calculado para um formulário personalizado de ocorrência em que é possível capturar o nome do gerente do usuário que criou a ocorrência. O processo é idêntico quando você deseja capturar o nome do gerente de um usuário que criou uma tarefa, um projeto, um portfólio, por exemplo.

1. Crie um formulário personalizado de problema e adicione um campo calculado a ele.

   Para obter informações sobre como criar um formulário personalizado e adicionar campos calculados a ele, consulte os seguintes artigos:

   * [Criar um formulário personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)
   * [Adicionar campos calculados a um formulário](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md)

1. Copie e cole o seguinte código do modo de texto no campo **Cálculo** do formulário personalizado:

   ```
   {owner}.{manager}.{name}
   ```

   >[!TIP]
   >
   >Os cálculos de campo personalizado diferenciam maiúsculas de minúsculas.

1. Clique em **Concluído** e depois em **Salvar + Fechar**.

   O gerente do usuário que criou o problema é exibido no campo calculado quando o formulário que contém o campo é anexado a um problema.
