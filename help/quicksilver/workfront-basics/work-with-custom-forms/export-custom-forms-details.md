---
title: Exportar formulários personalizados e detalhes do objeto
description: Exportar formulários personalizados e detalhes do objeto
author: Alina
draft: Probably
feature: Get Started with Workfront
exl-id: 4dc32da0-9680-4b7f-a959-d4a0652618c5
source-git-commit: 4ef71db5d93e314b746e8acdbf90fd041c6e71ae
workflow-type: tm+mt
source-wordcount: '549'
ht-degree: 1%

---

# Exportar formulários personalizados e detalhes do objeto

<!--Audited: 10/2025-->

É possível exportar as informações de Visão geral e formulário personalizado da seção Detalhes de um objeto para um arquivo do PDF. Em seguida, você pode imprimir ou compartilhar a PDF com outros usuários.

Essa funcionalidade é compatível com os seguintes objetos:

* Projetos
* Tarefas
* Problemas
* Portfólio
* Programas

<!--
* Billing records</p> <p>After you open a billing record on a project, you can use the Details area to attach a custom form to the record and fill it out. You can also export billing record information from the Details area.</p> </li>
  -->

>[!NOTE]
>
>Os campos na seção Detalhes que o administrador do Workfront ou do grupo removeu usando um modelo de layout não são exibidos.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Pacote do Adobe Workfront</p> </td> 
   <td>Qualquer</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Licença do Adobe Workfront</p> </td> 
   <td><p>Para problemas:</p>
   <ul><li><p>Colaborador ou superior</p></li>
   <li><p>Solicitante ou superior</p> </li></ul>
   <p>Para projetos e tarefas:</p>
   <ul><li><p>Leve ou superior</p></li>
   <li><p>Revisor ou superior</p></li></ul>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Visualização ou superior para projetos, tarefas e problemas</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Permissões de objeto</p> </td> 
   <td> <p>Visualize ou aumente as permissões do projeto, tarefa ou problema cujo formulário você deseja exportar</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:
<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Adobe Workfront plan*</p> </td> 
   <td>Any</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Adobe Workfront license*</p> </td> 
   <td> <p>Request or higher for issues</p> <p>Review or higher for projects and tasks</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"><strong>Access level configurations*</strong> </td> 
   <td> <p>View or higher for Projects, Tasks, and Issues</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Object permissions</p> </td> 
   <td> <p>View or higher permissions to the project, task, or issue whose form you want to export</p> <p>For information on requesting additional access, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Pré-requisitos

Antes de começar, você deve ter todos os itens a seguir:

1. Ter um formulário personalizado criado para um objeto específico do qual você deseja exportá-lo.
1. Ter o formulário personalizado anexado ao objeto

   Ou

   Ter o acesso correto para anexar um formulário personalizado e editar as informações no formulário.

Para obter informações sobre como criar formulários personalizados, consulte [Criar um formulário personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

Para obter informações sobre como anexar formulários a objetos, consulte [Adicionar um formulário personalizado a um objeto](../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

## Exportar informações na seção Detalhes

A exportação de informações da seção Detalhes de um objeto é idêntica para todos os objetos em que é suportada.

1. Vá para um projeto, tarefa, portfólio, programa ou problema para o qual você tenha pelo menos permissões de Exibição.
1. Clique no item **&quot;Detalhes&quot;** no painel esquerdo, como **Detalhes da tarefa**.
1. (Opcional) Se não houver nenhum formulário personalizado anexado ao objeto, comece digitando o nome de um formulário personalizado no **Adicionar campo de formulário personalizado**, em seguida, clique nele quando ele aparecer na lista.

   Você pode adicionar até 10 formulários.

1. (Opcional) Atualize as informações na seção Detalhes e clique em **Salvar alterações**.
1. Clique no menu suspenso **Exportar** no canto superior direito, selecione **Visão geral** ou os formulários que deseja exportar e clique em **Exportar**.

   Você também pode selecionar **Selecionar tudo** se desejar exportar a área Visão geral e todos os formulários personalizados.

   ![](assets/export-custom-form-button-menu.png)

   >[!TIP]
   >
   >Os seguintes cenários podem existir:
   >
   >   * Quando o administrador do grupo ou do Workfront desmarca todos os campos na área Visão geral e o objeto tem formulários personalizados anexados, a seção Visão geral não é exibida.
   >   * Quando o administrador do grupo ou do Workfront desmarca todos os campos na área Visão geral e o objeto não tem formulários personalizados anexados, o menu suspenso Exportar não fica visível.
   >   * Quando o objeto não tiver formulários personalizados anexados, você poderá exportar somente a área Visão geral.
   >   * Os campos personalizados que estão atrás da lógica e não estão visíveis no formulário não são exportados. Para obter informações sobre como adicionar lógica a um formulário personalizado, consulte [Adicionar regras de lógica a formulários e campos personalizados](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/display-skip-logic-form-designer.md).

   Um arquivo PDF é produzido e baixado no computador. O arquivo PDF contém as seguintes informações:

   * O nome do objeto ao qual o formulário está anexado
   * O nome do usuário que exportou o PDF
   * A data e a hora em que o PDF foi produzido
   * O nome dos formulários exportados
   * Informações dos campos preenchidos no formulário
