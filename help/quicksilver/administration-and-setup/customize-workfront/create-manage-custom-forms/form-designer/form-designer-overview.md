---
title: Visão geral do designer do formulário
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: Você pode criar um formulário personalizado que os usuários podem anexar a um objeto do Workfront. Os usuários que trabalham no objeto podem preencher o formulário personalizado para fornecer informações sobre o objeto.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: c2e2901b-0558-4a63-ae3c-4c3a6edf0ff0
source-git-commit: e34a0b3bf5e2c4dc794a7d7c85245bb4d11842be
workflow-type: tm+mt
source-wordcount: '402'
ht-degree: 1%

---

# Visão geral do designer do formulário

Você pode usar o novo designer de formulário para criar um formulário personalizado que os usuários podem anexar a um objeto do Workfront. Os usuários que trabalham no objeto podem preencher o formulário personalizado para fornecer informações sobre o objeto.

O novo designer de formulário tem um novo espaço de trabalho no estilo da tela de desenho que permite exibir os campos, a tela de desenho e as configurações de campo, tudo ao mesmo tempo. Ela também permite arrastar e soltar campos nas seções ao criar o formulário.

<!-- add screenshot when field settings empty state is ready -->

## Como acessar o novo designer de formulário

Há um novo botão na parte superior do novo designer de formulário e do construtor de formulários herdado. Você pode usar esse botão para alternar entre o construtor herdado e o novo designer.

![Mudar para o novo designer de formulário](assets/switch-views.png)

## Nova funcionalidade disponível com o designer de formulário

Com o novo designer de formulários, adicionamos a capacidade de:

* **Copiar um campo**: Agora é possível copiar campos existentes clicando no ícone Copiar nos campos diretamente da tela.

* **Alterar o tamanho para Texto descritivo**: agora é possível atribuir tamanhos pequeno, médio ou grande a campos de texto Descritivo. Também é possível usá-los na mesma linha com outros campos.

* **Usar uma seção padrão**: se o criador do formulário não tiver adicionado uma seção na parte superior do formulário, uma seção Padrão agora estará visível na tela, para que os usuários possam ajustar as permissões para campos que não tenham uma seção personalizada atribuída.

  >[!NOTE]
  >
  >A seção padrão não fica visível dentro dos objetos depois que o formulário é anexado ao objeto.

## Funcionalidade em breve

Os itens a seguir não estão disponíveis no momento no designer do formulário, mas serão adicionados em breve:

* Filtro para campos de digitação antecipada

>[!IMPORTANT]
>
>As configurações existentes para filtros de digitação antecipada não serão afetadas quando você trabalhar com o novo designer de formulário.

## Funcionalidade removida do designer do formulário

Removemos as seguintes funcionalidades do designer de formulário:

* Guias Configurações de formulário, Compartilhamento de formulários, Compartilhamento de campos

   * As configurações de formulário agora estão disponíveis na parte superior da tela

   * Guia principal Compartilhamento de formulário e subguia Compartilhamento de campo

  >[!NOTE]
  >
  >É possível controlar o compartilhamento de formulários e campos na área Configuração > Forms personalizado > Forms ou Campos.

* Rastrear alterações de campo nos campos de atualização

  >[!NOTE]
  >
  >Você pode encontrar isso em Configuração > Interface > Feeds de atualização
