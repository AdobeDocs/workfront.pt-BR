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
source-git-commit: 2a2f6d93c916863177d7a9d2f46f8124d1430354
workflow-type: tm+mt
source-wordcount: '345'
ht-degree: 1%

---

# Visão geral do designer do formulário

Você pode usar o novo designer de formulário para criar um formulário personalizado que os usuários podem anexar a um objeto do Workfront. Os usuários que trabalham no objeto podem preencher o formulário personalizado para fornecer informações sobre o objeto.

O novo designer de formulário tem um novo espaço de trabalho no estilo da tela de desenho que permite exibir os campos, a tela de desenho e as configurações de campo, tudo ao mesmo tempo. Ela também permite arrastar e soltar campos nas seções ao criar o formulário.

![Designer de formulário de exemplo](assets/form-designer-example.png)

## Como acessar o designer do formulário

Um botão na parte superior do novo designer de formulário e do construtor de formulários herdado permite alternar entre as versões.

![Mudar para o novo designer de formulário](assets/switch-views.png)

## Nova funcionalidade disponível com o designer de formulário

Com o novo designer de formulários, adicionamos a capacidade de:

* **Copiar um campo**: Agora é possível copiar campos existentes clicando no ícone Copiar nos campos diretamente da tela.

* **Alterar o tamanho para Texto descritivo**: agora é possível atribuir tamanhos pequeno, médio ou grande a campos de texto Descritivo. Também é possível usá-los na mesma linha com outros campos.

* **Usar uma seção padrão**: se o criador do formulário não tiver adicionado uma seção na parte superior do formulário, uma seção Padrão agora estará visível na tela, para que os usuários possam ajustar as permissões para campos que não tenham uma seção personalizada atribuída.

  >[!NOTE]
  >
  >A seção Padrão não estará visível dentro dos objetos depois que o formulário for anexado ao objeto.

* **Usar um campo Pesquisa externa**: esse tipo de campo chama uma API externa e retorna valores como opções em um campo suspenso.

## Funcionalidade removida do designer do formulário

Removemos as seguintes funcionalidades do designer de formulário:

* As configurações de formulário agora estão disponíveis na parte superior da tela

* Rastrear alterações de campo nos campos de atualização

  >[!NOTE]
  >
  >Você pode encontrar essa opção em Configurar > Interface > Atualizar feeds

