---
title: Visão geral do designer do formulário
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: Você pode criar um formulário personalizado que os usuários podem anexar a um objeto do Workfront. Os usuários que trabalham no objeto podem preencher o formulário personalizado para fornecer informações sobre o objeto.
author: Courtney
feature: System Setup and Administration
role: Admin
source-git-commit: 9b32c41c9f2971f3b0bbded230680677cc0b3c64
workflow-type: tm+mt
source-wordcount: '407'
ht-degree: 1%

---

# Visão geral do designer do formulário

{{highlighted-preview-article-level}}

Você pode usar o novo designer de formulário para criar um formulário personalizado que os usuários podem anexar a um objeto do Workfront. Os usuários que trabalham no objeto podem preencher o formulário personalizado para fornecer informações sobre o objeto.

O novo designer de formulário tem um novo espaço de trabalho no estilo da tela de desenho que permite exibir os campos, a tela de desenho e as configurações de campo, tudo ao mesmo tempo. Ela também permite arrastar e soltar campos nas seções ao criar o formulário.

<!-- add screenshot when field settings empty state is ready -->

## Como acessar o novo designer de formulário

Há um novo botão na parte superior do novo designer de formulário e do construtor de formulários herdado. Você pode usar esse botão para alternar entre o construtor herdado e o novo designer.

![](assets/switch-views.png)

## Nova funcionalidade disponível com o designer de formulário

Com o novo designer de formulários, adicionamos a capacidade de

* **Copiar um campo**: Agora é possível copiar campos existentes clicando no ícone Copiar nos campos diretamente da tela.

* **Alterar o tamanho para Texto descritivo**: agora é possível atribuir tamanhos pequeno, médio ou grande a campos de texto Descritivo. Também é possível usá-los na mesma linha com outros campos.

* **Usar uma seção padrão**: se o criador do formulário não tiver adicionado uma seção na parte superior do formulário, uma seção Padrão agora estará visível na tela, para que os usuários possam ajustar as permissões para campos que não tenham uma seção personalizada atribuída.

   >[!NOTE]
   >
   >A seção padrão não fica visível dentro dos objetos depois que o formulário é anexado ao objeto.

## Funcionalidade em breve

Os itens a seguir não estão disponíveis no momento no designer do formulário, mas serão adicionados em breve:

* Ajustar o tamanho do texto descritivo

* Lógica de exibição/salto

* Filtro para campos de digitação antecipada

>[!IMPORTANT]
>
>As configurações existentes para filtros de lógica e digitação antecipada não serão afetadas ao trabalhar com o novo designer de formulário.

## Funcionalidade removida do designer do formulário

Removemos as seguintes funcionalidades do designer de formulário interno:


* Guias Configurações de formulário, Compartilhamento de formulários, Compartilhamento de campos

   * As configurações de formulário agora estão disponíveis na parte superior da tela

   * Guia principal Compartilhamento de formulário e subguia Compartilhamento de campo
   >[!NOTE]
   >
   >É possível controlar o compartilhamento de formulários e campos na guia Configurar > Forms personalizado > Forms ou Campos.

* Rastrear alterações de campo nos campos de atualização
   >[!NOTE]
   >
   >Você pode encontrar isso em Configuração > Interface > Feeds de atualização
