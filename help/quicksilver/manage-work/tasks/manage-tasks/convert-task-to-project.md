---
product-area: projects
navigation-topic: manage-tasks
title: Converter uma tarefa em um projeto
description: Quando uma tarefa em um projeto requer uma quantidade maior de esforço para ser concluída do que você planejou originalmente, você pode convertê-la em um projeto.
author: Alina
feature: Work Management
exl-id: a45f0af4-1768-4f20-80d4-912e6fe0fc03
source-git-commit: dd7f61fcd92a43303be356dd3209ec6da6a063dd
workflow-type: tm+mt
source-wordcount: '602'
ht-degree: 0%

---

# Converter uma tarefa em um projeto

Quando uma tarefa em um projeto requer uma quantidade maior de esforço para ser concluída do que você planejou originalmente, você pode convertê-la em um projeto.

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plano Adobe Workfront*</td> 
   <td> <p>Qualquer Um</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Plano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a Tarefas e Projetos</p> <p>Exibir ou ter acesso superior a Modelos, ao converter em um projeto usando um modelo</p> <p>Observação: Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões para uma tarefa</p> <p>Visualizar permissões em um modelo, se estiver convertendo em um projeto usando um modelo</p> <p>Após criar o projeto, você tem permissões de gerenciamento para o projeto</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

## Considerações para conversão de tarefas em projetos

* A tarefa original é excluída.
* As aprovações de tarefa são excluídas.
* Todas as subtarefas, emissões e notas são acumuladas no novo projeto.
* Documentos, versões de documentos e provas são movidos para o novo projeto.
* O status e a porcentagem de conclusão de todas as subtarefas e problemas são preservados.
* Usuários compartilhados da tarefa se tornam usuários compartilhados no projeto.
* A data de início do projeto é definida como a data de início da tarefa.
* Se o status da tarefa for &quot;Novo&quot;, o status do projeto será definido como &quot;Planejamento&quot;.
* Se o status da tarefa for &#39;Em andamento&#39;, o status do projeto será definido como &#39;Atual&#39;.
* Se o status da tarefa for &#39;Concluído&#39;, o status do projeto será definido como &#39;Concluído&#39;.

## Converter uma tarefa em um projeto

1. Vá para a tarefa que deseja converter em um projeto.
1. Clique no botão **Mais** ícone ![](assets/more-icon.png), em seguida **Converter em projeto**.
1. Escolha as seguintes opções:

   * **Novo projeto**
   * Um modelo na **Selecionar a partir de modelos** seção

      ![](assets/convert-task-to-project-template-option-dropdown-nwe-350x209.png)

1. Clique em **Continuar** na notificação exibida.
1. No **Converter em projeto** , especifique o seguinte:

   * **Nome**: Dê um nome ao projeto. O nome padrão é o nome da tarefa.
   * (Opcional) **Descrição**: Descreva a finalidade deste projeto.
   * (Opcional e condicional) Se você tiver selecionado para criar um projeto a partir de um modelo, atualize os campos disponíveis no **Converter em projeto** caixa de diálogo.

      Para obter mais informações sobre como editar campos em projetos, consulte [Editar projetos](../../../manage-work/projects/manage-projects/edit-projects.md).

      >[!TIP]
      >
      >Para atualizar os campos na seção Finanças da caixa Converter em projeto , você deve ter o acesso Editar a Dados Financeiros em seu nível de acesso. Se você tiver o acesso de Exibição aos Dados Financeiros em seu nível de acesso , todas as informações financeiras do modelo serão transferidas para o novo projeto e não poderá editá-las enquanto converte o problema. Para obter mais informações, consulte [Conceder acesso aos dados financeiros](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md) e [Compartilhar um modelo](../../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md).

   * (Opcional) Adicionar **Forms personalizada** ao novo projeto.

      >[!TIP]
      Se um formulário personalizado de vários objetos anexado à tarefa for configurado para uso com tarefas e projetos, todas as informações salvas no formulário serão retidas quando você fizer a conversão.
      Se você estiver usando um modelo para a conversão e um formulário personalizado anexado ao modelo contiver um campo personalizado também encontrado em um formulário personalizado anexado à tarefa, o valor do campo da tarefa será usado para o novo projeto. No entanto, se o campo personalizado estiver em branco na tarefa, o valor do modelo será usado.

1. Clique em **Salvar alterações**.
