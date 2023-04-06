---
title: Visão geral do designer de formulários
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: É possível criar um formulário personalizado que os usuários podem anexar a um objeto do Workfront. Os usuários que trabalham no objeto podem preencher o formulário personalizado para fornecer informações sobre ele.
author: Courtney
feature: System Setup and Administration
role: Admin
source-git-commit: 6e06e7892542c7dd96b6bf8b857583333efc883d
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Visão geral do designer de formulários

Você pode usar o novo designer de formulário para criar um formulário personalizado que os usuários podem anexar a um objeto do Workfront. Os usuários que trabalham no objeto podem preencher o formulário personalizado para fornecer informações sobre ele.

O novo designer de formulário tem um novo espaço de trabalho de estilo tela que permite exibir os campos, a tela e as configurações de campo ao mesmo tempo. Também permite arrastar e soltar campos nas seções ao projetar o formulário.

<!-- add screenshot when field settings empty state is ready -->

## Como acessar o novo designer de formulário

Há um novo botão na parte superior do novo designer de formulário e do construtor de formulários herdado. Você pode usar esse botão para alternar entre o construtor herdado e o novo designer.

![](assets/switch-views.png)

## Nova funcionalidade disponível com o designer de formulário

Com o novo designer de formulário, adicionamos a capacidade de

* **Copiar um campo**: Agora é possível copiar campos existentes clicando no ícone Copiar nos campos diretamente da tela.

* **Alterar o tamanho do texto Descritivo**: Agora é possível atribuir tamanhos pequenos, médios ou grandes a campos de texto descritivo. Também é possível usá-los na mesma linha com outros campos.

* **Usar uma seção padrão**: Se o criador do formulário não tiver adicionado uma seção na parte superior do formulário, uma seção Padrão agora estará visível na tela, para que os usuários possam ajustar as permissões para campos que não têm nenhuma seção personalizada atribuída.

   >[!NOTE]
   >
   >A seção padrão não fica visível nos objetos depois que o formulário é anexado ao objeto.

## Funcionalidade em breve

Os itens a seguir não estão disponíveis no designer de formulários, mas serão adicionados em breve:

* Ajuste o tamanho do texto descritivo

* Exibir/ignorar lógica

* Filtrar para campos de digitação antecipada

>[!IMPORTANT]
>
>As configurações existentes para filtros de lógica e de digitação não serão afetadas quando você trabalhar com o novo designer de formulário.

## Funcionalidade removida do designer de formulários

Removemos a seguinte funcionalidade de dentro do designer de formulários:


* Configurações do formulário, Compartilhamento de formulário, Guias de Compartilhamento de campo

   * As configurações do formulário agora estão disponíveis na parte superior da tela

   * Guia principal Compartilhamento de formulário e subguia Compartilhamento de campo
   >[!NOTE]
   >
   >É possível controlar o compartilhamento de formulário e campo em Configurar > Forms personalizado > Forms ou guia Campos.

* Rastrear alterações de campo nos campos de atualização
   >[!NOTE]
   >
   >Você pode encontrar isso em Configuração > Interface > Atualizar feeds
