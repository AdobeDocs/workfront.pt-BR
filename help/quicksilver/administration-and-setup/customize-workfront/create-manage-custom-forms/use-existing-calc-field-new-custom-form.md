---
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
title: Reutilizar um campo personalizado calculado existente em um formulário personalizado com o construtor de formulários herdado
description: É possível usar o mesmo campo personalizado calculado em formulários personalizados que pertencem a objetos diferentes. Por exemplo, é possível usar o campo Lucro calculado criado para o formulário personalizado do projeto em um formulário personalizado de tarefa.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 24482fca-94e4-406d-9d62-3db9f51481e6
source-git-commit: ac5b7e0237dbcaea14010eda658f7d5a6be089cc
workflow-type: tm+mt
source-wordcount: '289'
ht-degree: 0%

---

# Reutilizar um campo personalizado calculado existente em um formulário personalizado com o construtor de formulários herdado

É possível usar o mesmo campo personalizado calculado em formulários personalizados que pertencem a objetos diferentes. Por exemplo, é possível usar o campo Lucro calculado criado para o formulário personalizado do projeto em um formulário personalizado de tarefa.

Para obter informações sobre como adicionar um campo personalizado calculado a um formulário personalizado, consulte [Adicionar dados calculados a um formulário personalizado com o construtor de formulários herdado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

Ao usar um campo personalizado calculado existente, o cálculo não é transferido para o novo formulário. Você deve adicionar o cálculo novamente, no mesmo campo, no novo formulário personalizado.

>[!TIP]
>
>Isso ocorre ao usar o cálculo armazenado na variável **Instruções** do formulário personalizado ajuda.

Também é possível ter um cálculo diferente para o mesmo campo, no novo formulário. Manter o mesmo nome para o campo personalizado calculado garante a coesão e a consistência em sua convenção de nomenclatura.

>[!IMPORTANT]
>
>Os campos personalizados calculados podem se tornar desatualizados ao longo do tempo. Para garantir que você sempre visualize o cálculo atualizado nesses campos, siga um destes procedimentos:
>
>* Depois de salvar um objeto em que você tenha editado dados em um formulário personalizado anexado, clique no ícone Mais ![](assets/more-icon.png) na página principal do objeto, em seguida, Recalcular expressões personalizadas.
>* Selecione a opção Recalcular expressões personalizadas ao editar objetos em massa.
>* Selecione a opção Atualizar cálculos anteriores ao editar um Campo personalizado calculado em um formulário personalizado.
>

