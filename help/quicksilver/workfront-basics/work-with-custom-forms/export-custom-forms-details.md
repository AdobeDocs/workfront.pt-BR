---
title: Exportar formulários personalizados e detalhes do objeto
description: Exportar formulários personalizados e detalhes do objeto
author: Alina
draft: Probably
feature: Get Started with Workfront
exl-id: 4dc32da0-9680-4b7f-a959-d4a0652618c5
source-git-commit: c21029e098f6b4f51f8698155e2b8a2e789c8bfc
workflow-type: tm+mt
source-wordcount: '594'
ht-degree: 1%

---

# Exportar formulários personalizados e detalhes do objeto

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

Você deve ter o seguinte:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>plano do Adobe Workfront*</p> </td> 
   <td>Qualquer</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Licença da Adobe Workfront*</p> </td> 
   <td> <p>Solicitação ou superior para problemas</p> <p>Revisar ou superior para projetos e tarefas</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"><strong>Configurações de nível de acesso*</strong> </td> 
   <td> <p>Visualização ou superior para projetos, tarefas e problemas</p> <p>Observação: se você ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode alterar seu nível de acesso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Permissões de objeto</p> </td> 
   <td> <p>Visualize ou aumente as permissões do projeto, tarefa ou problema cujo formulário você deseja exportar</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso aos objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qual plano, tipo de licença ou acesso você tem, contate o administrador do Workfront.

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
