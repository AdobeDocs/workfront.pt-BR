---
title: Criar ou editar uma condição personalizada
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-conditions
description: Como administrador do Adobe Workfront, você pode criar ou editar uma condição personalizada para projetos, tarefas e problemas para atender às necessidades da sua organização.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 5c950862-4358-4aab-997b-223972662150
source-git-commit: a54200ceeaadfeaac6767f06676cb11814959601
workflow-type: tm+mt
source-wordcount: '638'
ht-degree: 2%

---

# Criar ou editar uma condição personalizada

Como administrador do Adobe Workfront, você pode criar ou editar uma condição personalizada para projetos, tarefas e problemas para atender às necessidades da sua organização.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>plano do Adobe Workfront</td> 
   <td>Qualquer</td> 
  </tr> 
  <tr> 
   <td>Licença do Adobe Workfront</td> 
   <td>Plano</td> 
  </tr> 
  <tr> 
   <td>Configurações de nível de acesso</td> 
   <td> <p>Você deve ser um administrador do Workfront.</p> <p><b>OBSERVAÇÃO</b>: se você ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais no seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## Criar ou editar uma condição personalizada

{{step-1-to-setup}}

1. Clique em **Preferências do projeto** > **Condições**.

1. Clique na guia do tipo de objeto (**Projeto**, **Tarefa** ou **Problema**) que você deseja associar à condição.

1. Para criar uma nova condição, clique em **Adicionar uma Nova Condição**.

   Ou

   Para editar uma condição existente, passe o mouse sobre a condição que deseja editar, em seguida, clique no ícone **Editar** que aparece à direita.

   ![](assets/custom-condition-edit-nwe.jpg)

1. Configure sua condição personalizada usando as seguintes opções:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td>Nome da condição</td> 
      <td>(Obrigatório) Digite um nome descritivo para a condição.</td> 
     </tr> 
     <tr> 
      <td>Descrição</td> 
      <td>(Opcional) Digite uma descrição da finalidade da condição para aqueles que a usarão.</td> 
     </tr> 
     <tr> 
      <td>Cor</td> 
      <td>(Opcional) Clique no ícone de cor e escolha a cor desejada para a condição quando ela for exibida em projetos, tarefas ou problemas. Você também pode digitar um número hexadecimal.</td> 
     </tr> 
     <tr> 
      <td>Correspondente </td> 
      <td><p>(Obrigatório, somente para projetos) Clique na opção na lista suspensa que melhor descreve a função da nova condição. Por exemplo, para uma condição chamada Compartimento de rastreamento, você clicaria em No Target. Isso determina como as condições padrão funcionam. Todas as condições criadas devem ser iguais a uma das opções no menu suspenso.</p>
      <p>Para obter informações sobre condições padrão, consulte <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-projects.md" class="MCXref xref">Definir uma condição personalizada como padrão para projetos</a> e <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-tasks-issues.md" class="MCXref xref">Definir uma condição personalizada como padrão para tarefas e problemas</a>.</p>
      <p>Essa opção não poderá ser modificada depois que você terminar de criar a condição.</p></td> 
     </tr> 
     <tr> 
      <td>Chave</td> 
      <td><p>(Obrigatório) Para uma condição de projeto, digite uma abreviação alfanumérica que os usuários poderão reconhecer. Para tarefas ou problemas, digite um código numérico de dois dígitos de 01 a 99. </p>
      <p>Essa chave, que é usada na API e pode ser usada para fins de relatórios, deve ser exclusiva para cada objeto.</p>
      <p>Não é possível alterar a chave de uma condição depois de salvá-la. </p></td> 
     </tr> 
     <tr> 
      <td>Ocultar condição</td> 
      <td><p>(Opcional) Essa opção está disponível para condições personalizadas que você não deseja mais que as pessoas usem, mas que deseja manter por motivos históricos. </p>
      <p>Se você ocultar uma condição personalizada que tenha sido usada em itens de trabalho, ela continuará a aparecer nesses itens de trabalho depois de ocultá-la. </p></td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >Você pode padronizar a terminologia de condição e as cores em todos os três tipos de objeto. Para fazer isso, copie o Nome da condição e o código hexadecimal da Cor de uma guia (Projeto, Tarefa, Problema) para a condição correspondente nas outras duas guias.

1. (Opcional) Arraste ![](assets/move-icon---dots.png) qualquer condição para uma nova posição para reordenar a lista.

   Isso altera a ordem em que as condições são exibidas em projetos, tarefas e problemas:

   * Quando um usuário edita um projeto

     ![](assets/change-condition-edit-project.png)

   * Quando um usuário altera a condição de uma tarefa ou problema na guia Atualizações:

     ![](assets/change-condition-update-comment.png)

   * Quando um usuário altera a condição de uma tarefa ou problema em uma exibição de lista:

     ![](assets/change-conditions-list-dropdown-only.png)

1. Clique em **Salvar**.

Você pode definir sua condição personalizada como uma condição padrão para projetos ou tarefas e problemas. Para obter mais informações, consulte [Definir uma condição personalizada como padrão para projetos](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-projects.md) e [Definir uma condição personalizada como padrão para tarefas e problemas](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-tasks-issues.md).

Para obter mais informações sobre condições personalizadas, consulte [Condições personalizadas](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/custom-conditions.md).
