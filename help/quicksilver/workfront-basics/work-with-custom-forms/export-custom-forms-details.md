---
title: Exportar formulários personalizados e detalhes do objeto
description: Exportar formulários personalizados e detalhes do objeto
author: Alina
draft: Probably
feature: Get Started with Workfront
exl-id: 4dc32da0-9680-4b7f-a959-d4a0652618c5
source-git-commit: 1670edf153e57152e51adcfbda052eb74541d931
workflow-type: tm+mt
source-wordcount: '597'
ht-degree: 1%

---

# Exportar formulários personalizados e detalhes do objeto

É possível exportar a Visão geral e as informações personalizadas do formulário da seção Detalhes de um objeto para um arquivo PDF. Em seguida, é possível imprimir ou compartilhar o PDF com outros usuários.

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
>Os campos na seção Detalhes que seu Workfront ou administrador de grupo removeu usando um modelo de layout não são exibidos.

## Requisitos de acesso

Você deve ter o seguinte:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Plano Adobe Workfront*</p> </td> 
   <td>Qualquer Um</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Licença da Adobe Workfront*</p> </td> 
   <td> <p>Solicitação ou superior para problemas</p> <p>Revisar ou superior para projetos e tarefas</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"><strong>Configurações de nível de acesso*</strong> </td> 
   <td> <p>Exibir ou superior para Projetos, Tarefas e Problemas</p> <p>Observação: Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode alterar seu nível de acesso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Permissões de objeto</p> </td> 
   <td> <p>Exibir permissões ou permissões mais altas para o projeto, tarefa ou problema cujo formulário você deseja exportar</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

## Pré-requisitos

Antes de começar, você deve ter todos os itens a seguir:

1. Crie um formulário personalizado para um objeto específico do qual deseja exportá-lo.
1. Ter o formulário personalizado anexado ao objeto

   Ou

   Tenha o acesso correto para anexar um formulário personalizado e editar as informações no formulário.

Para obter informações sobre como criar formulários personalizados, consulte [Criar ou editar um formulário personalizado](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

Para obter informações sobre como anexar formulários a objetos, consulte [Adicionar um formulário personalizado a um objeto](../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

## Exportar informações na seção Detalhes

A exportação de informações da seção Detalhes de um objeto é idêntica para todos os objetos em que é compatível.

1. Vá para um projeto, tarefa, portfólio, programa ou problema para o qual tenha pelo menos permissões de Exibição.
1. Clique no botão **Item &quot;Detalhes&quot;** no painel esquerdo, como **Detalhes da tarefa**.
1. (Opcional) Se não houver um formulário personalizado anexado ao objeto, comece a digitar o nome de um formulário personalizado no **Adicionar campo de formulário personalizado**, depois clique nele quando ele aparecer na lista.

   É possível adicionar até 10 formulários.

1. (Opcional) Atualize as informações na seção Detalhes e clique em **Salvar alterações**.
1. Clique no botão **Exportar** no menu suspenso no canto superior direito, selecione **Visão geral** ou os formulários que deseja exportar, em seguida, clique em **Exportar**.

   Você também pode selecionar **Selecionar tudo** se quiser exportar a área Visão geral e todos os formulários personalizados.

   ![](assets/export-custom-form-button-menu.png)

   >[!TIP]
   >
   >Os seguintes cenários podem existir:
   >
   >   
   >   
   >   * Quando seu grupo ou administrador do Workfront desmarca todos os campos na área Visão geral e o objeto tem formulários personalizados anexados, a seção Visão geral não é exibida.
   >   * Quando o administrador do grupo ou do Workfront desmarca todos os campos na área Visão geral e o objeto não tem formulários personalizados anexados, o menu suspenso Exportar não fica visível.
   >   * Quando o objeto não tem formulários personalizados anexados, é possível exportar apenas a área Visão geral .
   >   * Campos personalizados que estão por trás da lógica e não estão visíveis no formulário não são exportados. Para obter informações sobre como adicionar lógica a um formulário personalizado, consulte [Adicionar lógica de exibição e ignorar lógica a um formulário personalizado](../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md).


   Um arquivo PDF é produzido e baixado no computador. O arquivo PDF contém as seguintes informações:

   * O nome do objeto ao qual o formulário está anexado
   * O nome do usuário que exportou o PDF
   * A data e a hora em que o PDF foi produzido
   * O nome dos formulários que você exportou
   * Informações dos campos preenchidos no formulário
