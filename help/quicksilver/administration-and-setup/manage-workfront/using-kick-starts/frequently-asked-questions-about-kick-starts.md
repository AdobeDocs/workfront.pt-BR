---
user-type: administrator
content-type: faq
product-area: system-administration
keywords: kickstart,kick-start,kickstarts,kick-starts
navigation-topic: use-kick-starts
title: Perguntas frequentes sobre o Kick-Starts
description: Encontre respostas para perguntas frequentes sobre a importação e exportação de dados do Workfront usando o Kick-Starts.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: f286e03e-93a8-43f5-8c2d-2c36203776a8
source-git-commit: 1ebdb3797e30a7e06f4dfd4a7e0e5f540351c126
workflow-type: tm+mt
source-wordcount: '415'
ht-degree: 0%

---

# Perguntas frequentes sobre o Kick-Starts

As perguntas a seguir são frequentes sobre o Kick-Starts:

## Por que estou recebendo esse erro ao tentar importar um arquivo de Início rápido: &quot;Seu arquivo estava correto, mas nada foi importado?&quot;

### Resposta

Uma das três coisas a seguir pode estar faltando no arquivo Kick-Start :

1. O **isNew** deve ser definida como **TRUE** para todos os itens que deseja importar. **isNew** deve ser **TRUE** porque você só pode importar novos dados com um Início rápido. Não é possível modificar dados existentes por meio do Início rápido. Você pode ter outras linhas na planilha com **isNew = FALSE** mas essas linhas não serão importadas.

1. &#x200B; O arquivo precisa ter uma linha vazia antes que os cabeçalhos dos dados sejam iniciados.
1. &#x200B; As folhas do Excel precisam ter os nomes corretos.

Ao trabalhar com o Kick-Starts, recomendamos baixar primeiro o Modelo de início, preenchê-lo manualmente com os dados corretos e importá-lo de volta para o Adobe Workfront.

Para obter mais informações sobre como importar dados corretamente no Workfront usando o Kick-Starts, consulte [Importar dados para o Adobe Workfront usando um modelo de Início rápido](../../../administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md).

## Por que estou recebendo esse erro ao tentar importar horas para o Workfront usando um arquivo de Início rápido: &quot;Usuário com valores de chave primária &quot;null&quot; não encontrado?&quot;

### Resposta

O erro se refere ao GUID do usuário associado às horas.

Para resolver isso:

1. Exportar um modelo de Início rápido em branco para o **Horas** somente para objetos.\
   Para obter mais informações sobre como exportar um arquivo de Início Rápido em branco, consulte &quot;Exportando o modelo de Início Rápido&quot; em  [Importar dados para o Adobe Workfront usando um modelo de Início rápido](../../../administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md).

1. Copie manualmente os dados do Início rápido original e cole-os no arquivo vazio.\
   Faça isso para cada coluna.
1. Tente importar o novo arquivo novamente.\
   O Início rápido deve ser importado com êxito.

## Por que o campo de país não está preenchido no perfil de usuário em uma importação de Início rápido?

### Problema

Ao importar um Início rápido do usuário com o campo **setCountry**, que os dados não vêm para o país no perfil do usuário.

### Resposta

Se o usuário estiver habilitado para o Gerenciamento de usuário unificado (UUM) ou para o Sistema Adobe Identity Management (IMS), a variável **País** só aceita valores de código de país (por exemplo, US, GB, IN). Verifique se a variável **setCountry** O campo no modelo de Início rápido está usando valores de código de país antes de importar.

Para obter mais informações sobre como importar dados corretamente no Workfront usando o Kick-Starts, consulte [Importar dados para o Adobe Workfront usando um modelo de Início rápido](/help/quicksilver/administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md).
