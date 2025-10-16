---
title: Adicionar ou excluir tipos de objetos de um formulário personalizado existente
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: Você pode adicionar ou remover tipos de objetos de formulários personalizados com o designer de formulários.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: c43ea6b2-7d5b-46f0-a092-f57128de60f0
source-git-commit: 15ac51cc13eeb57d2de194a9a6ceec7683acfbe6
workflow-type: tm+mt
source-wordcount: '461'
ht-degree: 0%

---

# Adicionar ou excluir tipos de objetos de um formulário personalizado existente

É possível adicionar ou excluir tipos de objetos de um formulário personalizado existente com o designer do formulário.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Pacote do Adobe Workfront</td> 
   <td><p>Qualquer</p></td> 
  </tr> 
  <tr> 
   <td>Licença do Adobe Workfront</td> 
   <td><p>Standard</p>
       <p>Plano</p></td>
  </tr> 
  <tr> 
   <td>Configurações de nível de acesso</td> 
   <td> <p>Acesso administrativo a formulários personalizados</p> </td> 
  </tr>  
 </tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Adicionar tipos de objeto a um formulário personalizado existente

Você pode adicionar outros tipos de objetos ao formulário para que ele possa ser anexado a vários objetos.

>[!NOTE]
>
>As permissões de quebra de seção podem ser afetadas pelo tipo de objeto. A permissão Edição limitada para quebras de seção de formulário personalizado está disponível somente para os tipos de objeto Projeto, Tarefa, Problema e Usuário.
>
>Para obter mais informações, consulte [Como vários tipos de objeto podem afetar as permissões de quebra de seção](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/organize-a-form.md#how-multiple-object-types-can-affect-section-break-permissions).


{{step-1-to-setup}}

1. Clique em **Forms Personalizado** no painel esquerdo.

   Na exibição exibida, você pode revisar todos os formulários personalizados que foram criados para sua organização. Você também pode ver quem criou cada formulário, com que tipo de objeto ele funciona e se ele está ativo.

1. Selecione o formulário personalizado ao qual você deseja adicionar outros tipos de objeto e clique em ![Ícone Editar](assets/edit-icon2.png).

1. Na parte superior do formulário, clique no sinal de adição + depois de **Tipos de objeto** e selecione o tipo desejado no menu exibido. Você pode repetir isso para adicionar quantos tipos de objetos desejar.

   ![Adicionar novo objeto](assets/add-new-object.png)

1. Clique em **Salvar e fechar**.

   >[!TIP]
   >
   >Você pode clicar em **Aplicar** a qualquer momento enquanto estiver criando um formulário personalizado para salvar suas alterações e manter o formulário aberto.

## Excluir tipos de objeto em um formulário personalizado

Você pode excluir tipos de objetos de um formulário personalizado existente. Um formulário personalizado deve ter pelo menos um tipo de objeto.

>[!CAUTION]
>
>Se as pessoas já tiverem anexado o formulário personalizado a objetos do tipo que você deseja excluir e adicionado dados a ele, esses dados serão excluídos permanentemente quando você excluir esse tipo de objeto no formulário. Pode incluir informações históricas que os usuários precisarão mais tarde.
>
>Em geral, recomendamos minimizar o número de vezes que você edita um formulário personalizado que já está em uso. Não há um sistema de notificação para alertar as pessoas que usam o formulário personalizado sobre suas alterações.

Para deletar um tipo de objeto:

{{step-1-to-setup}}

1. Clique em **Forms Personalizado** no painel esquerdo.
1. Selecione o formulário personalizado que deseja editar e clique em ![Ícone Editar](assets/edit-icon2.png).
1. Clique no X em qualquer um dos **Tipos de objeto** que deseja excluir do formulário.

   ![Excluir tipos de objetos](assets/delete-object-types.png)

1. (Opcional) Repita a etapa anterior para qualquer outro tipo de objeto que você deseja remover do formulário.
1. Clique em **Aplicar** e em **Salvar e fechar**.
