---
user-type: administrator
content-type: faq
product-area: system-administration
keywords: kickstart,kick-start,kickstarts,kick-starts
navigation-topic: use-kick-starts
title: Perguntas frequentes sobre Kick-Starts
description: Encontre respostas para perguntas frequentes sobre a importação e exportação de dados do Workfront usando o Kick-Starts.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: f286e03e-93a8-43f5-8c2d-2c36203776a8
source-git-commit: 1ebdb3797e30a7e06f4dfd4a7e0e5f540351c126
workflow-type: tm+mt
source-wordcount: '412'
ht-degree: 0%

---

# Perguntas frequentes sobre Kick-Starts

As perguntas a seguir são feitas com frequência sobre Kick-Starts:

## Por que estou recebendo este erro ao tentar importar um arquivo do Kickstart: &quot;Seu arquivo estava correto, mas nada foi importado?&quot;

### Responder

Um dos três itens a seguir pode estar faltando no arquivo Kick-Start:

1. A coluna **isNew** deve ser definida como **TRUE** para todos os itens que você deseja importar. **isNew** deve ser **TRUE** porque você só pode importar dados novos com um Kick-Start. Não é possível modificar dados existentes por meio do Kickstart. Você pode ter outras linhas na planilha com **isNew = FALSE**, mas essas linhas não serão importadas.

1. &#x200B;O arquivo precisa ter uma linha vazia antes do início dos cabeçalhos dos dados.
1. &#x200B;As planilhas do Excel precisam ter o(s) nome(s) correto(s).

Ao trabalhar com o Kick-Starts, recomendamos primeiro baixar o modelo de Kick-start, preenchê-lo manualmente com os dados corretos e importá-lo de volta para o Adobe Workfront.

Para obter mais informações sobre como importar dados corretamente no Workfront usando o Kick-Starts, consulte [Importar dados para o Adobe Workfront usando um modelo de Kick-Start](../../../administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md).

## Por que estou recebendo este erro ao tentar importar horas para o Workfront usando um arquivo do Kickstart: &quot;Usuário com valores de chave primária &quot;null&quot; não encontrado?&quot;

### Responder

O erro se refere à GUID do usuário associada às horas.

Para resolver isso:

1. Exportar um modelo de Início em branco somente para o objeto **Hours**.\
   Para obter mais informações sobre como exportar um arquivo do Kickstart em branco, consulte &quot;Exportando o Modelo do Kickstart&quot; em [Importar dados para o Adobe Workfront usando um modelo do Kickstart](../../../administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md).

1. Copie manualmente os dados do Kickstart original e cole-os no arquivo vazio.\
   Faça isso para cada coluna.
1. Tente importar o novo arquivo novamente.\
   O Kickstart deve ser importado com sucesso.

## Por que o campo do país não é preenchido no perfil do usuário em uma importação do Kickstart?

### Problema

Ao importar um Kickstart de usuário com o campo **setCountry**, esses dados não chegam ao país no perfil do usuário.

### Responder

Se o usuário estiver habilitado para Unified User Management (UUM) ou Adobe Identity Management System (IMS), o campo **País** só aceitará valores de código de país (por exemplo, EUA, GB, IN). Verifique se o campo **setCountry** no modelo de Início está usando valores de código de país antes de importar.

Para obter mais informações sobre como importar dados corretamente no Workfront usando o Kick-Starts, consulte [Importar dados para o Adobe Workfront usando um modelo de Kick-Start](/help/quicksilver/administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md).
